# Comparing `tmp/pytelerdac-0.2.0-cp38-cp38-manylinux1_x86_64.whl.zip` & `tmp/pytelerdac-0.3.0-cp38-cp38-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 159633 bytes, number of entries: 13
+Zip file size: 164415 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-22 07:53 pytelerdac/__init__.py
--rwxrwxr-x  2.0 unx   114776 b- defN 23-May-04 07:31 pytelerdac/rdac.cpython-38-x86_64-linux-gnu.so
+-rwxrwxr-x  2.0 unx   114776 b- defN 23-May-19 07:57 pytelerdac/rdac.cpython-38-x86_64-linux-gnu.so
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-24 07:47 pytelerdac/client/__init__.py
--rwxrwxr-x  2.0 unx    91800 b- defN 23-May-04 07:31 pytelerdac/client/http_client.cpython-38-x86_64-linux-gnu.so
+-rwxrwxr-x  2.0 unx    91800 b- defN 23-May-19 07:57 pytelerdac/client/http_client.cpython-38-x86_64-linux-gnu.so
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-24 07:47 pytelerdac/const/__init__.py
--rwxrwxr-x  2.0 unx    28032 b- defN 23-May-04 07:31 pytelerdac/const/public.cpython-38-x86_64-linux-gnu.so
+-rwxrwxr-x  2.0 unx    28032 b- defN 23-May-19 07:57 pytelerdac/const/public.cpython-38-x86_64-linux-gnu.so
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-24 07:49 pytelerdac/utils/__init__.py
--rwxrwxr-x  2.0 unx    40008 b- defN 23-May-04 07:31 pytelerdac/utils/device_utils.cpython-38-x86_64-linux-gnu.so
--rwxrwxr-x  2.0 unx   153112 b- defN 23-May-04 07:31 pytelerdac/utils/license_utils.cpython-38-x86_64-linux-gnu.so
--rw-rw-r--  2.0 unx      531 b- defN 23-May-04 07:31 pytelerdac-0.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      108 b- defN 23-May-04 07:31 pytelerdac-0.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-May-04 07:31 pytelerdac-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1206 b- defN 23-May-04 07:31 pytelerdac-0.2.0.dist-info/RECORD
-13 files, 429584 bytes uncompressed, 157567 bytes compressed:  63.3%
+-rwxrwxr-x  2.0 unx    49824 b- defN 23-May-19 07:57 pytelerdac/utils/device_utils.cpython-38-x86_64-linux-gnu.so
+-rwxrwxr-x  2.0 unx   153112 b- defN 23-May-19 07:57 pytelerdac/utils/license_utils.cpython-38-x86_64-linux-gnu.so
+-rw-rw-r--  2.0 unx      531 b- defN 23-May-19 07:57 pytelerdac-0.3.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      108 b- defN 23-May-19 07:57 pytelerdac-0.3.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-May-19 07:57 pytelerdac-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1206 b- defN 23-May-19 07:57 pytelerdac-0.3.0.dist-info/RECORD
+13 files, 439400 bytes uncompressed, 162349 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: pytelerdac/utils/device_utils.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
 Filename: pytelerdac/utils/license_utils.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
-Filename: pytelerdac-0.2.0.dist-info/METADATA
+Filename: pytelerdac-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: pytelerdac-0.2.0.dist-info/WHEEL
+Filename: pytelerdac-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytelerdac-0.2.0.dist-info/top_level.txt
+Filename: pytelerdac-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pytelerdac-0.2.0.dist-info/RECORD
+Filename: pytelerdac-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytelerdac/utils/device_utils.cpython-38-x86_64-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --file-header {}

```diff
@@ -4,17 +4,17 @@
   Data:                              2's complement, little endian
   Version:                           1 (current)
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
-  Entry point address:               0x2740
+  Entry point address:               0x2760
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          38088 (bytes into file)
+  Start of section headers:          47904 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         11
   Size of section headers:           64 (bytes)
   Number of section headers:         30
   Section header string table index: 29
```

### readelf --wide --program-header {}

```diff
@@ -1,25 +1,25 @@
 
 Elf file type is DYN (Shared object file)
-Entry point 0x2740
+Entry point 0x2760
 There are 11 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
-  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x001cf0 0x001cf0 R   0x1000
-  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x0032c9 0x0032c9 R E 0x1000
-  LOAD           0x006000 0x0000000000006000 0x0000000000006000 0x0007f8 0x0007f8 R   0x1000
-  LOAD           0x006d78 0x0000000000007d78 0x0000000000007d78 0x000908 0x000a90 RW  0x1000
-  DYNAMIC        0x006d88 0x0000000000007d88 0x0000000000007d88 0x0001d0 0x0001d0 RW  0x8
+  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x001f10 0x001f10 R   0x1000
+  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x0053bd 0x0053bd R E 0x1000
+  LOAD           0x008000 0x0000000000008000 0x0000000000008000 0x00098c 0x00098c R   0x1000
+  LOAD           0x008d78 0x0000000000009d78 0x0000000000009d78 0x000aa8 0x000cb0 RW  0x1000
+  DYNAMIC        0x008d88 0x0000000000009d88 0x0000000000009d88 0x0001d0 0x0001d0 RW  0x8
   NOTE           0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
   NOTE           0x0002c8 0x00000000000002c8 0x00000000000002c8 0x000024 0x000024 R   0x4
   GNU_PROPERTY   0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
-  GNU_EH_FRAME   0x0063f0 0x00000000000063f0 0x00000000000063f0 0x00007c 0x00007c R   0x4
+  GNU_EH_FRAME   0x008458 0x0000000000008458 0x0000000000008458 0x00009c 0x00009c R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
-  GNU_RELRO      0x006d78 0x0000000000007d78 0x0000000000007d78 0x000288 0x000288 R   0x1
+  GNU_RELRO      0x008d78 0x0000000000009d78 0x0000000000009d78 0x000288 0x000288 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
    00     .note.gnu.property .note.gnu.build-id .gnu.hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt 
    01     .init .plt .plt.got .plt.sec .text .fini 
    02     .rodata .eh_frame_hdr .eh_frame 
    03     .init_array .fini_array .dynamic .got .got.plt .data .bss
```

### readelf --wide --sections {}

```diff
@@ -1,39 +1,39 @@
-There are 30 section headers, starting at offset 0x94c8:
+There are 30 section headers, starting at offset 0xbb20:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .note.gnu.property NOTE            00000000000002a8 0002a8 000020 00   A  0   0  8
   [ 2] .note.gnu.build-id NOTE            00000000000002c8 0002c8 000024 00   A  0   0  4
   [ 3] .gnu.hash         GNU_HASH        00000000000002f0 0002f0 000028 00   A  4   0  8
-  [ 4] .dynsym           DYNSYM          0000000000000318 000318 000768 18   A  5   1  8
-  [ 5] .dynstr           STRTAB          0000000000000a80 000a80 0005cf 00   A  0   0  1
-  [ 6] .gnu.version      VERSYM          0000000000001050 001050 00009e 02   A  4   0  2
-  [ 7] .gnu.version_r    VERNEED         00000000000010f0 0010f0 000030 00   A  5   1  8
-  [ 8] .rela.dyn         RELA            0000000000001120 001120 000690 18   A  4   0  8
-  [ 9] .rela.plt         RELA            00000000000017b0 0017b0 000540 18  AI  4  23  8
+  [ 4] .dynsym           DYNSYM          0000000000000318 000318 000780 18   A  5   1  8
+  [ 5] .dynstr           STRTAB          0000000000000a98 000a98 0005dd 00   A  0   0  1
+  [ 6] .gnu.version      VERSYM          0000000000001076 001076 0000a0 02   A  4   0  2
+  [ 7] .gnu.version_r    VERNEED         0000000000001118 001118 000030 00   A  5   1  8
+  [ 8] .rela.dyn         RELA            0000000000001148 001148 000870 18   A  4   0  8
+  [ 9] .rela.plt         RELA            00000000000019b8 0019b8 000558 18  AI  4  23  8
   [10] .init             PROGBITS        0000000000002000 002000 00001b 00  AX  0   0  4
-  [11] .plt              PROGBITS        0000000000002020 002020 000390 10  AX  0   0 16
-  [12] .plt.got          PROGBITS        00000000000023b0 0023b0 000010 10  AX  0   0 16
-  [13] .plt.sec          PROGBITS        00000000000023c0 0023c0 000380 10  AX  0   0 16
-  [14] .text             PROGBITS        0000000000002740 002740 002b7c 00  AX  0   0 16
-  [15] .fini             PROGBITS        00000000000052bc 0052bc 00000d 00  AX  0   0  4
-  [16] .rodata           PROGBITS        0000000000006000 006000 0003f0 00   A  0   0 32
-  [17] .eh_frame_hdr     PROGBITS        00000000000063f0 0063f0 00007c 00   A  0   0  4
-  [18] .eh_frame         PROGBITS        0000000000006470 006470 000388 00   A  0   0  8
-  [19] .init_array       INIT_ARRAY      0000000000007d78 006d78 000008 08  WA  0   0  8
-  [20] .fini_array       FINI_ARRAY      0000000000007d80 006d80 000008 08  WA  0   0  8
-  [21] .dynamic          DYNAMIC         0000000000007d88 006d88 0001d0 10  WA  5   0  8
-  [22] .got              PROGBITS        0000000000007f58 006f58 0000a8 08  WA  0   0  8
-  [23] .got.plt          PROGBITS        0000000000008000 007000 0001d8 08  WA  0   0  8
-  [24] .data             PROGBITS        00000000000081e0 0071e0 0004a0 00  WA  0   0 32
-  [25] .bss              NOBITS          0000000000008680 007680 000188 00  WA  0   0 32
-  [26] .comment          PROGBITS        0000000000000000 007680 00002b 01  MS  0   0  1
-  [27] .symtab           SYMTAB          0000000000000000 0076b0 001038 18     28  95  8
-  [28] .strtab           STRTAB          0000000000000000 0086e8 000cd1 00      0   0  1
-  [29] .shstrtab         STRTAB          0000000000000000 0093b9 00010d 00      0   0  1
+  [11] .plt              PROGBITS        0000000000002020 002020 0003a0 10  AX  0   0 16
+  [12] .plt.got          PROGBITS        00000000000023c0 0023c0 000010 10  AX  0   0 16
+  [13] .plt.sec          PROGBITS        00000000000023d0 0023d0 000390 10  AX  0   0 16
+  [14] .text             PROGBITS        0000000000002760 002760 004c4f 00  AX  0   0 16
+  [15] .fini             PROGBITS        00000000000073b0 0073b0 00000d 00  AX  0   0  4
+  [16] .rodata           PROGBITS        0000000000008000 008000 000458 00   A  0   0 32
+  [17] .eh_frame_hdr     PROGBITS        0000000000008458 008458 00009c 00   A  0   0  4
+  [18] .eh_frame         PROGBITS        00000000000084f8 0084f8 000494 00   A  0   0  8
+  [19] .init_array       INIT_ARRAY      0000000000009d78 008d78 000008 08  WA  0   0  8
+  [20] .fini_array       FINI_ARRAY      0000000000009d80 008d80 000008 08  WA  0   0  8
+  [21] .dynamic          DYNAMIC         0000000000009d88 008d88 0001d0 10  WA  5   0  8
+  [22] .got              PROGBITS        0000000000009f58 008f58 0000a8 08  WA  0   0  8
+  [23] .got.plt          PROGBITS        000000000000a000 009000 0001e0 08  WA  0   0  8
+  [24] .data             PROGBITS        000000000000a1e0 0091e0 000640 00  WA  0   0 32
+  [25] .bss              NOBITS          000000000000a820 009820 000208 00  WA  0   0 32
+  [26] .comment          PROGBITS        0000000000000000 009820 00002b 01  MS  0   0  1
+  [27] .symtab           SYMTAB          0000000000000000 009850 0012d8 18     28 122  8
+  [28] .strtab           STRTAB          0000000000000000 00ab28 000ee4 00      0   0  1
+  [29] .shstrtab         STRTAB          0000000000000000 00ba0c 00010d 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

### readelf --wide --symbols {}

```diff
@@ -1,9 +1,9 @@
 
-Symbol table '.dynsym' contains 79 entries:
+Symbol table '.dynsym' contains 80 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_FromFormat
      2: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyList_New
      3: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_SystemError
      4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_SetItemString
      5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyMethod_Type
@@ -46,213 +46,242 @@
     42: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_New
     43: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_Get
     44: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_SetAttr
     45: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Occurred
     46: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyDict_GetItem_KnownHash
     47: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_GetItemString
     48: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyEval_EvalCodeEx
-    49: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_NoneStruct
-    50: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyImport_ImportModuleLevelObject
-    51: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Hash
-    52: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_TrueStruct
-    53: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFunction_Type
-    54: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_New
-    55: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyLong_Type
-    56: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFrame_Type
-    57: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyObject_GetDictPtr
-    58: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_FromString
-    59: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_InternFromString
-    60: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_ImportError
-    61: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_SetItem
-    62: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_AttributeError
-    63: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Call
-    64: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_Decode
-    65: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Format
-    66: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PySlice_New
-    67: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_NameError
-    68: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_FromStringAndSize
-    69: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModule_GetDict
-    70: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-    71: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_GetAttr
-    72: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCFunction_Type
-    73: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyMem_Malloc
-    74: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (3)
-    75: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_Pack
-    76: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND Py_GetVersion
-    77: 00000000000031d8    16 FUNC    GLOBAL DEFAULT   14 PyInit_device_utils
-    78: 00000000000086a0     4 OBJECT  GLOBAL DEFAULT   25 __pyx_module_is_main_pytelerdac__utils__device_utils
+    49: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Size
+    50: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_NoneStruct
+    51: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyImport_ImportModuleLevelObject
+    52: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Hash
+    53: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_TrueStruct
+    54: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFunction_Type
+    55: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_New
+    56: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyLong_Type
+    57: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFrame_Type
+    58: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyObject_GetDictPtr
+    59: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_FromString
+    60: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_InternFromString
+    61: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_ImportError
+    62: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_SetItem
+    63: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_AttributeError
+    64: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Call
+    65: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_Decode
+    66: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Format
+    67: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PySlice_New
+    68: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_NameError
+    69: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_FromStringAndSize
+    70: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModule_GetDict
+    71: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+    72: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_GetAttr
+    73: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCFunction_Type
+    74: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyMem_Malloc
+    75: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (3)
+    76: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_Pack
+    77: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND Py_GetVersion
+    78: 00000000000032c8    16 FUNC    GLOBAL DEFAULT   14 PyInit_device_utils
+    79: 000000000000a840     4 OBJECT  GLOBAL DEFAULT   25 __pyx_module_is_main_pytelerdac__utils__device_utils
 
-Symbol table '.symtab' contains 173 entries:
+Symbol table '.symtab' contains 201 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS device_utils.c
-     2: 00000000000032b0   119 FUNC    LOCAL  DEFAULT   14 __pyx_bisect_code_objects
-     3: 0000000000003330   166 FUNC    LOCAL  DEFAULT   14 __Pyx_PyFunction_FastCallNoKw
-     4: 00000000000087c0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_pyframe_localsplus_offset
-     5: 00000000000033e0  1516 FUNC    LOCAL  DEFAULT   14 __Pyx_AddTraceback
-     6: 00000000000087b0    16 OBJECT  LOCAL  DEFAULT   25 __pyx_code_cache
-     7: 00000000000087f8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_d
-     8: 00000000000087e8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_cython_runtime
-     9: 00000000000086b0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_dict_version.15866
-    10: 00000000000086a8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_dict_cached_value.15867
-    11: 0000000000008798     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_cline_in_traceback
-    12: 00000000000087e0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_empty_tuple
-    13: 00000000000087d8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_empty_bytes
-    14: 0000000000002740   126 FUNC    LOCAL  DEFAULT   14 __Pyx_copy_spec_to_module
-    15: 00000000000027be   356 FUNC    LOCAL  DEFAULT   14 __pyx_pymod_create
-    16: 0000000000008200     8 OBJECT  LOCAL  DEFAULT   24 main_interpreter_id.15670
-    17: 0000000000008800     8 OBJECT  LOCAL  DEFAULT   25 __pyx_m
-    18: 00000000000039d0   357 FUNC    LOCAL  DEFAULT   14 __Pyx_PyFunction_FastCallDict.constprop.0
-    19: 0000000000003b40   116 FUNC    LOCAL  DEFAULT   14 __Pyx_GetBuiltinName
-    20: 00000000000087f0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_b
-    21: 0000000000003bc0   116 FUNC    LOCAL  DEFAULT   14 __Pyx__GetModuleGlobalName
-    22: 0000000000002922  2230 FUNC    LOCAL  DEFAULT   14 __pyx_pymod_exec_device_utils
-    23: 00000000000087d4     4 OBJECT  LOCAL  DEFAULT   25 __pyx_lineno
-    24: 00000000000087c8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_filename
-    25: 00000000000087d0     4 OBJECT  LOCAL  DEFAULT   25 __pyx_clineno
-    26: 0000000000008280   800 OBJECT  LOCAL  DEFAULT   24 __pyx_string_tab
-    27: 0000000000008710     8 OBJECT  LOCAL  DEFAULT   25 __pyx_int_2
-    28: 0000000000008708     8 OBJECT  LOCAL  DEFAULT   25 __pyx_int_neg_12
-    29: 0000000000008750     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_main
-    30: 0000000000008748     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_name
-    31: 0000000000008730     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_range
-    32: 0000000000008700     8 OBJECT  LOCAL  DEFAULT   25 __pyx_slice_
-    33: 0000000000008790     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_e
-    34: 0000000000008758     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_mac
-    35: 0000000000008788     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_get_device_id
-    36: 0000000000008738     8 OBJECT  LOCAL  DEFAULT   25 __pyx_kp_s_pytelerdac_utils_device_utils_py
-    37: 0000000000008718     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_uuid
-    38: 0000000000008740     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_pytelerdac_utils_device_utils
-    39: 0000000000008660    32 OBJECT  LOCAL  DEFAULT   24 __pyx_mdef_10pytelerdac_5utils_12device_utils_1get_device_id
-    40: 0000000000008728     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_test
-    41: 0000000000003c40  5756 FUNC    LOCAL  DEFAULT   14 __pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id
-    42: 00000000000086d0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_dict_version.15592
-    43: 00000000000086c8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_dict_cached_value.15593
-    44: 00000000000087a8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_UUID
-    45: 00000000000086c0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_dict_version.15595
-    46: 00000000000086b8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_dict_cached_value.15596
-    47: 0000000000008780     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_getnode
-    48: 0000000000008768     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_int
-    49: 0000000000008778     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_hex
-    50: 0000000000008720     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_upper
-    51: 00000000000087a0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_kp_s__2
-    52: 00000000000085a0   104 OBJECT  LOCAL  DEFAULT   24 __pyx_moduledef
-    53: 00000000000063ce     5 OBJECT  LOCAL  DEFAULT   16 __pyx_k_UUID
-    54: 00000000000063df     2 OBJECT  LOCAL  DEFAULT   16 __pyx_k__2
-    55: 0000000000006350    19 OBJECT  LOCAL  DEFAULT   16 __pyx_k_cline_in_traceback
-    56: 00000000000063e1     2 OBJECT  LOCAL  DEFAULT   16 __pyx_k_e
-    57: 0000000000006368    14 OBJECT  LOCAL  DEFAULT   16 __pyx_k_get_device_id
-    58: 0000000000006378     8 OBJECT  LOCAL  DEFAULT   16 __pyx_k_getnode
-    59: 00000000000063db     4 OBJECT  LOCAL  DEFAULT   16 __pyx_k_hex
-    60: 0000000000008770     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_import
-    61: 0000000000006380    11 OBJECT  LOCAL  DEFAULT   16 __pyx_k_import
-    62: 00000000000063d7     4 OBJECT  LOCAL  DEFAULT   16 __pyx_k_int
-    63: 0000000000008760     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_join
-    64: 00000000000063c9     5 OBJECT  LOCAL  DEFAULT   16 __pyx_k_join
-    65: 00000000000063d3     4 OBJECT  LOCAL  DEFAULT   16 __pyx_k_mac
-    66: 00000000000063c0     9 OBJECT  LOCAL  DEFAULT   16 __pyx_k_main
-    67: 00000000000063b0     9 OBJECT  LOCAL  DEFAULT   16 __pyx_k_name
-    68: 0000000000006330    30 OBJECT  LOCAL  DEFAULT   16 __pyx_k_pytelerdac_utils_device_utils
-    69: 0000000000006300    34 OBJECT  LOCAL  DEFAULT   16 __pyx_k_pytelerdac_utils_device_utils_py
-    70: 0000000000006391     6 OBJECT  LOCAL  DEFAULT   16 __pyx_k_range
-    71: 00000000000063a0     9 OBJECT  LOCAL  DEFAULT   16 __pyx_k_test
-    72: 000000000000638b     6 OBJECT  LOCAL  DEFAULT   16 __pyx_k_upper
-    73: 0000000000006397     5 OBJECT  LOCAL  DEFAULT   16 __pyx_k_uuid
-    74: 00000000000086e0    32 OBJECT  LOCAL  DEFAULT   25 __pyx_methods
-    75: 0000000000008620    48 OBJECT  LOCAL  DEFAULT   24 __pyx_moduledef_slots
-    76: 0000000000008220    71 OBJECT  LOCAL  DEFAULT   24 __pyx_doc_10pytelerdac_5utils_12device_utils_get_device_id
-    77: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    78: 00000000000031f0     0 FUNC    LOCAL  DEFAULT   14 deregister_tm_clones
-    79: 0000000000003220     0 FUNC    LOCAL  DEFAULT   14 register_tm_clones
-    80: 0000000000003260     0 FUNC    LOCAL  DEFAULT   14 __do_global_dtors_aux
-    81: 0000000000008680     1 OBJECT  LOCAL  DEFAULT   25 completed.8061
-    82: 0000000000007d80     0 OBJECT  LOCAL  DEFAULT   20 __do_global_dtors_aux_fini_array_entry
-    83: 00000000000032a0     0 FUNC    LOCAL  DEFAULT   14 frame_dummy
-    84: 0000000000007d78     0 OBJECT  LOCAL  DEFAULT   19 __frame_dummy_init_array_entry
-    85: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    86: 00000000000067f4     0 OBJECT  LOCAL  DEFAULT   18 __FRAME_END__
-    87: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
-    88: 00000000000052bc     0 FUNC    LOCAL  DEFAULT   15 _fini
-    89: 00000000000081e0     0 OBJECT  LOCAL  DEFAULT   24 __dso_handle
-    90: 0000000000007d88     0 OBJECT  LOCAL  DEFAULT   21 _DYNAMIC
-    91: 00000000000063f0     0 NOTYPE  LOCAL  DEFAULT   17 __GNU_EH_FRAME_HDR
-    92: 0000000000008680     0 OBJECT  LOCAL  DEFAULT   24 __TMC_END__
-    93: 0000000000008000     0 OBJECT  LOCAL  DEFAULT   23 _GLOBAL_OFFSET_TABLE_
-    94: 0000000000002000     0 FUNC    LOCAL  DEFAULT   10 _init
-    95: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_FromFormat
-    96: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyList_New
-    97: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_SystemError
-    98: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_SetItemString
-    99: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyMethod_Type
-   100: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
-   101: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFloat_Type
-   102: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyThreadState_UncheckedGet
-   103: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModuleDef_Init
-   104: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFrame_New
-   105: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCFunction_NewEx
-   106: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyNumber_Add
-   107: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_GetAttrString
-   108: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_Join
-   109: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyImport_AddModule
-   110: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyBytes_FromStringAndSize
-   111: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_SetAttrString
-   112: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_WarnEx
-   113: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_Dealloc
-   114: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModule_NewObject
-   115: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCode_New
-   116: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyImport_GetModuleDict
-   117: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@GLIBC_2.4
-   118: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_RuntimeError
-   119: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_SetString
-   120: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_TypeError
-   121: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyInterpreterState_GetID
-   122: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyEval_EvalFrameEx
-   123: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyMem_Realloc
-   124: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_ExceptionMatches
-   125: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyOS_snprintf
-   126: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTraceBack_Here
-   127: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Not
-   128: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFloat_FromDouble
-   129: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyLong_FromLong
-   130: 00000000000031d8    16 FUNC    GLOBAL DEFAULT   14 PyInit_device_utils
-   131: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Clear
-   132: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyList_Append
-   133: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_CheckRecursiveCall
-   134: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_CheckRecursionLimit
-   135: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_FalseStruct
-   136: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
-   137: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_New
-   138: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_Get
-   139: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_SetAttr
-   140: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Occurred
-   141: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyDict_GetItem_KnownHash
-   142: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_GetItemString
-   143: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyEval_EvalCodeEx
-   144: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_NoneStruct
-   145: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyImport_ImportModuleLevelObject
-   146: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Hash
-   147: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_TrueStruct
-   148: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFunction_Type
-   149: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_New
-   150: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyLong_Type
-   151: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFrame_Type
-   152: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyObject_GetDictPtr
-   153: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_FromString
-   154: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_InternFromString
-   155: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_ImportError
-   156: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_SetItem
-   157: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_AttributeError
-   158: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Call
-   159: 00000000000086a0     4 OBJECT  GLOBAL DEFAULT   25 __pyx_module_is_main_pytelerdac__utils__device_utils
-   160: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_Decode
-   161: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Format
-   162: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PySlice_New
-   163: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_NameError
-   164: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_FromStringAndSize
-   165: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModule_GetDict
-   166: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-   167: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_GetAttr
-   168: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCFunction_Type
-   169: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyMem_Malloc
-   170: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
-   171: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_Pack
-   172: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND Py_GetVersion
+     2: 00000000000033a0   119 FUNC    LOCAL  DEFAULT   14 __pyx_bisect_code_objects
+     3: 0000000000003420   166 FUNC    LOCAL  DEFAULT   14 __Pyx_PyFunction_FastCallNoKw
+     4: 000000000000a9e0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_pyframe_localsplus_offset
+     5: 0000000000002760   126 FUNC    LOCAL  DEFAULT   14 __Pyx_copy_spec_to_module
+     6: 00000000000027de   356 FUNC    LOCAL  DEFAULT   14 __pyx_pymod_create
+     7: 000000000000a200     8 OBJECT  LOCAL  DEFAULT   24 main_interpreter_id.15716
+     8: 000000000000aa20     8 OBJECT  LOCAL  DEFAULT   25 __pyx_m
+     9: 0000000000002942   198 FUNC    LOCAL  DEFAULT   14 __Pyx_Import.constprop.0
+    10: 00000000000034d0   357 FUNC    LOCAL  DEFAULT   14 __Pyx_PyFunction_FastCallDict.constprop.0
+    11: 0000000000003640   116 FUNC    LOCAL  DEFAULT   14 __Pyx_GetBuiltinName
+    12: 000000000000aa10     8 OBJECT  LOCAL  DEFAULT   25 __pyx_b
+    13: 00000000000036c0   116 FUNC    LOCAL  DEFAULT   14 __Pyx__GetModuleGlobalName
+    14: 000000000000aa18     8 OBJECT  LOCAL  DEFAULT   25 __pyx_d
+    15: 0000000000003740   698 FUNC    LOCAL  DEFAULT   14 __Pyx_PyObject_CallOneArg
+    16: 0000000000003a00   591 FUNC    LOCAL  DEFAULT   14 __Pyx_PyObject_Call2Args
+    17: 0000000000003c50  1516 FUNC    LOCAL  DEFAULT   14 __Pyx_AddTraceback
+    18: 000000000000a9d0    16 OBJECT  LOCAL  DEFAULT   25 __pyx_code_cache
+    19: 000000000000aa08     8 OBJECT  LOCAL  DEFAULT   25 __pyx_cython_runtime
+    20: 000000000000a850     8 OBJECT  LOCAL  DEFAULT   25 __pyx_dict_version.15922
+    21: 000000000000a848     8 OBJECT  LOCAL  DEFAULT   25 __pyx_dict_cached_value.15923
+    22: 000000000000a9a8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_cline_in_traceback
+    23: 000000000000aa00     8 OBJECT  LOCAL  DEFAULT   25 __pyx_empty_tuple
+    24: 000000000000a9f8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_empty_bytes
+    25: 0000000000002a08  2240 FUNC    LOCAL  DEFAULT   14 __pyx_pymod_exec_device_utils
+    26: 000000000000a9f4     4 OBJECT  LOCAL  DEFAULT   25 __pyx_lineno
+    27: 000000000000a9e8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_filename
+    28: 000000000000a9f0     4 OBJECT  LOCAL  DEFAULT   25 __pyx_clineno
+    29: 000000000000a280  1200 OBJECT  LOCAL  DEFAULT   24 __pyx_string_tab
+    30: 000000000000a8d8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_int_2
+    31: 000000000000a8d0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_int_neg_12
+    32: 000000000000a950     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_main
+    33: 000000000000a948     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_name
+    34: 000000000000a920     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_range
+    35: 000000000000a9b0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_kp_s__2
+    36: 000000000000a9c0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_kp_s_
+    37: 000000000000a8c0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_tuple__3
+    38: 000000000000a8c8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_slice__4
+    39: 000000000000a998     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_e
+    40: 000000000000a958     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_mac
+    41: 000000000000a908     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_result
+    42: 000000000000a990     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_get_device_id
+    43: 000000000000a928     8 OBJECT  LOCAL  DEFAULT   25 __pyx_kp_s_pytelerdac_utils_device_utils_py
+    44: 000000000000a940     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_os
+    45: 000000000000a8e0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_uuid
+    46: 000000000000a930     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_pytelerdac_utils_device_utils
+    47: 000000000000a800    32 OBJECT  LOCAL  DEFAULT   24 __pyx_mdef_10pytelerdac_5utils_12device_utils_1get_device_id
+    48: 000000000000a8f0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_test
+    49: 0000000000004240   497 FUNC    LOCAL  DEFAULT   14 __Pyx_PyObject_CallNoArg
+    50: 0000000000004440 12143 FUNC    LOCAL  DEFAULT   14 __pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id
+    51: 000000000000a880     8 OBJECT  LOCAL  DEFAULT   25 __pyx_dict_version.15620
+    52: 000000000000a878     8 OBJECT  LOCAL  DEFAULT   25 __pyx_dict_cached_value.15621
+    53: 000000000000a938     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_popen
+    54: 000000000000a978     8 OBJECT  LOCAL  DEFAULT   25 __pyx_kp_s_ifconfig_mlan0_grep_ether_awk_pr
+    55: 000000000000a918     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_read
+    56: 000000000000a8f8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_strip
+    57: 000000000000a9a0     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_close
+    58: 000000000000a900     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_split
+    59: 000000000000a870     8 OBJECT  LOCAL  DEFAULT   25 __pyx_dict_version.15637
+    60: 000000000000a868     8 OBJECT  LOCAL  DEFAULT   25 __pyx_dict_cached_value.15638
+    61: 000000000000a9b8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_UUID
+    62: 000000000000a860     8 OBJECT  LOCAL  DEFAULT   25 __pyx_dict_version.15639
+    63: 000000000000a858     8 OBJECT  LOCAL  DEFAULT   25 __pyx_dict_cached_value.15640
+    64: 000000000000a988     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_getnode
+    65: 000000000000a968     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_int
+    66: 000000000000a980     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_hex
+    67: 000000000000a8e8     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_upper
+    68: 000000000000a910     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_replace
+    69: 000000000000a740   104 OBJECT  LOCAL  DEFAULT   24 __pyx_moduledef
+    70: 000000000000844e     2 OBJECT  LOCAL  DEFAULT   16 __pyx_k_
+    71: 0000000000008436     5 OBJECT  LOCAL  DEFAULT   16 __pyx_k_UUID
+    72: 000000000000844a     2 OBJECT  LOCAL  DEFAULT   16 __pyx_k__2
+    73: 0000000000008390    19 OBJECT  LOCAL  DEFAULT   16 __pyx_k_cline_in_traceback
+    74: 00000000000083f9     6 OBJECT  LOCAL  DEFAULT   16 __pyx_k_close
+    75: 000000000000844c     2 OBJECT  LOCAL  DEFAULT   16 __pyx_k_e
+    76: 00000000000083a8    14 OBJECT  LOCAL  DEFAULT   16 __pyx_k_get_device_id
+    77: 00000000000083c0     8 OBJECT  LOCAL  DEFAULT   16 __pyx_k_getnode
+    78: 0000000000008443     4 OBJECT  LOCAL  DEFAULT   16 __pyx_k_hex
+    79: 0000000000008340    47 OBJECT  LOCAL  DEFAULT   16 __pyx_k_ifconfig_mlan0_grep_ether_awk_pr
+    80: 000000000000a970     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_import
+    81: 00000000000083d0    11 OBJECT  LOCAL  DEFAULT   16 __pyx_k_import
+    82: 000000000000843f     4 OBJECT  LOCAL  DEFAULT   16 __pyx_k_int
+    83: 000000000000a960     8 OBJECT  LOCAL  DEFAULT   25 __pyx_n_s_join
+    84: 0000000000008431     5 OBJECT  LOCAL  DEFAULT   16 __pyx_k_join
+    85: 000000000000843b     4 OBJECT  LOCAL  DEFAULT   16 __pyx_k_mac
+    86: 0000000000008428     9 OBJECT  LOCAL  DEFAULT   16 __pyx_k_main
+    87: 0000000000008418     9 OBJECT  LOCAL  DEFAULT   16 __pyx_k_name
+    88: 0000000000008447     3 OBJECT  LOCAL  DEFAULT   16 __pyx_k_os
+    89: 00000000000083f3     6 OBJECT  LOCAL  DEFAULT   16 __pyx_k_popen
+    90: 0000000000008370    30 OBJECT  LOCAL  DEFAULT   16 __pyx_k_pytelerdac_utils_device_utils
+    91: 0000000000008300    34 OBJECT  LOCAL  DEFAULT   16 __pyx_k_pytelerdac_utils_device_utils_py
+    92: 00000000000083ed     6 OBJECT  LOCAL  DEFAULT   16 __pyx_k_range
+    93: 0000000000008411     5 OBJECT  LOCAL  DEFAULT   16 __pyx_k_read
+    94: 00000000000083b8     8 OBJECT  LOCAL  DEFAULT   16 __pyx_k_replace
+    95: 00000000000083c8     7 OBJECT  LOCAL  DEFAULT   16 __pyx_k_result
+    96: 00000000000083e7     6 OBJECT  LOCAL  DEFAULT   16 __pyx_k_split
+    97: 00000000000083e1     6 OBJECT  LOCAL  DEFAULT   16 __pyx_k_strip
+    98: 0000000000008408     9 OBJECT  LOCAL  DEFAULT   16 __pyx_k_test
+    99: 00000000000083db     6 OBJECT  LOCAL  DEFAULT   16 __pyx_k_upper
+   100: 00000000000083ff     5 OBJECT  LOCAL  DEFAULT   16 __pyx_k_uuid
+   101: 000000000000a8a0    32 OBJECT  LOCAL  DEFAULT   25 __pyx_methods
+   102: 000000000000a7c0    48 OBJECT  LOCAL  DEFAULT   24 __pyx_moduledef_slots
+   103: 000000000000a220    71 OBJECT  LOCAL  DEFAULT   24 __pyx_doc_10pytelerdac_5utils_12device_utils_get_device_id
+   104: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
+   105: 00000000000032e0     0 FUNC    LOCAL  DEFAULT   14 deregister_tm_clones
+   106: 0000000000003310     0 FUNC    LOCAL  DEFAULT   14 register_tm_clones
+   107: 0000000000003350     0 FUNC    LOCAL  DEFAULT   14 __do_global_dtors_aux
+   108: 000000000000a820     1 OBJECT  LOCAL  DEFAULT   25 completed.8061
+   109: 0000000000009d80     0 OBJECT  LOCAL  DEFAULT   20 __do_global_dtors_aux_fini_array_entry
+   110: 0000000000003390     0 FUNC    LOCAL  DEFAULT   14 frame_dummy
+   111: 0000000000009d78     0 OBJECT  LOCAL  DEFAULT   19 __frame_dummy_init_array_entry
+   112: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
+   113: 0000000000008988     0 OBJECT  LOCAL  DEFAULT   18 __FRAME_END__
+   114: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
+   115: 00000000000073b0     0 FUNC    LOCAL  DEFAULT   15 _fini
+   116: 000000000000a1e0     0 OBJECT  LOCAL  DEFAULT   24 __dso_handle
+   117: 0000000000009d88     0 OBJECT  LOCAL  DEFAULT   21 _DYNAMIC
+   118: 0000000000008458     0 NOTYPE  LOCAL  DEFAULT   17 __GNU_EH_FRAME_HDR
+   119: 000000000000a820     0 OBJECT  LOCAL  DEFAULT   24 __TMC_END__
+   120: 000000000000a000     0 OBJECT  LOCAL  DEFAULT   23 _GLOBAL_OFFSET_TABLE_
+   121: 0000000000002000     0 FUNC    LOCAL  DEFAULT   10 _init
+   122: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_FromFormat
+   123: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyList_New
+   124: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_SystemError
+   125: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_SetItemString
+   126: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyMethod_Type
+   127: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
+   128: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFloat_Type
+   129: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyThreadState_UncheckedGet
+   130: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModuleDef_Init
+   131: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFrame_New
+   132: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCFunction_NewEx
+   133: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyNumber_Add
+   134: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_GetAttrString
+   135: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_Join
+   136: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyImport_AddModule
+   137: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyBytes_FromStringAndSize
+   138: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_SetAttrString
+   139: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_WarnEx
+   140: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_Dealloc
+   141: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModule_NewObject
+   142: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCode_New
+   143: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyImport_GetModuleDict
+   144: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@GLIBC_2.4
+   145: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_RuntimeError
+   146: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_SetString
+   147: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_TypeError
+   148: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyInterpreterState_GetID
+   149: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyEval_EvalFrameEx
+   150: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyMem_Realloc
+   151: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_ExceptionMatches
+   152: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyOS_snprintf
+   153: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTraceBack_Here
+   154: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Not
+   155: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFloat_FromDouble
+   156: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyLong_FromLong
+   157: 00000000000032c8    16 FUNC    GLOBAL DEFAULT   14 PyInit_device_utils
+   158: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Clear
+   159: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyList_Append
+   160: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_CheckRecursiveCall
+   161: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_CheckRecursionLimit
+   162: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_FalseStruct
+   163: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
+   164: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_New
+   165: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_Get
+   166: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_SetAttr
+   167: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Occurred
+   168: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyDict_GetItem_KnownHash
+   169: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_GetItemString
+   170: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyEval_EvalCodeEx
+   171: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Size
+   172: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_NoneStruct
+   173: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyImport_ImportModuleLevelObject
+   174: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Hash
+   175: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_TrueStruct
+   176: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFunction_Type
+   177: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_New
+   178: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyLong_Type
+   179: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFrame_Type
+   180: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyObject_GetDictPtr
+   181: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_FromString
+   182: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_InternFromString
+   183: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_ImportError
+   184: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_SetItem
+   185: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_AttributeError
+   186: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Call
+   187: 000000000000a840     4 OBJECT  GLOBAL DEFAULT   25 __pyx_module_is_main_pytelerdac__utils__device_utils
+   188: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_Decode
+   189: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Format
+   190: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PySlice_New
+   191: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_NameError
+   192: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_FromStringAndSize
+   193: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModule_GetDict
+   194: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+   195: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_GetAttr
+   196: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCFunction_Type
+   197: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyMem_Malloc
+   198: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
+   199: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_Pack
+   200: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND Py_GetVersion
```

### readelf --wide --relocs {}

```diff
@@ -1,132 +1,153 @@
 
-Relocation section '.rela.dyn' at offset 0x1120 contains 70 entries:
+Relocation section '.rela.dyn' at offset 0x1148 contains 90 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000007d78  0000000000000008 R_X86_64_RELATIVE                         32a0
-0000000000007d80  0000000000000008 R_X86_64_RELATIVE                         3260
-00000000000081e0  0000000000000008 R_X86_64_RELATIVE                         81e0
-0000000000008280  0000000000000008 R_X86_64_RELATIVE                         87a8
-0000000000008288  0000000000000008 R_X86_64_RELATIVE                         63ce
-00000000000082a8  0000000000000008 R_X86_64_RELATIVE                         87a0
-00000000000082b0  0000000000000008 R_X86_64_RELATIVE                         63df
-00000000000082d0  0000000000000008 R_X86_64_RELATIVE                         8798
-00000000000082d8  0000000000000008 R_X86_64_RELATIVE                         6350
-00000000000082f8  0000000000000008 R_X86_64_RELATIVE                         8790
-0000000000008300  0000000000000008 R_X86_64_RELATIVE                         63e1
-0000000000008320  0000000000000008 R_X86_64_RELATIVE                         8788
-0000000000008328  0000000000000008 R_X86_64_RELATIVE                         6368
-0000000000008348  0000000000000008 R_X86_64_RELATIVE                         8780
-0000000000008350  0000000000000008 R_X86_64_RELATIVE                         6378
-0000000000008370  0000000000000008 R_X86_64_RELATIVE                         8778
-0000000000008378  0000000000000008 R_X86_64_RELATIVE                         63db
-0000000000008398  0000000000000008 R_X86_64_RELATIVE                         8770
-00000000000083a0  0000000000000008 R_X86_64_RELATIVE                         6380
-00000000000083c0  0000000000000008 R_X86_64_RELATIVE                         8768
-00000000000083c8  0000000000000008 R_X86_64_RELATIVE                         63d7
-00000000000083e8  0000000000000008 R_X86_64_RELATIVE                         8760
-00000000000083f0  0000000000000008 R_X86_64_RELATIVE                         63c9
-0000000000008410  0000000000000008 R_X86_64_RELATIVE                         8758
-0000000000008418  0000000000000008 R_X86_64_RELATIVE                         63d3
-0000000000008438  0000000000000008 R_X86_64_RELATIVE                         8750
-0000000000008440  0000000000000008 R_X86_64_RELATIVE                         63c0
-0000000000008460  0000000000000008 R_X86_64_RELATIVE                         8748
-0000000000008468  0000000000000008 R_X86_64_RELATIVE                         63b0
-0000000000008488  0000000000000008 R_X86_64_RELATIVE                         8740
-0000000000008490  0000000000000008 R_X86_64_RELATIVE                         6330
-00000000000084b0  0000000000000008 R_X86_64_RELATIVE                         8738
-00000000000084b8  0000000000000008 R_X86_64_RELATIVE                         6300
-00000000000084d8  0000000000000008 R_X86_64_RELATIVE                         8730
-00000000000084e0  0000000000000008 R_X86_64_RELATIVE                         6391
-0000000000008500  0000000000000008 R_X86_64_RELATIVE                         8728
-0000000000008508  0000000000000008 R_X86_64_RELATIVE                         63a0
-0000000000008528  0000000000000008 R_X86_64_RELATIVE                         8720
-0000000000008530  0000000000000008 R_X86_64_RELATIVE                         638b
-0000000000008550  0000000000000008 R_X86_64_RELATIVE                         8718
-0000000000008558  0000000000000008 R_X86_64_RELATIVE                         6397
-00000000000085c8  0000000000000008 R_X86_64_RELATIVE                         62b0
-00000000000085e0  0000000000000008 R_X86_64_RELATIVE                         86e0
-00000000000085e8  0000000000000008 R_X86_64_RELATIVE                         8620
-0000000000008628  0000000000000008 R_X86_64_RELATIVE                         27be
-0000000000008638  0000000000000008 R_X86_64_RELATIVE                         2922
-0000000000008660  0000000000000008 R_X86_64_RELATIVE                         62e2
-0000000000008668  0000000000000008 R_X86_64_RELATIVE                         3c40
-0000000000008678  0000000000000008 R_X86_64_RELATIVE                         8220
-0000000000007f58  0000000300000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_SystemError + 0
-0000000000007f60  0000000500000006 R_X86_64_GLOB_DAT      0000000000000000 PyMethod_Type + 0
-0000000000007f68  0000000600000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
-0000000000007f70  0000000700000006 R_X86_64_GLOB_DAT      0000000000000000 PyFloat_Type + 0
-0000000000007f78  0000001800000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_RuntimeError + 0
-0000000000007f80  0000001a00000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_TypeError + 0
-0000000000007f88  0000002700000006 R_X86_64_GLOB_DAT      0000000000000000 _Py_CheckRecursionLimit + 0
-0000000000007f90  0000002800000006 R_X86_64_GLOB_DAT      0000000000000000 _Py_FalseStruct + 0
-0000000000007f98  0000002900000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
-0000000000007fa0  0000003100000006 R_X86_64_GLOB_DAT      0000000000000000 _Py_NoneStruct + 0
-0000000000007fa8  0000003400000006 R_X86_64_GLOB_DAT      0000000000000000 _Py_TrueStruct + 0
-0000000000007fb0  0000003500000006 R_X86_64_GLOB_DAT      0000000000000000 PyFunction_Type + 0
-0000000000007fb8  0000003700000006 R_X86_64_GLOB_DAT      0000000000000000 PyLong_Type + 0
-0000000000007fc0  0000003800000006 R_X86_64_GLOB_DAT      0000000000000000 PyFrame_Type + 0
-0000000000007fc8  0000003c00000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_ImportError + 0
-0000000000007fd0  0000003e00000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_AttributeError + 0
-0000000000007fd8  0000004e00000006 R_X86_64_GLOB_DAT      00000000000086a0 __pyx_module_is_main_pytelerdac__utils__device_utils + 0
-0000000000007fe0  0000004300000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_NameError + 0
-0000000000007fe8  0000004600000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
-0000000000007ff0  0000004800000006 R_X86_64_GLOB_DAT      0000000000000000 PyCFunction_Type + 0
-0000000000007ff8  0000004a00000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
+0000000000009d78  0000000000000008 R_X86_64_RELATIVE                         3390
+0000000000009d80  0000000000000008 R_X86_64_RELATIVE                         3350
+000000000000a1e0  0000000000000008 R_X86_64_RELATIVE                         a1e0
+000000000000a280  0000000000000008 R_X86_64_RELATIVE                         a9c0
+000000000000a288  0000000000000008 R_X86_64_RELATIVE                         844e
+000000000000a2a8  0000000000000008 R_X86_64_RELATIVE                         a9b8
+000000000000a2b0  0000000000000008 R_X86_64_RELATIVE                         8436
+000000000000a2d0  0000000000000008 R_X86_64_RELATIVE                         a9b0
+000000000000a2d8  0000000000000008 R_X86_64_RELATIVE                         844a
+000000000000a2f8  0000000000000008 R_X86_64_RELATIVE                         a9a8
+000000000000a300  0000000000000008 R_X86_64_RELATIVE                         8390
+000000000000a320  0000000000000008 R_X86_64_RELATIVE                         a9a0
+000000000000a328  0000000000000008 R_X86_64_RELATIVE                         83f9
+000000000000a348  0000000000000008 R_X86_64_RELATIVE                         a998
+000000000000a350  0000000000000008 R_X86_64_RELATIVE                         844c
+000000000000a370  0000000000000008 R_X86_64_RELATIVE                         a990
+000000000000a378  0000000000000008 R_X86_64_RELATIVE                         83a8
+000000000000a398  0000000000000008 R_X86_64_RELATIVE                         a988
+000000000000a3a0  0000000000000008 R_X86_64_RELATIVE                         83c0
+000000000000a3c0  0000000000000008 R_X86_64_RELATIVE                         a980
+000000000000a3c8  0000000000000008 R_X86_64_RELATIVE                         8443
+000000000000a3e8  0000000000000008 R_X86_64_RELATIVE                         a978
+000000000000a3f0  0000000000000008 R_X86_64_RELATIVE                         8340
+000000000000a410  0000000000000008 R_X86_64_RELATIVE                         a970
+000000000000a418  0000000000000008 R_X86_64_RELATIVE                         83d0
+000000000000a438  0000000000000008 R_X86_64_RELATIVE                         a968
+000000000000a440  0000000000000008 R_X86_64_RELATIVE                         843f
+000000000000a460  0000000000000008 R_X86_64_RELATIVE                         a960
+000000000000a468  0000000000000008 R_X86_64_RELATIVE                         8431
+000000000000a488  0000000000000008 R_X86_64_RELATIVE                         a958
+000000000000a490  0000000000000008 R_X86_64_RELATIVE                         843b
+000000000000a4b0  0000000000000008 R_X86_64_RELATIVE                         a950
+000000000000a4b8  0000000000000008 R_X86_64_RELATIVE                         8428
+000000000000a4d8  0000000000000008 R_X86_64_RELATIVE                         a948
+000000000000a4e0  0000000000000008 R_X86_64_RELATIVE                         8418
+000000000000a500  0000000000000008 R_X86_64_RELATIVE                         a940
+000000000000a508  0000000000000008 R_X86_64_RELATIVE                         8447
+000000000000a528  0000000000000008 R_X86_64_RELATIVE                         a938
+000000000000a530  0000000000000008 R_X86_64_RELATIVE                         83f3
+000000000000a550  0000000000000008 R_X86_64_RELATIVE                         a930
+000000000000a558  0000000000000008 R_X86_64_RELATIVE                         8370
+000000000000a578  0000000000000008 R_X86_64_RELATIVE                         a928
+000000000000a580  0000000000000008 R_X86_64_RELATIVE                         8300
+000000000000a5a0  0000000000000008 R_X86_64_RELATIVE                         a920
+000000000000a5a8  0000000000000008 R_X86_64_RELATIVE                         83ed
+000000000000a5c8  0000000000000008 R_X86_64_RELATIVE                         a918
+000000000000a5d0  0000000000000008 R_X86_64_RELATIVE                         8411
+000000000000a5f0  0000000000000008 R_X86_64_RELATIVE                         a910
+000000000000a5f8  0000000000000008 R_X86_64_RELATIVE                         83b8
+000000000000a618  0000000000000008 R_X86_64_RELATIVE                         a908
+000000000000a620  0000000000000008 R_X86_64_RELATIVE                         83c8
+000000000000a640  0000000000000008 R_X86_64_RELATIVE                         a900
+000000000000a648  0000000000000008 R_X86_64_RELATIVE                         83e7
+000000000000a668  0000000000000008 R_X86_64_RELATIVE                         a8f8
+000000000000a670  0000000000000008 R_X86_64_RELATIVE                         83e1
+000000000000a690  0000000000000008 R_X86_64_RELATIVE                         a8f0
+000000000000a698  0000000000000008 R_X86_64_RELATIVE                         8408
+000000000000a6b8  0000000000000008 R_X86_64_RELATIVE                         a8e8
+000000000000a6c0  0000000000000008 R_X86_64_RELATIVE                         83db
+000000000000a6e0  0000000000000008 R_X86_64_RELATIVE                         a8e0
+000000000000a6e8  0000000000000008 R_X86_64_RELATIVE                         83ff
+000000000000a768  0000000000000008 R_X86_64_RELATIVE                         82b3
+000000000000a780  0000000000000008 R_X86_64_RELATIVE                         a8a0
+000000000000a788  0000000000000008 R_X86_64_RELATIVE                         a7c0
+000000000000a7c8  0000000000000008 R_X86_64_RELATIVE                         27de
+000000000000a7d8  0000000000000008 R_X86_64_RELATIVE                         2a08
+000000000000a800  0000000000000008 R_X86_64_RELATIVE                         82e5
+000000000000a808  0000000000000008 R_X86_64_RELATIVE                         4440
+000000000000a818  0000000000000008 R_X86_64_RELATIVE                         a220
+0000000000009f58  0000000300000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_SystemError + 0
+0000000000009f60  0000000500000006 R_X86_64_GLOB_DAT      0000000000000000 PyMethod_Type + 0
+0000000000009f68  0000000600000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
+0000000000009f70  0000000700000006 R_X86_64_GLOB_DAT      0000000000000000 PyFloat_Type + 0
+0000000000009f78  0000001800000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_RuntimeError + 0
+0000000000009f80  0000001a00000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_TypeError + 0
+0000000000009f88  0000002700000006 R_X86_64_GLOB_DAT      0000000000000000 _Py_CheckRecursionLimit + 0
+0000000000009f90  0000002800000006 R_X86_64_GLOB_DAT      0000000000000000 _Py_FalseStruct + 0
+0000000000009f98  0000002900000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
+0000000000009fa0  0000003200000006 R_X86_64_GLOB_DAT      0000000000000000 _Py_NoneStruct + 0
+0000000000009fa8  0000003500000006 R_X86_64_GLOB_DAT      0000000000000000 _Py_TrueStruct + 0
+0000000000009fb0  0000003600000006 R_X86_64_GLOB_DAT      0000000000000000 PyFunction_Type + 0
+0000000000009fb8  0000003800000006 R_X86_64_GLOB_DAT      0000000000000000 PyLong_Type + 0
+0000000000009fc0  0000003900000006 R_X86_64_GLOB_DAT      0000000000000000 PyFrame_Type + 0
+0000000000009fc8  0000003d00000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_ImportError + 0
+0000000000009fd0  0000003f00000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_AttributeError + 0
+0000000000009fd8  0000004f00000006 R_X86_64_GLOB_DAT      000000000000a840 __pyx_module_is_main_pytelerdac__utils__device_utils + 0
+0000000000009fe0  0000004400000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_NameError + 0
+0000000000009fe8  0000004700000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
+0000000000009ff0  0000004900000006 R_X86_64_GLOB_DAT      0000000000000000 PyCFunction_Type + 0
+0000000000009ff8  0000004b00000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
 
-Relocation section '.rela.plt' at offset 0x17b0 contains 56 entries:
+Relocation section '.rela.plt' at offset 0x19b8 contains 57 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000008018  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_FromFormat + 0
-0000000000008020  0000000200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyList_New + 0
-0000000000008028  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_SetItemString + 0
-0000000000008030  0000000800000007 R_X86_64_JUMP_SLOT     0000000000000000 _PyThreadState_UncheckedGet + 0
-0000000000008038  0000000900000007 R_X86_64_JUMP_SLOT     0000000000000000 PyModuleDef_Init + 0
-0000000000008040  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyFrame_New + 0
-0000000000008048  0000000b00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCFunction_NewEx + 0
-0000000000008050  0000000c00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyNumber_Add + 0
-0000000000008058  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_GetAttrString + 0
-0000000000008060  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_Join + 0
-0000000000008068  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyImport_AddModule + 0
-0000000000008070  0000001000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyBytes_FromStringAndSize + 0
-0000000000008078  0000001100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_SetAttrString + 0
-0000000000008080  0000001200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_WarnEx + 0
-0000000000008088  0000001300000007 R_X86_64_JUMP_SLOT     0000000000000000 _Py_Dealloc + 0
-0000000000008090  0000001400000007 R_X86_64_JUMP_SLOT     0000000000000000 PyModule_NewObject + 0
-0000000000008098  0000001500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCode_New + 0
-00000000000080a0  0000001600000007 R_X86_64_JUMP_SLOT     0000000000000000 PyImport_GetModuleDict + 0
-00000000000080a8  0000001700000007 R_X86_64_JUMP_SLOT     0000000000000000 __stack_chk_fail@GLIBC_2.4 + 0
-00000000000080b0  0000001900000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_SetString + 0
-00000000000080b8  0000001b00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyInterpreterState_GetID + 0
-00000000000080c0  0000001c00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyEval_EvalFrameEx + 0
-00000000000080c8  0000001d00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyMem_Realloc + 0
-00000000000080d0  0000001e00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_ExceptionMatches + 0
-00000000000080d8  0000001f00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyOS_snprintf + 0
-00000000000080e0  0000002000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyTraceBack_Here + 0
-00000000000080e8  0000002100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_Not + 0
-00000000000080f0  0000002200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyFloat_FromDouble + 0
-00000000000080f8  0000002300000007 R_X86_64_JUMP_SLOT     0000000000000000 PyLong_FromLong + 0
-0000000000008100  0000002400000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Clear + 0
-0000000000008108  0000002500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyList_Append + 0
-0000000000008110  0000002600000007 R_X86_64_JUMP_SLOT     0000000000000000 _Py_CheckRecursiveCall + 0
-0000000000008118  0000002a00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyTuple_New + 0
-0000000000008120  0000002b00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyThreadState_Get + 0
-0000000000008128  0000002c00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_SetAttr + 0
-0000000000008130  0000002d00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Occurred + 0
-0000000000008138  0000002e00000007 R_X86_64_JUMP_SLOT     0000000000000000 _PyDict_GetItem_KnownHash + 0
-0000000000008140  0000002f00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_GetItemString + 0
-0000000000008148  0000003000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyEval_EvalCodeEx + 0
-0000000000008150  0000003200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyImport_ImportModuleLevelObject + 0
-0000000000008158  0000003300000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_Hash + 0
-0000000000008160  0000003600000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_New + 0
-0000000000008168  0000003900000007 R_X86_64_JUMP_SLOT     0000000000000000 _PyObject_GetDictPtr + 0
-0000000000008170  0000003a00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_FromString + 0
-0000000000008178  0000003b00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_InternFromString + 0
-0000000000008180  0000003d00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_SetItem + 0
-0000000000008188  0000003f00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_Call + 0
-0000000000008190  0000004000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_Decode + 0
-0000000000008198  0000004100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Format + 0
-00000000000081a0  0000004200000007 R_X86_64_JUMP_SLOT     0000000000000000 PySlice_New + 0
-00000000000081a8  0000004400000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_FromStringAndSize + 0
-00000000000081b0  0000004500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyModule_GetDict + 0
-00000000000081b8  0000004700000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_GetAttr + 0
-00000000000081c0  0000004900000007 R_X86_64_JUMP_SLOT     0000000000000000 PyMem_Malloc + 0
-00000000000081c8  0000004b00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyTuple_Pack + 0
-00000000000081d0  0000004c00000007 R_X86_64_JUMP_SLOT     0000000000000000 Py_GetVersion + 0
+000000000000a018  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_FromFormat + 0
+000000000000a020  0000000200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyList_New + 0
+000000000000a028  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_SetItemString + 0
+000000000000a030  0000000800000007 R_X86_64_JUMP_SLOT     0000000000000000 _PyThreadState_UncheckedGet + 0
+000000000000a038  0000000900000007 R_X86_64_JUMP_SLOT     0000000000000000 PyModuleDef_Init + 0
+000000000000a040  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyFrame_New + 0
+000000000000a048  0000000b00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCFunction_NewEx + 0
+000000000000a050  0000000c00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyNumber_Add + 0
+000000000000a058  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_GetAttrString + 0
+000000000000a060  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_Join + 0
+000000000000a068  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyImport_AddModule + 0
+000000000000a070  0000001000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyBytes_FromStringAndSize + 0
+000000000000a078  0000001100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_SetAttrString + 0
+000000000000a080  0000001200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_WarnEx + 0
+000000000000a088  0000001300000007 R_X86_64_JUMP_SLOT     0000000000000000 _Py_Dealloc + 0
+000000000000a090  0000001400000007 R_X86_64_JUMP_SLOT     0000000000000000 PyModule_NewObject + 0
+000000000000a098  0000001500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCode_New + 0
+000000000000a0a0  0000001600000007 R_X86_64_JUMP_SLOT     0000000000000000 PyImport_GetModuleDict + 0
+000000000000a0a8  0000001700000007 R_X86_64_JUMP_SLOT     0000000000000000 __stack_chk_fail@GLIBC_2.4 + 0
+000000000000a0b0  0000001900000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_SetString + 0
+000000000000a0b8  0000001b00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyInterpreterState_GetID + 0
+000000000000a0c0  0000001c00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyEval_EvalFrameEx + 0
+000000000000a0c8  0000001d00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyMem_Realloc + 0
+000000000000a0d0  0000001e00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_ExceptionMatches + 0
+000000000000a0d8  0000001f00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyOS_snprintf + 0
+000000000000a0e0  0000002000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyTraceBack_Here + 0
+000000000000a0e8  0000002100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_Not + 0
+000000000000a0f0  0000002200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyFloat_FromDouble + 0
+000000000000a0f8  0000002300000007 R_X86_64_JUMP_SLOT     0000000000000000 PyLong_FromLong + 0
+000000000000a100  0000002400000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Clear + 0
+000000000000a108  0000002500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyList_Append + 0
+000000000000a110  0000002600000007 R_X86_64_JUMP_SLOT     0000000000000000 _Py_CheckRecursiveCall + 0
+000000000000a118  0000002a00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyTuple_New + 0
+000000000000a120  0000002b00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyThreadState_Get + 0
+000000000000a128  0000002c00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_SetAttr + 0
+000000000000a130  0000002d00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Occurred + 0
+000000000000a138  0000002e00000007 R_X86_64_JUMP_SLOT     0000000000000000 _PyDict_GetItem_KnownHash + 0
+000000000000a140  0000002f00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_GetItemString + 0
+000000000000a148  0000003000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyEval_EvalCodeEx + 0
+000000000000a150  0000003100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_Size + 0
+000000000000a158  0000003300000007 R_X86_64_JUMP_SLOT     0000000000000000 PyImport_ImportModuleLevelObject + 0
+000000000000a160  0000003400000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_Hash + 0
+000000000000a168  0000003700000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_New + 0
+000000000000a170  0000003a00000007 R_X86_64_JUMP_SLOT     0000000000000000 _PyObject_GetDictPtr + 0
+000000000000a178  0000003b00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_FromString + 0
+000000000000a180  0000003c00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_InternFromString + 0
+000000000000a188  0000003e00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_SetItem + 0
+000000000000a190  0000004000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_Call + 0
+000000000000a198  0000004100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_Decode + 0
+000000000000a1a0  0000004200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Format + 0
+000000000000a1a8  0000004300000007 R_X86_64_JUMP_SLOT     0000000000000000 PySlice_New + 0
+000000000000a1b0  0000004500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_FromStringAndSize + 0
+000000000000a1b8  0000004600000007 R_X86_64_JUMP_SLOT     0000000000000000 PyModule_GetDict + 0
+000000000000a1c0  0000004800000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_GetAttr + 0
+000000000000a1c8  0000004a00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyMem_Malloc + 0
+000000000000a1d0  0000004c00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyTuple_Pack + 0
+000000000000a1d8  0000004d00000007 R_X86_64_JUMP_SLOT     0000000000000000 Py_GetVersion + 0
```

### readelf --wide --dynamic {}

```diff
@@ -1,28 +1,28 @@
 
-Dynamic section at offset 0x6d88 contains 25 entries:
+Dynamic section at offset 0x8d88 contains 25 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x000000000000000f (RPATH)              Library rpath: [/home/imason/anaconda3/envs/backend/lib]
  0x000000000000000c (INIT)               0x2000
- 0x000000000000000d (FINI)               0x52bc
- 0x0000000000000019 (INIT_ARRAY)         0x7d78
+ 0x000000000000000d (FINI)               0x73b0
+ 0x0000000000000019 (INIT_ARRAY)         0x9d78
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
- 0x000000000000001a (FINI_ARRAY)         0x7d80
+ 0x000000000000001a (FINI_ARRAY)         0x9d80
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x2f0
- 0x0000000000000005 (STRTAB)             0xa80
+ 0x0000000000000005 (STRTAB)             0xa98
  0x0000000000000006 (SYMTAB)             0x318
- 0x000000000000000a (STRSZ)              1487 (bytes)
+ 0x000000000000000a (STRSZ)              1501 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
- 0x0000000000000003 (PLTGOT)             0x8000
- 0x0000000000000002 (PLTRELSZ)           1344 (bytes)
+ 0x0000000000000003 (PLTGOT)             0xa000
+ 0x0000000000000002 (PLTRELSZ)           1368 (bytes)
  0x0000000000000014 (PLTREL)             RELA
- 0x0000000000000017 (JMPREL)             0x17b0
- 0x0000000000000007 (RELA)               0x1120
- 0x0000000000000008 (RELASZ)             1680 (bytes)
+ 0x0000000000000017 (JMPREL)             0x19b8
+ 0x0000000000000007 (RELA)               0x1148
+ 0x0000000000000008 (RELASZ)             2160 (bytes)
  0x0000000000000009 (RELAENT)            24 (bytes)
- 0x000000006ffffffe (VERNEED)            0x10f0
+ 0x000000006ffffffe (VERNEED)            0x1118
  0x000000006fffffff (VERNEEDNUM)         1
- 0x000000006ffffff0 (VERSYM)             0x1050
- 0x000000006ffffff9 (RELACOUNT)          49
+ 0x000000006ffffff0 (VERSYM)             0x1076
+ 0x000000006ffffff9 (RELACOUNT)          69
  0x0000000000000000 (NULL)               0x0
```

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 47106a7a74ef7e6168a31eaf1af39867dca0683a
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: a1405a0e79f6fa5635952b242d5071a11e4c0a10
```

### readelf --wide --version-info {}

```diff
@@ -1,10 +1,10 @@
 
-Version symbols section '.gnu.version' contains 79 entries:
- Addr: 0x0000000000001050  Offset: 0x00001050  Link: 4 (.dynsym)
+Version symbols section '.gnu.version' contains 80 entries:
+ Addr: 0x0000000000001076  Offset: 0x00001076  Link: 4 (.dynsym)
   000:   0 (*local*)       0 (*local*)       0 (*local*)       0 (*local*)    
   004:   0 (*local*)       0 (*local*)       0 (*local*)       0 (*local*)    
   008:   0 (*local*)       0 (*local*)       0 (*local*)       0 (*local*)    
   00c:   0 (*local*)       0 (*local*)       0 (*local*)       0 (*local*)    
   010:   0 (*local*)       0 (*local*)       0 (*local*)       0 (*local*)    
   014:   0 (*local*)       0 (*local*)       0 (*local*)       2 (GLIBC_2.4)  
   018:   0 (*local*)       0 (*local*)       0 (*local*)       0 (*local*)    
@@ -15,15 +15,15 @@
   02c:   0 (*local*)       0 (*local*)       0 (*local*)       0 (*local*)    
   030:   0 (*local*)       0 (*local*)       0 (*local*)       0 (*local*)    
   034:   0 (*local*)       0 (*local*)       0 (*local*)       0 (*local*)    
   038:   0 (*local*)       0 (*local*)       0 (*local*)       0 (*local*)    
   03c:   0 (*local*)       0 (*local*)       0 (*local*)       0 (*local*)    
   040:   0 (*local*)       0 (*local*)       0 (*local*)       0 (*local*)    
   044:   0 (*local*)       0 (*local*)       0 (*local*)       0 (*local*)    
-  048:   0 (*local*)       0 (*local*)       3 (GLIBC_2.2.5)   0 (*local*)    
-  04c:   0 (*local*)       1 (*global*)      1 (*global*)   
+  048:   0 (*local*)       0 (*local*)       0 (*local*)       3 (GLIBC_2.2.5)
+  04c:   0 (*local*)       0 (*local*)       1 (*global*)      1 (*global*)   
 
 Version needs section '.gnu.version_r' contains 1 entry:
- Addr: 0x00000000000010f0  Offset: 0x000010f0  Link: 5 (.dynstr)
+ Addr: 0x0000000000001118  Offset: 0x00001118  Link: 5 (.dynstr)
   000000: Version: 1  File: libc.so.6  Cnt: 2
   0x0010:   Name: GLIBC_2.2.5  Flags: none  Version: 3
   0x0020:   Name: GLIBC_2.4  Flags: none  Version: 2
```

### readelf --wide --debug-dump=frames {}

```diff
@@ -9,439 +9,578 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 0000000000000024 0000001c FDE cie=00000000 pc=0000000000002020..00000000000023b0
+00000018 0000000000000024 0000001c FDE cie=00000000 pc=0000000000002020..00000000000023c0
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 6 to 0000000000002026
   DW_CFA_def_cfa_offset: 24
   DW_CFA_advance_loc: 10 to 0000000000002030
   DW_CFA_def_cfa_expression (DW_OP_breg7 (rsp): 8; DW_OP_breg16 (rip): 0; DW_OP_lit15; DW_OP_and; DW_OP_lit10; DW_OP_ge; DW_OP_lit3; DW_OP_shl; DW_OP_plus)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000040 0000000000000014 00000044 FDE cie=00000000 pc=00000000000023b0..00000000000023c0
+00000040 0000000000000014 00000044 FDE cie=00000000 pc=00000000000023c0..00000000000023d0
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000058 0000000000000014 0000005c FDE cie=00000000 pc=00000000000023c0..0000000000002740
+00000058 0000000000000014 0000005c FDE cie=00000000 pc=00000000000023d0..0000000000002760
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000070 0000000000000010 00000074 FDE cie=00000000 pc=00000000000032b0..0000000000003327
+00000070 0000000000000010 00000074 FDE cie=00000000 pc=00000000000033a0..0000000000003417
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000084 000000000000003c 00000088 FDE cie=00000000 pc=0000000000003330..00000000000033d6
-  DW_CFA_advance_loc: 2 to 0000000000003332
+00000084 000000000000003c 00000088 FDE cie=00000000 pc=0000000000003420..00000000000034c6
+  DW_CFA_advance_loc: 2 to 0000000000003422
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 5 to 0000000000003337
+  DW_CFA_advance_loc: 5 to 0000000000003427
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000003339
+  DW_CFA_advance_loc: 2 to 0000000000003429
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 4 to 000000000000333d
+  DW_CFA_advance_loc: 4 to 000000000000342d
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 4 to 0000000000003341
+  DW_CFA_advance_loc: 4 to 0000000000003431
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc1: 113 to 00000000000033b2
+  DW_CFA_advance_loc1: 113 to 00000000000034a2
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 4 to 00000000000033b6
+  DW_CFA_advance_loc: 4 to 00000000000034a6
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000033b8
+  DW_CFA_advance_loc: 2 to 00000000000034a8
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000033ba
+  DW_CFA_advance_loc: 2 to 00000000000034aa
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000033bc
+  DW_CFA_advance_loc: 2 to 00000000000034ac
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 4 to 00000000000033c0
+  DW_CFA_advance_loc: 4 to 00000000000034b0
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000000c4 000000000000008c 000000c8 FDE cie=00000000 pc=00000000000033e0..00000000000039cc
-  DW_CFA_advance_loc: 2 to 00000000000033e2
+000000c4 0000000000000038 000000c8 FDE cie=00000000 pc=0000000000002760..00000000000027de
+  DW_CFA_advance_loc: 2 to 0000000000002762
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 00000000000033e4
+  DW_CFA_offset: r14 (r14) at cfa-16
+  DW_CFA_advance_loc: 5 to 0000000000002767
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 00000000000033e6
+  DW_CFA_offset: r13 (r13) at cfa-24
+  DW_CFA_advance_loc: 8 to 000000000000276f
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 5 to 00000000000033eb
-  DW_CFA_def_cfa_offset: 40
-  DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 4 to 00000000000033ef
-  DW_CFA_def_cfa_offset: 48
-  DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 00000000000033f3
-  DW_CFA_def_cfa_offset: 56
-  DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 6 to 00000000000033f9
-  DW_CFA_def_cfa_offset: 96
-  DW_CFA_advance_loc1: 165 to 000000000000349e
-  DW_CFA_remember_state
-  DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 000000000000349f
-  DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000034a0
+  DW_CFA_offset: r12 (r12) at cfa-32
+  DW_CFA_advance_loc: 1 to 0000000000002770
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000034a2
-  DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000034a4
-  DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000034a6
-  DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000034a8
-  DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 00000000000034b0
-  DW_CFA_restore_state
-  DW_CFA_advance_loc: 22 to 00000000000034c6
-  DW_CFA_remember_state
-  DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 00000000000034c7
+  DW_CFA_offset: r6 (rbp) at cfa-40
+  DW_CFA_advance_loc: 1 to 0000000000002771
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000034c8
+  DW_CFA_offset: r3 (rbx) at cfa-48
+  DW_CFA_advance_loc1: 98 to 00000000000027d3
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000034ca
+  DW_CFA_advance_loc: 4 to 00000000000027d7
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000034cc
+  DW_CFA_advance_loc: 2 to 00000000000027d9
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000034ce
+  DW_CFA_advance_loc: 2 to 00000000000027db
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000034d0
+  DW_CFA_advance_loc: 2 to 00000000000027dd
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 00000000000034d8
-  DW_CFA_restore_state
-  DW_CFA_advance_loc2: 375 to 000000000000364f
-  DW_CFA_def_cfa_offset: 104
-  DW_CFA_advance_loc: 20 to 0000000000003663
-  DW_CFA_def_cfa_offset: 112
-  DW_CFA_advance_loc: 1 to 0000000000003664
-  DW_CFA_def_cfa_offset: 120
-  DW_CFA_advance_loc: 2 to 0000000000003666
-  DW_CFA_def_cfa_offset: 128
-  DW_CFA_advance_loc: 1 to 0000000000003667
-  DW_CFA_def_cfa_offset: 136
-  DW_CFA_advance_loc: 1 to 0000000000003668
-  DW_CFA_def_cfa_offset: 144
-  DW_CFA_advance_loc: 1 to 0000000000003669
-  DW_CFA_def_cfa_offset: 152
-  DW_CFA_advance_loc: 1 to 000000000000366a
-  DW_CFA_def_cfa_offset: 160
-  DW_CFA_advance_loc: 1 to 000000000000366b
-  DW_CFA_def_cfa_offset: 168
-  DW_CFA_advance_loc: 1 to 000000000000366c
-  DW_CFA_def_cfa_offset: 176
-  DW_CFA_advance_loc: 9 to 0000000000003675
-  DW_CFA_def_cfa_offset: 96
-  DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000154 0000000000000038 00000158 FDE cie=00000000 pc=0000000000002740..00000000000027be
-  DW_CFA_advance_loc: 2 to 0000000000002742
+00000100 0000000000000038 00000104 FDE cie=00000000 pc=00000000000027de..0000000000002942
+  DW_CFA_advance_loc: 6 to 00000000000027e4
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 5 to 0000000000002747
+  DW_CFA_advance_loc: 2 to 00000000000027e6
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 8 to 000000000000274f
+  DW_CFA_advance_loc: 5 to 00000000000027eb
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 1 to 0000000000002750
+  DW_CFA_advance_loc: 1 to 00000000000027ec
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000002751
+  DW_CFA_advance_loc: 1 to 00000000000027ed
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_offset: r3 (rbx) at cfa-48
-  DW_CFA_advance_loc1: 98 to 00000000000027b3
+  DW_CFA_advance_loc2: 330 to 0000000000002937
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 4 to 00000000000027b7
+  DW_CFA_advance_loc: 4 to 000000000000293b
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000027b9
+  DW_CFA_advance_loc: 2 to 000000000000293d
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000027bb
+  DW_CFA_advance_loc: 2 to 000000000000293f
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000027bd
+  DW_CFA_advance_loc: 2 to 0000000000002941
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
+  DW_CFA_nop
 
-00000190 0000000000000038 00000194 FDE cie=00000000 pc=00000000000027be..0000000000002922
-  DW_CFA_advance_loc: 6 to 00000000000027c4
+0000013c 0000000000000038 00000140 FDE cie=00000000 pc=0000000000002942..0000000000002a08
+  DW_CFA_advance_loc: 2 to 0000000000002944
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc: 2 to 00000000000027c6
+  DW_CFA_offset: r15 (r15) at cfa-16
+  DW_CFA_advance_loc: 7 to 000000000000294b
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_offset: r13 (r13) at cfa-24
-  DW_CFA_advance_loc: 5 to 00000000000027cb
+  DW_CFA_offset: r14 (r14) at cfa-24
+  DW_CFA_advance_loc: 2 to 000000000000294d
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_offset: r12 (r12) at cfa-32
-  DW_CFA_advance_loc: 1 to 00000000000027cc
+  DW_CFA_offset: r13 (r13) at cfa-32
+  DW_CFA_advance_loc: 2 to 000000000000294f
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_offset: r6 (rbp) at cfa-40
-  DW_CFA_advance_loc: 1 to 00000000000027cd
+  DW_CFA_offset: r12 (r12) at cfa-40
+  DW_CFA_advance_loc: 4 to 0000000000002953
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc2: 330 to 0000000000002917
+  DW_CFA_offset: r6 (rbp) at cfa-48
+  DW_CFA_advance_loc1: 169 to 00000000000029fc
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 4 to 000000000000291b
+  DW_CFA_advance_loc: 5 to 0000000000002a01
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000291d
+  DW_CFA_advance_loc: 2 to 0000000000002a03
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000291f
+  DW_CFA_advance_loc: 2 to 0000000000002a05
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000002921
+  DW_CFA_advance_loc: 2 to 0000000000002a07
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
-  DW_CFA_nop
 
-000001cc 000000000000005c 000001d0 FDE cie=00000000 pc=00000000000039d0..0000000000003b35
-  DW_CFA_advance_loc: 2 to 00000000000039d2
+00000178 000000000000005c 0000017c FDE cie=00000000 pc=00000000000034d0..0000000000003635
+  DW_CFA_advance_loc: 2 to 00000000000034d2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 00000000000039d4
+  DW_CFA_advance_loc: 2 to 00000000000034d4
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 00000000000039d6
+  DW_CFA_advance_loc: 2 to 00000000000034d6
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 00000000000039d8
+  DW_CFA_advance_loc: 2 to 00000000000034d8
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 4 to 00000000000039dc
+  DW_CFA_advance_loc: 4 to 00000000000034dc
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 3 to 00000000000039df
+  DW_CFA_advance_loc: 3 to 00000000000034df
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 00000000000039e6
+  DW_CFA_advance_loc: 7 to 00000000000034e6
   DW_CFA_def_cfa_offset: 64
-  DW_CFA_advance_loc1: 87 to 0000000000003a3d
+  DW_CFA_advance_loc1: 87 to 000000000000353d
   DW_CFA_def_cfa_offset: 72
-  DW_CFA_advance_loc: 10 to 0000000000003a47
+  DW_CFA_advance_loc: 10 to 0000000000003547
   DW_CFA_def_cfa_offset: 80
-  DW_CFA_advance_loc: 7 to 0000000000003a4e
+  DW_CFA_advance_loc: 7 to 000000000000354e
   DW_CFA_def_cfa_offset: 88
-  DW_CFA_advance_loc: 3 to 0000000000003a51
+  DW_CFA_advance_loc: 3 to 0000000000003551
   DW_CFA_def_cfa_offset: 96
-  DW_CFA_advance_loc: 2 to 0000000000003a53
+  DW_CFA_advance_loc: 2 to 0000000000003553
   DW_CFA_def_cfa_offset: 104
-  DW_CFA_advance_loc: 2 to 0000000000003a55
+  DW_CFA_advance_loc: 2 to 0000000000003555
   DW_CFA_def_cfa_offset: 112
-  DW_CFA_advance_loc: 9 to 0000000000003a5e
+  DW_CFA_advance_loc: 9 to 000000000000355e
   DW_CFA_def_cfa_offset: 64
-  DW_CFA_advance_loc: 47 to 0000000000003a8d
+  DW_CFA_advance_loc: 47 to 000000000000358d
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 0000000000003a91
+  DW_CFA_advance_loc: 4 to 0000000000003591
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000003a92
+  DW_CFA_advance_loc: 1 to 0000000000003592
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000003a94
+  DW_CFA_advance_loc: 2 to 0000000000003594
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000003a96
+  DW_CFA_advance_loc: 2 to 0000000000003596
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000003a98
+  DW_CFA_advance_loc: 2 to 0000000000003598
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000003a9a
+  DW_CFA_advance_loc: 2 to 000000000000359a
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 6 to 0000000000003aa0
+  DW_CFA_advance_loc: 6 to 00000000000035a0
   DW_CFA_restore_state
 
-0000022c 0000000000000030 00000230 FDE cie=00000000 pc=0000000000003b40..0000000000003bb4
-  DW_CFA_advance_loc: 2 to 0000000000003b42
+000001d8 0000000000000030 000001dc FDE cie=00000000 pc=0000000000003640..00000000000036b4
+  DW_CFA_advance_loc: 2 to 0000000000003642
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 5 to 0000000000003b47
+  DW_CFA_advance_loc: 5 to 0000000000003647
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 7 to 0000000000003b4e
+  DW_CFA_advance_loc: 7 to 000000000000364e
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 37 to 0000000000003b73
+  DW_CFA_advance_loc: 37 to 0000000000003673
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 5 to 0000000000003b78
+  DW_CFA_advance_loc: 5 to 0000000000003678
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000003b7a
+  DW_CFA_advance_loc: 2 to 000000000000367a
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 6 to 0000000000003b80
+  DW_CFA_advance_loc: 6 to 0000000000003680
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 44 to 0000000000003bac
+  DW_CFA_advance_loc: 44 to 00000000000036ac
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 5 to 0000000000003bb1
+  DW_CFA_advance_loc: 5 to 00000000000036b1
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000003bb3
+  DW_CFA_advance_loc: 2 to 00000000000036b3
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
 
-00000260 0000000000000048 00000264 FDE cie=00000000 pc=0000000000003bc0..0000000000003c34
-  DW_CFA_advance_loc: 2 to 0000000000003bc2
+0000020c 0000000000000048 00000210 FDE cie=00000000 pc=00000000000036c0..0000000000003734
+  DW_CFA_advance_loc: 2 to 00000000000036c2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r13 (r13) at cfa-16
-  DW_CFA_advance_loc: 8 to 0000000000003bca
+  DW_CFA_advance_loc: 8 to 00000000000036ca
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r12 (r12) at cfa-24
-  DW_CFA_advance_loc: 1 to 0000000000003bcb
+  DW_CFA_advance_loc: 1 to 00000000000036cb
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r6 (rbp) at cfa-32
-  DW_CFA_advance_loc: 4 to 0000000000003bcf
+  DW_CFA_advance_loc: 4 to 00000000000036cf
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r3 (rbx) at cfa-40
-  DW_CFA_advance_loc: 7 to 0000000000003bd6
+  DW_CFA_advance_loc: 7 to 00000000000036d6
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 51 to 0000000000003c09
+  DW_CFA_advance_loc: 51 to 0000000000003709
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 4 to 0000000000003c0d
+  DW_CFA_advance_loc: 4 to 000000000000370d
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 0000000000003c0e
+  DW_CFA_advance_loc: 1 to 000000000000370e
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000003c10
+  DW_CFA_advance_loc: 2 to 0000000000003710
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000003c12
+  DW_CFA_advance_loc: 2 to 0000000000003712
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 6 to 0000000000003c18
+  DW_CFA_advance_loc: 6 to 0000000000003718
   DW_CFA_restore_state
-  DW_CFA_advance_loc: 14 to 0000000000003c26
+  DW_CFA_advance_loc: 14 to 0000000000003726
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 4 to 0000000000003c2a
+  DW_CFA_advance_loc: 4 to 000000000000372a
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 1 to 0000000000003c2b
+  DW_CFA_advance_loc: 1 to 000000000000372b
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000003c2d
+  DW_CFA_advance_loc: 2 to 000000000000372d
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000003c2f
+  DW_CFA_advance_loc: 2 to 000000000000372f
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000002ac 0000000000000074 000002b0 FDE cie=00000000 pc=0000000000002922..00000000000031d8
-  DW_CFA_advance_loc: 6 to 0000000000002928
+00000258 0000000000000040 0000025c FDE cie=00000000 pc=0000000000003740..00000000000039fa
+  DW_CFA_advance_loc: 2 to 0000000000003742
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r14 (r14) at cfa-16
+  DW_CFA_advance_loc: 2 to 0000000000003744
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_offset: r13 (r13) at cfa-24
+  DW_CFA_advance_loc: 2 to 0000000000003746
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_offset: r12 (r12) at cfa-32
+  DW_CFA_advance_loc: 1 to 0000000000003747
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_offset: r6 (rbp) at cfa-40
+  DW_CFA_advance_loc: 4 to 000000000000374b
+  DW_CFA_def_cfa_offset: 48
+  DW_CFA_offset: r3 (rbx) at cfa-48
+  DW_CFA_advance_loc: 4 to 000000000000374f
+  DW_CFA_def_cfa_offset: 64
+  DW_CFA_advance_loc1: 150 to 00000000000037e5
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 48
+  DW_CFA_advance_loc: 4 to 00000000000037e9
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 1 to 00000000000037ea
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 2 to 00000000000037ec
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 00000000000037ee
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 00000000000037f0
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 8 to 00000000000037f8
+  DW_CFA_restore_state
+  DW_CFA_nop
+
+0000029c 0000000000000038 000002a0 FDE cie=00000000 pc=0000000000003a00..0000000000003c4f
+  DW_CFA_advance_loc: 2 to 0000000000003a02
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r13 (r13) at cfa-16
+  DW_CFA_advance_loc: 5 to 0000000000003a07
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_offset: r12 (r12) at cfa-24
+  DW_CFA_advance_loc: 1 to 0000000000003a08
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_offset: r6 (rbp) at cfa-32
+  DW_CFA_advance_loc: 4 to 0000000000003a0c
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_offset: r3 (rbx) at cfa-40
+  DW_CFA_advance_loc: 7 to 0000000000003a13
+  DW_CFA_def_cfa_offset: 80
+  DW_CFA_advance_loc1: 246 to 0000000000003b09
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 4 to 0000000000003b0d
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 1 to 0000000000003b0e
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 0000000000003b10
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 0000000000003b12
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 6 to 0000000000003b18
+  DW_CFA_restore_state
+  DW_CFA_nop
+
+000002d8 000000000000008c 000002dc FDE cie=00000000 pc=0000000000003c50..000000000000423c
+  DW_CFA_advance_loc: 2 to 0000000000003c52
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 000000000000292a
+  DW_CFA_advance_loc: 2 to 0000000000003c54
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 000000000000292c
+  DW_CFA_advance_loc: 2 to 0000000000003c56
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 000000000000292e
+  DW_CFA_advance_loc: 5 to 0000000000003c5b
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 000000000000292f
+  DW_CFA_advance_loc: 4 to 0000000000003c5f
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 0000000000002933
+  DW_CFA_advance_loc: 4 to 0000000000003c63
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 000000000000293a
+  DW_CFA_advance_loc: 6 to 0000000000003c69
+  DW_CFA_def_cfa_offset: 96
+  DW_CFA_advance_loc1: 165 to 0000000000003d0e
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 56
+  DW_CFA_advance_loc: 1 to 0000000000003d0f
+  DW_CFA_def_cfa_offset: 48
+  DW_CFA_advance_loc: 1 to 0000000000003d10
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 2 to 0000000000003d12
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 2 to 0000000000003d14
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 0000000000003d16
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 0000000000003d18
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 8 to 0000000000003d20
+  DW_CFA_restore_state
+  DW_CFA_advance_loc: 22 to 0000000000003d36
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 56
+  DW_CFA_advance_loc: 1 to 0000000000003d37
+  DW_CFA_def_cfa_offset: 48
+  DW_CFA_advance_loc: 1 to 0000000000003d38
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 2 to 0000000000003d3a
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 2 to 0000000000003d3c
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 0000000000003d3e
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 0000000000003d40
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 8 to 0000000000003d48
+  DW_CFA_restore_state
+  DW_CFA_advance_loc2: 375 to 0000000000003ebf
+  DW_CFA_def_cfa_offset: 104
+  DW_CFA_advance_loc: 20 to 0000000000003ed3
+  DW_CFA_def_cfa_offset: 112
+  DW_CFA_advance_loc: 1 to 0000000000003ed4
+  DW_CFA_def_cfa_offset: 120
+  DW_CFA_advance_loc: 2 to 0000000000003ed6
+  DW_CFA_def_cfa_offset: 128
+  DW_CFA_advance_loc: 1 to 0000000000003ed7
+  DW_CFA_def_cfa_offset: 136
+  DW_CFA_advance_loc: 1 to 0000000000003ed8
+  DW_CFA_def_cfa_offset: 144
+  DW_CFA_advance_loc: 1 to 0000000000003ed9
+  DW_CFA_def_cfa_offset: 152
+  DW_CFA_advance_loc: 1 to 0000000000003eda
+  DW_CFA_def_cfa_offset: 160
+  DW_CFA_advance_loc: 1 to 0000000000003edb
+  DW_CFA_def_cfa_offset: 168
+  DW_CFA_advance_loc: 1 to 0000000000003edc
+  DW_CFA_def_cfa_offset: 176
+  DW_CFA_advance_loc: 9 to 0000000000003ee5
+  DW_CFA_def_cfa_offset: 96
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+
+00000368 0000000000000064 0000036c FDE cie=00000000 pc=0000000000002a08..00000000000032c8
+  DW_CFA_advance_loc: 6 to 0000000000002a0e
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r13 (r13) at cfa-16
+  DW_CFA_advance_loc: 2 to 0000000000002a10
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_offset: r12 (r12) at cfa-24
+  DW_CFA_advance_loc: 1 to 0000000000002a11
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_offset: r6 (rbp) at cfa-32
+  DW_CFA_advance_loc: 4 to 0000000000002a15
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_offset: r3 (rbx) at cfa-40
+  DW_CFA_advance_loc: 7 to 0000000000002a1c
+  DW_CFA_def_cfa_offset: 272
+  DW_CFA_advance_loc2: 1508 to 0000000000003000
+  DW_CFA_def_cfa_offset: 280
+  DW_CFA_advance_loc: 14 to 000000000000300e
   DW_CFA_def_cfa_offset: 288
-  DW_CFA_advance_loc2: 1468 to 0000000000002ef6
+  DW_CFA_advance_loc: 2 to 0000000000003010
   DW_CFA_def_cfa_offset: 296
-  DW_CFA_advance_loc: 14 to 0000000000002f04
+  DW_CFA_advance_loc: 6 to 0000000000003016
   DW_CFA_def_cfa_offset: 304
-  DW_CFA_advance_loc: 2 to 0000000000002f06
+  DW_CFA_advance_loc: 6 to 000000000000301c
   DW_CFA_def_cfa_offset: 312
-  DW_CFA_advance_loc: 6 to 0000000000002f0c
+  DW_CFA_advance_loc: 1 to 000000000000301d
   DW_CFA_def_cfa_offset: 320
-  DW_CFA_advance_loc: 6 to 0000000000002f12
+  DW_CFA_advance_loc: 1 to 000000000000301e
   DW_CFA_def_cfa_offset: 328
-  DW_CFA_advance_loc: 1 to 0000000000002f13
+  DW_CFA_advance_loc: 1 to 000000000000301f
   DW_CFA_def_cfa_offset: 336
-  DW_CFA_advance_loc: 1 to 0000000000002f14
+  DW_CFA_advance_loc: 1 to 0000000000003020
   DW_CFA_def_cfa_offset: 344
-  DW_CFA_advance_loc: 1 to 0000000000002f15
+  DW_CFA_advance_loc: 1 to 0000000000003021
   DW_CFA_def_cfa_offset: 352
-  DW_CFA_advance_loc: 1 to 0000000000002f16
-  DW_CFA_def_cfa_offset: 360
-  DW_CFA_advance_loc: 1 to 0000000000002f17
-  DW_CFA_def_cfa_offset: 368
-  DW_CFA_advance_loc: 14 to 0000000000002f25
-  DW_CFA_def_cfa_offset: 288
-  DW_CFA_advance_loc2: 680 to 00000000000031cd
-  DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 00000000000031ce
+  DW_CFA_advance_loc: 14 to 000000000000302f
+  DW_CFA_def_cfa_offset: 272
+  DW_CFA_advance_loc2: 658 to 00000000000032c1
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 1 to 00000000000032c2
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 1 to 00000000000032c3
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 00000000000032c5
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 00000000000032c7
+  DW_CFA_def_cfa_offset: 8
+
+000003d0 000000000000005c 000003d4 FDE cie=00000000 pc=0000000000004240..0000000000004431
+  DW_CFA_advance_loc: 2 to 0000000000004242
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r13 (r13) at cfa-16
+  DW_CFA_advance_loc: 2 to 0000000000004244
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_offset: r12 (r12) at cfa-24
+  DW_CFA_advance_loc: 1 to 0000000000004245
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_offset: r6 (rbp) at cfa-32
+  DW_CFA_advance_loc: 4 to 0000000000004249
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_offset: r3 (rbx) at cfa-40
+  DW_CFA_advance_loc: 4 to 000000000000424d
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000031cf
+  DW_CFA_advance_loc1: 146 to 00000000000042df
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 4 to 00000000000042e3
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 1 to 00000000000042e4
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 00000000000042e6
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 00000000000042e8
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 8 to 00000000000042f0
+  DW_CFA_restore_state
+  DW_CFA_advance_loc1: 164 to 0000000000004394
+  DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000031d1
+  DW_CFA_advance_loc: 5 to 0000000000004399
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000031d3
+  DW_CFA_advance_loc: 1 to 000000000000439a
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000031d5
+  DW_CFA_advance_loc: 2 to 000000000000439c
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000031d7
+  DW_CFA_advance_loc: 2 to 000000000000439e
   DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 10 to 00000000000043a8
+  DW_CFA_restore_state
+  DW_CFA_advance_loc: 60 to 00000000000043e4
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 9 to 00000000000043ed
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 1 to 00000000000043ee
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 00000000000043f0
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 00000000000043f2
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 14 to 0000000000004400
+  DW_CFA_restore_state
 
-00000324 0000000000000048 00000328 FDE cie=00000000 pc=0000000000003c40..00000000000052bc
-  DW_CFA_advance_loc: 6 to 0000000000003c46
+00000430 0000000000000048 00000434 FDE cie=00000000 pc=0000000000004440..00000000000073af
+  DW_CFA_advance_loc: 6 to 0000000000004446
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000003c48
+  DW_CFA_advance_loc: 2 to 0000000000004448
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000003c4a
+  DW_CFA_advance_loc: 2 to 000000000000444a
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 0000000000003c4c
+  DW_CFA_advance_loc: 2 to 000000000000444c
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000003c4d
+  DW_CFA_advance_loc: 1 to 000000000000444d
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 0000000000003c4e
+  DW_CFA_advance_loc: 1 to 000000000000444e
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 4 to 0000000000003c52
-  DW_CFA_def_cfa_offset: 96
-  DW_CFA_advance_loc2: 2208 to 00000000000044f2
+  DW_CFA_advance_loc: 4 to 0000000000004452
+  DW_CFA_def_cfa_offset: 112
+  DW_CFA_advance_loc2: 3206 to 00000000000050d8
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 00000000000044f6
+  DW_CFA_advance_loc: 4 to 00000000000050dc
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000044f7
+  DW_CFA_advance_loc: 1 to 00000000000050dd
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000044f9
+  DW_CFA_advance_loc: 2 to 00000000000050df
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000044fb
+  DW_CFA_advance_loc: 2 to 00000000000050e1
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000044fd
+  DW_CFA_advance_loc: 2 to 00000000000050e3
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 00000000000044ff
+  DW_CFA_advance_loc: 2 to 00000000000050e5
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000004500
+  DW_CFA_advance_loc: 11 to 00000000000050f0
   DW_CFA_restore_state
 
-00000370 0000000000000010 00000374 FDE cie=00000000 pc=00000000000031d8..00000000000031e8
+0000047c 0000000000000010 00000480 FDE cie=00000000 pc=00000000000032c8..00000000000032d8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000384 ZERO terminator
+00000490 ZERO terminator
```

### strings --all --bytes=8 {}

```diff
@@ -2,196 +2,227 @@
 _ITM_deregisterTMCloneTable
 _ITM_registerTMCloneTable
 __cxa_finalize
 _PyThreadState_UncheckedGet
 PyFrame_New
 PyEval_EvalFrameEx
 _Py_Dealloc
-PyTraceBack_Here
-_PyObject_GetDictPtr
-_Py_FalseStruct
-_Py_TrueStruct
-PyObject_Not
-PyErr_Clear
-PyObject_SetAttr
-PyUnicode_FromString
-PyUnicode_FromFormat
-PyCode_New
-PyMem_Realloc
-_PyDict_GetItem_KnownHash
-PyMem_Malloc
-PyObject_GetAttr
 PyObject_GetAttrString
 _Py_NoneStruct
 PyDict_SetItemString
 PyExc_AttributeError
 PyErr_ExceptionMatches
+PyErr_Clear
 PyThreadState_Get
 PyInterpreterState_GetID
 PyExc_ImportError
 PyErr_SetString
 PyModule_NewObject
 PyModule_GetDict
+PyList_New
+PyDict_New
+PyImport_ImportModuleLevelObject
 _Py_CheckRecursionLimit
 PyEval_EvalCodeEx
 _Py_CheckRecursiveCall
+PyObject_GetAttr
 PyExc_NameError
 PyErr_Format
+_PyDict_GetItem_KnownHash
 PyErr_Occurred
+PyFunction_Type
+PyCFunction_Type
+PyTuple_New
+PyExc_SystemError
+PyObject_Call
+__stack_chk_fail
+PyTraceBack_Here
+_PyObject_GetDictPtr
+_Py_FalseStruct
+_Py_TrueStruct
+PyObject_Not
+PyObject_SetAttr
+PyUnicode_FromString
+PyUnicode_FromFormat
+PyCode_New
+PyMem_Realloc
+PyMem_Malloc
 PyExc_RuntimeError
 PyOS_snprintf
 Py_GetVersion
 PyErr_WarnEx
 PyFrame_Type
-PyTuple_New
 PyBytes_FromStringAndSize
 PyUnicode_FromStringAndSize
 PyImport_AddModule
 PyObject_SetAttrString
 PyUnicode_InternFromString
 PyUnicode_Decode
 PyObject_Hash
 PyLong_FromLong
 __pyx_module_is_main_pytelerdac__utils__device_utils
 PyImport_GetModuleDict
 PyDict_GetItemString
-PySlice_New
 PyTuple_Pack
-PyList_New
-PyDict_New
-PyImport_ImportModuleLevelObject
+PySlice_New
 PyDict_SetItem
 PyCFunction_NewEx
-__stack_chk_fail
 PyMethod_Type
-PyFunction_Type
-PyCFunction_Type
+PyObject_Size
 PyLong_Type
 PyUnicode_Join
 PyExc_TypeError
-PyExc_SystemError
-PyObject_Call
 PyFloat_Type
 PyNumber_Add
 PyList_Append
 PyFloat_FromDouble
 PyInit_device_utils
 PyModuleDef_Init
 libc.so.6
 GLIBC_2.2.5
 GLIBC_2.4
 /home/imason/anaconda3/envs/backend/lib
-AWAVAUATUH
+AVAUATE1
+A\A]A^A_
+AWAVAUATI
 []A\A]A^A_
+AVAUATUH
+[]A\A]A^
 ([]A\A]A^A_
 ([]A\A]A^A_
 AQSAUUPPPPP
-AWAVAUATI
-[]A\A]A^A_
 AWAVAUATUSH
 []A\A]A^A_
-pytelerdac/utils/device_utils.c
 Interpreter change detected - this module can only be loaded into one interpreter per process.
  while calling a Python object
+NULL result without error in PyObject_Call
+pytelerdac/utils/device_utils.c
 Module 'device_utils' has already been imported. Re-initialisation is not supported.
 compiletime version %s of module '%.100s' does not match runtime version %s
 pytelerdac/utils/device_utils.pyx
 init pytelerdac.utils.device_utils
-NULL result without error in PyObject_Call
-'%.200s' object is unsliceable
 pytelerdac.utils.device_utils.get_device_id
-%s (%s:%d)
+'%.200s' object is unsliceable
 __loader__
 __file__
 __package__
 __path__
 submodule_search_locations
 name '%U' is not defined
+%s (%s:%d)
 pytelerdac.utils.device_utils
 builtins
 cython_runtime
 __builtins__
 get_device_id
 pytelerdac/utils/device_utils.pyx
+ifconfig mlan0 | grep ether | awk '{print $2}'
 pytelerdac.utils.device_utils
 cline_in_traceback
 get_device_id
 __import__
 __test__
 __name__
 __main__
     :return:
 GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
 device_utils.c
 __pyx_bisect_code_objects
 __Pyx_PyFunction_FastCallNoKw
 __pyx_pyframe_localsplus_offset
+__Pyx_copy_spec_to_module
+__pyx_pymod_create
+main_interpreter_id.15716
+__Pyx_Import.constprop.0
+__Pyx_PyFunction_FastCallDict.constprop.0
+__Pyx_GetBuiltinName
+__Pyx__GetModuleGlobalName
+__Pyx_PyObject_CallOneArg
+__Pyx_PyObject_Call2Args
 __Pyx_AddTraceback
 __pyx_code_cache
 __pyx_cython_runtime
-__pyx_dict_version.15866
-__pyx_dict_cached_value.15867
+__pyx_dict_version.15922
+__pyx_dict_cached_value.15923
 __pyx_n_s_cline_in_traceback
 __pyx_empty_tuple
 __pyx_empty_bytes
-__Pyx_copy_spec_to_module
-__pyx_pymod_create
-main_interpreter_id.15670
-__Pyx_PyFunction_FastCallDict.constprop.0
-__Pyx_GetBuiltinName
-__Pyx__GetModuleGlobalName
 __pyx_pymod_exec_device_utils
 __pyx_lineno
 __pyx_filename
 __pyx_clineno
 __pyx_string_tab
 __pyx_int_2
 __pyx_int_neg_12
 __pyx_n_s_main
 __pyx_n_s_name
 __pyx_n_s_range
-__pyx_slice_
+__pyx_kp_s__2
+__pyx_kp_s_
+__pyx_tuple__3
+__pyx_slice__4
 __pyx_n_s_e
 __pyx_n_s_mac
+__pyx_n_s_result
 __pyx_n_s_get_device_id
 __pyx_kp_s_pytelerdac_utils_device_utils_py
+__pyx_n_s_os
 __pyx_n_s_uuid
 __pyx_n_s_pytelerdac_utils_device_utils
 __pyx_mdef_10pytelerdac_5utils_12device_utils_1get_device_id
 __pyx_n_s_test
+__Pyx_PyObject_CallNoArg
 __pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id
-__pyx_dict_version.15592
-__pyx_dict_cached_value.15593
+__pyx_dict_version.15620
+__pyx_dict_cached_value.15621
+__pyx_n_s_popen
+__pyx_kp_s_ifconfig_mlan0_grep_ether_awk_pr
+__pyx_n_s_read
+__pyx_n_s_strip
+__pyx_n_s_close
+__pyx_n_s_split
+__pyx_dict_version.15637
+__pyx_dict_cached_value.15638
 __pyx_n_s_UUID
-__pyx_dict_version.15595
-__pyx_dict_cached_value.15596
+__pyx_dict_version.15639
+__pyx_dict_cached_value.15640
 __pyx_n_s_getnode
 __pyx_n_s_int
 __pyx_n_s_hex
 __pyx_n_s_upper
-__pyx_kp_s__2
+__pyx_n_s_replace
 __pyx_moduledef
+__pyx_k_
 __pyx_k_UUID
 __pyx_k__2
 __pyx_k_cline_in_traceback
+__pyx_k_close
 __pyx_k_e
 __pyx_k_get_device_id
 __pyx_k_getnode
 __pyx_k_hex
+__pyx_k_ifconfig_mlan0_grep_ether_awk_pr
 __pyx_n_s_import
 __pyx_k_import
 __pyx_k_int
 __pyx_n_s_join
 __pyx_k_join
 __pyx_k_mac
 __pyx_k_main
 __pyx_k_name
+__pyx_k_os
+__pyx_k_popen
 __pyx_k_pytelerdac_utils_device_utils
 __pyx_k_pytelerdac_utils_device_utils_py
 __pyx_k_range
+__pyx_k_read
+__pyx_k_replace
+__pyx_k_result
+__pyx_k_split
+__pyx_k_strip
 __pyx_k_test
 __pyx_k_upper
 __pyx_k_uuid
 __pyx_methods
 __pyx_moduledef_slots
 __pyx_doc_10pytelerdac_5utils_12device_utils_get_device_id
 crtstuff.c
@@ -252,14 +283,15 @@
 PyTuple_New
 PyThreadState_Get
 PyObject_SetAttr
 PyErr_Occurred
 _PyDict_GetItem_KnownHash
 PyDict_GetItemString
 PyEval_EvalCodeEx
+PyObject_Size
 _Py_NoneStruct
 PyImport_ImportModuleLevelObject
 PyObject_Hash
 _Py_TrueStruct
 PyFunction_Type
 PyDict_New
 PyLong_Type
```

### readelf --wide --decompress --hex-dump=.gnu.hash {}

```diff
@@ -1,6 +1,6 @@
 
 Hex dump of section '.gnu.hash':
-  0x000002f0 02000000 4d000000 01000000 06000000 ....M...........
-  0x00000300 02000000 82000080 00000000 4d000000 ............M...
+  0x000002f0 02000000 4e000000 01000000 06000000 ....N...........
+  0x00000300 02000000 82000080 00000000 4e000000 ............N...
   0x00000310 c089c767 e1afc071                   ...g...q
```

### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -1,96 +1,97 @@
 
 Hex dump of section '.dynstr':
-  0x00000a80 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
-  0x00000a90 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
-  0x00000aa0 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
-  0x00000ab0 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
-  0x00000ac0 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
-  0x00000ad0 6c697a65 005f5079 54687265 61645374 lize._PyThreadSt
-  0x00000ae0 6174655f 556e6368 65636b65 64476574 ate_UncheckedGet
-  0x00000af0 00507946 72616d65 5f4e6577 00507945 .PyFrame_New.PyE
-  0x00000b00 76616c5f 4576616c 4672616d 65457800 val_EvalFrameEx.
-  0x00000b10 5f50795f 4465616c 6c6f6300 50795472 _Py_Dealloc.PyTr
-  0x00000b20 61636542 61636b5f 48657265 005f5079 aceBack_Here._Py
-  0x00000b30 4f626a65 63745f47 65744469 63745074 Object_GetDictPt
-  0x00000b40 72005f50 795f4661 6c736553 74727563 r._Py_FalseStruc
-  0x00000b50 74005f50 795f5472 75655374 72756374 t._Py_TrueStruct
-  0x00000b60 0050794f 626a6563 745f4e6f 74005079 .PyObject_Not.Py
-  0x00000b70 4572725f 436c6561 72005079 4f626a65 Err_Clear.PyObje
-  0x00000b80 63745f53 65744174 74720050 79556e69 ct_SetAttr.PyUni
-  0x00000b90 636f6465 5f46726f 6d537472 696e6700 code_FromString.
-  0x00000ba0 5079556e 69636f64 655f4672 6f6d466f PyUnicode_FromFo
-  0x00000bb0 726d6174 00507943 6f64655f 4e657700 rmat.PyCode_New.
-  0x00000bc0 50794d65 6d5f5265 616c6c6f 63005f50 PyMem_Realloc._P
-  0x00000bd0 79446963 745f4765 74497465 6d5f4b6e yDict_GetItem_Kn
-  0x00000be0 6f776e48 61736800 50794d65 6d5f4d61 ownHash.PyMem_Ma
-  0x00000bf0 6c6c6f63 0050794f 626a6563 745f4765 lloc.PyObject_Ge
-  0x00000c00 74417474 72005079 4f626a65 63745f47 tAttr.PyObject_G
-  0x00000c10 65744174 74725374 72696e67 005f5079 etAttrString._Py
-  0x00000c20 5f4e6f6e 65537472 75637400 50794469 _NoneStruct.PyDi
-  0x00000c30 63745f53 65744974 656d5374 72696e67 ct_SetItemString
-  0x00000c40 00507945 78635f41 74747269 62757465 .PyExc_Attribute
-  0x00000c50 4572726f 72005079 4572725f 45786365 Error.PyErr_Exce
-  0x00000c60 7074696f 6e4d6174 63686573 00507954 ptionMatches.PyT
-  0x00000c70 68726561 64537461 74655f47 65740050 hreadState_Get.P
-  0x00000c80 79496e74 65727072 65746572 53746174 yInterpreterStat
-  0x00000c90 655f4765 74494400 50794578 635f496d e_GetID.PyExc_Im
-  0x00000ca0 706f7274 4572726f 72005079 4572725f portError.PyErr_
-  0x00000cb0 53657453 7472696e 67005079 4d6f6475 SetString.PyModu
-  0x00000cc0 6c655f4e 65774f62 6a656374 0050794d le_NewObject.PyM
-  0x00000cd0 6f64756c 655f4765 74446963 74005f50 odule_GetDict._P
-  0x00000ce0 795f4368 65636b52 65637572 73696f6e y_CheckRecursion
-  0x00000cf0 4c696d69 74005079 4576616c 5f457661 Limit.PyEval_Eva
-  0x00000d00 6c436f64 65457800 5f50795f 43686563 lCodeEx._Py_Chec
-  0x00000d10 6b526563 75727369 76654361 6c6c0050 kRecursiveCall.P
-  0x00000d20 79457863 5f4e616d 65457272 6f720050 yExc_NameError.P
-  0x00000d30 79457272 5f466f72 6d617400 50794572 yErr_Format.PyEr
-  0x00000d40 725f4f63 63757272 65640050 79457863 r_Occurred.PyExc
-  0x00000d50 5f52756e 74696d65 4572726f 72005079 _RuntimeError.Py
-  0x00000d60 4f535f73 6e707269 6e746600 50795f47 OS_snprintf.Py_G
-  0x00000d70 65745665 7273696f 6e005079 4572725f etVersion.PyErr_
-  0x00000d80 5761726e 45780050 79467261 6d655f54 WarnEx.PyFrame_T
-  0x00000d90 79706500 50795475 706c655f 4e657700 ype.PyTuple_New.
-  0x00000da0 50794279 7465735f 46726f6d 53747269 PyBytes_FromStri
-  0x00000db0 6e67416e 6453697a 65005079 556e6963 ngAndSize.PyUnic
-  0x00000dc0 6f64655f 46726f6d 53747269 6e67416e ode_FromStringAn
-  0x00000dd0 6453697a 65005079 496d706f 72745f41 dSize.PyImport_A
-  0x00000de0 64644d6f 64756c65 0050794f 626a6563 ddModule.PyObjec
-  0x00000df0 745f5365 74417474 72537472 696e6700 t_SetAttrString.
-  0x00000e00 5079556e 69636f64 655f496e 7465726e PyUnicode_Intern
-  0x00000e10 46726f6d 53747269 6e670050 79556e69 FromString.PyUni
-  0x00000e20 636f6465 5f446563 6f646500 50794f62 code_Decode.PyOb
-  0x00000e30 6a656374 5f486173 68005079 4c6f6e67 ject_Hash.PyLong
-  0x00000e40 5f46726f 6d4c6f6e 67005f5f 7079785f _FromLong.__pyx_
-  0x00000e50 6d6f6475 6c655f69 735f6d61 696e5f70 module_is_main_p
-  0x00000e60 7974656c 65726461 635f5f75 74696c73 ytelerdac__utils
-  0x00000e70 5f5f6465 76696365 5f757469 6c730050 __device_utils.P
-  0x00000e80 79496d70 6f72745f 4765744d 6f64756c yImport_GetModul
-  0x00000e90 65446963 74005079 44696374 5f476574 eDict.PyDict_Get
-  0x00000ea0 4974656d 53747269 6e670050 79536c69 ItemString.PySli
-  0x00000eb0 63655f4e 65770050 79547570 6c655f50 ce_New.PyTuple_P
-  0x00000ec0 61636b00 50794c69 73745f4e 65770050 ack.PyList_New.P
-  0x00000ed0 79446963 745f4e65 77005079 496d706f yDict_New.PyImpo
-  0x00000ee0 72745f49 6d706f72 744d6f64 756c654c rt_ImportModuleL
-  0x00000ef0 6576656c 4f626a65 63740050 79446963 evelObject.PyDic
-  0x00000f00 745f5365 74497465 6d005079 4346756e t_SetItem.PyCFun
-  0x00000f10 6374696f 6e5f4e65 77457800 5f5f7374 ction_NewEx.__st
-  0x00000f20 61636b5f 63686b5f 6661696c 0050794d ack_chk_fail.PyM
-  0x00000f30 6574686f 645f5479 70650050 7946756e ethod_Type.PyFun
-  0x00000f40 6374696f 6e5f5479 70650050 79434675 ction_Type.PyCFu
-  0x00000f50 6e637469 6f6e5f54 79706500 50794c6f nction_Type.PyLo
-  0x00000f60 6e675f54 79706500 5079556e 69636f64 ng_Type.PyUnicod
-  0x00000f70 655f4a6f 696e0050 79457863 5f547970 e_Join.PyExc_Typ
-  0x00000f80 65457272 6f720050 79457863 5f537973 eError.PyExc_Sys
-  0x00000f90 74656d45 72726f72 0050794f 626a6563 temError.PyObjec
-  0x00000fa0 745f4361 6c6c0050 79466c6f 61745f54 t_Call.PyFloat_T
-  0x00000fb0 79706500 50794e75 6d626572 5f416464 ype.PyNumber_Add
-  0x00000fc0 0050794c 6973745f 41707065 6e640050 .PyList_Append.P
-  0x00000fd0 79466c6f 61745f46 726f6d44 6f75626c yFloat_FromDoubl
-  0x00000fe0 65005079 496e6974 5f646576 6963655f e.PyInit_device_
-  0x00000ff0 7574696c 73005079 4d6f6475 6c654465 utils.PyModuleDe
-  0x00001000 665f496e 6974006c 6962632e 736f2e36 f_Init.libc.so.6
-  0x00001010 00474c49 42435f32 2e322e35 00474c49 .GLIBC_2.2.5.GLI
-  0x00001020 42435f32 2e34002f 686f6d65 2f696d61 BC_2.4./home/ima
-  0x00001030 736f6e2f 616e6163 6f6e6461 332f656e son/anaconda3/en
-  0x00001040 76732f62 61636b65 6e642f6c 696200   vs/backend/lib.
+  0x00000a98 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
+  0x00000aa8 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
+  0x00000ab8 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
+  0x00000ac8 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
+  0x00000ad8 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
+  0x00000ae8 6c697a65 005f5079 54687265 61645374 lize._PyThreadSt
+  0x00000af8 6174655f 556e6368 65636b65 64476574 ate_UncheckedGet
+  0x00000b08 00507946 72616d65 5f4e6577 00507945 .PyFrame_New.PyE
+  0x00000b18 76616c5f 4576616c 4672616d 65457800 val_EvalFrameEx.
+  0x00000b28 5f50795f 4465616c 6c6f6300 50794f62 _Py_Dealloc.PyOb
+  0x00000b38 6a656374 5f476574 41747472 53747269 ject_GetAttrStri
+  0x00000b48 6e67005f 50795f4e 6f6e6553 74727563 ng._Py_NoneStruc
+  0x00000b58 74005079 44696374 5f536574 4974656d t.PyDict_SetItem
+  0x00000b68 53747269 6e670050 79457863 5f417474 String.PyExc_Att
+  0x00000b78 72696275 74654572 726f7200 50794572 ributeError.PyEr
+  0x00000b88 725f4578 63657074 696f6e4d 61746368 r_ExceptionMatch
+  0x00000b98 65730050 79457272 5f436c65 61720050 es.PyErr_Clear.P
+  0x00000ba8 79546872 65616453 74617465 5f476574 yThreadState_Get
+  0x00000bb8 00507949 6e746572 70726574 65725374 .PyInterpreterSt
+  0x00000bc8 6174655f 47657449 44005079 4578635f ate_GetID.PyExc_
+  0x00000bd8 496d706f 72744572 726f7200 50794572 ImportError.PyEr
+  0x00000be8 725f5365 74537472 696e6700 50794d6f r_SetString.PyMo
+  0x00000bf8 64756c65 5f4e6577 4f626a65 63740050 dule_NewObject.P
+  0x00000c08 794d6f64 756c655f 47657444 69637400 yModule_GetDict.
+  0x00000c18 50794c69 73745f4e 65770050 79446963 PyList_New.PyDic
+  0x00000c28 745f4e65 77005079 496d706f 72745f49 t_New.PyImport_I
+  0x00000c38 6d706f72 744d6f64 756c654c 6576656c mportModuleLevel
+  0x00000c48 4f626a65 6374005f 50795f43 6865636b Object._Py_Check
+  0x00000c58 52656375 7273696f 6e4c696d 69740050 RecursionLimit.P
+  0x00000c68 79457661 6c5f4576 616c436f 64654578 yEval_EvalCodeEx
+  0x00000c78 005f5079 5f436865 636b5265 63757273 ._Py_CheckRecurs
+  0x00000c88 69766543 616c6c00 50794f62 6a656374 iveCall.PyObject
+  0x00000c98 5f476574 41747472 00507945 78635f4e _GetAttr.PyExc_N
+  0x00000ca8 616d6545 72726f72 00507945 72725f46 ameError.PyErr_F
+  0x00000cb8 6f726d61 74005f50 79446963 745f4765 ormat._PyDict_Ge
+  0x00000cc8 74497465 6d5f4b6e 6f776e48 61736800 tItem_KnownHash.
+  0x00000cd8 50794572 725f4f63 63757272 65640050 PyErr_Occurred.P
+  0x00000ce8 7946756e 6374696f 6e5f5479 70650050 yFunction_Type.P
+  0x00000cf8 79434675 6e637469 6f6e5f54 79706500 yCFunction_Type.
+  0x00000d08 50795475 706c655f 4e657700 50794578 PyTuple_New.PyEx
+  0x00000d18 635f5379 7374656d 4572726f 72005079 c_SystemError.Py
+  0x00000d28 4f626a65 63745f43 616c6c00 5f5f7374 Object_Call.__st
+  0x00000d38 61636b5f 63686b5f 6661696c 00507954 ack_chk_fail.PyT
+  0x00000d48 72616365 4261636b 5f486572 65005f50 raceBack_Here._P
+  0x00000d58 794f626a 6563745f 47657444 69637450 yObject_GetDictP
+  0x00000d68 7472005f 50795f46 616c7365 53747275 tr._Py_FalseStru
+  0x00000d78 6374005f 50795f54 72756553 74727563 ct._Py_TrueStruc
+  0x00000d88 74005079 4f626a65 63745f4e 6f740050 t.PyObject_Not.P
+  0x00000d98 794f626a 6563745f 53657441 74747200 yObject_SetAttr.
+  0x00000da8 5079556e 69636f64 655f4672 6f6d5374 PyUnicode_FromSt
+  0x00000db8 72696e67 00507955 6e69636f 64655f46 ring.PyUnicode_F
+  0x00000dc8 726f6d46 6f726d61 74005079 436f6465 romFormat.PyCode
+  0x00000dd8 5f4e6577 0050794d 656d5f52 65616c6c _New.PyMem_Reall
+  0x00000de8 6f630050 794d656d 5f4d616c 6c6f6300 oc.PyMem_Malloc.
+  0x00000df8 50794578 635f5275 6e74696d 65457272 PyExc_RuntimeErr
+  0x00000e08 6f720050 794f535f 736e7072 696e7466 or.PyOS_snprintf
+  0x00000e18 0050795f 47657456 65727369 6f6e0050 .Py_GetVersion.P
+  0x00000e28 79457272 5f576172 6e457800 50794672 yErr_WarnEx.PyFr
+  0x00000e38 616d655f 54797065 00507942 79746573 ame_Type.PyBytes
+  0x00000e48 5f46726f 6d537472 696e6741 6e645369 _FromStringAndSi
+  0x00000e58 7a650050 79556e69 636f6465 5f46726f ze.PyUnicode_Fro
+  0x00000e68 6d537472 696e6741 6e645369 7a650050 mStringAndSize.P
+  0x00000e78 79496d70 6f72745f 4164644d 6f64756c yImport_AddModul
+  0x00000e88 65005079 4f626a65 63745f53 65744174 e.PyObject_SetAt
+  0x00000e98 74725374 72696e67 00507955 6e69636f trString.PyUnico
+  0x00000ea8 64655f49 6e746572 6e46726f 6d537472 de_InternFromStr
+  0x00000eb8 696e6700 5079556e 69636f64 655f4465 ing.PyUnicode_De
+  0x00000ec8 636f6465 0050794f 626a6563 745f4861 code.PyObject_Ha
+  0x00000ed8 73680050 794c6f6e 675f4672 6f6d4c6f sh.PyLong_FromLo
+  0x00000ee8 6e67005f 5f707978 5f6d6f64 756c655f ng.__pyx_module_
+  0x00000ef8 69735f6d 61696e5f 70797465 6c657264 is_main_pytelerd
+  0x00000f08 61635f5f 7574696c 735f5f64 65766963 ac__utils__devic
+  0x00000f18 655f7574 696c7300 5079496d 706f7274 e_utils.PyImport
+  0x00000f28 5f476574 4d6f6475 6c654469 63740050 _GetModuleDict.P
+  0x00000f38 79446963 745f4765 74497465 6d537472 yDict_GetItemStr
+  0x00000f48 696e6700 50795475 706c655f 5061636b ing.PyTuple_Pack
+  0x00000f58 00507953 6c696365 5f4e6577 00507944 .PySlice_New.PyD
+  0x00000f68 6963745f 53657449 74656d00 50794346 ict_SetItem.PyCF
+  0x00000f78 756e6374 696f6e5f 4e657745 78005079 unction_NewEx.Py
+  0x00000f88 4d657468 6f645f54 79706500 50794f62 Method_Type.PyOb
+  0x00000f98 6a656374 5f53697a 65005079 4c6f6e67 ject_Size.PyLong
+  0x00000fa8 5f547970 65005079 556e6963 6f64655f _Type.PyUnicode_
+  0x00000fb8 4a6f696e 00507945 78635f54 79706545 Join.PyExc_TypeE
+  0x00000fc8 72726f72 00507946 6c6f6174 5f547970 rror.PyFloat_Typ
+  0x00000fd8 65005079 4e756d62 65725f41 64640050 e.PyNumber_Add.P
+  0x00000fe8 794c6973 745f4170 70656e64 00507946 yList_Append.PyF
+  0x00000ff8 6c6f6174 5f46726f 6d446f75 626c6500 loat_FromDouble.
+  0x00001008 5079496e 69745f64 65766963 655f7574 PyInit_device_ut
+  0x00001018 696c7300 50794d6f 64756c65 4465665f ils.PyModuleDef_
+  0x00001028 496e6974 006c6962 632e736f 2e360047 Init.libc.so.6.G
+  0x00001038 4c494243 5f322e32 2e350047 4c494243 LIBC_2.2.5.GLIBC
+  0x00001048 5f322e34 002f686f 6d652f69 6d61736f _2.4./home/imaso
+  0x00001058 6e2f616e 61636f6e 6461332f 656e7673 n/anaconda3/envs
+  0x00001068 2f626163 6b656e64 2f6c6962 00       /backend/lib.
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.init {}

```diff
@@ -3,13 +3,13 @@
 
 Disassembly of section .init:
 
 0000000000002000 <_init>:
 _init():
 	endbr64
 	sub    $0x8,%rsp
-	mov    0x5f89(%rip),%rax        
+	mov    0x7f89(%rip),%rax        
 	test   %rax,%rax
 	je     2016 <_init+0x16>
 	call   *%rax
 	add    $0x8,%rsp
 	ret
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt {}

```diff
@@ -1,15 +1,15 @@
 
 
 
 Disassembly of section .plt:
 
 0000000000002020 <.plt>:
-	push   0x5fe2(%rip)        
-	bnd jmp *0x5fe3(%rip)        
+	push   0x7fe2(%rip)        
+	bnd jmp *0x7fe3(%rip)        
 	nopl   (%rax)
 	endbr64
 	push   $0x0
 	bnd jmp 2020 <_init+0x20>
 	nop
 	endbr64
 	push   $0x1
@@ -227,7 +227,11 @@
 	push   $0x36
 	bnd jmp 2020 <_init+0x20>
 	nop
 	endbr64
 	push   $0x37
 	bnd jmp 2020 <_init+0x20>
 	nop
+	endbr64
+	push   $0x38
+	bnd jmp 2020 <_init+0x20>
+	nop
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt.got {}

```diff
@@ -1,9 +1,9 @@
 
 
 
 Disassembly of section .plt.got:
 
-00000000000023b0 <__cxa_finalize@plt>:
+00000000000023c0 <__cxa_finalize@plt>:
 	endbr64
-	bnd jmp *0x5c3d(%rip)        
+	bnd jmp *0x7c2d(%rip)        
 	nopl   0x0(%rax,%rax,1)
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt.sec {}

```diff
@@ -1,284 +1,289 @@
 
 
 
 Disassembly of section .plt.sec:
 
-00000000000023c0 <PyUnicode_FromFormat@plt>:
+00000000000023d0 <PyUnicode_FromFormat@plt>:
 	endbr64
-	bnd jmp *0x5c4d(%rip)        
+	bnd jmp *0x7c3d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000023d0 <PyList_New@plt>:
+00000000000023e0 <PyList_New@plt>:
 	endbr64
-	bnd jmp *0x5c45(%rip)        
+	bnd jmp *0x7c35(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000023e0 <PyDict_SetItemString@plt>:
+00000000000023f0 <PyDict_SetItemString@plt>:
 	endbr64
-	bnd jmp *0x5c3d(%rip)        
+	bnd jmp *0x7c2d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000023f0 <_PyThreadState_UncheckedGet@plt>:
+0000000000002400 <_PyThreadState_UncheckedGet@plt>:
 	endbr64
-	bnd jmp *0x5c35(%rip)        
+	bnd jmp *0x7c25(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002400 <PyModuleDef_Init@plt>:
+0000000000002410 <PyModuleDef_Init@plt>:
 	endbr64
-	bnd jmp *0x5c2d(%rip)        
+	bnd jmp *0x7c1d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002410 <PyFrame_New@plt>:
+0000000000002420 <PyFrame_New@plt>:
 	endbr64
-	bnd jmp *0x5c25(%rip)        
+	bnd jmp *0x7c15(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002420 <PyCFunction_NewEx@plt>:
+0000000000002430 <PyCFunction_NewEx@plt>:
 	endbr64
-	bnd jmp *0x5c1d(%rip)        
+	bnd jmp *0x7c0d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002430 <PyNumber_Add@plt>:
+0000000000002440 <PyNumber_Add@plt>:
 	endbr64
-	bnd jmp *0x5c15(%rip)        
+	bnd jmp *0x7c05(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002440 <PyObject_GetAttrString@plt>:
+0000000000002450 <PyObject_GetAttrString@plt>:
 	endbr64
-	bnd jmp *0x5c0d(%rip)        
+	bnd jmp *0x7bfd(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002450 <PyUnicode_Join@plt>:
+0000000000002460 <PyUnicode_Join@plt>:
 	endbr64
-	bnd jmp *0x5c05(%rip)        
+	bnd jmp *0x7bf5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002460 <PyImport_AddModule@plt>:
+0000000000002470 <PyImport_AddModule@plt>:
 	endbr64
-	bnd jmp *0x5bfd(%rip)        
+	bnd jmp *0x7bed(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002470 <PyBytes_FromStringAndSize@plt>:
+0000000000002480 <PyBytes_FromStringAndSize@plt>:
 	endbr64
-	bnd jmp *0x5bf5(%rip)        
+	bnd jmp *0x7be5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002480 <PyObject_SetAttrString@plt>:
+0000000000002490 <PyObject_SetAttrString@plt>:
 	endbr64
-	bnd jmp *0x5bed(%rip)        
+	bnd jmp *0x7bdd(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002490 <PyErr_WarnEx@plt>:
+00000000000024a0 <PyErr_WarnEx@plt>:
 	endbr64
-	bnd jmp *0x5be5(%rip)        
+	bnd jmp *0x7bd5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000024a0 <_Py_Dealloc@plt>:
+00000000000024b0 <_Py_Dealloc@plt>:
 	endbr64
-	bnd jmp *0x5bdd(%rip)        
+	bnd jmp *0x7bcd(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000024b0 <PyModule_NewObject@plt>:
+00000000000024c0 <PyModule_NewObject@plt>:
 	endbr64
-	bnd jmp *0x5bd5(%rip)        
+	bnd jmp *0x7bc5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000024c0 <PyCode_New@plt>:
+00000000000024d0 <PyCode_New@plt>:
 	endbr64
-	bnd jmp *0x5bcd(%rip)        
+	bnd jmp *0x7bbd(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000024d0 <PyImport_GetModuleDict@plt>:
+00000000000024e0 <PyImport_GetModuleDict@plt>:
 	endbr64
-	bnd jmp *0x5bc5(%rip)        
+	bnd jmp *0x7bb5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000024e0 <__stack_chk_fail@plt>:
+00000000000024f0 <__stack_chk_fail@plt>:
 	endbr64
-	bnd jmp *0x5bbd(%rip)        
+	bnd jmp *0x7bad(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000024f0 <PyErr_SetString@plt>:
+0000000000002500 <PyErr_SetString@plt>:
 	endbr64
-	bnd jmp *0x5bb5(%rip)        
+	bnd jmp *0x7ba5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002500 <PyInterpreterState_GetID@plt>:
+0000000000002510 <PyInterpreterState_GetID@plt>:
 	endbr64
-	bnd jmp *0x5bad(%rip)        
+	bnd jmp *0x7b9d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002510 <PyEval_EvalFrameEx@plt>:
+0000000000002520 <PyEval_EvalFrameEx@plt>:
 	endbr64
-	bnd jmp *0x5ba5(%rip)        
+	bnd jmp *0x7b95(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002520 <PyMem_Realloc@plt>:
+0000000000002530 <PyMem_Realloc@plt>:
 	endbr64
-	bnd jmp *0x5b9d(%rip)        
+	bnd jmp *0x7b8d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002530 <PyErr_ExceptionMatches@plt>:
+0000000000002540 <PyErr_ExceptionMatches@plt>:
 	endbr64
-	bnd jmp *0x5b95(%rip)        
+	bnd jmp *0x7b85(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002540 <PyOS_snprintf@plt>:
+0000000000002550 <PyOS_snprintf@plt>:
 	endbr64
-	bnd jmp *0x5b8d(%rip)        
+	bnd jmp *0x7b7d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002550 <PyTraceBack_Here@plt>:
+0000000000002560 <PyTraceBack_Here@plt>:
 	endbr64
-	bnd jmp *0x5b85(%rip)        
+	bnd jmp *0x7b75(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002560 <PyObject_Not@plt>:
+0000000000002570 <PyObject_Not@plt>:
 	endbr64
-	bnd jmp *0x5b7d(%rip)        
+	bnd jmp *0x7b6d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002570 <PyFloat_FromDouble@plt>:
+0000000000002580 <PyFloat_FromDouble@plt>:
 	endbr64
-	bnd jmp *0x5b75(%rip)        
+	bnd jmp *0x7b65(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002580 <PyLong_FromLong@plt>:
+0000000000002590 <PyLong_FromLong@plt>:
 	endbr64
-	bnd jmp *0x5b6d(%rip)        
+	bnd jmp *0x7b5d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002590 <PyErr_Clear@plt>:
+00000000000025a0 <PyErr_Clear@plt>:
 	endbr64
-	bnd jmp *0x5b65(%rip)        
+	bnd jmp *0x7b55(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000025a0 <PyList_Append@plt>:
+00000000000025b0 <PyList_Append@plt>:
 	endbr64
-	bnd jmp *0x5b5d(%rip)        
+	bnd jmp *0x7b4d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000025b0 <_Py_CheckRecursiveCall@plt>:
+00000000000025c0 <_Py_CheckRecursiveCall@plt>:
 	endbr64
-	bnd jmp *0x5b55(%rip)        
+	bnd jmp *0x7b45(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000025c0 <PyTuple_New@plt>:
+00000000000025d0 <PyTuple_New@plt>:
 	endbr64
-	bnd jmp *0x5b4d(%rip)        
+	bnd jmp *0x7b3d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000025d0 <PyThreadState_Get@plt>:
+00000000000025e0 <PyThreadState_Get@plt>:
 	endbr64
-	bnd jmp *0x5b45(%rip)        
+	bnd jmp *0x7b35(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000025e0 <PyObject_SetAttr@plt>:
+00000000000025f0 <PyObject_SetAttr@plt>:
 	endbr64
-	bnd jmp *0x5b3d(%rip)        
+	bnd jmp *0x7b2d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000025f0 <PyErr_Occurred@plt>:
+0000000000002600 <PyErr_Occurred@plt>:
 	endbr64
-	bnd jmp *0x5b35(%rip)        
+	bnd jmp *0x7b25(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002600 <_PyDict_GetItem_KnownHash@plt>:
+0000000000002610 <_PyDict_GetItem_KnownHash@plt>:
 	endbr64
-	bnd jmp *0x5b2d(%rip)        
+	bnd jmp *0x7b1d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002610 <PyDict_GetItemString@plt>:
+0000000000002620 <PyDict_GetItemString@plt>:
 	endbr64
-	bnd jmp *0x5b25(%rip)        
+	bnd jmp *0x7b15(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002620 <PyEval_EvalCodeEx@plt>:
+0000000000002630 <PyEval_EvalCodeEx@plt>:
 	endbr64
-	bnd jmp *0x5b1d(%rip)        
+	bnd jmp *0x7b0d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002630 <PyImport_ImportModuleLevelObject@plt>:
+0000000000002640 <PyObject_Size@plt>:
 	endbr64
-	bnd jmp *0x5b15(%rip)        
+	bnd jmp *0x7b05(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002640 <PyObject_Hash@plt>:
+0000000000002650 <PyImport_ImportModuleLevelObject@plt>:
 	endbr64
-	bnd jmp *0x5b0d(%rip)        
+	bnd jmp *0x7afd(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002650 <PyDict_New@plt>:
+0000000000002660 <PyObject_Hash@plt>:
 	endbr64
-	bnd jmp *0x5b05(%rip)        
+	bnd jmp *0x7af5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002660 <_PyObject_GetDictPtr@plt>:
+0000000000002670 <PyDict_New@plt>:
 	endbr64
-	bnd jmp *0x5afd(%rip)        
+	bnd jmp *0x7aed(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002670 <PyUnicode_FromString@plt>:
+0000000000002680 <_PyObject_GetDictPtr@plt>:
 	endbr64
-	bnd jmp *0x5af5(%rip)        
+	bnd jmp *0x7ae5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002680 <PyUnicode_InternFromString@plt>:
+0000000000002690 <PyUnicode_FromString@plt>:
 	endbr64
-	bnd jmp *0x5aed(%rip)        
+	bnd jmp *0x7add(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002690 <PyDict_SetItem@plt>:
+00000000000026a0 <PyUnicode_InternFromString@plt>:
 	endbr64
-	bnd jmp *0x5ae5(%rip)        
+	bnd jmp *0x7ad5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000026a0 <PyObject_Call@plt>:
+00000000000026b0 <PyDict_SetItem@plt>:
 	endbr64
-	bnd jmp *0x5add(%rip)        
+	bnd jmp *0x7acd(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000026b0 <PyUnicode_Decode@plt>:
+00000000000026c0 <PyObject_Call@plt>:
 	endbr64
-	bnd jmp *0x5ad5(%rip)        
+	bnd jmp *0x7ac5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000026c0 <PyErr_Format@plt>:
+00000000000026d0 <PyUnicode_Decode@plt>:
 	endbr64
-	bnd jmp *0x5acd(%rip)        
+	bnd jmp *0x7abd(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000026d0 <PySlice_New@plt>:
+00000000000026e0 <PyErr_Format@plt>:
 	endbr64
-	bnd jmp *0x5ac5(%rip)        
+	bnd jmp *0x7ab5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000026e0 <PyUnicode_FromStringAndSize@plt>:
+00000000000026f0 <PySlice_New@plt>:
 	endbr64
-	bnd jmp *0x5abd(%rip)        
+	bnd jmp *0x7aad(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-00000000000026f0 <PyModule_GetDict@plt>:
+0000000000002700 <PyUnicode_FromStringAndSize@plt>:
 	endbr64
-	bnd jmp *0x5ab5(%rip)        
+	bnd jmp *0x7aa5(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002700 <PyObject_GetAttr@plt>:
+0000000000002710 <PyModule_GetDict@plt>:
 	endbr64
-	bnd jmp *0x5aad(%rip)        
+	bnd jmp *0x7a9d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002710 <PyMem_Malloc@plt>:
+0000000000002720 <PyObject_GetAttr@plt>:
 	endbr64
-	bnd jmp *0x5aa5(%rip)        
+	bnd jmp *0x7a95(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002720 <PyTuple_Pack@plt>:
+0000000000002730 <PyMem_Malloc@plt>:
 	endbr64
-	bnd jmp *0x5a9d(%rip)        
+	bnd jmp *0x7a8d(%rip)        
 	nopl   0x0(%rax,%rax,1)
 
-0000000000002730 <Py_GetVersion@plt>:
+0000000000002740 <PyTuple_Pack@plt>:
 	endbr64
-	bnd jmp *0x5a95(%rip)        
+	bnd jmp *0x7a85(%rip)        
+	nopl   0x0(%rax,%rax,1)
+
+0000000000002750 <Py_GetVersion@plt>:
+	endbr64
+	bnd jmp *0x7a7d(%rip)        
 	nopl   0x0(%rax,%rax,1)
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1,2632 +1,4532 @@
 
 
 
 Disassembly of section .text:
 
-0000000000002740 <__Pyx_copy_spec_to_module>:
+0000000000002760 <__Pyx_copy_spec_to_module>:
 __Pyx_copy_spec_to_module():
 	push   %r14
 	mov    %rcx,%r14
 	push   %r13
 	mov    %rsi,%r13
 	mov    %rdx,%rsi
 	push   %r12
 	push   %rbp
 	push   %rbx
 	mov    %r8d,%ebx
-	call   2440 <PyObject_GetAttrString@plt>
+	call   2450 <PyObject_GetAttrString@plt>
 	test   %rax,%rax
-	je     2793 <__Pyx_copy_spec_to_module+0x53>
-	cmp    0x583b(%rip),%rax        
+	je     27b3 <__Pyx_copy_spec_to_module+0x53>
+	cmp    0x781b(%rip),%rax        
 	mov    %rax,%rbp
-	jne    2772 <__Pyx_copy_spec_to_module+0x32>
+	jne    2792 <__Pyx_copy_spec_to_module+0x32>
 	xor    %r12d,%r12d
 	and    $0x1,%bl
-	je     2783 <__Pyx_copy_spec_to_module+0x43>
+	je     27a3 <__Pyx_copy_spec_to_module+0x43>
 	mov    %rbp,%rdx
 	mov    %r14,%rsi
 	mov    %r13,%rdi
-	call   23e0 <PyDict_SetItemString@plt>
+	call   23f0 <PyDict_SetItemString@plt>
 	mov    %eax,%r12d
 	decq   0x0(%rbp)
-	jne    27b2 <__Pyx_copy_spec_to_module+0x72>
+	jne    27d2 <__Pyx_copy_spec_to_module+0x72>
 	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    27b2 <__Pyx_copy_spec_to_module+0x72>
-	mov    0x5836(%rip),%rax        
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    27d2 <__Pyx_copy_spec_to_module+0x72>
+	mov    0x7816(%rip),%rax        
 	or     $0xffffffff,%r12d
 	mov    (%rax),%rdi
-	call   2530 <PyErr_ExceptionMatches@plt>
+	call   2540 <PyErr_ExceptionMatches@plt>
 	test   %eax,%eax
-	je     27b2 <__Pyx_copy_spec_to_module+0x72>
-	call   2590 <PyErr_Clear@plt>
+	je     27d2 <__Pyx_copy_spec_to_module+0x72>
+	call   25a0 <PyErr_Clear@plt>
 	xor    %r12d,%r12d
 	pop    %rbx
 	mov    %r12d,%eax
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 
-00000000000027be <__pyx_pymod_create>:
+00000000000027de <__pyx_pymod_create>:
 __pyx_pymod_create():
 	endbr64
 	push   %r14
 	push   %r13
 	mov    %rdi,%r13
 	push   %r12
 	push   %rbp
 	push   %rcx
-	call   25d0 <PyThreadState_Get@plt>
+	call   25e0 <PyThreadState_Get@plt>
 	mov    0x10(%rax),%rdi
-	call   2500 <PyInterpreterState_GetID@plt>
-	mov    0x5a1e(%rip),%rdx        
+	call   2510 <PyInterpreterState_GetID@plt>
+	mov    0x79fe(%rip),%rdx        
 	cmp    $0xffffffffffffffff,%rdx
-	jne    27f6 <__pyx_pymod_create+0x38>
-	mov    %rax,0x5a11(%rip)        
+	jne    2816 <__pyx_pymod_create+0x38>
+	mov    %rax,0x79f1(%rip)        
 	inc    %rax
-	je     2811 <__pyx_pymod_create+0x53>
-	jmp    2819 <__pyx_pymod_create+0x5b>
+	je     2831 <__pyx_pymod_create+0x53>
+	jmp    2839 <__pyx_pymod_create+0x5b>
 	cmp    %rdx,%rax
-	je     2819 <__pyx_pymod_create+0x5b>
-	mov    0x57c6(%rip),%rax        
-	lea    0x3817(%rip),%rsi        
+	je     2839 <__pyx_pymod_create+0x5b>
+	mov    0x77a6(%rip),%rax        
+	lea    0x57d7(%rip),%rsi        
 	mov    (%rax),%rdi
-	call   24f0 <PyErr_SetString@plt>
+	call   2500 <PyErr_SetString@plt>
 	xor    %r12d,%r12d
-	jmp    2916 <__pyx_pymod_create+0x158>
-	mov    0x5fe0(%rip),%r12        
+	jmp    2936 <__pyx_pymod_create+0x158>
+	mov    0x81e0(%rip),%r12        
 	test   %r12,%r12
-	je     282e <__pyx_pymod_create+0x70>
+	je     284e <__pyx_pymod_create+0x70>
 	incq   (%r12)
-	jmp    2916 <__pyx_pymod_create+0x158>
-	lea    0x39ea(%rip),%rsi        
+	jmp    2936 <__pyx_pymod_create+0x158>
+	lea    0x59c2(%rip),%rsi        
 	mov    %r13,%rdi
-	call   2440 <PyObject_GetAttrString@plt>
+	call   2450 <PyObject_GetAttrString@plt>
 	mov    %rax,%r14
 	test   %rax,%rax
-	je     2811 <__pyx_pymod_create+0x53>
+	je     2831 <__pyx_pymod_create+0x53>
 	mov    %rax,%rdi
-	call   24b0 <PyModule_NewObject@plt>
+	call   24c0 <PyModule_NewObject@plt>
 	decq   (%r14)
 	mov    %rax,%rbp
-	jne    285d <__pyx_pymod_create+0x9f>
+	jne    287d <__pyx_pymod_create+0x9f>
 	mov    %r14,%rdi
-	call   24a0 <_Py_Dealloc@plt>
+	call   24b0 <_Py_Dealloc@plt>
 	test   %rbp,%rbp
-	je     2811 <__pyx_pymod_create+0x53>
+	je     2831 <__pyx_pymod_create+0x53>
 	mov    %rbp,%rdi
-	call   26f0 <PyModule_GetDict@plt>
+	call   2710 <PyModule_GetDict@plt>
 	mov    %rax,%r14
 	test   %rax,%rax
-	je     2904 <__pyx_pymod_create+0x146>
+	je     2924 <__pyx_pymod_create+0x146>
 	mov    $0x1,%r8d
-	lea    0x39a1(%rip),%rcx        
+	lea    0x5979(%rip),%rcx        
 	mov    %rax,%rsi
 	mov    %r13,%rdi
-	lea    0x399f(%rip),%rdx        
-	call   2740 <__Pyx_copy_spec_to_module>
+	lea    0x5977(%rip),%rdx        
+	call   2760 <__Pyx_copy_spec_to_module>
 	test   %eax,%eax
-	js     2904 <__pyx_pymod_create+0x146>
+	js     2924 <__pyx_pymod_create+0x146>
 	mov    $0x1,%r8d
-	lea    0x3990(%rip),%rcx        
+	lea    0x5968(%rip),%rcx        
 	mov    %r14,%rsi
 	mov    %r13,%rdi
-	lea    0x398c(%rip),%rdx        
-	call   2740 <__Pyx_copy_spec_to_module>
+	lea    0x5964(%rip),%rdx        
+	call   2760 <__Pyx_copy_spec_to_module>
 	test   %eax,%eax
-	js     2904 <__pyx_pymod_create+0x146>
+	js     2924 <__pyx_pymod_create+0x146>
 	mov    $0x1,%r8d
-	lea    0x397d(%rip),%rcx        
+	lea    0x5955(%rip),%rcx        
 	mov    %r14,%rsi
 	mov    %r13,%rdi
-	lea    0x397c(%rip),%rdx        
-	call   2740 <__Pyx_copy_spec_to_module>
+	lea    0x5954(%rip),%rdx        
+	call   2760 <__Pyx_copy_spec_to_module>
 	test   %eax,%eax
-	js     2904 <__pyx_pymod_create+0x146>
+	js     2924 <__pyx_pymod_create+0x146>
 	xor    %r8d,%r8d
-	lea    0x3970(%rip),%rcx        
+	lea    0x5948(%rip),%rcx        
 	mov    %r14,%rsi
 	mov    %r13,%rdi
-	lea    0x396c(%rip),%rdx        
-	call   2740 <__Pyx_copy_spec_to_module>
+	lea    0x5944(%rip),%rdx        
+	call   2760 <__Pyx_copy_spec_to_module>
 	test   %eax,%eax
-	js     2904 <__pyx_pymod_create+0x146>
+	js     2924 <__pyx_pymod_create+0x146>
 	mov    %rbp,%r12
-	jmp    2916 <__pyx_pymod_create+0x158>
+	jmp    2936 <__pyx_pymod_create+0x158>
 	decq   0x0(%rbp)
-	jne    2811 <__pyx_pymod_create+0x53>
+	jne    2831 <__pyx_pymod_create+0x53>
 	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
+	call   24b0 <_Py_Dealloc@plt>
 	pop    %rdx
 	mov    %r12,%rax
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 
-0000000000002922 <__pyx_pymod_exec_device_utils>:
-__pyx_pymod_exec_device_utils():
-	endbr64
+0000000000002942 <__Pyx_Import.constprop.0>:
+__Pyx_Import.constprop.0():
 	push   %r15
+	mov    %rdi,%r15
+	xor    %edi,%edi
 	push   %r14
 	push   %r13
 	push   %r12
+	xor    %r12d,%r12d
+	push   %rbp
+	call   23e0 <PyList_New@plt>
+	test   %rax,%rax
+	je     29fb <__Pyx_Import.constprop.0+0xb9>
+	mov    0x80b8(%rip),%rdi        
+	mov    %rax,%r13
+	call   2710 <PyModule_GetDict@plt>
+	mov    %rax,%r14
+	test   %rax,%rax
+	je     29d5 <__Pyx_Import.constprop.0+0x93>
+	call   2670 <PyDict_New@plt>
+	mov    %rax,%rbp
+	test   %rax,%rax
+	je     29d5 <__Pyx_Import.constprop.0+0x93>
+	mov    $0x1,%r8d
+	mov    %r13,%rcx
+	mov    %rax,%rdx
+	mov    %r14,%rsi
+	mov    %r15,%rdi
+	call   2650 <PyImport_ImportModuleLevelObject@plt>
+	mov    %rax,%r12
+	test   %rax,%rax
+	jne    29da <__Pyx_Import.constprop.0+0x98>
+	mov    0x761d(%rip),%rax        
+	mov    (%rax),%rdi
+	call   2540 <PyErr_ExceptionMatches@plt>
+	test   %eax,%eax
+	je     29da <__Pyx_Import.constprop.0+0x98>
+	call   25a0 <PyErr_Clear@plt>
+	xor    %r8d,%r8d
+	mov    %r13,%rcx
+	mov    %rbp,%rdx
+	mov    %r14,%rsi
+	mov    %r15,%rdi
+	call   2650 <PyImport_ImportModuleLevelObject@plt>
+	mov    %rax,%r12
+	jmp    29da <__Pyx_Import.constprop.0+0x98>
+	xor    %ebp,%ebp
+	xor    %r12d,%r12d
+	decq   0x0(%r13)
+	jne    29e8 <__Pyx_Import.constprop.0+0xa6>
+	mov    %r13,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	test   %rbp,%rbp
+	je     29fb <__Pyx_Import.constprop.0+0xb9>
+	decq   0x0(%rbp)
+	jne    29fb <__Pyx_Import.constprop.0+0xb9>
+	mov    %rbp,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	pop    %rbp
+	mov    %r12,%rax
+	pop    %r12
+	pop    %r13
+	pop    %r14
+	pop    %r15
+	ret
+
+0000000000002a08 <__pyx_pymod_exec_device_utils>:
+__pyx_pymod_exec_device_utils():
+	endbr64
+	push   %r13
+	push   %r12
 	push   %rbp
 	mov    %rdi,%rbp
 	push   %rbx
 	sub    $0xe8,%rsp
-	mov    0x5ebf(%rip),%rdx        
+	mov    0x7ffd(%rip),%rdx        
 	mov    %fs:0x28,%rax
 	mov    %rax,0xd8(%rsp)
 	xor    %eax,%eax
 	test   %rdx,%rdx
-	je     2980 <__pyx_pymod_exec_device_utils+0x5e>
+	je     2a62 <__pyx_pymod_exec_device_utils+0x5a>
 	cmp    %rdi,%rdx
-	je     31ae <__pyx_pymod_exec_device_utils+0x88c>
-	mov    0x560f(%rip),%rax        
-	lea    0x3730(%rip),%rsi        
+	je     32a2 <__pyx_pymod_exec_device_utils+0x89a>
+	mov    0x752d(%rip),%rax        
+	lea    0x567e(%rip),%rsi        
 	mov    (%rax),%rdi
-	call   24f0 <PyErr_SetString@plt>
+	call   2500 <PyErr_SetString@plt>
 	or     $0xffffffff,%eax
-	jmp    31ae <__pyx_pymod_exec_device_utils+0x88c>
+	jmp    32a2 <__pyx_pymod_exec_device_utils+0x89a>
 	lea    0x8(%rsp),%r13
 	mov    $0x8,%r8d
 	xor    %eax,%eax
 	mov    $0x3,%ecx
-	lea    0x38fd(%rip),%rdx        
+	lea    0x581e(%rip),%rdx        
 	mov    $0x4,%esi
 	mov    %r13,%rdi
-	call   2540 <PyOS_snprintf@plt>
+	call   2550 <PyOS_snprintf@plt>
 	lea    0xc(%rsp),%rbx
-	call   2730 <Py_GetVersion@plt>
-	lea    0x38e5(%rip),%rdx        
+	call   2750 <Py_GetVersion@plt>
+	lea    0x5806(%rip),%rdx        
 	mov    $0x4,%esi
 	mov    %rbx,%rdi
 	mov    %rax,%rcx
 	xor    %eax,%eax
-	call   2540 <PyOS_snprintf@plt>
+	call   2550 <PyOS_snprintf@plt>
 	mov    0xc(%rsp),%al
 	cmp    %al,0x8(%rsp)
-	jne    29dd <__pyx_pymod_exec_device_utils+0xbb>
+	jne    2abf <__pyx_pymod_exec_device_utils+0xb7>
 	mov    0xe(%rsp),%al
 	cmp    %al,0xa(%rsp)
-	je     2a3f <__pyx_pymod_exec_device_utils+0x11d>
+	je     2b21 <__pyx_pymod_exec_device_utils+0x119>
 	lea    0x10(%rsp),%r12
 	mov    $0xc8,%esi
 	xor    %eax,%eax
 	mov    %rbx,%r9
-	lea    0x3705(%rip),%rdx        
+	lea    0x5653(%rip),%rdx        
 	mov    %r12,%rdi
-	lea    0x38a2(%rip),%r8        
+	lea    0x57c3(%rip),%r8        
 	mov    %r13,%rcx
-	call   2540 <PyOS_snprintf@plt>
+	call   2550 <PyOS_snprintf@plt>
 	xor    %edi,%edi
 	mov    $0x1,%edx
 	mov    %r12,%rsi
-	call   2490 <PyErr_WarnEx@plt>
+	call   24a0 <PyErr_WarnEx@plt>
 	test   %eax,%eax
-	jns    2a3f <__pyx_pymod_exec_device_utils+0x11d>
-	lea    0x3729(%rip),%rax        
-	movl   $0x1,0x5dab(%rip)        
-	mov    %rax,0x5d98(%rip)        
-	movl   $0x65b,0x5d96(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
-	mov    0x557a(%rip),%rax        
+	jns    2b21 <__pyx_pymod_exec_device_utils+0x119>
+	lea    0x5677(%rip),%rax        
+	movl   $0x1,0x7ee9(%rip)        
+	mov    %rax,0x7ed6(%rip)        
+	movl   $0x747,0x7ed4(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
+	mov    0x7498(%rip),%rax        
 	xor    %edi,%edi
 	mov    0x20(%rax),%rax
 	sub    $0x8,%rax
-	mov    %rax,0x5d69(%rip)        
-	call   25c0 <PyTuple_New@plt>
-	mov    %rax,0x5d7d(%rip)        
-	test   %rax,%rax
-	jne    2a8f <__pyx_pymod_exec_device_utils+0x16d>
-	lea    0x36d9(%rip),%rax        
-	movl   $0x1,0x5d5b(%rip)        
-	mov    %rax,0x5d48(%rip)        
-	movl   $0x65f,0x5d46(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
+	mov    %rax,0x7ea7(%rip)        
+	call   25d0 <PyTuple_New@plt>
+	mov    %rax,0x7ebb(%rip)        
+	test   %rax,%rax
+	jne    2b71 <__pyx_pymod_exec_device_utils+0x169>
+	lea    0x5627(%rip),%rax        
+	movl   $0x1,0x7e99(%rip)        
+	mov    %rax,0x7e86(%rip)        
+	movl   $0x74b,0x7e84(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
 	xor    %esi,%esi
-	lea    0x3786(%rip),%rdi        
-	call   2470 <PyBytes_FromStringAndSize@plt>
-	mov    %rax,0x5d34(%rip)        
-	test   %rax,%rax
-	jne    2ad0 <__pyx_pymod_exec_device_utils+0x1ae>
-	lea    0x3698(%rip),%rax        
-	movl   $0x1,0x5d1a(%rip)        
-	mov    %rax,0x5d07(%rip)        
-	movl   $0x660,0x5d05(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
+	lea    0x571e(%rip),%rdi        
+	call   2480 <PyBytes_FromStringAndSize@plt>
+	mov    %rax,0x7e72(%rip)        
+	test   %rax,%rax
+	jne    2bb2 <__pyx_pymod_exec_device_utils+0x1aa>
+	lea    0x55e6(%rip),%rax        
+	movl   $0x1,0x7e58(%rip)        
+	mov    %rax,0x7e45(%rip)        
+	movl   $0x74c,0x7e43(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
 	xor    %esi,%esi
-	lea    0x3745(%rip),%rdi        
-	call   26e0 <PyUnicode_FromStringAndSize@plt>
+	lea    0x56dd(%rip),%rdi        
+	call   2700 <PyUnicode_FromStringAndSize@plt>
 	test   %rax,%rax
-	jne    2b0a <__pyx_pymod_exec_device_utils+0x1e8>
-	lea    0x365e(%rip),%rax        
-	movl   $0x1,0x5ce0(%rip)        
-	mov    %rax,0x5ccd(%rip)        
-	movl   $0x661,0x5ccb(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
+	jne    2bec <__pyx_pymod_exec_device_utils+0x1e4>
+	lea    0x55ac(%rip),%rax        
+	movl   $0x1,0x7e1e(%rip)        
+	mov    %rax,0x7e0b(%rip)        
+	movl   $0x74d,0x7e09(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
 	incq   0x0(%rbp)
 	mov    %rbp,%rdi
-	mov    %rbp,0x5ce8(%rip)        
-	call   26f0 <PyModule_GetDict@plt>
-	mov    %rax,0x5cd4(%rip)        
-	test   %rax,%rax
-	jne    2b50 <__pyx_pymod_exec_device_utils+0x22e>
-	lea    0x3618(%rip),%rax        
-	movl   $0x1,0x5c9a(%rip)        
-	mov    %rax,0x5c87(%rip)        
-	movl   $0x687,0x5c85(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
+	mov    %rbp,0x7e26(%rip)        
+	call   2710 <PyModule_GetDict@plt>
+	mov    %rax,0x7e12(%rip)        
+	test   %rax,%rax
+	jne    2c32 <__pyx_pymod_exec_device_utils+0x22a>
+	lea    0x5566(%rip),%rax        
+	movl   $0x1,0x7dd8(%rip)        
+	mov    %rax,0x7dc5(%rip)        
+	movl   $0x773,0x7dc3(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
 	incq   (%rax)
-	lea    0x3763(%rip),%rdi        
-	call   2460 <PyImport_AddModule@plt>
-	mov    %rax,0x5c8a(%rip)        
-	test   %rax,%rax
-	jne    2b92 <__pyx_pymod_exec_device_utils+0x270>
-	lea    0x35d6(%rip),%rax        
-	movl   $0x1,0x5c58(%rip)        
-	mov    %rax,0x5c45(%rip)        
-	movl   $0x689,0x5c43(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
-	lea    0x372d(%rip),%rdi        
-	call   2460 <PyImport_AddModule@plt>
-	mov    %rax,0x5c43(%rip)        
-	test   %rax,%rax
-	jne    2bd1 <__pyx_pymod_exec_device_utils+0x2af>
-	lea    0x3597(%rip),%rax        
-	movl   $0x1,0x5c19(%rip)        
-	mov    %rax,0x5c06(%rip)        
-	movl   $0x68a,0x5c04(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
-	mov    0x5c18(%rip),%rdx        
-	mov    0x5c21(%rip),%rdi        
-	lea    0x36ef(%rip),%rsi        
-	call   2480 <PyObject_SetAttrString@plt>
-	test   %eax,%eax
-	jns    2c16 <__pyx_pymod_exec_device_utils+0x2f4>
-	lea    0x3552(%rip),%rax        
-	movl   $0x1,0x5bd4(%rip)        
-	mov    %rax,0x5bc1(%rip)        
-	movl   $0x68e,0x5bbf(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
-	lea    0x5663(%rip),%rbx        
-	mov    (%rbx),%rbp
-	test   %rbp,%rbp
-	je     2ca2 <__pyx_pymod_exec_device_utils+0x380>
-	mov    0x20(%rbx),%al
-	or     0x21(%rbx),%al
-	mov    0x8(%rbx),%rdi
-	je     2c6b <__pyx_pymod_exec_device_utils+0x349>
-	cmpb   $0x0,0x22(%rbx)
-	je     2c42 <__pyx_pymod_exec_device_utils+0x320>
-	call   2680 <PyUnicode_InternFromString@plt>
-	mov    %rax,0x0(%rbp)
-	jmp    2c7c <__pyx_pymod_exec_device_utils+0x35a>
-	mov    0x10(%rbx),%rax
-	mov    0x18(%rbx),%rdx
+	lea    0x5684(%rip),%rdi        
+	call   2470 <PyImport_AddModule@plt>
+	mov    %rax,0x7dc8(%rip)        
+	test   %rax,%rax
+	jne    2c74 <__pyx_pymod_exec_device_utils+0x26c>
+	lea    0x5524(%rip),%rax        
+	movl   $0x1,0x7d96(%rip)        
+	mov    %rax,0x7d83(%rip)        
+	movl   $0x775,0x7d81(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
+	lea    0x564e(%rip),%rdi        
+	call   2470 <PyImport_AddModule@plt>
+	mov    %rax,0x7d81(%rip)        
+	test   %rax,%rax
+	jne    2cb3 <__pyx_pymod_exec_device_utils+0x2ab>
+	lea    0x54e5(%rip),%rax        
+	movl   $0x1,0x7d57(%rip)        
+	mov    %rax,0x7d44(%rip)        
+	movl   $0x776,0x7d42(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
+	mov    0x7d56(%rip),%rdx        
+	mov    0x7d5f(%rip),%rdi        
+	lea    0x5610(%rip),%rsi        
+	call   2490 <PyObject_SetAttrString@plt>
+	test   %eax,%eax
+	jns    2cf8 <__pyx_pymod_exec_device_utils+0x2f0>
+	lea    0x54a0(%rip),%rax        
+	movl   $0x1,0x7d12(%rip)        
+	mov    %rax,0x7cff(%rip)        
+	movl   $0x77a,0x7cfd(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
+	lea    0x7581(%rip),%rbp        
+	mov    0x0(%rbp),%rbx
+	test   %rbx,%rbx
+	je     2d7f <__pyx_pymod_exec_device_utils+0x377>
+	mov    0x20(%rbp),%al
+	or     0x21(%rbp),%al
+	mov    0x8(%rbp),%rdi
+	je     2d4b <__pyx_pymod_exec_device_utils+0x343>
+	cmpb   $0x0,0x22(%rbp)
+	je     2d24 <__pyx_pymod_exec_device_utils+0x31c>
+	call   26a0 <PyUnicode_InternFromString@plt>
+	mov    %rax,(%rbx)
+	jmp    2d5b <__pyx_pymod_exec_device_utils+0x353>
+	mov    0x10(%rbp),%rax
+	mov    0x18(%rbp),%rdx
 	lea    -0x1(%rax),%rsi
 	test   %rdx,%rdx
-	je     2c60 <__pyx_pymod_exec_device_utils+0x33e>
+	je     2d41 <__pyx_pymod_exec_device_utils+0x339>
 	xor    %ecx,%ecx
-	call   26b0 <PyUnicode_Decode@plt>
-	mov    %rax,0x0(%rbp)
-	jmp    2c7c <__pyx_pymod_exec_device_utils+0x35a>
-	call   26e0 <PyUnicode_FromStringAndSize@plt>
-	mov    %rax,0x0(%rbp)
-	jmp    2c7c <__pyx_pymod_exec_device_utils+0x35a>
-	mov    0x10(%rbx),%rax
+	call   26d0 <PyUnicode_Decode@plt>
+	mov    %rax,(%rbx)
+	jmp    2d5b <__pyx_pymod_exec_device_utils+0x353>
+	call   2700 <PyUnicode_FromStringAndSize@plt>
+	mov    %rax,(%rbx)
+	jmp    2d5b <__pyx_pymod_exec_device_utils+0x353>
+	mov    0x10(%rbp),%rax
 	lea    -0x1(%rax),%rsi
-	call   2470 <PyBytes_FromStringAndSize@plt>
-	mov    %rax,0x0(%rbp)
-	mov    (%rbx),%rax
+	call   2480 <PyBytes_FromStringAndSize@plt>
+	mov    %rax,(%rbx)
+	mov    0x0(%rbp),%rax
 	mov    (%rax),%rdi
 	test   %rdi,%rdi
-	je     2db6 <__pyx_pymod_exec_device_utils+0x494>
-	call   2640 <PyObject_Hash@plt>
+	je     2e93 <__pyx_pymod_exec_device_utils+0x48b>
+	call   2660 <PyObject_Hash@plt>
 	inc    %rax
-	je     2db6 <__pyx_pymod_exec_device_utils+0x494>
-	add    $0x28,%rbx
-	jmp    2c1d <__pyx_pymod_exec_device_utils+0x2fb>
+	je     2e93 <__pyx_pymod_exec_device_utils+0x48b>
+	add    $0x28,%rbp
+	jmp    2cff <__pyx_pymod_exec_device_utils+0x2f7>
 	mov    $0x2,%edi
-	call   2580 <PyLong_FromLong@plt>
-	mov    %rax,0x5a5d(%rip)        
+	call   2590 <PyLong_FromLong@plt>
+	mov    %rax,0x7b48(%rip)        
 	test   %rax,%rax
-	je     2db6 <__pyx_pymod_exec_device_utils+0x494>
+	je     2e93 <__pyx_pymod_exec_device_utils+0x48b>
 	mov    $0xfffffffffffffff4,%rdi
-	call   2580 <PyLong_FromLong@plt>
-	mov    %rax,0x5a39(%rip)        
+	call   2590 <PyLong_FromLong@plt>
+	mov    %rax,0x7b24(%rip)        
 	test   %rax,%rax
-	je     2db6 <__pyx_pymod_exec_device_utils+0x494>
-	mov    0x52f9(%rip),%rax        
+	je     2e93 <__pyx_pymod_exec_device_utils+0x48b>
+	mov    0x721c(%rip),%rax        
 	cmpl   $0x0,(%rax)
-	je     2ddd <__pyx_pymod_exec_device_utils+0x4bb>
-	mov    0x5a61(%rip),%rdx        
-	mov    0x5a52(%rip),%rsi        
-	mov    0x5b03(%rip),%rdi        
-	call   25e0 <PyObject_SetAttr@plt>
-	test   %eax,%eax
-	jns    2ddd <__pyx_pymod_exec_device_utils+0x4bb>
-	lea    0x3437(%rip),%rax        
-	movl   $0x1,0x5ab9(%rip)        
-	mov    %rax,0x5aa6(%rip)        
-	movl   $0x695,0x5aa4(%rip)        
-	cmpq   $0x0,0x5acc(%rip)        
-	je     2d82 <__pyx_pymod_exec_device_utils+0x460>
-	cmpq   $0x0,0x5aba(%rip)        
-	je     2d5f <__pyx_pymod_exec_device_utils+0x43d>
-	mov    0x5a81(%rip),%rcx        
-	mov    0x5a87(%rip),%edx        
-	lea    0x341c(%rip),%rdi        
-	mov    0x5a76(%rip),%esi        
-	call   33e0 <__Pyx_AddTraceback>
-	mov    0x5a9a(%rip),%rdi        
+	je     2eba <__pyx_pymod_exec_device_utils+0x4b2>
+	mov    0x7b84(%rip),%rdx        
+	mov    0x7b75(%rip),%rsi        
+	mov    0x7c46(%rip),%rdi        
+	call   25f0 <PyObject_SetAttr@plt>
+	test   %eax,%eax
+	jns    2eba <__pyx_pymod_exec_device_utils+0x4b2>
+	lea    0x538a(%rip),%rax        
+	movl   $0x1,0x7bfc(%rip)        
+	mov    %rax,0x7be9(%rip)        
+	movl   $0x781,0x7be7(%rip)        
+	cmpq   $0x0,0x7c0f(%rip)        
+	je     2e5f <__pyx_pymod_exec_device_utils+0x457>
+	cmpq   $0x0,0x7bfd(%rip)        
+	je     2e3c <__pyx_pymod_exec_device_utils+0x434>
+	mov    0x7bc4(%rip),%rcx        
+	mov    0x7bca(%rip),%edx        
+	lea    0x536f(%rip),%rdi        
+	mov    0x7bb9(%rip),%esi        
+	call   3c50 <__Pyx_AddTraceback>
+	mov    0x7bdd(%rip),%rdi        
 	test   %rdi,%rdi
-	je     2da2 <__pyx_pymod_exec_device_utils+0x480>
+	je     2e7f <__pyx_pymod_exec_device_utils+0x477>
 	decq   (%rdi)
-	movq   $0x0,0x5a87(%rip)        
-	jne    2da2 <__pyx_pymod_exec_device_utils+0x480>
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    2da2 <__pyx_pymod_exec_device_utils+0x480>
-	call   25f0 <PyErr_Occurred@plt>
-	test   %rax,%rax
-	jne    2da2 <__pyx_pymod_exec_device_utils+0x480>
-	mov    0x5235(%rip),%rax        
-	lea    0x33d6(%rip),%rsi        
+	movq   $0x0,0x7bca(%rip)        
+	jne    2e7f <__pyx_pymod_exec_device_utils+0x477>
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    2e7f <__pyx_pymod_exec_device_utils+0x477>
+	call   2600 <PyErr_Occurred@plt>
+	test   %rax,%rax
+	jne    2e7f <__pyx_pymod_exec_device_utils+0x477>
+	mov    0x7158(%rip),%rax        
+	lea    0x5329(%rip),%rsi        
 	mov    (%rax),%rdi
-	call   24f0 <PyErr_SetString@plt>
+	call   2500 <PyErr_SetString@plt>
 	xor    %eax,%eax
-	cmpq   $0x0,0x5a54(%rip)        
+	cmpq   $0x0,0x7b97(%rip)        
 	sete   %al
 	neg    %eax
-	jmp    31ae <__pyx_pymod_exec_device_utils+0x88c>
-	lea    0x338b(%rip),%rax        
-	movl   $0x1,0x5a0d(%rip)        
-	mov    %rax,0x59fa(%rip)        
-	movl   $0x690,0x59f8(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
-	call   24d0 <PyImport_GetModuleDict@plt>
-	mov    %rax,%r12
-	test   %rax,%rax
-	jne    2e11 <__pyx_pymod_exec_device_utils+0x4ef>
-	lea    0x3357(%rip),%rax        
-	movl   $0x1,0x59d9(%rip)        
-	mov    %rax,0x59c6(%rip)        
-	movl   $0x699,0x59c4(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
-	lea    0x3487(%rip),%rsi        
+	jmp    32a2 <__pyx_pymod_exec_device_utils+0x89a>
+	lea    0x52de(%rip),%rax        
+	movl   $0x1,0x7b50(%rip)        
+	mov    %rax,0x7b3d(%rip)        
+	movl   $0x77c,0x7b3b(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
+	call   24e0 <PyImport_GetModuleDict@plt>
+	mov    %rax,%rbp
+	test   %rax,%rax
+	jne    2eee <__pyx_pymod_exec_device_utils+0x4e6>
+	lea    0x52aa(%rip),%rax        
+	movl   $0x1,0x7b1c(%rip)        
+	mov    %rax,0x7b09(%rip)        
+	movl   $0x785,0x7b07(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
+	lea    0x53ad(%rip),%rsi        
 	mov    %rax,%rdi
-	call   2610 <PyDict_GetItemString@plt>
+	call   2620 <PyDict_GetItemString@plt>
+	test   %rax,%rax
+	jne    2f43 <__pyx_pymod_exec_device_utils+0x53b>
+	mov    0x7b17(%rip),%rdx        
+	lea    0x5392(%rip),%rsi        
+	mov    %rbp,%rdi
+	call   23f0 <PyDict_SetItemString@plt>
+	test   %eax,%eax
+	jns    2f43 <__pyx_pymod_exec_device_utils+0x53b>
+	lea    0x5255(%rip),%rax        
+	movl   $0x1,0x7ac7(%rip)        
+	mov    %rax,0x7ab4(%rip)        
+	movl   $0x787,0x7ab2(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
+	mov    0x79d6(%rip),%rdi        
+	call   3640 <__Pyx_GetBuiltinName>
+	test   %rax,%rax
+	jne    2f7b <__pyx_pymod_exec_device_utils+0x573>
+	lea    0x521d(%rip),%rax        
+	movl   $0x1,0x7a8f(%rip)        
+	mov    %rax,0x7a7c(%rip)        
+	movl   $0x78c,0x7a7a(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
+	mov    0x7a2e(%rip),%rdx        
+	mov    0x7a37(%rip),%rsi        
+	mov    $0x2,%edi
+	xor    %eax,%eax
+	call   2740 <PyTuple_Pack@plt>
+	mov    %rax,0x7924(%rip)        
 	test   %rax,%rax
-	jne    2e66 <__pyx_pymod_exec_device_utils+0x544>
-	mov    0x59d4(%rip),%rdx        
-	lea    0x346c(%rip),%rsi        
-	mov    %r12,%rdi
-	call   23e0 <PyDict_SetItemString@plt>
-	test   %eax,%eax
-	jns    2e66 <__pyx_pymod_exec_device_utils+0x544>
-	lea    0x3302(%rip),%rax        
-	movl   $0x1,0x5984(%rip)        
-	mov    %rax,0x5971(%rip)        
-	movl   $0x69b,0x596f(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
-	mov    0x58c3(%rip),%rdi        
-	call   3b40 <__Pyx_GetBuiltinName>
-	test   %rax,%rax
-	jne    2e9e <__pyx_pymod_exec_device_utils+0x57c>
-	lea    0x32ca(%rip),%rax        
-	movl   $0x1,0x594c(%rip)        
-	mov    %rax,0x5939(%rip)        
-	movl   $0x6a0,0x5937(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
-	mov    0x50fb(%rip),%rsi        
-	mov    0x585c(%rip),%rdi        
+	je     306f <__pyx_pymod_exec_device_utils+0x667>
+	mov    0x6ff4(%rip),%rsi        
+	mov    0x791d(%rip),%rdi        
 	mov    %rsi,%rdx
-	call   26d0 <PySlice_New@plt>
-	mov    %rax,0x5845(%rip)        
+	call   26f0 <PySlice_New@plt>
+	mov    %rax,0x7906(%rip)        
 	test   %rax,%rax
-	je     2f67 <__pyx_pymod_exec_device_utils+0x645>
-	mov    0x58c5(%rip),%rdx        
-	mov    0x5886(%rip),%rsi        
+	je     306f <__pyx_pymod_exec_device_utils+0x667>
+	mov    0x79c6(%rip),%rcx        
+	mov    0x797f(%rip),%rdx        
 	xor    %eax,%eax
-	mov    $0x2,%edi
-	call   2720 <PyTuple_Pack@plt>
-	test   %rax,%rax
-	je     2f67 <__pyx_pymod_exec_device_utils+0x645>
-	mov    0x58f2(%rip),%rdx        
-	mov    0x58e3(%rip),%r9        
+	mov    $0x3,%edi
+	mov    0x7921(%rip),%rsi        
+	call   2740 <PyTuple_Pack@plt>
+	test   %rax,%rax
+	je     306f <__pyx_pymod_exec_device_utils+0x667>
+	mov    0x7a08(%rip),%rdx        
+	mov    0x79f9(%rip),%r9        
 	push   %rcx
 	mov    $0x3,%r8d
 	xor    %ecx,%ecx
 	xor    %esi,%esi
 	xor    %edi,%edi
 	push   %r9
-	push   $0x4
-	push   0x587c(%rip)        
-	push   0x5826(%rip)        
+	push   $0x5
+	push   0x797a(%rip)        
+	push   0x790c(%rip)        
 	push   %rdx
 	push   %rdx
 	push   %rax
 	push   %rdx
 	push   %rdx
-	mov    $0x2,%edx
-	call   24c0 <PyCode_New@plt>
+	mov    $0x3,%edx
+	call   24d0 <PyCode_New@plt>
 	add    $0x50,%rsp
 	test   %rax,%rax
-	je     2f67 <__pyx_pymod_exec_device_utils+0x645>
-	xor    %edi,%edi
-	mov    0x57e5(%rip),%r15        
-	call   23d0 <PyList_New@plt>
-	mov    %rax,%r13
-	test   %rax,%rax
-	jne    2f8e <__pyx_pymod_exec_device_utils+0x66c>
-	lea    0x3201(%rip),%rax        
-	movl   $0x1,0x5883(%rip)        
-	mov    %rax,0x5870(%rip)        
-	movl   $0x6b5,0x586e(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
-	lea    0x31da(%rip),%rax        
-	movl   $0x1,0x585c(%rip)        
-	mov    %rax,0x5849(%rip)        
-	movl   $0x6a2,0x5847(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
-	mov    0x586b(%rip),%rdi        
-	call   26f0 <PyModule_GetDict@plt>
-	mov    %rax,%r14
-	test   %rax,%rax
-	je     2fff <__pyx_pymod_exec_device_utils+0x6dd>
-	call   2650 <PyDict_New@plt>
-	mov    %rax,%r12
-	test   %rax,%rax
-	je     2fff <__pyx_pymod_exec_device_utils+0x6dd>
-	mov    $0x1,%r8d
-	mov    %r13,%rcx
-	mov    %rax,%rdx
-	mov    %r14,%rsi
-	mov    %r15,%rdi
-	call   2630 <PyImport_ImportModuleLevelObject@plt>
+	je     306f <__pyx_pymod_exec_device_utils+0x667>
+	mov    0x7905(%rip),%rdi        
+	call   2942 <__Pyx_Import.constprop.0>
 	mov    %rax,%rbp
 	test   %rax,%rax
-	jne    3002 <__pyx_pymod_exec_device_utils+0x6e0>
-	mov    0x4ff3(%rip),%rax        
-	mov    (%rax),%rdi
-	call   2530 <PyErr_ExceptionMatches@plt>
+	jne    3096 <__pyx_pymod_exec_device_utils+0x68e>
+	lea    0x5129(%rip),%rax        
+	movl   $0x1,0x799b(%rip)        
+	mov    %rax,0x7988(%rip)        
+	movl   $0x7a1,0x7986(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
+	lea    0x5102(%rip),%rax        
+	movl   $0x1,0x7974(%rip)        
+	mov    %rax,0x7961(%rip)        
+	movl   $0x78e,0x795f(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
+	mov    0x78a3(%rip),%rsi        
+	mov    0x7974(%rip),%rdi        
+	mov    %rax,%rdx
+	call   26b0 <PyDict_SetItem@plt>
 	test   %eax,%eax
-	je     3002 <__pyx_pymod_exec_device_utils+0x6e0>
-	call   2590 <PyErr_Clear@plt>
-	xor    %r8d,%r8d
-	mov    %r13,%rcx
-	mov    %r12,%rdx
-	mov    %r14,%rsi
-	mov    %r15,%rdi
-	call   2630 <PyImport_ImportModuleLevelObject@plt>
+	jns    30d7 <__pyx_pymod_exec_device_utils+0x6cf>
+	lea    0x50c1(%rip),%rax        
+	movl   $0x1,0x7933(%rip)        
+	mov    %rax,0x7920(%rip)        
+	movl   $0x7a3,0x791e(%rip)        
+	jmp    328b <__pyx_pymod_exec_device_utils+0x883>
+	decq   0x0(%rbp)
+	jne    30e5 <__pyx_pymod_exec_device_utils+0x6dd>
+	mov    %rbp,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x77f4(%rip),%rdi        
+	call   2942 <__Pyx_Import.constprop.0>
 	mov    %rax,%rbp
-	jmp    3002 <__pyx_pymod_exec_device_utils+0x6e0>
-	xor    %r12d,%r12d
-	decq   0x0(%r13)
-	jne    3010 <__pyx_pymod_exec_device_utils+0x6ee>
-	mov    %r13,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	test   %r12,%r12
-	je     3023 <__pyx_pymod_exec_device_utils+0x701>
-	decq   (%r12)
-	jne    3023 <__pyx_pymod_exec_device_utils+0x701>
-	mov    %r12,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	test   %rbp,%rbp
-	je     2f40 <__pyx_pymod_exec_device_utils+0x61e>
-	mov    0x56e5(%rip),%rsi        
-	mov    0x57be(%rip),%rdi        
-	mov    %rbp,%rdx
-	call   2690 <PyDict_SetItem@plt>
+	test   %rax,%rax
+	jne    3120 <__pyx_pymod_exec_device_utils+0x718>
+	lea    0x5078(%rip),%rax        
+	movl   $0x2,0x78ea(%rip)        
+	mov    %rax,0x78d7(%rip)        
+	movl   $0x7ac,0x78d5(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
+	mov    0x77b9(%rip),%rsi        
+	mov    0x78ea(%rip),%rdi        
+	mov    %rax,%rdx
+	call   26b0 <PyDict_SetItem@plt>
 	test   %eax,%eax
-	jns    306d <__pyx_pymod_exec_device_utils+0x74b>
-	lea    0x30fb(%rip),%rax        
-	movl   $0x1,0x577d(%rip)        
-	mov    %rax,0x576a(%rip)        
-	movl   $0x6b7,0x5768(%rip)        
-	jmp    3197 <__pyx_pymod_exec_device_utils+0x875>
+	jns    3161 <__pyx_pymod_exec_device_utils+0x759>
+	lea    0x5037(%rip),%rax        
+	movl   $0x2,0x78a9(%rip)        
+	mov    %rax,0x7896(%rip)        
+	movl   $0x7ae,0x7894(%rip)        
+	jmp    328b <__pyx_pymod_exec_device_utils+0x883>
 	decq   0x0(%rbp)
-	jne    307b <__pyx_pymod_exec_device_utils+0x759>
+	jne    316f <__pyx_pymod_exec_device_utils+0x767>
 	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	mov    0x56be(%rip),%rdx        
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x77ba(%rip),%rdx        
 	xor    %esi,%esi
-	lea    0x55d5(%rip),%rdi        
-	call   2420 <PyCFunction_NewEx@plt>
+	lea    0x7681(%rip),%rdi        
+	call   2430 <PyCFunction_NewEx@plt>
 	mov    %rax,%rbp
 	test   %rax,%rax
-	jne    30bf <__pyx_pymod_exec_device_utils+0x79d>
-	lea    0x30a9(%rip),%rax        
-	movl   $0x4,0x572b(%rip)        
-	mov    %rax,0x5718(%rip)        
-	movl   $0x6c1,0x5716(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
-	mov    0x56c2(%rip),%rsi        
-	mov    0x572b(%rip),%rdi        
+	jne    31b3 <__pyx_pymod_exec_device_utils+0x7ab>
+	lea    0x4fe5(%rip),%rax        
+	movl   $0x5,0x7857(%rip)        
+	mov    %rax,0x7844(%rip)        
+	movl   $0x7b8,0x7842(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
+	mov    0x77d6(%rip),%rsi        
+	mov    0x7857(%rip),%rdi        
 	mov    %rax,%rdx
-	call   2690 <PyDict_SetItem@plt>
+	call   26b0 <PyDict_SetItem@plt>
 	test   %eax,%eax
-	jns    3100 <__pyx_pymod_exec_device_utils+0x7de>
-	lea    0x3068(%rip),%rax        
-	movl   $0x4,0x56ea(%rip)        
-	mov    %rax,0x56d7(%rip)        
-	movl   $0x6c3,0x56d5(%rip)        
-	jmp    3197 <__pyx_pymod_exec_device_utils+0x875>
+	jns    31f4 <__pyx_pymod_exec_device_utils+0x7ec>
+	lea    0x4fa4(%rip),%rax        
+	movl   $0x5,0x7816(%rip)        
+	mov    %rax,0x7803(%rip)        
+	movl   $0x7ba,0x7801(%rip)        
+	jmp    328b <__pyx_pymod_exec_device_utils+0x883>
 	decq   0x0(%rbp)
-	jne    310e <__pyx_pymod_exec_device_utils+0x7ec>
+	jne    3202 <__pyx_pymod_exec_device_utils+0x7fa>
 	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	call   2650 <PyDict_New@plt>
+	call   24b0 <_Py_Dealloc@plt>
+	call   2670 <PyDict_New@plt>
 	mov    %rax,%rbp
 	test   %rax,%rax
-	jne    3142 <__pyx_pymod_exec_device_utils+0x820>
-	lea    0x3026(%rip),%rax        
-	movl   $0x1,0x56a8(%rip)        
-	mov    %rax,0x5695(%rip)        
-	movl   $0x6cb,0x5693(%rip)        
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
-	mov    0x55df(%rip),%rsi        
-	mov    0x56a8(%rip),%rdi        
+	jne    3236 <__pyx_pymod_exec_device_utils+0x82e>
+	lea    0x4f62(%rip),%rax        
+	movl   $0x1,0x77d4(%rip)        
+	mov    %rax,0x77c1(%rip)        
+	movl   $0x7c2,0x77bf(%rip)        
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
+	mov    0x76b3(%rip),%rsi        
+	mov    0x77d4(%rip),%rdi        
 	mov    %rax,%rdx
-	call   2690 <PyDict_SetItem@plt>
+	call   26b0 <PyDict_SetItem@plt>
 	test   %eax,%eax
-	jns    3180 <__pyx_pymod_exec_device_utils+0x85e>
-	lea    0x2fe5(%rip),%rax        
-	movl   $0x1,0x5667(%rip)        
-	mov    %rax,0x5654(%rip)        
-	movl   $0x6cd,0x5652(%rip)        
-	jmp    3197 <__pyx_pymod_exec_device_utils+0x875>
+	jns    3274 <__pyx_pymod_exec_device_utils+0x86c>
+	lea    0x4f21(%rip),%rax        
+	movl   $0x1,0x7793(%rip)        
+	mov    %rax,0x7780(%rip)        
+	movl   $0x7c4,0x777e(%rip)        
+	jmp    328b <__pyx_pymod_exec_device_utils+0x883>
 	decq   0x0(%rbp)
-	jne    2da2 <__pyx_pymod_exec_device_utils+0x480>
+	jne    2e7f <__pyx_pymod_exec_device_utils+0x477>
 	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    2da2 <__pyx_pymod_exec_device_utils+0x480>
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    2e7f <__pyx_pymod_exec_device_utils+0x477>
 	decq   0x0(%rbp)
-	jne    2d2c <__pyx_pymod_exec_device_utils+0x40a>
+	jne    2e09 <__pyx_pymod_exec_device_utils+0x401>
 	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    2d2c <__pyx_pymod_exec_device_utils+0x40a>
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    2e09 <__pyx_pymod_exec_device_utils+0x401>
 	mov    0xd8(%rsp),%rcx
 	xor    %fs:0x28,%rcx
-	je     31c6 <__pyx_pymod_exec_device_utils+0x8a4>
-	call   24e0 <__stack_chk_fail@plt>
+	je     32ba <__pyx_pymod_exec_device_utils+0x8b2>
+	call   24f0 <__stack_chk_fail@plt>
 	add    $0xe8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
-	pop    %r14
-	pop    %r15
 	ret
 
-00000000000031d8 <PyInit_device_utils>:
+00000000000032c8 <PyInit_device_utils>:
 PyInit_device_utils():
 	endbr64
-	lea    0x53bd(%rip),%rdi        
-	jmp    2400 <PyModuleDef_Init@plt>
+	lea    0x746d(%rip),%rdi        
+	jmp    2410 <PyModuleDef_Init@plt>
 	nopl   0x0(%rax,%rax,1)
 
-00000000000031f0 <deregister_tm_clones>:
+00000000000032e0 <deregister_tm_clones>:
 deregister_tm_clones():
-	lea    0x5489(%rip),%rdi        
-	lea    0x5482(%rip),%rax        
+	lea    0x7539(%rip),%rdi        
+	lea    0x7532(%rip),%rax        
 	cmp    %rdi,%rax
-	je     3218 <deregister_tm_clones+0x28>
-	mov    0x4d5e(%rip),%rax        
+	je     3308 <deregister_tm_clones+0x28>
+	mov    0x6c6e(%rip),%rax        
 	test   %rax,%rax
-	je     3218 <deregister_tm_clones+0x28>
+	je     3308 <deregister_tm_clones+0x28>
 	jmp    *%rax
 	nopl   0x0(%rax)
 	ret
 	nopl   0x0(%rax)
 
-0000000000003220 <register_tm_clones>:
+0000000000003310 <register_tm_clones>:
 register_tm_clones():
-	lea    0x5459(%rip),%rdi        
-	lea    0x5452(%rip),%rsi        
+	lea    0x7509(%rip),%rdi        
+	lea    0x7502(%rip),%rsi        
 	sub    %rdi,%rsi
 	mov    %rsi,%rax
 	shr    $0x3f,%rsi
 	sar    $0x3,%rax
 	add    %rax,%rsi
 	sar    %rsi
-	je     3258 <register_tm_clones+0x38>
-	mov    0x4d9d(%rip),%rax        
+	je     3348 <register_tm_clones+0x38>
+	mov    0x6cad(%rip),%rax        
 	test   %rax,%rax
-	je     3258 <register_tm_clones+0x38>
+	je     3348 <register_tm_clones+0x38>
 	jmp    *%rax
 	nopw   0x0(%rax,%rax,1)
 	ret
 	nopl   0x0(%rax)
 
-0000000000003260 <__do_global_dtors_aux>:
+0000000000003350 <__do_global_dtors_aux>:
 __do_global_dtors_aux():
 	endbr64
-	cmpb   $0x0,0x5415(%rip)        
-	jne    3298 <__do_global_dtors_aux+0x38>
+	cmpb   $0x0,0x74c5(%rip)        
+	jne    3388 <__do_global_dtors_aux+0x38>
 	push   %rbp
-	cmpq   $0x0,0x4d82(%rip)        
+	cmpq   $0x0,0x6c92(%rip)        
 	mov    %rsp,%rbp
-	je     3287 <__do_global_dtors_aux+0x27>
-	mov    0x4f5e(%rip),%rdi        
-	call   23b0 <__cxa_finalize@plt>
-	call   31f0 <deregister_tm_clones>
-	movb   $0x1,0x53ed(%rip)        
+	je     3377 <__do_global_dtors_aux+0x27>
+	mov    0x6e6e(%rip),%rdi        
+	call   23c0 <__cxa_finalize@plt>
+	call   32e0 <deregister_tm_clones>
+	movb   $0x1,0x749d(%rip)        
 	pop    %rbp
 	ret
 	nopl   (%rax)
 	ret
 	nopl   0x0(%rax)
 
-00000000000032a0 <frame_dummy>:
+0000000000003390 <frame_dummy>:
 frame_dummy():
 	endbr64
-	jmp    3220 <register_tm_clones>
+	jmp    3310 <register_tm_clones>
 	nopl   0x0(%rax)
 
-00000000000032b0 <__pyx_bisect_code_objects>:
+00000000000033a0 <__pyx_bisect_code_objects>:
 __pyx_bisect_code_objects():
 	mov    %esi,%r8d
 	mov    %esi,%eax
 	sub    $0x1,%r8d
-	js     3320 <__pyx_bisect_code_objects+0x70>
+	js     3410 <__pyx_bisect_code_objects+0x70>
 	movslq %r8d,%rcx
 	shl    $0x4,%rcx
 	cmp    %edx,0x8(%rdi,%rcx,1)
-	jl     3318 <__pyx_bisect_code_objects+0x68>
+	jl     3408 <__pyx_bisect_code_objects+0x68>
 	test   %r8d,%r8d
-	jle    3320 <__pyx_bisect_code_objects+0x70>
+	jle    3410 <__pyx_bisect_code_objects+0x70>
 	xor    %esi,%esi
-	jmp    32e2 <__pyx_bisect_code_objects+0x32>
+	jmp    33d2 <__pyx_bisect_code_objects+0x32>
 	nopl   0x0(%rax)
-	jge    3313 <__pyx_bisect_code_objects+0x63>
+	jge    3403 <__pyx_bisect_code_objects+0x63>
 	lea    0x1(%rax),%esi
 	cmp    %esi,%r8d
-	jle    3309 <__pyx_bisect_code_objects+0x59>
+	jle    33f9 <__pyx_bisect_code_objects+0x59>
 	mov    %r8d,%ecx
 	sub    %esi,%ecx
 	mov    %ecx,%eax
 	shr    $0x1f,%eax
 	add    %ecx,%eax
 	sar    %eax
 	add    %esi,%eax
 	movslq %eax,%rcx
 	shl    $0x4,%rcx
 	mov    0x8(%rdi,%rcx,1),%ecx
 	cmp    %edx,%ecx
-	jle    32d8 <__pyx_bisect_code_objects+0x28>
+	jle    33c8 <__pyx_bisect_code_objects+0x28>
 	mov    %eax,%r8d
 	cmp    %esi,%r8d
-	jg     32e2 <__pyx_bisect_code_objects+0x32>
+	jg     33d2 <__pyx_bisect_code_objects+0x32>
 	cmp    %ecx,%edx
 	setg   %dl
 	movzbl %dl,%edx
 	add    %edx,%eax
 	ret
 	nopl   0x0(%rax)
 	ret
 	nopl   0x0(%rax)
 	mov    0x8(%rdi),%ecx
 	xor    %eax,%eax
-	jmp    3309 <__pyx_bisect_code_objects+0x59>
+	jmp    33f9 <__pyx_bisect_code_objects+0x59>
 	nopw   0x0(%rax,%rax,1)
 
-0000000000003330 <__Pyx_PyFunction_FastCallNoKw>:
+0000000000003420 <__Pyx_PyFunction_FastCallNoKw>:
 __Pyx_PyFunction_FastCallNoKw():
 	push   %r14
 	mov    %rcx,%r14
 	push   %r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	mov    %rsi,%rbp
 	push   %rbx
 	mov    %rdx,%rbx
-	call   23f0 <_PyThreadState_UncheckedGet@plt>
+	call   2400 <_PyThreadState_UncheckedGet@plt>
 	xor    %ecx,%ecx
 	mov    %r14,%rdx
 	mov    %r12,%rsi
 	mov    %rax,%rdi
 	mov    %rax,%r13
-	call   2410 <PyFrame_New@plt>
+	call   2420 <PyFrame_New@plt>
 	test   %rax,%rax
-	je     33d1 <__Pyx_PyFunction_FastCallNoKw+0xa1>
-	mov    0x5458(%rip),%rcx        
+	je     34c1 <__Pyx_PyFunction_FastCallNoKw+0xa1>
+	mov    0x7588(%rip),%rcx        
 	mov    %rax,%r12
 	xor    %eax,%eax
 	add    %r12,%rcx
 	test   %rbx,%rbx
-	jle    338e <__Pyx_PyFunction_FastCallNoKw+0x5e>
+	jle    347e <__Pyx_PyFunction_FastCallNoKw+0x5e>
 	nopl   (%rax)
 	mov    0x0(%rbp,%rax,8),%rdx
 	addq   $0x1,(%rdx)
 	mov    %rdx,(%rcx,%rax,8)
 	add    $0x1,%rax
 	cmp    %rax,%rbx
-	jne    3378 <__Pyx_PyFunction_FastCallNoKw+0x48>
+	jne    3468 <__Pyx_PyFunction_FastCallNoKw+0x48>
 	xor    %esi,%esi
 	mov    %r12,%rdi
-	call   2510 <PyEval_EvalFrameEx@plt>
+	call   2520 <PyEval_EvalFrameEx@plt>
 	mov    %rax,%r14
 	mov    0x20(%r13),%eax
 	lea    0x1(%rax),%edx
 	mov    %edx,0x20(%r13)
 	subq   $0x1,(%r12)
-	je     33c0 <__Pyx_PyFunction_FastCallNoKw+0x90>
+	je     34b0 <__Pyx_PyFunction_FastCallNoKw+0x90>
 	mov    %eax,0x20(%r13)
 	pop    %rbx
 	mov    %r14,%rax
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	ret
 	nopl   (%rax)
 	mov    %r12,%rdi
-	call   24a0 <_Py_Dealloc@plt>
+	call   24b0 <_Py_Dealloc@plt>
 	mov    0x20(%r13),%eax
 	sub    $0x1,%eax
-	jmp    33ad <__Pyx_PyFunction_FastCallNoKw+0x7d>
+	jmp    349d <__Pyx_PyFunction_FastCallNoKw+0x7d>
 	xor    %r14d,%r14d
-	jmp    33b1 <__Pyx_PyFunction_FastCallNoKw+0x81>
+	jmp    34a1 <__Pyx_PyFunction_FastCallNoKw+0x81>
+	cs nopw 0x0(%rax,%rax,1)
+
+00000000000034d0 <__Pyx_PyFunction_FastCallDict.constprop.0>:
+__Pyx_PyFunction_FastCallDict.constprop.0():
+	push   %r15
+	push   %r14
+	push   %r13
+	push   %r12
+	mov    %rsi,%r12
+	push   %rbp
+	mov    %edx,%ebp
+	push   %rbx
+	mov    %rdi,%rbx
+	sub    $0x8,%rsp
+	mov    0x10(%rdi),%r15
+	mov    0x18(%rdi),%r14
+	mov    0x20(%rdi),%r13
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%ecx
+	lea    0x1(%rcx),%edx
+	mov    %edx,0x20(%rax)
+	mov    0x6a81(%rip),%rax        
+	cmp    (%rax),%edx
+	jg     35b8 <__Pyx_PyFunction_FastCallDict.constprop.0+0xe8>
+	mov    0x18(%r15),%eax
+	test   %eax,%eax
+	jne    3522 <__Pyx_PyFunction_FastCallDict.constprop.0+0x52>
+	cmpl   $0x43,0x24(%r15)
+	je     35d8 <__Pyx_PyFunction_FastCallDict.constprop.0+0x108>
+	mov    0x30(%rbx),%rcx
+	mov    0x28(%rbx),%rdx
+	xor    %eax,%eax
+	test   %r13,%r13
+	je     3539 <__Pyx_PyFunction_FastCallDict.constprop.0+0x69>
+	mov    0x10(%r13),%rax
+	add    $0x18,%r13
+	sub    $0x8,%rsp
+	xor    %r9d,%r9d
+	mov    %ebp,%r8d
+	mov    %r14,%rsi
+	push   %rcx
+	mov    %r15,%rdi
+	mov    %r12,%rcx
+	push   %rdx
+	xor    %edx,%edx
+	push   %rax
+	push   %r13
+	push   $0x0
+	call   2630 <PyEval_EvalCodeEx@plt>
+	add    $0x30,%rsp
+	mov    %rax,%r12
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%esi
+	lea    -0x1(%rsi),%edx
+	mov    %edx,0x20(%rax)
+	mov    0x6a12(%rip),%rax        
+	mov    (%rax),%eax
+	cmp    $0xc8,%eax
+	jg     35a0 <__Pyx_PyFunction_FastCallDict.constprop.0+0xd0>
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%eax
+	cmp    %eax,%edx
+	jl     35a7 <__Pyx_PyFunction_FastCallDict.constprop.0+0xd7>
+	add    $0x8,%rsp
+	mov    %r12,%rax
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
+	pop    %r14
+	pop    %r15
+	ret
+	nopl   0x0(%rax,%rax,1)
+	sub    $0x32,%eax
+	cmp    %eax,%edx
+	jge    3589 <__Pyx_PyFunction_FastCallDict.constprop.0+0xb9>
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	jmp    3589 <__Pyx_PyFunction_FastCallDict.constprop.0+0xb9>
+	nopw   0x0(%rax,%rax,1)
+	lea    0x4aa1(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     350f <__Pyx_PyFunction_FastCallDict.constprop.0+0x3f>
+	xor    %r12d,%r12d
+	jmp    3589 <__Pyx_PyFunction_FastCallDict.constprop.0+0xb9>
+	nopl   0x0(%rax)
+	test   %r13,%r13
+	je     3600 <__Pyx_PyFunction_FastCallDict.constprop.0+0x130>
+	mov    0x10(%r13),%rax
+	add    $0x18,%r13
+	test   %ebp,%ebp
+	jne    35f2 <__Pyx_PyFunction_FastCallDict.constprop.0+0x122>
+	movslq 0x10(%r15),%rdx
+	cmp    %rax,%rdx
+	je     361f <__Pyx_PyFunction_FastCallDict.constprop.0+0x14f>
+	mov    0x30(%rbx),%rcx
+	mov    0x28(%rbx),%rdx
+	jmp    3539 <__Pyx_PyFunction_FastCallDict.constprop.0+0x69>
+	nop
+	cmp    %ebp,0x10(%r15)
+	jne    35f2 <__Pyx_PyFunction_FastCallDict.constprop.0+0x122>
+	mov    %r12,%rsi
+	movslq %ebp,%rdx
+	mov    %r14,%rcx
+	mov    %r15,%rdi
+	call   3420 <__Pyx_PyFunction_FastCallNoKw>
+	mov    %rax,%r12
+	jmp    3561 <__Pyx_PyFunction_FastCallDict.constprop.0+0x91>
+	mov    %r14,%rcx
+	mov    %r13,%rsi
+	mov    %r15,%rdi
+	call   3420 <__Pyx_PyFunction_FastCallNoKw>
+	mov    %rax,%r12
+	jmp    3561 <__Pyx_PyFunction_FastCallDict.constprop.0+0x91>
+	data16 cs nopw 0x0(%rax,%rax,1)
+
+0000000000003640 <__Pyx_GetBuiltinName>:
+__Pyx_GetBuiltinName():
+	push   %r13
+	mov    %rdi,%r13
+	push   %r12
+	mov    %r13,%rsi
+	sub    $0x8,%rsp
+	mov    0x73bb(%rip),%rdi        
+	mov    0x8(%rdi),%rax
+	mov    0x90(%rax),%rax
+	test   %rax,%rax
+	je     3680 <__Pyx_GetBuiltinName+0x40>
+	call   *%rax
+	mov    %rax,%r12
+	test   %r12,%r12
+	je     368d <__Pyx_GetBuiltinName+0x4d>
+	add    $0x8,%rsp
+	mov    %r12,%rax
+	pop    %r12
+	pop    %r13
+	ret
+	nopl   0x0(%rax,%rax,1)
+	call   2720 <PyObject_GetAttr@plt>
+	mov    %rax,%r12
+	test   %r12,%r12
+	jne    366f <__Pyx_GetBuiltinName+0x2f>
+	mov    0x694c(%rip),%rax        
+	mov    %r13,%rdx
+	lea    0x4bd7(%rip),%rsi        
+	mov    (%rax),%rdi
+	xor    %eax,%eax
+	call   26e0 <PyErr_Format@plt>
+	add    $0x8,%rsp
+	mov    %r12,%rax
+	pop    %r12
+	pop    %r13
+	ret
+	data16 cs nopw 0x0(%rax,%rax,1)
+	nop
+
+00000000000036c0 <__Pyx__GetModuleGlobalName>:
+__Pyx__GetModuleGlobalName():
+	push   %r13
+	mov    %rsi,%r13
+	mov    %rdi,%rsi
+	push   %r12
+	push   %rbp
+	mov    %rdi,%rbp
+	push   %rbx
+	mov    %rdx,%rbx
+	sub    $0x8,%rsp
+	mov    0x18(%rdi),%rdx
+	mov    0x7337(%rip),%rdi        
+	call   2610 <_PyDict_GetItem_KnownHash@plt>
+	mov    %rax,%r12
+	mov    0x7328(%rip),%rax        
+	mov    0x18(%rax),%rax
+	mov    %rax,0x0(%r13)
+	mov    %r12,(%rbx)
+	test   %r12,%r12
+	je     3718 <__Pyx__GetModuleGlobalName+0x58>
+	addq   $0x1,(%r12)
+	add    $0x8,%rsp
+	mov    %r12,%rax
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
+	ret
+	nopl   0x0(%rax,%rax,1)
+	call   2600 <PyErr_Occurred@plt>
+	test   %rax,%rax
+	jne    3705 <__Pyx__GetModuleGlobalName+0x45>
+	add    $0x8,%rsp
+	mov    %rbp,%rdi
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
+	jmp    3640 <__Pyx_GetBuiltinName>
+	data16 cs nopw 0x0(%rax,%rax,1)
+	nop
+
+0000000000003740 <__Pyx_PyObject_CallOneArg>:
+__Pyx_PyObject_CallOneArg():
+	push   %r14
+	push   %r13
+	push   %r12
+	push   %rbp
+	mov    %rdi,%rbp
+	push   %rbx
+	sub    $0x10,%rsp
+	mov    0x8(%rdi),%rax
+	cmp    0x6856(%rip),%rax        
+	mov    %rsi,0x8(%rsp)
+	je     38d0 <__Pyx_PyObject_CallOneArg+0x190>
+	cmp    0x6884(%rip),%rax        
+	jne    3820 <__Pyx_PyObject_CallOneArg+0xe0>
+	mov    0x10(%rdi),%rdx
+	mov    0x10(%rdx),%eax
+	test   $0x8,%al
+	je     3818 <__Pyx_PyObject_CallOneArg+0xd8>
+	mov    0x8(%rsp),%r14
+	mov    0x8(%rdx),%r12
+	xor    %r13d,%r13d
+	test   $0x20,%al
+	je     37f8 <__Pyx_PyObject_CallOneArg+0xb8>
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x67eb(%rip),%rbx        
+	mov    0x20(%rax),%ecx
+	lea    0x1(%rcx),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%rbx),%edx
+	jg     3908 <__Pyx_PyObject_CallOneArg+0x1c8>
+	mov    %r14,%rsi
+	mov    %r13,%rdi
+	call   *%r12
+	mov    %rax,%r12
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%esi
+	lea    -0x1(%rsi),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%rbx),%eax
+	lea    -0x32(%rax),%ecx
+	cmp    $0xc8,%eax
+	jle    3800 <__Pyx_PyObject_CallOneArg+0xc0>
+	cmp    %ecx,%edx
+	jl     380a <__Pyx_PyObject_CallOneArg+0xca>
+	test   %r12,%r12
+	je     38f0 <__Pyx_PyObject_CallOneArg+0x1b0>
+	add    $0x10,%rsp
+	mov    %r12,%rax
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
+	pop    %r14
+	ret
+	nopl   0x0(%rax)
+	mov    0x18(%rdi),%r13
+	jmp    3791 <__Pyx_PyObject_CallOneArg+0x51>
+	xchg   %ax,%ax
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%ecx
+	cmp    %ecx,%edx
+	jge    37d8 <__Pyx_PyObject_CallOneArg+0x98>
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	jmp    37d8 <__Pyx_PyObject_CallOneArg+0x98>
+	nopl   (%rax)
+	test   $0x80,%al
+	jne    3920 <__Pyx_PyObject_CallOneArg+0x1e0>
+	mov    $0x1,%edi
+	mov    0x8(%rsp),%rbx
+	call   25d0 <PyTuple_New@plt>
+	mov    %rax,%r13
+	test   %rax,%rax
+	je     38fd <__Pyx_PyObject_CallOneArg+0x1bd>
+	addq   $0x1,(%rbx)
+	mov    %rbx,0x18(%rax)
+	mov    0x8(%rbp),%rax
+	mov    0x80(%rax),%r12
+	test   %r12,%r12
+	je     3980 <__Pyx_PyObject_CallOneArg+0x240>
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%ebx
+	lea    0x1(%rbx),%edx
+	mov    0x671f(%rip),%rbx        
+	mov    %edx,0x20(%rax)
+	cmp    (%rbx),%edx
+	jg     3998 <__Pyx_PyObject_CallOneArg+0x258>
+	xor    %edx,%edx
+	mov    %r13,%rsi
+	mov    %rbp,%rdi
+	call   *%r12
+	mov    %rax,%r12
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%ecx
+	lea    -0x1(%rcx),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%rbx),%eax
+	lea    -0x32(%rax),%ecx
+	cmp    $0xc8,%eax
+	jg     38a2 <__Pyx_PyObject_CallOneArg+0x162>
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%ecx
+	cmp    %ecx,%edx
+	jl     3970 <__Pyx_PyObject_CallOneArg+0x230>
+	test   %r12,%r12
+	je     39c0 <__Pyx_PyObject_CallOneArg+0x280>
+	subq   $0x1,0x0(%r13)
+	jne    37e1 <__Pyx_PyObject_CallOneArg+0xa1>
+	mov    %r13,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    37e1 <__Pyx_PyObject_CallOneArg+0xa1>
+	nopl   0x0(%rax,%rax,1)
+	lea    0x8(%rsp),%rsi
+	mov    $0x1,%edx
+	call   34d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
+	mov    %rax,%r12
+	jmp    37e1 <__Pyx_PyObject_CallOneArg+0xa1>
+	nopw   0x0(%rax,%rax,1)
+	call   2600 <PyErr_Occurred@plt>
+	mov    %rax,%r12
+	test   %rax,%rax
+	je     394b <__Pyx_PyObject_CallOneArg+0x20b>
+	xor    %r12d,%r12d
+	jmp    37e1 <__Pyx_PyObject_CallOneArg+0xa1>
+	nopl   (%rax)
+	lea    0x4751(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     37ae <__Pyx_PyObject_CallOneArg+0x6e>
+	jmp    38fd <__Pyx_PyObject_CallOneArg+0x1bd>
+	xchg   %ax,%ax
+	mov    0x8(%rdx),%r8
+	xor    %edi,%edi
+	test   $0x20,%al
+	jne    392e <__Pyx_PyObject_CallOneArg+0x1ee>
+	mov    0x18(%rbp),%rdi
+	lea    0x8(%rsp),%rsi
+	test   $0x2,%al
+	jne    39e8 <__Pyx_PyObject_CallOneArg+0x2a8>
+	mov    $0x1,%edx
+	call   *%r8
+	mov    %rax,%r12
+	jmp    37e1 <__Pyx_PyObject_CallOneArg+0xa1>
+	mov    0x6606(%rip),%rax        
+	lea    0x4727(%rip),%rsi        
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
+	jmp    37e1 <__Pyx_PyObject_CallOneArg+0xa1>
 	cs nopw 0x0(%rax,%rax,1)
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	jmp    38aa <__Pyx_PyObject_CallOneArg+0x16a>
+	xchg   %ax,%ax
+	xor    %edx,%edx
+	mov    %r13,%rsi
+	mov    %rbp,%rdi
+	call   26c0 <PyObject_Call@plt>
+	mov    %rax,%r12
+	jmp    38b3 <__Pyx_PyObject_CallOneArg+0x173>
+	nopl   (%rax)
+	lea    0x46c1(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     3874 <__Pyx_PyObject_CallOneArg+0x134>
+	nopl   0x0(%rax)
+	xor    %r12d,%r12d
+	jmp    38b3 <__Pyx_PyObject_CallOneArg+0x173>
+	nopl   0x0(%rax,%rax,1)
+	call   2600 <PyErr_Occurred@plt>
+	mov    %rax,%r12
+	test   %rax,%rax
+	jne    39b0 <__Pyx_PyObject_CallOneArg+0x270>
+	mov    0x6584(%rip),%rax        
+	lea    0x46a5(%rip),%rsi        
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
+	jmp    38b3 <__Pyx_PyObject_CallOneArg+0x173>
+	xor    %ecx,%ecx
+	mov    $0x1,%edx
+	call   *%r8
+	mov    %rax,%r12
+	jmp    37e1 <__Pyx_PyObject_CallOneArg+0xa1>
+	nopw   0x0(%rax,%rax,1)
 
-00000000000033e0 <__Pyx_AddTraceback>:
+0000000000003a00 <__Pyx_PyObject_Call2Args>:
+__Pyx_PyObject_Call2Args():
+	push   %r13
+	mov    %rsi,%r13
+	push   %r12
+	push   %rbp
+	mov    %rdi,%rbp
+	push   %rbx
+	mov    %rdx,%rbx
+	sub    $0x28,%rsp
+	mov    %fs:0x28,%rax
+	mov    %rax,0x18(%rsp)
+	xor    %eax,%eax
+	mov    0x8(%rdi),%rax
+	cmp    0x6582(%rip),%rax        
+	je     3ba0 <__Pyx_PyObject_Call2Args+0x1a0>
+	cmp    0x65b5(%rip),%rax        
+	je     3b18 <__Pyx_PyObject_Call2Args+0x118>
+	mov    $0x2,%edi
+	call   25d0 <PyTuple_New@plt>
+	mov    %rax,%r12
+	test   %rax,%rax
+	je     3bc0 <__Pyx_PyObject_Call2Args+0x1c0>
+	addq   $0x1,0x0(%r13)
+	mov    %r13,0x18(%rax)
+	addq   $0x1,(%rbx)
+	mov    %rbx,0x20(%rax)
+	mov    0x8(%rbp),%rax
+	addq   $0x1,0x0(%rbp)
+	mov    0x80(%rax),%r13
+	test   %r13,%r13
+	je     3bd0 <__Pyx_PyObject_Call2Args+0x1d0>
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x64fb(%rip),%rbx        
+	mov    0x20(%rax),%ecx
+	lea    0x1(%rcx),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%rbx),%edx
+	jg     3be8 <__Pyx_PyObject_Call2Args+0x1e8>
+	xor    %edx,%edx
+	mov    %r12,%rsi
+	mov    %rbp,%rdi
+	call   *%r13
+	mov    %rax,%r13
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%ecx
+	lea    -0x1(%rcx),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%rbx),%eax
+	lea    -0x32(%rax),%ecx
+	cmp    $0xc8,%eax
+	jle    3b60 <__Pyx_PyObject_Call2Args+0x160>
+	cmp    %ecx,%edx
+	jl     3b6e <__Pyx_PyObject_Call2Args+0x16e>
+	test   %r13,%r13
+	je     3c10 <__Pyx_PyObject_Call2Args+0x210>
+	subq   $0x1,(%r12)
+	je     3b90 <__Pyx_PyObject_Call2Args+0x190>
+	subq   $0x1,0x0(%rbp)
+	je     3b80 <__Pyx_PyObject_Call2Args+0x180>
+	mov    0x18(%rsp),%rax
+	xor    %fs:0x28,%rax
+	jne    3c4a <__Pyx_PyObject_Call2Args+0x24a>
+	add    $0x28,%rsp
+	mov    %r13,%rax
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
+	ret
+	nopl   0x0(%rax,%rax,1)
+	mov    0x10(%rdi),%rdx
+	mov    0x10(%rdx),%eax
+	mov    %eax,%ecx
+	and    $0xffffff8d,%ecx
+	cmp    $0x80,%ecx
+	jne    3a41 <__Pyx_PyObject_Call2Args+0x41>
+	mov    %rsi,(%rsp)
+	mov    0x8(%rdx),%r8
+	xor    %edi,%edi
+	mov    %rbx,0x8(%rsp)
+	test   $0x20,%al
+	jne    3b47 <__Pyx_PyObject_Call2Args+0x147>
+	mov    0x18(%rbp),%rdi
+	mov    %rsp,%rsi
+	test   $0x2,%al
+	jne    3c38 <__Pyx_PyObject_Call2Args+0x238>
+	mov    $0x2,%edx
+	call   *%r8
+	mov    %rax,%r13
+	jmp    3af1 <__Pyx_PyObject_Call2Args+0xf1>
+	nop
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%ecx
+	cmp    %ecx,%edx
+	jge    3ad2 <__Pyx_PyObject_Call2Args+0xd2>
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	jmp    3ad2 <__Pyx_PyObject_Call2Args+0xd2>
+	nopl   0x0(%rax)
+	mov    %rbp,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    3af1 <__Pyx_PyObject_Call2Args+0xf1>
+	nopl   (%rax)
+	mov    %r12,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    3ae6 <__Pyx_PyObject_Call2Args+0xe6>
+	nopl   (%rax)
+	mov    %rsi,(%rsp)
+	mov    %rsp,%rsi
+	mov    %rdx,0x8(%rsp)
+	mov    $0x2,%edx
+	call   34d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
+	mov    %rax,%r13
+	jmp    3af1 <__Pyx_PyObject_Call2Args+0xf1>
+	xchg   %ax,%ax
+	xor    %r13d,%r13d
+	jmp    3af1 <__Pyx_PyObject_Call2Args+0xf1>
+	nopl   0x0(%rax,%rax,1)
+	xor    %edx,%edx
+	mov    %r12,%rsi
+	mov    %rbp,%rdi
+	call   26c0 <PyObject_Call@plt>
+	mov    %rax,%r13
+	jmp    3adb <__Pyx_PyObject_Call2Args+0xdb>
+	nopl   (%rax)
+	lea    0x4471(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     3a9e <__Pyx_PyObject_Call2Args+0x9e>
+	nopl   0x0(%rax)
+	xor    %r13d,%r13d
+	jmp    3adb <__Pyx_PyObject_Call2Args+0xdb>
+	nopl   0x0(%rax,%rax,1)
+	call   2600 <PyErr_Occurred@plt>
+	mov    %rax,%r13
+	test   %rax,%rax
+	jne    3c00 <__Pyx_PyObject_Call2Args+0x200>
+	mov    0x6334(%rip),%rax        
+	lea    0x4455(%rip),%rsi        
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
+	jmp    3adb <__Pyx_PyObject_Call2Args+0xdb>
+	xor    %ecx,%ecx
+	mov    $0x2,%edx
+	call   *%r8
+	mov    %rax,%r13
+	jmp    3af1 <__Pyx_PyObject_Call2Args+0xf1>
+	call   24f0 <__stack_chk_fail@plt>
+	nop
+
+0000000000003c50 <__Pyx_AddTraceback>:
 __Pyx_AddTraceback():
 	push   %r15
 	push   %r14
 	push   %r13
 	mov    %rdi,%r13
 	push   %r12
 	mov    %esi,%r12d
 	push   %rbp
 	mov    %rcx,%rbp
 	push   %rbx
 	mov    %edx,%ebx
 	sub    $0x28,%rsp
-	call   23f0 <_PyThreadState_UncheckedGet@plt>
+	call   2400 <_PyThreadState_UncheckedGet@plt>
 	mov    %rax,%r15
 	test   %r12d,%r12d
-	jne    34d8 <__Pyx_AddTraceback+0xf8>
+	jne    3d48 <__Pyx_AddTraceback+0xf8>
 	test   %ebx,%ebx
-	je     3750 <__Pyx_AddTraceback+0x370>
+	je     3fc0 <__Pyx_AddTraceback+0x370>
 	mov    %ebx,%r14d
 	xor    %r12d,%r12d
-	mov    0x5399(%rip),%rdi        
+	mov    0x6d49(%rip),%rdi        
 	test   %rdi,%rdi
-	je     3600 <__Pyx_AddTraceback+0x220>
-	mov    0x5381(%rip),%r9d        
+	je     3e70 <__Pyx_AddTraceback+0x220>
+	mov    0x6d31(%rip),%r9d        
 	mov    %r14d,%edx
 	mov    %r9d,%esi
-	call   32b0 <__pyx_bisect_code_objects>
+	call   33a0 <__pyx_bisect_code_objects>
 	cmp    %eax,%r9d
-	jle    3600 <__Pyx_AddTraceback+0x220>
+	jle    3e70 <__Pyx_AddTraceback+0x220>
 	cltq
 	shl    $0x4,%rax
 	add    %rdi,%rax
 	cmp    %r14d,0x8(%rax)
-	jne    3600 <__Pyx_AddTraceback+0x220>
+	jne    3e70 <__Pyx_AddTraceback+0x220>
 	mov    (%rax),%r12
 	addq   $0x1,(%r12)
-	mov    0x5393(%rip),%rdx        
+	mov    0x6d43(%rip),%rdx        
 	xor    %ecx,%ecx
 	mov    %r12,%rsi
 	mov    %r15,%rdi
-	call   2410 <PyFrame_New@plt>
+	call   2420 <PyFrame_New@plt>
 	mov    %rax,%rbp
 	test   %rax,%rax
-	je     37e0 <__Pyx_AddTraceback+0x400>
+	je     4050 <__Pyx_AddTraceback+0x400>
 	mov    %ebx,0x6c(%rax)
 	mov    %rax,%rdi
-	call   2550 <PyTraceBack_Here@plt>
+	call   2560 <PyTraceBack_Here@plt>
 	subq   $0x1,(%r12)
-	je     34b0 <__Pyx_AddTraceback+0xd0>
+	je     3d20 <__Pyx_AddTraceback+0xd0>
 	subq   $0x1,0x0(%rbp)
 	mov    %rbp,%rdi
-	je     34c2 <__Pyx_AddTraceback+0xe2>
+	je     3d32 <__Pyx_AddTraceback+0xe2>
 	add    $0x28,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   0x0(%rax)
 	mov    %r12,%rdi
-	call   24a0 <_Py_Dealloc@plt>
+	call   24b0 <_Py_Dealloc@plt>
 	subq   $0x1,0x0(%rbp)
 	mov    %rbp,%rdi
-	jne    349a <__Pyx_AddTraceback+0xba>
+	jne    3d0a <__Pyx_AddTraceback+0xba>
 	add    $0x28,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
-	jmp    24a0 <_Py_Dealloc@plt>
+	jmp    24b0 <_Py_Dealloc@plt>
 	nopl   (%rax)
-	mov    0x5309(%rip),%rdi        
+	mov    0x6cb9(%rip),%rdi        
 	test   %rdi,%rdi
-	je     35ec <__Pyx_AddTraceback+0x20c>
+	je     3e5c <__Pyx_AddTraceback+0x20c>
 	mov    0x58(%rax),%rax
 	mov    0x60(%r15),%r14
 	movq   $0x0,0x58(%r15)
 	movq   $0x0,0x60(%r15)
 	mov    %rax,(%rsp)
 	mov    0x68(%r15),%rax
 	movq   $0x0,0x68(%r15)
 	mov    %rax,0x8(%rsp)
-	call   2660 <_PyObject_GetDictPtr@plt>
+	call   2680 <_PyObject_GetDictPtr@plt>
 	mov    %rax,%rcx
 	test   %rax,%rax
-	je     3860 <__Pyx_AddTraceback+0x480>
+	je     40d0 <__Pyx_AddTraceback+0x480>
 	mov    (%rax),%rdi
-	mov    0x5180(%rip),%rax        
+	mov    0x6ab0(%rip),%rax        
 	cmp    %rax,0x18(%rdi)
-	jne    38d0 <__Pyx_AddTraceback+0x4f0>
-	mov    0x5167(%rip),%r8        
+	jne    4140 <__Pyx_AddTraceback+0x4f0>
+	mov    0x6a97(%rip),%r8        
 	test   %r8,%r8
-	je     3578 <__Pyx_AddTraceback+0x198>
-	mov    0x4a43(%rip),%rax        
+	je     3de8 <__Pyx_AddTraceback+0x198>
+	mov    0x61d3(%rip),%rax        
 	cmp    %rax,%r8
-	je     3567 <__Pyx_AddTraceback+0x187>
-	cmp    0x4a4f(%rip),%r8        
-	je     3595 <__Pyx_AddTraceback+0x1b5>
+	je     3dd7 <__Pyx_AddTraceback+0x187>
+	cmp    0x61df(%rip),%r8        
+	je     3e05 <__Pyx_AddTraceback+0x1b5>
 	mov    %r8,%rdi
-	call   2560 <PyObject_Not@plt>
+	call   2570 <PyObject_Not@plt>
 	test   %eax,%eax
-	je     3595 <__Pyx_AddTraceback+0x1b5>
+	je     3e05 <__Pyx_AddTraceback+0x1b5>
 	xor    %r12d,%r12d
-	jmp    3595 <__Pyx_AddTraceback+0x1b5>
-	call   2590 <PyErr_Clear@plt>
+	jmp    3e05 <__Pyx_AddTraceback+0x1b5>
+	call   25a0 <PyErr_Clear@plt>
 	nopl   0x0(%rax)
-	mov    0x4a11(%rip),%rdx        
-	mov    0x5212(%rip),%rsi        
+	mov    0x61a1(%rip),%rdx        
+	mov    0x6bb2(%rip),%rsi        
 	xor    %r12d,%r12d
-	mov    0x5258(%rip),%rdi        
-	call   25e0 <PyObject_SetAttr@plt>
+	mov    0x6c08(%rip),%rdi        
+	call   25f0 <PyObject_SetAttr@plt>
 	mov    (%rsp),%rax
 	mov    0x58(%r15),%rdi
 	mov    0x60(%r15),%r9
 	mov    0x68(%r15),%r8
 	mov    %r14,0x60(%r15)
 	mov    %rax,0x58(%r15)
 	mov    0x8(%rsp),%rax
 	mov    %rax,0x68(%r15)
 	test   %rdi,%rdi
-	je     35c5 <__Pyx_AddTraceback+0x1e5>
+	je     3e35 <__Pyx_AddTraceback+0x1e5>
 	subq   $0x1,(%rdi)
-	je     3808 <__Pyx_AddTraceback+0x428>
+	je     4078 <__Pyx_AddTraceback+0x428>
 	test   %r9,%r9
-	je     35d4 <__Pyx_AddTraceback+0x1f4>
+	je     3e44 <__Pyx_AddTraceback+0x1f4>
 	subq   $0x1,(%r9)
-	je     3828 <__Pyx_AddTraceback+0x448>
+	je     4098 <__Pyx_AddTraceback+0x448>
 	test   %r8,%r8
-	je     35e3 <__Pyx_AddTraceback+0x203>
+	je     3e53 <__Pyx_AddTraceback+0x203>
 	subq   $0x1,(%r8)
-	je     37f8 <__Pyx_AddTraceback+0x418>
+	je     4068 <__Pyx_AddTraceback+0x418>
 	test   %r12d,%r12d
-	je     340a <__Pyx_AddTraceback+0x2a>
+	je     3c7a <__Pyx_AddTraceback+0x2a>
 	mov    %r12d,%r14d
 	neg    %r14d
-	jmp    3418 <__Pyx_AddTraceback+0x38>
+	jmp    3c88 <__Pyx_AddTraceback+0x38>
 	nopw   0x0(%rax,%rax,1)
 	mov    %rbp,%rdi
-	call   2670 <PyUnicode_FromString@plt>
+	call   2690 <PyUnicode_FromString@plt>
 	mov    %rax,%rbp
 	test   %rax,%rax
-	je     349a <__Pyx_AddTraceback+0xba>
+	je     3d0a <__Pyx_AddTraceback+0xba>
 	test   %r12d,%r12d
-	je     3767 <__Pyx_AddTraceback+0x387>
+	je     3fd7 <__Pyx_AddTraceback+0x387>
 	mov    %r13,%rsi
 	mov    %r12d,%ecx
-	lea    0x29d6(%rip),%rdx        
+	lea    0x4216(%rip),%rdx        
 	xor    %eax,%eax
-	lea    0x2be1(%rip),%rdi        
-	call   23c0 <PyUnicode_FromFormat@plt>
+	lea    0x43eb(%rip),%rdi        
+	call   23d0 <PyUnicode_FromFormat@plt>
 	mov    %rax,%r13
 	test   %r13,%r13
-	je     3490 <__Pyx_AddTraceback+0xb0>
-	mov    0x5195(%rip),%rax        
+	je     3d00 <__Pyx_AddTraceback+0xb0>
+	mov    0x6b45(%rip),%rax        
 	sub    $0x8,%rsp
 	xor    %r8d,%r8d
 	xor    %ecx,%ecx
-	mov    0x517d(%rip),%r9        
+	mov    0x6b2d(%rip),%r9        
 	xor    %edx,%edx
 	xor    %esi,%esi
 	xor    %edi,%edi
 	push   %r9
 	push   %rbx
 	push   %r13
 	push   %rbp
 	push   %rax
 	push   %rax
 	push   %rax
 	push   %rax
 	push   %rax
-	call   24c0 <PyCode_New@plt>
+	call   24d0 <PyCode_New@plt>
 	add    $0x50,%rsp
 	mov    %rax,%r12
 	mov    0x0(%rbp),%rax
 	sub    $0x1,%rax
 	mov    %rax,0x0(%rbp)
 	test   %rax,%rax
-	je     3850 <__Pyx_AddTraceback+0x470>
+	je     40c0 <__Pyx_AddTraceback+0x470>
 	subq   $0x1,0x0(%r13)
-	je     3840 <__Pyx_AddTraceback+0x460>
+	je     40b0 <__Pyx_AddTraceback+0x460>
 	test   %r12,%r12
-	je     349a <__Pyx_AddTraceback+0xba>
-	mov    0x5110(%rip),%rdi        
+	je     3d0a <__Pyx_AddTraceback+0xba>
+	mov    0x6ac0(%rip),%rdi        
 	test   %r14d,%r14d
-	je     345e <__Pyx_AddTraceback+0x7e>
+	je     3cce <__Pyx_AddTraceback+0x7e>
 	test   %rdi,%rdi
-	je     3910 <__Pyx_AddTraceback+0x530>
-	mov    0x50ef(%rip),%r9d        
+	je     4180 <__Pyx_AddTraceback+0x530>
+	mov    0x6a9f(%rip),%r9d        
 	mov    %r14d,%edx
 	mov    %r9d,%esi
-	call   32b0 <__pyx_bisect_code_objects>
+	call   33a0 <__pyx_bisect_code_objects>
 	movslq %eax,%rbp
 	cmp    %ebp,%r9d
-	jle    3780 <__Pyx_AddTraceback+0x3a0>
+	jle    3ff0 <__Pyx_AddTraceback+0x3a0>
 	movslq %ebp,%rsi
 	shl    $0x4,%rsi
 	add    %rdi,%rsi
 	cmp    %r14d,0x8(%rsi)
-	je     3995 <__Pyx_AddTraceback+0x5b5>
-	mov    0x50c2(%rip),%eax        
+	je     4205 <__Pyx_AddTraceback+0x5b5>
+	mov    0x6a72(%rip),%eax        
 	cmp    %eax,%r9d
-	je     378f <__Pyx_AddTraceback+0x3af>
+	je     3fff <__Pyx_AddTraceback+0x3af>
 	lea    -0x1(%r9),%ecx
 	mov    %r9d,%edx
 	movslq %ecx,%rcx
 	shl    $0x4,%rcx
 	add    %rdi,%rcx
 	nopl   0x0(%rax)
 	movdqu (%rcx),%xmm0
 	movslq %edx,%rax
 	sub    $0x1,%edx
 	sub    $0x10,%rcx
 	shl    $0x4,%rax
 	movups %xmm0,(%rdi,%rax,1)
 	cmp    %edx,%ebp
-	jl     3710 <__Pyx_AddTraceback+0x330>
+	jl     3f80 <__Pyx_AddTraceback+0x330>
 	add    $0x1,%r9d
 	mov    %r14d,0x8(%rsi)
 	mov    %r12,(%rsi)
-	mov    %r9d,0x5074(%rip)        
+	mov    %r9d,0x6a24(%rip)        
 	addq   $0x1,(%r12)
-	jmp    345e <__Pyx_AddTraceback+0x7e>
+	jmp    3cce <__Pyx_AddTraceback+0x7e>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    %rbp,%rdi
-	call   2670 <PyUnicode_FromString@plt>
+	call   2690 <PyUnicode_FromString@plt>
 	mov    %rax,%rbp
 	test   %rax,%rax
-	je     349a <__Pyx_AddTraceback+0xba>
+	je     3d0a <__Pyx_AddTraceback+0xba>
 	xor    %r14d,%r14d
 	mov    %r13,%rdi
-	call   2670 <PyUnicode_FromString@plt>
+	call   2690 <PyUnicode_FromString@plt>
 	mov    %rax,%r13
-	jmp    363b <__Pyx_AddTraceback+0x25b>
+	jmp    3eab <__Pyx_AddTraceback+0x25b>
 	nopw   0x0(%rax,%rax,1)
-	mov    0x502e(%rip),%eax        
+	mov    0x69de(%rip),%eax        
 	cmp    %eax,%r9d
-	jne    3950 <__Pyx_AddTraceback+0x570>
+	jne    41c0 <__Pyx_AddTraceback+0x570>
 	lea    0x40(%rax),%r13d
 	movslq %r13d,%rsi
 	shl    $0x4,%rsi
-	call   2520 <PyMem_Realloc@plt>
+	call   2530 <PyMem_Realloc@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
-	je     345e <__Pyx_AddTraceback+0x7e>
+	je     3cce <__Pyx_AddTraceback+0x7e>
 	movslq %ebp,%rsi
-	mov    0x4ffb(%rip),%r9d        
-	mov    %rax,0x4ffc(%rip)        
+	mov    0x69ab(%rip),%r9d        
+	mov    %rax,0x69ac(%rip)        
 	shl    $0x4,%rsi
-	mov    %r13d,0x4fed(%rip)        
+	mov    %r13d,0x699d(%rip)        
 	add    %rax,%rsi
 	cmp    %r9d,%ebp
-	jl     36fb <__Pyx_AddTraceback+0x31b>
-	jmp    372a <__Pyx_AddTraceback+0x34a>
+	jl     3f6b <__Pyx_AddTraceback+0x31b>
+	jmp    3f9a <__Pyx_AddTraceback+0x34a>
 	nopl   0x0(%rax,%rax,1)
 	subq   $0x1,(%r12)
-	jne    349a <__Pyx_AddTraceback+0xba>
+	jne    3d0a <__Pyx_AddTraceback+0xba>
 	mov    %r12,%rdi
-	jmp    34c2 <__Pyx_AddTraceback+0xe2>
+	jmp    3d32 <__Pyx_AddTraceback+0xe2>
 	nopl   0x0(%rax,%rax,1)
 	mov    %r8,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    35e3 <__Pyx_AddTraceback+0x203>
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    3e53 <__Pyx_AddTraceback+0x203>
 	nopl   (%rax)
 	mov    %r8,0x8(%rsp)
 	mov    %r9,(%rsp)
-	call   24a0 <_Py_Dealloc@plt>
+	call   24b0 <_Py_Dealloc@plt>
 	mov    0x8(%rsp),%r8
 	mov    (%rsp),%r9
-	jmp    35c5 <__Pyx_AddTraceback+0x1e5>
+	jmp    3e35 <__Pyx_AddTraceback+0x1e5>
 	nopl   0x0(%rax)
 	mov    %r9,%rdi
 	mov    %r8,(%rsp)
-	call   24a0 <_Py_Dealloc@plt>
+	call   24b0 <_Py_Dealloc@plt>
 	mov    (%rsp),%r8
-	jmp    35d4 <__Pyx_AddTraceback+0x1f4>
+	jmp    3e44 <__Pyx_AddTraceback+0x1f4>
 	nopl   (%rax)
 	mov    %r13,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    3698 <__Pyx_AddTraceback+0x2b8>
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    3f08 <__Pyx_AddTraceback+0x2b8>
 	nopl   (%rax)
 	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    368d <__Pyx_AddTraceback+0x2ad>
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    3efd <__Pyx_AddTraceback+0x2ad>
 	nopl   (%rax)
-	mov    0x4f81(%rip),%rdi        
-	mov    0x4f2a(%rip),%rsi        
+	mov    0x6931(%rip),%rdi        
+	mov    0x68ca(%rip),%rsi        
 	mov    0x8(%rdi),%rax
 	mov    0x90(%rax),%rax
 	test   %rax,%rax
-	je     39bf <__Pyx_AddTraceback+0x5df>
+	je     422f <__Pyx_AddTraceback+0x5df>
 	call   *%rax
 	mov    %rax,%rdi
 	test   %rdi,%rdi
-	je     356c <__Pyx_AddTraceback+0x18c>
+	je     3ddc <__Pyx_AddTraceback+0x18c>
 	mov    %rdi,0x10(%rsp)
-	call   2560 <PyObject_Not@plt>
+	call   2570 <PyObject_Not@plt>
 	mov    0x10(%rsp),%rdi
 	test   %eax,%eax
 	mov    (%rdi),%rax
-	jne    3960 <__Pyx_AddTraceback+0x580>
+	jne    41d0 <__Pyx_AddTraceback+0x580>
 	sub    $0x1,%rax
 	mov    %rax,(%rdi)
-	je     39af <__Pyx_AddTraceback+0x5cf>
-	mov    0x46d2(%rip),%rax        
-	cmp    %rax,0x46e3(%rip)        
-	jne    3595 <__Pyx_AddTraceback+0x1b5>
-	jmp    3567 <__Pyx_AddTraceback+0x187>
-	mov    0x4ec1(%rip),%rsi        
+	je     421f <__Pyx_AddTraceback+0x5cf>
+	mov    0x5e62(%rip),%rax        
+	cmp    %rax,0x5e73(%rip)        
+	jne    3e05 <__Pyx_AddTraceback+0x1b5>
+	jmp    3dd7 <__Pyx_AddTraceback+0x187>
+	mov    0x6861(%rip),%rsi        
 	mov    %rcx,0x10(%rsp)
 	mov    0x18(%rsi),%rdx
-	call   2600 <_PyDict_GetItem_KnownHash@plt>
+	call   2610 <_PyDict_GetItem_KnownHash@plt>
 	mov    0x10(%rsp),%rcx
-	mov    %rax,0x4db7(%rip)        
+	mov    %rax,0x66e7(%rip)        
 	mov    %rax,%r8
 	mov    (%rcx),%rax
 	mov    0x18(%rax),%rax
-	mov    %rax,0x4dae(%rip)        
-	jmp    3541 <__Pyx_AddTraceback+0x161>
+	mov    %rax,0x66de(%rip)        
+	jmp    3db1 <__Pyx_AddTraceback+0x161>
 	nopw   0x0(%rax,%rax,1)
 	mov    $0x400,%edi
-	call   2710 <PyMem_Malloc@plt>
+	call   2730 <PyMem_Malloc@plt>
 	test   %rax,%rax
-	je     345e <__Pyx_AddTraceback+0x7e>
+	je     3cce <__Pyx_AddTraceback+0x7e>
 	movabs $0x4000000001,%rsi
-	mov    %rax,0x4e84(%rip)        
-	mov    %rsi,0x4e75(%rip)        
+	mov    %rax,0x6834(%rip)        
+	mov    %rsi,0x6825(%rip)        
 	mov    %r14d,0x8(%rax)
 	mov    %r12,(%rax)
 	addq   $0x1,(%r12)
-	jmp    345e <__Pyx_AddTraceback+0x7e>
+	jmp    3cce <__Pyx_AddTraceback+0x7e>
 	nopl   0x0(%rax)
 	shl    $0x4,%rbp
 	lea    (%rdi,%rbp,1),%rsi
-	jmp    372a <__Pyx_AddTraceback+0x34a>
+	jmp    3f9a <__Pyx_AddTraceback+0x34a>
 	nopl   (%rax)
 	sub    $0x1,%rax
 	mov    %rax,(%rdi)
-	jne    3567 <__Pyx_AddTraceback+0x187>
-	mov    0x461c(%rip),%rax        
+	jne    3dd7 <__Pyx_AddTraceback+0x187>
+	mov    0x5dac(%rip),%rax        
 	mov    %rax,%r8
 	mov    %rax,0x18(%rsp)
 	mov    %r8,0x10(%rsp)
-	call   24a0 <_Py_Dealloc@plt>
+	call   24b0 <_Py_Dealloc@plt>
 	mov    0x10(%rsp),%r8
 	mov    0x18(%rsp),%rax
-	jmp    354d <__Pyx_AddTraceback+0x16d>
+	jmp    3dbd <__Pyx_AddTraceback+0x16d>
 	mov    (%rsi),%rdi
 	mov    %r12,(%rsi)
 	subq   $0x1,(%rdi)
-	jne    345e <__Pyx_AddTraceback+0x7e>
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    345e <__Pyx_AddTraceback+0x7e>
-	mov    0x45f2(%rip),%r8        
-	mov    0x45d3(%rip),%rax        
-	jmp    3977 <__Pyx_AddTraceback+0x597>
-	call   2700 <PyObject_GetAttr@plt>
+	jne    3cce <__Pyx_AddTraceback+0x7e>
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    3cce <__Pyx_AddTraceback+0x7e>
+	mov    0x5d82(%rip),%r8        
+	mov    0x5d63(%rip),%rax        
+	jmp    41e7 <__Pyx_AddTraceback+0x597>
+	call   2720 <PyObject_GetAttr@plt>
 	mov    %rax,%rdi
-	jmp    3887 <__Pyx_AddTraceback+0x4a7>
+	jmp    40f7 <__Pyx_AddTraceback+0x4a7>
 	nopl   0x0(%rax)
 
-00000000000039d0 <__Pyx_PyFunction_FastCallDict.constprop.0>:
-__Pyx_PyFunction_FastCallDict.constprop.0():
-	push   %r15
-	push   %r14
+0000000000004240 <__Pyx_PyObject_CallNoArg>:
+__Pyx_PyObject_CallNoArg():
 	push   %r13
 	push   %r12
-	mov    %rsi,%r12
 	push   %rbp
-	mov    %edx,%ebp
+	mov    %rdi,%rbp
 	push   %rbx
-	mov    %rdi,%rbx
 	sub    $0x8,%rsp
-	mov    0x10(%rdi),%r15
-	mov    0x18(%rdi),%r14
-	mov    0x20(%rdi),%r13
-	call   25d0 <PyThreadState_Get@plt>
-	mov    0x20(%rax),%ecx
-	lea    0x1(%rcx),%edx
+	mov    0x8(%rdi),%rax
+	cmp    0x5d58(%rip),%rax        
+	je     4390 <__Pyx_PyObject_CallNoArg+0x150>
+	cmp    0x5d8b(%rip),%rax        
+	jne    4310 <__Pyx_PyObject_CallNoArg+0xd0>
+	mov    0x10(%rdi),%rcx
+	mov    0x10(%rcx),%edx
+	test   $0x4,%dl
+	je     4310 <__Pyx_PyObject_CallNoArg+0xd0>
+	xor    %r13d,%r13d
+	and    $0x20,%edx
+	mov    0x8(%rcx),%r12
+	je     42f0 <__Pyx_PyObject_CallNoArg+0xb0>
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x5cf5(%rip),%rbx        
+	mov    0x20(%rax),%esi
+	lea    0x1(%rsi),%edx
 	mov    %edx,0x20(%rax)
-	mov    0x4581(%rip),%rax        
-	cmp    (%rax),%edx
-	jg     3ab8 <__Pyx_PyFunction_FastCallDict.constprop.0+0xe8>
-	mov    0x18(%r15),%eax
-	test   %eax,%eax
-	jne    3a22 <__Pyx_PyFunction_FastCallDict.constprop.0+0x52>
-	cmpl   $0x43,0x24(%r15)
-	je     3ad8 <__Pyx_PyFunction_FastCallDict.constprop.0+0x108>
-	mov    0x30(%rbx),%rcx
-	mov    0x28(%rbx),%rdx
-	xor    %eax,%eax
-	test   %r13,%r13
-	je     3a39 <__Pyx_PyFunction_FastCallDict.constprop.0+0x69>
-	mov    0x10(%r13),%rax
-	add    $0x18,%r13
-	sub    $0x8,%rsp
-	xor    %r9d,%r9d
-	mov    %ebp,%r8d
-	mov    %r14,%rsi
-	push   %rcx
-	mov    %r15,%rdi
-	mov    %r12,%rcx
-	push   %rdx
-	xor    %edx,%edx
-	push   %rax
-	push   %r13
-	push   $0x0
-	call   2620 <PyEval_EvalCodeEx@plt>
-	add    $0x30,%rsp
+	cmp    (%rbx),%edx
+	jg     43c0 <__Pyx_PyObject_CallNoArg+0x180>
+	xor    %esi,%esi
+	mov    %r13,%rdi
+	call   *%r12
 	mov    %rax,%r12
-	call   25d0 <PyThreadState_Get@plt>
+	call   25e0 <PyThreadState_Get@plt>
+	mov    (%rbx),%ecx
 	mov    0x20(%rax),%esi
 	lea    -0x1(%rsi),%edx
 	mov    %edx,0x20(%rax)
-	mov    0x4512(%rip),%rax        
-	mov    (%rax),%eax
-	cmp    $0xc8,%eax
-	jg     3aa0 <__Pyx_PyFunction_FastCallDict.constprop.0+0xd0>
-	sar    $0x2,%eax
-	lea    (%rax,%rax,2),%eax
+	lea    -0x32(%rcx),%eax
+	cmp    $0xc8,%ecx
+	jle    4300 <__Pyx_PyObject_CallNoArg+0xc0>
 	cmp    %eax,%edx
-	jl     3aa7 <__Pyx_PyFunction_FastCallDict.constprop.0+0xd7>
+	jl     4380 <__Pyx_PyObject_CallNoArg+0x140>
+	test   %r12,%r12
+	je     43a8 <__Pyx_PyObject_CallNoArg+0x168>
 	add    $0x8,%rsp
 	mov    %r12,%rax
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
-	pop    %r14
-	pop    %r15
 	ret
-	nopl   0x0(%rax,%rax,1)
-	sub    $0x32,%eax
+	nopl   0x0(%rax)
+	mov    0x18(%rdi),%r13
+	jmp    4287 <__Pyx_PyObject_CallNoArg+0x47>
+	cs nopw 0x0(%rax,%rax,1)
+	sar    $0x2,%ecx
+	lea    (%rcx,%rcx,2),%eax
 	cmp    %eax,%edx
-	jge    3a89 <__Pyx_PyFunction_FastCallDict.constprop.0+0xb9>
-	call   25d0 <PyThreadState_Get@plt>
-	movb   $0x0,0x24(%rax)
-	jmp    3a89 <__Pyx_PyFunction_FastCallDict.constprop.0+0xb9>
-	nopw   0x0(%rax,%rax,1)
-	lea    0x25c1(%rip),%rdi        
-	call   25b0 <_Py_CheckRecursiveCall@plt>
-	test   %eax,%eax
-	je     3a0f <__Pyx_PyFunction_FastCallDict.constprop.0+0x3f>
-	xor    %r12d,%r12d
-	jmp    3a89 <__Pyx_PyFunction_FastCallDict.constprop.0+0xb9>
+	jge    42d2 <__Pyx_PyObject_CallNoArg+0x92>
+	jmp    4380 <__Pyx_PyObject_CallNoArg+0x140>
 	nopl   0x0(%rax)
-	test   %r13,%r13
-	je     3b00 <__Pyx_PyFunction_FastCallDict.constprop.0+0x130>
-	mov    0x10(%r13),%rax
-	add    $0x18,%r13
-	cmp    $0x1,%ebp
-	je     3af3 <__Pyx_PyFunction_FastCallDict.constprop.0+0x123>
-	movslq 0x10(%r15),%rdx
-	cmp    %rax,%rdx
-	je     3b1f <__Pyx_PyFunction_FastCallDict.constprop.0+0x14f>
-	mov    0x30(%rbx),%rcx
-	mov    0x28(%rbx),%rdx
-	jmp    3a39 <__Pyx_PyFunction_FastCallDict.constprop.0+0x69>
-	cmp    %ebp,0x10(%r15)
-	jne    3af3 <__Pyx_PyFunction_FastCallDict.constprop.0+0x123>
-	mov    %r12,%rsi
-	movslq %ebp,%rdx
-	mov    %r14,%rcx
-	mov    %r15,%rdi
-	call   3330 <__Pyx_PyFunction_FastCallNoKw>
-	mov    %rax,%r12
-	jmp    3a61 <__Pyx_PyFunction_FastCallDict.constprop.0+0x91>
-	mov    %r14,%rcx
-	mov    %r13,%rsi
-	mov    %r15,%rdi
-	call   3330 <__Pyx_PyFunction_FastCallNoKw>
-	mov    %rax,%r12
-	jmp    3a61 <__Pyx_PyFunction_FastCallDict.constprop.0+0x91>
-	data16 cs nopw 0x0(%rax,%rax,1)
-
-0000000000003b40 <__Pyx_GetBuiltinName>:
-__Pyx_GetBuiltinName():
-	push   %r13
-	mov    %rdi,%r13
-	push   %r12
-	mov    %r13,%rsi
-	sub    $0x8,%rsp
-	mov    0x4c9b(%rip),%rdi        
-	mov    0x8(%rdi),%rax
-	mov    0x90(%rax),%rax
-	test   %rax,%rax
-	je     3b80 <__Pyx_GetBuiltinName+0x40>
-	call   *%rax
-	mov    %rax,%r12
-	test   %r12,%r12
-	je     3b8d <__Pyx_GetBuiltinName+0x4d>
-	add    $0x8,%rsp
-	mov    %r12,%rax
-	pop    %r12
-	pop    %r13
-	ret
-	nopl   0x0(%rax,%rax,1)
-	call   2700 <PyObject_GetAttr@plt>
-	mov    %rax,%r12
+	mov    0x80(%rax),%r12
+	mov    0x66e2(%rip),%r13        
 	test   %r12,%r12
-	jne    3b6f <__Pyx_GetBuiltinName+0x2f>
-	mov    0x444c(%rip),%rax        
-	mov    %r13,%rdx
-	lea    0x26df(%rip),%rsi        
-	mov    (%rax),%rdi
-	xor    %eax,%eax
-	call   26c0 <PyErr_Format@plt>
-	add    $0x8,%rsp
-	mov    %r12,%rax
-	pop    %r12
-	pop    %r13
-	ret
-	data16 cs nopw 0x0(%rax,%rax,1)
-	nop
-
-0000000000003bc0 <__Pyx__GetModuleGlobalName>:
-__Pyx__GetModuleGlobalName():
-	push   %r13
-	mov    %rsi,%r13
-	mov    %rdi,%rsi
-	push   %r12
-	push   %rbp
-	mov    %rdi,%rbp
-	push   %rbx
-	mov    %rdx,%rbx
-	sub    $0x8,%rsp
-	mov    0x18(%rdi),%rdx
-	mov    0x4c17(%rip),%rdi        
-	call   2600 <_PyDict_GetItem_KnownHash@plt>
+	je     43e0 <__Pyx_PyObject_CallNoArg+0x1a0>
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%ebx
+	lea    0x1(%rbx),%edx
+	mov    0x5c4f(%rip),%rbx        
+	mov    %edx,0x20(%rax)
+	cmp    (%rbx),%edx
+	jg     4400 <__Pyx_PyObject_CallNoArg+0x1c0>
+	xor    %edx,%edx
+	mov    %r13,%rsi
+	mov    %rbp,%rdi
+	call   *%r12
 	mov    %rax,%r12
-	mov    0x4c08(%rip),%rax        
-	mov    0x18(%rax),%rax
-	mov    %rax,0x0(%r13)
-	mov    %r12,(%rbx)
-	test   %r12,%r12
-	je     3c18 <__Pyx__GetModuleGlobalName+0x58>
-	addq   $0x1,(%r12)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%esi
+	lea    -0x1(%rsi),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%rbx),%eax
+	lea    -0x32(%rax),%ecx
+	cmp    $0xc8,%eax
+	jg     4372 <__Pyx_PyObject_CallNoArg+0x132>
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%ecx
+	cmp    %ecx,%edx
+	jge    42d2 <__Pyx_PyObject_CallNoArg+0x92>
+	nopw   0x0(%rax,%rax,1)
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	jmp    42d2 <__Pyx_PyObject_CallNoArg+0x92>
+	xchg   %ax,%ax
 	add    $0x8,%rsp
-	mov    %r12,%rax
+	xor    %edx,%edx
+	xor    %esi,%esi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
-	ret
+	jmp    34d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
 	nopl   0x0(%rax,%rax,1)
-	call   25f0 <PyErr_Occurred@plt>
+	call   2600 <PyErr_Occurred@plt>
+	mov    %rax,%r12
 	test   %rax,%rax
-	jne    3c05 <__Pyx__GetModuleGlobalName+0x45>
+	je     4416 <__Pyx_PyObject_CallNoArg+0x1d6>
+	xor    %r12d,%r12d
+	jmp    42db <__Pyx_PyObject_CallNoArg+0x9b>
+	nopl   (%rax)
+	lea    0x3c99(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     42a4 <__Pyx_PyObject_CallNoArg+0x64>
+	jmp    43b5 <__Pyx_PyObject_CallNoArg+0x175>
+	cs nopw 0x0(%rax,%rax,1)
 	add    $0x8,%rsp
+	mov    %r13,%rsi
 	mov    %rbp,%rdi
+	xor    %edx,%edx
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
-	jmp    3b40 <__Pyx_GetBuiltinName>
+	jmp    26c0 <PyObject_Call@plt>
+	nopw   0x0(%rax,%rax,1)
+	lea    0x3c59(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     4344 <__Pyx_PyObject_CallNoArg+0x104>
+	jmp    43b5 <__Pyx_PyObject_CallNoArg+0x175>
+	mov    0x5b3b(%rip),%rax        
+	lea    0x3c5c(%rip),%rsi        
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
+	jmp    42db <__Pyx_PyObject_CallNoArg+0x9b>
 	data16 cs nopw 0x0(%rax,%rax,1)
-	nop
+	nopl   0x0(%rax)
 
-0000000000003c40 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id>:
+0000000000004440 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id>:
 __pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id():
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
-	sub    $0x28,%rsp
-	mov    0x4a77(%rip),%rbx        
+	sub    $0x38,%rsp
+	mov    0x6427(%rip),%rcx        
 	mov    %fs:0x28,%rax
-	mov    %rax,0x18(%rsp)
+	mov    %rax,0x28(%rsp)
 	xor    %eax,%eax
-	mov    0x4b88(%rip),%rax        
-	cmp    %rbx,0x18(%rax)
-	jne    4450 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x810>
-	mov    0x4a47(%rip),%r12        
-	test   %r12,%r12
-	je     4598 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x958>
-	addq   $0x1,(%r12)
-	mov    0x8(%r12),%rax
-	mov    0x4b0d(%rip),%rsi        
-	mov    %r12,%rdi
+	mov    0x65a8(%rip),%rax        
+	cmp    %rcx,0x18(%rax)
+	jne    5640 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1200>
+	mov    0x63f7(%rip),%rbp        
+	test   %rbp,%rbp
+	je     57c8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1388>
+	addq   $0x1,0x0(%rbp)
+	mov    0x8(%rbp),%rax
+	mov    0x649e(%rip),%rsi        
+	mov    %rbp,%rdi
 	mov    0x90(%rax),%rax
 	test   %rax,%rax
-	je     4540 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x900>
+	je     57e0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x13a0>
 	call   *%rax
-	mov    %rax,%r14
-	mov    (%r12),%rax
+	mov    %rax,%r12
+	mov    0x0(%rbp),%rax
 	lea    -0x1(%rax),%rdx
-	test   %r14,%r14
-	je     4550 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x910>
-	mov    %rdx,(%r12)
+	test   %r12,%r12
+	je     57f0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x13b0>
+	mov    %rdx,0x0(%rbp)
 	test   %rdx,%rdx
-	je     4238 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x5f8>
-	call   2650 <PyDict_New@plt>
+	je     4ef8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xab8>
+	mov    0x8(%r12),%rax
+	cmp    0x5a84(%rip),%rax        
+	je     5840 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1400>
+	mov    0x648f(%rip),%r13        
+	cmp    0x5ac0(%rip),%rax        
+	mov    %r13,0x20(%rsp)
+	je     5c30 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x17f0>
+	cmp    0x5aee(%rip),%rax        
+	jne    5c60 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1820>
+	mov    0x10(%r12),%rdx
+	mov    0x10(%rdx),%eax
+	test   $0x8,%al
+	je     6600 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x21c0>
+	mov    0x8(%rdx),%rbp
+	xor    %r14d,%r14d
+	test   $0x20,%al
+	jne    4528 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe8>
+	mov    0x18(%r12),%r14
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x5a54(%rip),%r15        
+	mov    0x20(%rax),%ebx
+	lea    0x1(%rbx),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%r15),%edx
+	jg     66e0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x22a0>
+	mov    %r14,%rdi
+	mov    %r13,%rsi
+	call   *%rbp
+	mov    %rax,%r14
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%ecx
+	lea    -0x1(%rcx),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%r15),%eax
+	cmp    $0xc8,%eax
+	jle    5830 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x13f0>
+	sub    $0x32,%eax
+	cmp    %eax,%edx
+	jl     5a30 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x15f0>
+	test   %r14,%r14
+	je     6720 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x22e0>
+	mov    %r12,%r13
+	test   %r14,%r14
+	je     5bc0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1780>
+	subq   $0x1,0x0(%r13)
+	je     51c0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd80>
+	mov    0x8(%r14),%rax
+	mov    0x6375(%rip),%rsi        
+	mov    %r14,%rdi
+	mov    0x90(%rax),%rax
+	test   %rax,%rax
+	je     58e0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x14a0>
+	call   *%rax
+	mov    %rax,%rbp
+	test   %rbp,%rbp
+	je     58f0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x14b0>
+	mov    0x8(%rbp),%rax
+	cmp    0x5991(%rip),%rax        
+	jne    4f08 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xac8>
+	mov    0x18(%rbp),%rbx
+	test   %rbx,%rbx
+	je     4f08 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xac8>
+	mov    0x10(%rbp),%r12
+	addq   $0x1,(%rbx)
+	addq   $0x1,(%r12)
+	subq   $0x1,0x0(%rbp)
+	je     5370 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf30>
+	mov    0x59af(%rip),%rcx        
+	mov    0x8(%r12),%rax
+	mov    %rbx,0x20(%rsp)
+	mov    %rcx,0x8(%rsp)
+	cmp    %rcx,%rax
+	je     60a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1c60>
+	cmp    0x59d0(%rip),%rax        
+	jne    53b0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf70>
+	mov    0x10(%r12),%rdx
+	mov    0x10(%rdx),%eax
+	test   $0x8,%al
+	je     6290 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1e50>
+	mov    0x8(%rdx),%rbp
+	xor    %r13d,%r13d
+	test   $0x20,%al
+	jne    4646 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x206>
+	mov    0x18(%r12),%r13
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x5936(%rip),%r15        
+	mov    0x20(%rax),%ecx
+	lea    0x1(%rcx),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%r15),%edx
+	jg     6380 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1f40>
+	mov    %r13,%rdi
+	mov    %rbx,%rsi
+	call   *%rbp
 	mov    %rax,%r13
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%edi
+	lea    -0x1(%rdi),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%r15),%eax
+	cmp    $0xc8,%eax
+	jle    5610 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11d0>
+	sub    $0x32,%eax
+	cmp    %eax,%edx
+	jl     58c0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1480>
+	test   %r13,%r13
+	je     60e0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1ca0>
+	subq   $0x1,(%rbx)
+	je     5452 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1012>
+	subq   $0x1,(%r12)
+	je     52a8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe68>
+	mov    0x8(%r13),%rax
+	mov    0x6239(%rip),%rsi        
+	mov    %r13,%rdi
+	mov    0x90(%rax),%rax
 	test   %rax,%rax
-	je     45b0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x970>
-	mov    0x4b0f(%rip),%rax        
-	mov    0x49d0(%rip),%rbx        
-	cmp    %rbx,0x18(%rax)
-	jne    4680 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xa40>
-	mov    0x49b7(%rip),%rbp        
+	je     5990 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1550>
+	call   *%rax
+	mov    %rax,%r12
+	mov    0x0(%r13),%rax
+	sub    $0x1,%rax
+	test   %r12,%r12
+	je     59a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1560>
+	mov    %rax,0x0(%r13)
+	test   %rax,%rax
+	je     5380 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf40>
+	mov    0x8(%r12),%rax
+	cmp    0x585f(%rip),%rax        
+	jne    50f0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xcb0>
+	mov    0x18(%r12),%rbx
+	test   %rbx,%rbx
+	je     50f0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xcb0>
+	mov    0x10(%r12),%r13
+	addq   $0x1,(%rbx)
+	addq   $0x1,0x0(%r13)
+	subq   $0x1,(%r12)
+	je     53a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf60>
+	mov    %rbx,0x20(%rsp)
+	mov    0x8(%r13),%rax
+	cmp    0x8(%rsp),%rax
+	je     62c8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1e88>
+	cmp    0x58a7(%rip),%rax        
+	jne    5550 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1110>
+	mov    0x10(%r13),%rdx
+	mov    0x10(%rdx),%eax
+	test   $0x8,%al
+	je     64c0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2080>
+	mov    0x8(%rdx),%rbp
+	xor    %r12d,%r12d
+	test   $0x20,%al
+	jne    476d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x32d>
+	mov    0x18(%r13),%r12
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x580f(%rip),%r15        
+	mov    0x20(%rax),%ecx
+	lea    0x1(%rcx),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%r15),%edx
+	jg     6638 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x21f8>
+	mov    %r12,%rdi
+	mov    %rbx,%rsi
+	call   *%rbp
+	mov    %rax,%rbp
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%edi
+	lea    -0x1(%rdi),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%r15),%eax
+	cmp    $0xc8,%eax
+	jle    57b8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1378>
+	sub    $0x32,%eax
+	cmp    %eax,%edx
+	jl     5970 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1530>
 	test   %rbp,%rbp
-	je     48c8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc88>
-	addq   $0x1,0x0(%rbp)
+	je     6320 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1ee0>
+	subq   $0x1,(%rbx)
+	je     55f0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11b0>
+	subq   $0x1,0x0(%r13)
+	je     5390 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf50>
+	mov    0x8(%r14),%rax
+	mov    0x61ba(%rip),%rsi        
+	mov    %r14,%rdi
+	mov    0x90(%rax),%rax
+	test   %rax,%rax
+	je     5de0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x19a0>
+	call   *%rax
+	mov    %rax,%r12
+	test   %r12,%r12
+	je     5db0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1970>
+	mov    0x8(%r12),%rax
+	cmp    0x574d(%rip),%rax        
+	jne    51d0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd90>
+	mov    0x18(%r12),%rbx
+	test   %rbx,%rbx
+	je     51d0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd90>
+	mov    0x10(%r12),%r13
+	addq   $0x1,(%rbx)
+	addq   $0x1,0x0(%r13)
+	subq   $0x1,(%r12)
+	je     5540 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1100>
+	mov    %rbx,0x20(%rsp)
+	mov    0x8(%r13),%rax
+	cmp    0x8(%rsp),%rax
+	je     6518 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x20d8>
+	cmp    0x5795(%rip),%rax        
+	jne    56e0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x12a0>
+	mov    0x10(%r13),%rdx
+	mov    0x10(%rdx),%eax
+	test   $0x8,%al
+	je     6750 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2310>
+	mov    0x8(%rdx),%rcx
+	xor    %r12d,%r12d
+	mov    %rcx,0x10(%rsp)
+	test   $0x20,%al
+	jne    4884 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x444>
+	mov    0x18(%r13),%r12
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x56f8(%rip),%r15        
+	mov    0x20(%rax),%edi
+	lea    0x1(%rdi),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%r15),%edx
+	jg     6950 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2510>
+	mov    %rbx,%rsi
+	mov    %r12,%rdi
+	mov    0x10(%rsp),%rax
+	call   *%rax
+	mov    %rax,0x10(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x10(%rsp),%r8
+	mov    0x20(%rax),%esi
+	lea    -0x1(%rsi),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%r15),%eax
+	cmp    $0xc8,%eax
+	jle    58d0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1490>
+	sub    $0x32,%eax
+	cmp    %eax,%edx
+	jl     5d90 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1950>
+	test   %r8,%r8
+	je     65b8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2178>
+	subq   $0x1,(%rbx)
+	je     5792 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1352>
+	subq   $0x1,0x0(%r13)
+	je     5528 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x10e8>
+	subq   $0x1,(%r8)
+	je     5518 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x10d8>
 	mov    0x8(%rbp),%rax
-	mov    0x4a66(%rip),%rsi        
+	mov    0x5fed(%rip),%rsi        
 	mov    %rbp,%rdi
 	mov    0x90(%rax),%rax
 	test   %rax,%rax
-	je     48e0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xca0>
+	je     5ec0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1a80>
 	call   *%rax
 	mov    %rax,%rbx
 	test   %rbx,%rbx
-	je     48f0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xcb0>
-	subq   $0x1,0x0(%rbp)
-	je     4248 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x608>
+	je     5e90 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1a50>
 	mov    0x8(%rbx),%rax
-	cmp    0x420f(%rip),%rax        
-	je     4928 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xce8>
-	mov    0x4252(%rip),%rsi        
-	mov    %rsi,(%rsp)
-	cmp    %rsi,%rax
-	je     4a18 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xdd8>
-	cmp    0x427e(%rip),%rax        
-	jne    4268 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x628>
-	mov    0x10(%rbx),%rcx
+	cmp    0x5621(%rip),%rax        
+	jne    52b8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe78>
+	mov    0x18(%rbx),%r13
+	test   %r13,%r13
+	je     52b8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe78>
+	mov    0x10(%rbx),%r12
+	addq   $0x1,0x0(%r13)
+	addq   $0x1,(%r12)
+	subq   $0x1,(%rbx)
+	je     56d0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1290>
+	mov    0x604f(%rip),%rdx        
+	mov    %r13,%rsi
+	mov    %r12,%rdi
+	call   3a00 <__Pyx_PyObject_Call2Args>
+	subq   $0x1,0x0(%r13)
+	mov    %rax,%r9
+	je     5898 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1458>
+	test   %r9,%r9
+	je     5fa0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1b60>
+	subq   $0x1,(%r12)
+	je     5620 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11e0>
+	mov    %r9,%rdi
+	mov    %r9,0x10(%rsp)
+	call   2640 <PyObject_Size@plt>
+	mov    0x10(%rsp),%r9
+	cmp    $0xffffffffffffffff,%rax
+	mov    %rax,%r12
+	je     6000 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1bc0>
+	subq   $0x1,(%r9)
+	je     56c0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1280>
+	cmp    $0x6,%r12
+	je     5a40 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1600>
+	mov    0x6040(%rip),%rax        
+	mov    0x5e91(%rip),%rsi        
+	cmp    %rsi,0x18(%rax)
+	jne    63c0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1f80>
+	mov    0x5e78(%rip),%r12        
+	test   %r12,%r12
+	je     6580 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2140>
+	addq   $0x1,(%r12)
+	mov    0x8(%r12),%rax
+	mov    0x5fae(%rip),%rsi        
+	mov    %r12,%rdi
+	mov    0x90(%rax),%rax
+	test   %rax,%rax
+	je     6570 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2130>
+	call   *%rax
+	mov    %rax,%r13
+	mov    (%r12),%rax
+	lea    -0x1(%rax),%rdx
+	test   %r13,%r13
+	je     6538 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x20f8>
+	mov    %rdx,(%r12)
+	test   %rdx,%rdx
+	je     5980 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1540>
+	call   2670 <PyDict_New@plt>
+	mov    %rax,%r12
+	test   %rax,%rax
+	je     6658 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2218>
+	mov    0x5fc0(%rip),%rax        
+	mov    0x5e01(%rip),%rbx        
+	cmp    %rbx,0x18(%rax)
+	jne    67f0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x23b0>
+	mov    0x5de8(%rip),%r8        
+	test   %r8,%r8
+	je     6980 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2540>
+	addq   $0x1,(%r8)
+	mov    0x8(%r8),%rax
+	mov    %r8,0x10(%rsp)
+	mov    %r8,%rdi
+	mov    0x5ef8(%rip),%rsi        
+	mov    0x90(%rax),%rax
+	test   %rax,%rax
+	je     69d0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2590>
+	call   *%rax
+	mov    0x10(%rsp),%r8
+	mov    %rax,%r9
+	test   %r9,%r9
+	je     6998 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2558>
+	subq   $0x1,(%r8)
+	je     5e38 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x19f8>
+	mov    0x8(%r9),%rax
+	cmp    0x5498(%rip),%rax        
+	je     6a40 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2600>
+	cmp    0x8(%rsp),%rax
+	je     6b68 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2728>
+	cmp    0x5510(%rip),%rax        
+	jne    6430 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1ff0>
+	mov    0x10(%r9),%rcx
 	mov    0x10(%rcx),%edx
 	test   $0x4,%dl
-	je     4268 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x628>
-	xor    %r15d,%r15d
+	je     6430 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1ff0>
+	xor    %r8d,%r8d
 	and    $0x20,%edx
-	mov    0x8(%rcx),%rbp
-	jne    3d98 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x158>
-	mov    0x18(%rbx),%r15
-	call   25d0 <PyThreadState_Get@plt>
-	mov    0x20(%rax),%ecx
-	lea    0x1(%rcx),%edx
-	mov    0x41de(%rip),%rcx        
+	mov    0x8(%rcx),%rbx
+	je     5c10 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x17d0>
+	mov    %r8,0x10(%rsp)
+	mov    %r9,0x8(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x8(%rsp),%r9
+	mov    0x10(%rsp),%r8
+	mov    0x20(%rax),%edi
+	mov    0x545f(%rip),%r15        
+	lea    0x1(%rdi),%edx
+	cmp    (%r15),%edx
 	mov    %edx,0x20(%rax)
-	cmp    (%rcx),%edx
-	jg     4c58 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1018>
-	mov    %rcx,0x8(%rsp)
+	jg     6d9b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x295b>
+	mov    %r9,0x10(%rsp)
 	xor    %esi,%esi
-	mov    %r15,%rdi
-	call   *%rbp
-	mov    %rax,%rbp
-	call   25d0 <PyThreadState_Get@plt>
-	mov    0x8(%rsp),%rcx
-	mov    0x20(%rax),%edi
-	lea    -0x1(%rdi),%edx
+	mov    %r8,%rdi
+	call   *%rbx
+	mov    %rax,0x8(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x8(%rsp),%r8
+	mov    0x10(%rsp),%r9
+	mov    0x20(%rax),%ebx
+	lea    -0x1(%rbx),%edx
 	mov    %edx,0x20(%rax)
-	mov    (%rcx),%eax
-	lea    -0x32(%rax),%ecx
+	mov    (%r15),%eax
 	cmp    $0xc8,%eax
-	jg     3de9 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1a9>
+	lea    -0x32(%rax),%ecx
+	jg     4b74 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x734>
 	sar    $0x2,%eax
 	lea    (%rax,%rax,2),%ecx
 	cmp    %ecx,%edx
-	jl     42c0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x680>
-	test   %rbp,%rbp
-	je     4ad0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe90>
-	subq   $0x1,(%rbx)
-	je     42b0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x670>
-	mov    0x495d(%rip),%rsi        
-	mov    %rbp,%rdx
-	mov    %r13,%rdi
-	call   2690 <PyDict_SetItem@plt>
+	jl     5f28 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1ae8>
+	test   %r8,%r8
+	je     6bb0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2770>
+	subq   $0x1,(%r9)
+	je     5e70 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1a30>
+	mov    0x5dd2(%rip),%rsi        
+	mov    %r8,%rdx
+	mov    %r12,%rdi
+	mov    %r8,0x8(%rsp)
+	call   26b0 <PyDict_SetItem@plt>
+	mov    0x8(%rsp),%r8
 	test   %eax,%eax
-	js     47a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb60>
-	subq   $0x1,0x0(%rbp)
-	je     43b0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x770>
-	mov    0x8(%r14),%rax
-	mov    0x49ac(%rip),%r15        
-	mov    0x80(%rax),%rbp
-	test   %rbp,%rbp
-	je     4b00 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xec0>
-	call   25d0 <PyThreadState_Get@plt>
-	mov    0x4138(%rip),%rcx        
-	mov    0x20(%rax),%ebx
-	lea    0x1(%rbx),%edx
-	mov    %edx,0x20(%rax)
-	cmp    (%rcx),%edx
-	jg     4bd0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf90>
+	js     6918 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x24d8>
+	subq   $0x1,(%r8)
+	je     5fd0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1b90>
+	mov    0x8(%r13),%rax
+	mov    0x5e38(%rip),%rbx        
+	mov    0x80(%rax),%rcx
+	test   %rcx,%rcx
+	je     6c30 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x27f0>
 	mov    %rcx,0x8(%rsp)
-	mov    %r13,%rdx
-	mov    %r15,%rsi
-	mov    %r14,%rdi
-	call   *%rbp
-	mov    %rax,%rbp
-	call   25d0 <PyThreadState_Get@plt>
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x539f(%rip),%r15        
 	mov    0x20(%rax),%ecx
-	lea    -0x1(%rcx),%edx
+	lea    0x1(%rcx),%edx
+	cmp    (%r15),%edx
 	mov    0x8(%rsp),%rcx
 	mov    %edx,0x20(%rax)
-	mov    (%rcx),%eax
-	lea    -0x32(%rax),%ecx
+	jg     6d0d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x28cd>
+	mov    %r12,%rdx
+	mov    %rbx,%rsi
+	mov    %r13,%rdi
+	call   *%rcx
+	mov    %rax,0x8(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x8(%rsp),%r8
+	mov    0x20(%rax),%ebx
+	lea    -0x1(%rbx),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%r15),%eax
 	cmp    $0xc8,%eax
-	jg     3e99 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x259>
-	sar    $0x2,%eax
-	lea    (%rax,%rax,2),%ecx
+	lea    -0x32(%rax),%ecx
+	jle    5c00 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x17c0>
 	cmp    %ecx,%edx
-	jl     43e0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x7a0>
-	test   %rbp,%rbp
-	je     4c28 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xfe8>
-	subq   $0x1,(%r14)
-	je     43d0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x790>
+	jl     60c0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1c80>
+	test   %r8,%r8
+	je     6d72 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2932>
 	subq   $0x1,0x0(%r13)
-	je     43c0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x780>
-	mov    0x8(%rbp),%rax
-	mov    0x48ae(%rip),%rsi        
-	mov    %rbp,%rdi
+	je     6080 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1c40>
+	subq   $0x1,(%r12)
+	je     6060 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1c20>
+	mov    0x8(%r8),%rax
+	mov    %r8,0x8(%rsp)
+	mov    %r8,%rdi
+	mov    0x5d12(%rip),%rsi        
 	mov    0x90(%rax),%rax
 	test   %rax,%rax
-	je     4bc0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf80>
+	je     6d60 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2920>
 	call   *%rax
-	mov    %rax,%r14
-	mov    0x0(%rbp),%rax
-	sub    $0x1,%rax
-	test   %r14,%r14
-	je     4bf8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xfb8>
-	mov    %rax,0x0(%rbp)
-	test   %rax,%rax
-	je     43f0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x7b0>
-	mov    0x8(%r14),%rdx
+	mov    0x8(%rsp),%r8
+	mov    %rax,%r12
+	test   %r12,%r12
+	je     6d30 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x28f0>
+	subq   $0x1,(%r8)
+	je     61f0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1db0>
+	mov    0x8(%r12),%rdx
 	mov    0x70(%rdx),%rax
 	test   %rax,%rax
-	je     4750 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb10>
+	je     68b0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2470>
 	mov    0x8(%rax),%rax
 	test   %rax,%rax
-	je     4750 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb10>
-	mov    0x47db(%rip),%rsi        
-	mov    %r14,%rdi
+	je     68b0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2470>
+	mov    0x5c07(%rip),%rsi        
+	mov    %r12,%rdi
 	call   *%rax
-	mov    %rax,%rbp
+	mov    %rax,%r8
 	test   %rax,%rax
-	je     476c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb2c>
-	subq   $0x1,(%r14)
-	je     4410 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x7d0>
-	mov    0x8(%rbp),%rax
-	mov    0x47d5(%rip),%rsi        
-	mov    %rbp,%rdi
+	je     68cc <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x248c>
+	subq   $0x1,(%r12)
+	je     62e8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1ea8>
+	mov    0x8(%r8),%rax
+	mov    %r8,0x8(%rsp)
+	mov    %r8,%rdi
+	mov    0x5bf8(%rip),%rsi        
 	mov    0x90(%rax),%rax
 	test   %rax,%rax
-	je     4d10 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x10d0>
+	je     6e91 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2a51>
 	call   *%rax
-	mov    %rax,%r14
-	mov    0x0(%rbp),%rax
-	sub    $0x1,%rax
-	test   %r14,%r14
-	je     4d20 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x10e0>
-	mov    %rax,0x0(%rbp)
-	test   %rax,%rax
-	je     4430 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x7f0>
-	mov    0x8(%r14),%rax
-	cmp    0x3fd4(%rip),%rax        
-	jne    42d0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x690>
-	mov    0x18(%r14),%r12
-	test   %r12,%r12
-	je     42d0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x690>
-	mov    0x10(%r14),%rbp
-	addq   $0x1,(%r12)
-	addq   $0x1,0x0(%rbp)
-	subq   $0x1,(%r14)
-	je     4258 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x618>
-	mov    %r12,0x10(%rsp)
-	mov    0x8(%rbp),%rax
-	cmp    (%rsp),%rax
-	je     4df0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11b0>
-	cmp    0x401f(%rip),%rax        
-	jne    47d8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb98>
-	mov    0x10(%rbp),%rdx
-	mov    0x10(%rdx),%eax
-	test   $0x8,%al
-	je     4e90 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1250>
-	mov    0x8(%rdx),%rbx
-	xor    %r13d,%r13d
-	test   $0x20,%al
-	jne    3ff5 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x3b5>
-	mov    0x18(%rbp),%r13
-	call   25d0 <PyThreadState_Get@plt>
-	mov    0x20(%rax),%ecx
-	lea    0x1(%rcx),%edx
-	mov    0x3f81(%rip),%rcx        
-	mov    %edx,0x20(%rax)
-	cmp    (%rcx),%edx
-	jg     4f00 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x12c0>
-	mov    %rcx,(%rsp)
-	mov    %r13,%rdi
-	mov    %r12,%rsi
-	call   *%rbx
-	mov    %rax,%rbx
-	call   25d0 <PyThreadState_Get@plt>
-	mov    (%rsp),%rcx
-	mov    0x20(%rax),%edi
-	lea    -0x1(%rdi),%edx
-	mov    %edx,0x20(%rax)
-	mov    (%rcx),%eax
-	cmp    $0xc8,%eax
-	jle    4a78 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe38>
-	sub    $0x32,%eax
-	cmp    %eax,%edx
-	jl     4cf8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x10b8>
+	mov    0x8(%rsp),%r8
+	mov    %rax,%r15
+	test   %r15,%r15
+	je     6e6a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2a2a>
+	subq   $0x1,(%r8)
+	je     5c50 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1810>
+	mov    0x523c(%rip),%rax        
+	cmp    %rax,0x8(%r15)
+	jne    5f50 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1b10>
+	mov    0x18(%r15),%rbx
 	test   %rbx,%rbx
-	je     4e10 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11d0>
+	je     5f50 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1b10>
+	mov    0x10(%r15),%r12
+	addq   $0x1,(%rbx)
+	addq   $0x1,(%r12)
+	subq   $0x1,(%r15)
+	je     5d10 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x18d0>
+	mov    %rbx,%rsi
+	mov    %r12,%rdi
+	call   3740 <__Pyx_PyObject_CallOneArg>
+	subq   $0x1,(%rbx)
+	mov    %rax,%r13
+	je     68f8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x24b8>
+	test   %r13,%r13
+	je     6ec5 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2a85>
 	subq   $0x1,(%r12)
-	je     4880 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc40>
+	je     6508 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x20c8>
 	subq   $0x1,0x0(%rbp)
-	je     4530 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x8f0>
+	je     64f8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x20b8>
 	xor    %edi,%edi
-	xor    %r12d,%r12d
-	xor    %r15d,%r15d
-	call   23d0 <PyList_New@plt>
-	mov    %rax,%rbp
+	xor    %ebp,%ebp
+	xor    %ebx,%ebx
+	call   23e0 <PyList_New@plt>
+	mov    %rax,%r9
 	test   %rax,%rax
-	je     4d50 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1110>
-	mov    %r15,%rdi
-	call   2580 <PyLong_FromLong@plt>
-	mov    %rax,%r13
+	je     6eec <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2aac>
+	mov    %rbx,%rdi
+	mov    %r9,0x8(%rsp)
+	call   2590 <PyLong_FromLong@plt>
+	mov    0x8(%rsp),%r9
 	test   %rax,%rax
-	je     41c1 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x581>
-	test   %r12,%r12
-	je     40a7 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x467>
-	subq   $0x1,(%r12)
-	je     4440 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x800>
-	mov    0x8(%r13),%rdx
-	cmp    0x3f06(%rip),%rdx        
-	mov    0x4657(%rip),%rsi        
-	jne    4ba0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf60>
-	mov    0x10(%r13),%rax
+	mov    %rax,%r15
+	je     6bf0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x27b0>
+	test   %rbp,%rbp
+	je     4dce <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x98e>
+	subq   $0x1,0x0(%rbp)
+	je     63a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1f60>
+	mov    0x8(%r15),%rdx
+	cmp    0x51df(%rip),%rdx        
+	mov    0x5af8(%rip),%rsi        
+	jne    6cc2 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2882>
+	mov    0x10(%r15),%rax
 	lea    0x1(%rax),%rcx
 	cmp    $0x2,%rcx
-	ja     4c80 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1040>
+	ja     6dc8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2988>
 	test   %rax,%rax
-	je     4ca8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1068>
-	mov    0x18(%r13),%edx
+	je     6e0f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x29cf>
+	mov    0x18(%r15),%edx
 	mov    $0x2,%edi
 	sub    %rdx,%rdi
 	lea    0x2(%rdx),%rcx
 	cmp    $0xffffffffffffffff,%rax
 	cmovne %rcx,%rdi
-	call   2580 <PyLong_FromLong@plt>
-	mov    %rax,%r14
-	test   %r14,%r14
-	je     4b70 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf30>
-	mov    0x8(%rbx),%rax
-	mov    0x70(%rax),%r12
-	test   %r12,%r12
-	je     4628 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x9e8>
-	cmpq   $0x0,0x8(%r12)
-	je     4628 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x9e8>
-	mov    0x3e79(%rip),%rdx        
-	mov    %r14,%rsi
-	mov    %r13,%rdi
-	call   26d0 <PySlice_New@plt>
-	test   %rax,%rax
-	je     4644 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xa04>
-	mov    %rax,(%rsp)
-	mov    %rax,%rsi
-	mov    %rbx,%rdi
-	call   *0x8(%r12)
-	mov    (%rsp),%r8
+	mov    %r9,0x8(%rsp)
+	call   2590 <PyLong_FromLong@plt>
+	mov    0x8(%rsp),%r9
 	mov    %rax,%r12
-	subq   $0x1,(%r8)
-	je     4520 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x8e0>
 	test   %r12,%r12
-	je     4644 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xa04>
-	subq   $0x1,(%r14)
-	je     4400 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x7c0>
-	mov    0x10(%rbp),%rax
-	cmp    0x20(%rbp),%rax
-	jge    4cb8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1078>
-	mov    0x18(%rbp),%rdx
-	addq   $0x1,(%r12)
-	mov    %r12,(%rdx,%rax,8)
-	add    $0x1,%rax
-	mov    %rax,0x10(%rbp)
-	subq   $0x1,(%r12)
-	je     4420 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x7e0>
-	add    $0x2,%r15
-	cmp    $0xc,%r15
-	je     45e8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x9a8>
+	je     6c95 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2855>
+	mov    0x8(%r13),%rax
+	mov    0x70(%rax),%rcx
+	test   %rcx,%rcx
+	je     6788 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2348>
+	cmpq   $0x0,0x8(%rcx)
+	mov    %rcx,0x8(%rsp)
+	je     6788 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2348>
+	mov    0x5144(%rip),%rdx        
+	mov    %r12,%rsi
 	mov    %r15,%rdi
-	mov    %r13,%r12
-	call   2580 <PyLong_FromLong@plt>
-	mov    %rax,%r13
+	mov    %r9,0x10(%rsp)
+	call   26f0 <PySlice_New@plt>
+	mov    0x10(%rsp),%r9
 	test   %rax,%rax
-	jne    4097 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x457>
-	lea    0x1f80(%rip),%rax        
-	xor    %r14d,%r14d
-	mov    %r12,%r13
-	movl   $0xa,0x45fc(%rip)        
-	mov    %rax,0x45e9(%rip)        
-	movl   $0x50a,0x45e7(%rip)        
+	mov    %rax,%rbp
+	je     67ae <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x236e>
+	mov    0x8(%rsp),%rcx
+	mov    %rax,%rsi
+	mov    %r13,%rdi
+	call   *0x8(%rcx)
 	subq   $0x1,0x0(%rbp)
-	je     4ac0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe80>
-	test   %r14,%r14
-	je     5295 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1655>
-	mov    (%r14),%rax
-	mov    %rbx,%r12
-	mov    %r14,%rbp
-	sub    $0x1,%rax
-	nopw   0x0(%rax,%rax,1)
-	mov    %rax,0x0(%rbp)
-	xor    %ebx,%ebx
-	xor    %r15d,%r15d
-	test   %rax,%rax
-	jne    44a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x860>
-	nopw   0x0(%rax,%rax,1)
-	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    4704 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xac4>
-	nopl   (%rax)
-	mov    %r12,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    3cd1 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x91>
-	nopl   (%rax)
+	mov    0x10(%rsp),%r9
+	mov    %rax,%r8
+	je     64a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2060>
+	test   %r8,%r8
+	je     67ae <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x236e>
+	subq   $0x1,(%r12)
+	je     6268 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1e28>
+	mov    0x10(%r9),%rax
+	cmp    0x20(%r9),%rax
+	jge    6e19 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x29d9>
+	mov    0x18(%r9),%rdx
+	addq   $0x1,(%r8)
+	mov    %r8,(%rdx,%rax,8)
+	add    $0x1,%rax
+	mov    %rax,0x10(%r9)
+	subq   $0x1,(%r8)
+	je     6360 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1f20>
+	add    $0x2,%rbx
+	cmp    $0xc,%rbx
+	je     6690 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2250>
+	mov    %r15,%rbp
+	jmp    4da0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x960>
+	nopl   0x0(%rax)
 	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    3d46 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x106>
-	nopl   (%rax)
-	mov    %r14,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    3fb7 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x377>
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    44d0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x90>
 	nopl   (%rax)
-	mov    0x80(%rax),%rbp
-	mov    0x456a(%rip),%r15        
-	test   %rbp,%rbp
-	je     4f21 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x12e1>
-	call   25d0 <PyThreadState_Get@plt>
-	mov    0x20(%rax),%ecx
-	lea    0x1(%rcx),%edx
-	mov    0x3cf7(%rip),%rcx        
-	mov    %edx,0x20(%rax)
-	cmp    (%rcx),%edx
-	jg     4f39 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x12f9>
+	mov    0x50a1(%rip),%rcx        
 	mov    %rcx,0x8(%rsp)
-	xor    %edx,%edx
-	mov    %r15,%rsi
-	mov    %rbx,%rdi
-	call   *%rbp
-	jmp    3dc1 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x181>
-	mov    %rbx,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    3e04 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1c4>
-	nopl   (%rax)
-	call   25d0 <PyThreadState_Get@plt>
-	movb   $0x0,0x24(%rax)
-	jmp    3df1 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1b1>
-	xchg   %ax,%ax
-	cmp    (%rsp),%rax
-	je     4dd8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1198>
-	cmp    0x3d0f(%rip),%rax        
-	jne    4d80 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1140>
-	mov    0x10(%r14),%rcx
+	cmp    %rcx,%rax
+	je     5fe0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1ba0>
+	cmp    0x50cc(%rip),%rax        
+	jne    59d8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1598>
+	mov    0x10(%rbp),%rcx
 	mov    0x10(%rcx),%edx
 	test   $0x4,%dl
-	je     4d80 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1140>
-	xor    %ebp,%ebp
+	je     59d8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1598>
+	xor    %r13d,%r13d
 	and    $0x20,%edx
-	mov    0x8(%rcx),%rbx
-	jne    4306 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x6c6>
-	mov    0x18(%r14),%rbp
-	call   25d0 <PyThreadState_Get@plt>
+	mov    0x8(%rcx),%r12
+	jne    4f4a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb0a>
+	mov    0x18(%rbp),%r13
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x5032(%rip),%r15        
 	mov    0x20(%rax),%ecx
 	lea    0x1(%rcx),%edx
-	mov    0x3c70(%rip),%rcx        
 	mov    %edx,0x20(%rax)
-	cmp    (%rcx),%edx
-	jg     4ec8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1288>
-	mov    %rbp,%rdi
-	mov    %rcx,(%rsp)
+	cmp    (%r15),%edx
+	jg     6300 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1ec0>
+	mov    %r13,%rdi
 	xor    %esi,%esi
-	call   *%rbx
-	mov    %rax,%rbx
-	call   25d0 <PyThreadState_Get@plt>
+	call   *%r12
+	mov    %rax,%r13
+	call   25e0 <PyThreadState_Get@plt>
 	mov    0x20(%rax),%edi
 	lea    -0x1(%rdi),%edx
-	mov    (%rsp),%rcx
 	mov    %edx,0x20(%rax)
-	mov    (%rcx),%eax
+	mov    (%r15),%eax
 	lea    -0x32(%rax),%ecx
 	cmp    $0xc8,%eax
-	jg     4355 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x715>
+	jg     4f94 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb54>
 	sar    $0x2,%eax
 	lea    (%rax,%rax,2),%ecx
 	cmp    %ecx,%edx
-	jl     4b60 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf20>
-	mov    %r14,%rbp
-	test   %rbx,%rbx
-	jne    405f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x41f>
-	call   25f0 <PyErr_Occurred@plt>
+	jl     56b0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1270>
+	mov    %rbp,%r12
+	test   %r13,%r13
+	jne    46a9 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x269>
+	call   2600 <PyErr_Occurred@plt>
 	test   %rax,%rax
-	je     51cd <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x158d>
-	lea    0x1dca(%rip),%rax        
-	xor    %r12d,%r12d
-	xor    %r13d,%r13d
-	movl   $0x9,0x4446(%rip)        
-	mov    %rax,0x4433(%rip)        
-	movl   $0x4fb,0x4431(%rip)        
-	mov    (%r14),%rax
-	lea    -0x1(%rax),%rdx
-	jmp    457b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x93b>
-	nopl   0x0(%rax,%rax,1)
-	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    3e29 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1e9>
-	nopl   (%rax)
-	mov    %r13,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    3ebf <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x27f>
-	nopl   (%rax)
-	mov    %r14,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    3eb4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x274>
-	nopl   (%rax)
-	call   25d0 <PyThreadState_Get@plt>
-	movb   $0x0,0x24(%rax)
-	jmp    3ea1 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x261>
-	xchg   %ax,%ax
-	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    3f00 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2c0>
-	nopl   (%rax)
-	mov    %r14,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    416e <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x52e>
-	nopl   (%rax)
-	mov    %r14,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    3f40 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x300>
-	nopl   (%rax)
-	mov    %r12,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    419c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x55c>
-	nopl   (%rax)
-	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    3f81 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x341>
-	nopl   (%rax)
-	mov    %r12,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    40a7 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x467>
-	nopl   (%rax)
-	mov    0x42c1(%rip),%rdi        
-	lea    0x426a(%rip),%rdx        
-	lea    0x426b(%rip),%rsi        
-	call   3bc0 <__Pyx__GetModuleGlobalName>
-	mov    %rax,%r12
-	test   %r12,%r12
-	jne    3c8f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x4f>
-	lea    0x1ccb(%rip),%rax        
-	movl   $0x9,0x434d(%rip)        
-	mov    %rax,0x433a(%rip)        
-	movl   $0x4c5,0x4338(%rip)        
-	xor    %r13d,%r13d
+	jne    4fd0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb90>
+	mov    0x4f9f(%rip),%rax        
+	lea    0x30c0(%rip),%rsi        
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
 	nopl   0x0(%rax,%rax,1)
-	mov    0x4321(%rip),%rcx        
-	mov    0x4327(%rip),%edx        
-	lea    0x1d34(%rip),%rdi        
-	mov    0x4316(%rip),%esi        
-	call   33e0 <__Pyx_AddTraceback>
-	test   %r12,%r12
-	je     44ce <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x88e>
+	lea    0x31a1(%rip),%rax        
+	xor    %ebp,%ebp
+	movl   $0xb,0x5a11(%rip)        
+	mov    %rax,0x59fe(%rip)        
+	movl   $0x50d,0x59fc(%rip)        
+	xor    %r15d,%r15d
+	xor    %r8d,%r8d
 	subq   $0x1,(%r12)
-	je     4510 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x8d0>
-	xor    %r12d,%r12d
+	jne    604c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1c0c>
+	xor    %r9d,%r9d
+	xor    %ebx,%ebx
+	xor    %r13d,%r13d
+	mov    %r12,%rdi
+	mov    %r8,0x10(%rsp)
+	mov    %r9,0x8(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
 	test   %r13,%r13
-	je     44da <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x89a>
-	subq   $0x1,0x0(%r13)
-	je     4500 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x8c0>
-	mov    0x18(%rsp),%rax
+	mov    0x8(%rsp),%r9
+	mov    0x10(%rsp),%r8
+	je     5043 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc03>
+	mov    0x0(%r13),%rax
+	sub    $0x1,%rax
+	mov    %rax,0x0(%r13)
+	test   %rax,%rax
+	je     54a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1060>
+	test   %r8,%r8
+	je     5052 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc12>
+	subq   $0x1,(%r8)
+	je     54c8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1088>
+	test   %rbx,%rbx
+	je     5061 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc21>
+	subq   $0x1,(%rbx)
+	je     54e0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x10a0>
+	test   %r9,%r9
+	je     5070 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc30>
+	subq   $0x1,(%r9)
+	je     5490 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1050>
+	mov    0x5971(%rip),%rcx        
+	mov    0x5977(%rip),%edx        
+	lea    0x3144(%rip),%rdi        
+	mov    0x5966(%rip),%esi        
+	call   3c50 <__Pyx_AddTraceback>
+	test   %r14,%r14
+	je     50a1 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc61>
+	subq   $0x1,(%r14)
+	je     5500 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x10c0>
+	xor    %r14d,%r14d
+	test   %rbp,%rbp
+	je     50b1 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc71>
+	subq   $0x1,0x0(%rbp)
+	je     5470 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1030>
+	test   %r15,%r15
+	je     50c0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc80>
+	subq   $0x1,(%r15)
+	je     5480 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1040>
+	mov    0x28(%rsp),%rax
 	xor    %fs:0x28,%rax
-	jne    520a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x15ca>
-	add    $0x28,%rsp
-	mov    %r12,%rax
+	jne    7306 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2ec6>
+	add    $0x38,%rsp
+	mov    %r14,%rax
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
+	cs nopw 0x0(%rax,%rax,1)
+	cmp    0x8(%rsp),%rax
+	je     6200 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1dc0>
+	cmp    0x4eee(%rip),%rax        
+	jne    5df0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x19b0>
+	mov    0x10(%r12),%rcx
+	mov    0x10(%rcx),%edx
+	test   $0x4,%dl
+	je     5df0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x19b0>
+	xor    %r13d,%r13d
+	and    $0x20,%edx
+	mov    0x8(%rcx),%rbp
+	jne    512a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xcea>
+	mov    0x18(%r12),%r13
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x4e52(%rip),%r15        
+	mov    0x20(%rax),%ebx
+	lea    0x1(%rbx),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%r15),%edx
+	jg     6598 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2158>
+	xor    %esi,%esi
 	mov    %r13,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    44da <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x89a>
-	nopw   0x0(%rax,%rax,1)
+	call   *%rbp
+	mov    %rax,%rbp
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%esi
+	lea    -0x1(%rsi),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%r15),%eax
+	lea    -0x32(%rax),%ecx
+	cmp    $0xc8,%eax
+	jg     5173 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd33>
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%ecx
+	cmp    %ecx,%edx
+	jl     58b0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1470>
+	mov    %r12,%r13
+	test   %rbp,%rbp
+	jne    47d0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x390>
+	call   2600 <PyErr_Occurred@plt>
+	test   %rax,%rax
+	je     71f8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2db8>
+	lea    0x2fdc(%rip),%rax        
 	xor    %ebp,%ebp
+	movl   $0xb,0x584c(%rip)        
+	mov    %rax,0x5839(%rip)        
+	movl   $0x51f,0x5837(%rip)        
+	jmp    4ff4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xbb4>
+	xchg   %ax,%ax
+	mov    %r13,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    4598 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x158>
+	nopl   (%rax)
+	cmp    0x8(%rsp),%rax
+	je     6410 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1fd0>
+	cmp    0x4e0e(%rip),%rax        
+	jne    5ed0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1a90>
+	mov    0x10(%r12),%rcx
+	mov    0x10(%rcx),%edx
+	test   $0x4,%dl
+	je     5ed0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1a90>
+	xor    %ebx,%ebx
+	and    $0x20,%edx
+	mov    0x8(%rcx),%r13
+	jne    5209 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xdc9>
+	mov    0x18(%r12),%rbx
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x4d73(%rip),%r15        
+	mov    0x20(%rax),%edi
+	lea    0x1(%rdi),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%r15),%edx
+	jg     6860 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2420>
+	xor    %esi,%esi
+	mov    %rbx,%rdi
+	call   *%r13
+	mov    %rax,0x10(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%esi
+	lea    -0x1(%rsi),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%r15),%eax
+	mov    0x10(%rsp),%r8
+	cmp    $0xc8,%eax
+	lea    -0x32(%rax),%ecx
+	jg     525a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe1a>
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%ecx
+	cmp    %ecx,%edx
+	jl     5950 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1510>
+	mov    %r12,%r13
+	test   %r8,%r8
+	jne    48f3 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x4b3>
+	call   2600 <PyErr_Occurred@plt>
+	test   %rax,%rax
+	je     725f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2e1f>
+	lea    0x2ef5(%rip),%rax        
+	movl   $0xc,0x5767(%rip)        
+	mov    %rax,0x5754(%rip)        
+	movl   $0x53a,0x5752(%rip)        
+	jmp    4ff4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xbb4>
+	nopl   0x0(%rax,%rax,1)
 	mov    %r12,%rdi
-	mov    %rbp,%r12
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    44ce <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x88e>
-	nop
-	mov    %r8,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    415b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x51b>
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    46b4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x274>
 	nopl   (%rax)
+	mov    0x5701(%rip),%r13        
+	mov    %r13,0x20(%rsp)
+	cmp    0x8(%rsp),%rax
+	je     6700 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x22c0>
+	cmp    0x4d1a(%rip),%rax        
+	jne    6120 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1ce0>
+	mov    0x10(%rbx),%rdx
+	mov    0x10(%rdx),%eax
+	test   $0x8,%al
+	je     69e8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x25a8>
+	mov    0x8(%rdx),%rcx
+	xor    %r12d,%r12d
+	mov    %rcx,0x10(%rsp)
+	test   $0x20,%al
+	jne    52ff <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xebf>
+	mov    0x18(%rbx),%r12
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x4c7d(%rip),%r15        
+	mov    0x20(%rax),%edi
+	lea    0x1(%rdi),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%r15),%edx
+	jg     6ad8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2698>
+	mov    %r13,%rsi
+	mov    %r12,%rdi
+	mov    0x10(%rsp),%rax
+	call   *%rax
+	mov    %rax,0x10(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x10(%rsp),%r9
+	mov    0x20(%rax),%esi
+	lea    -0x1(%rsi),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%r15),%eax
+	cmp    $0xc8,%eax
+	jle    5940 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1500>
+	sub    $0x32,%eax
+	cmp    %eax,%edx
+	jl     5e50 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1a10>
+	test   %r9,%r9
+	je     6af8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x26b8>
+	mov    %rbx,%r12
+	jmp    498a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x54a>
+	nopl   0x0(%rax)
 	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    406a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x42a>
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    45fa <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1ba>
 	nopl   (%rax)
-	call   2700 <PyObject_GetAttr@plt>
-	mov    %rax,%r14
-	jmp    3cb3 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x73>
+	mov    %r13,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    46f5 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2b5>
 	nopl   (%rax)
-	lea    0x1bf1(%rip),%rax        
-	mov    %r12,%r14
-	xor    %r13d,%r13d
-	xor    %r12d,%r12d
-	mov    %rax,0x4261(%rip)        
-	movl   $0x9,0x4263(%rip)        
-	movl   $0x4c7,0x4255(%rip)        
-	mov    %rdx,(%r14)
-	test   %rdx,%rdx
-	jne    44a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x860>
-	mov    %r14,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    44a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x860>
-	nopl   0x0(%rax)
-	mov    0x4179(%rip),%rdi        
-	call   3b40 <__Pyx_GetBuiltinName>
-	mov    %rax,%r12
-	jmp    446d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x82d>
-	nopl   0x0(%rax)
-	subq   $0x1,(%r14)
-	mov    $0x0,%r12d
-	lea    0x1b87(%rip),%rax        
-	mov    %rax,0x4200(%rip)        
-	movl   $0x9,0x4202(%rip)        
-	movl   $0x4ca,0x41f4(%rip)        
-	jne    44a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x860>
-	jmp    4587 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x947>
-	nopl   0x0(%rax)
-	mov    0x41b1(%rip),%rdi        
-	mov    %rbp,%rsi
-	call   2450 <PyUnicode_Join@plt>
-	mov    %rax,%r12
-	test   %rax,%rax
-	je     4f5c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x131c>
-	subq   $0x1,0x0(%rbp)
-	je     4a88 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe48>
-	subq   $0x1,(%rbx)
-	jne    44d3 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x893>
-	mov    %r12,%rbp
-	mov    %rbx,%r12
-	jmp    4512 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x8d2>
-	nopl   0x0(%rax,%rax,1)
-	mov    0x18(%rax),%rdx
-	mov    0x394d(%rip),%rax        
-	lea    0x1b8e(%rip),%rsi        
-	mov    (%rax),%rdi
-	xor    %eax,%eax
-	call   26c0 <PyErr_Format@plt>
-	subq   $0x1,0x0(%rbp)
-	lea    0x1af8(%rip),%rax        
-	mov    %rax,0x4171(%rip)        
-	movl   $0xa,0x4173(%rip)        
-	movl   $0x510,0x4165(%rip)        
-	je     4aa8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe68>
-	mov    (%r14),%rax
-	mov    %rbx,%r12
-	lea    -0x1(%rax),%rdx
-	jmp    457b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x93b>
-	mov    0x4091(%rip),%rdi        
-	lea    0x402a(%rip),%rdx        
-	lea    0x402b(%rip),%rsi        
-	call   3bc0 <__Pyx__GetModuleGlobalName>
+	mov    %r13,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    47db <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x39b>
+	nopl   (%rax)
+	mov    %r12,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    472e <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2ee>
+	nopl   (%rax)
+	mov    $0x1,%edi
+	call   25d0 <PyTuple_New@plt>
 	mov    %rax,%rbp
-	test   %rbp,%rbp
-	jne    3d0f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xcf>
-	lea    0x1a9b(%rip),%rax        
-	xor    %ebx,%ebx
-	xor    %r15d,%r15d
-	movl   $0x9,0x4118(%rip)        
-	mov    %rax,0x4105(%rip)        
-	mov    0x0(%r13),%rax
-	movl   $0x4cc,0x40ff(%rip)        
-	sub    $0x1,%rax
-	mov    %rax,0x0(%r13)
 	test   %rax,%rax
-	je     5288 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1648>
-	subq   $0x1,(%r14)
-	mov    $0x0,%r13d
-	mov    $0x0,%r12d
-	je     4740 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb00>
-	test   %rbp,%rbp
-	je     4704 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xac4>
+	je     6100 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1cc0>
+	addq   $0x1,(%rbx)
+	mov    %rbx,0x18(%rax)
+	mov    0x8(%r12),%rax
+	mov    0x80(%rax),%r13
+	test   %r13,%r13
+	je     6ffd <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2bbd>
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x4b99(%rip),%r15        
+	mov    0x20(%rax),%ecx
+	lea    0x1(%rcx),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%r15),%edx
+	jg     7052 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2c12>
+	xor    %edx,%edx
+	mov    %r12,%rdi
+	mov    %rbp,%rsi
+	call   *%r13
+	mov    %rax,%r13
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%edi
+	lea    -0x1(%rdi),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%r15),%eax
+	lea    -0x32(%rax),%ecx
+	cmp    $0xc8,%eax
+	jg     5430 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xff0>
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%ecx
+	cmp    %ecx,%edx
+	jl     6b28 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x26e8>
+	test   %r13,%r13
+	je     707b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2c3b>
 	subq   $0x1,0x0(%rbp)
-	je     4228 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x5e8>
-	test   %r15,%r15
-	je     470f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xacf>
-	subq   $0x1,(%r15)
-	je     4730 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xaf0>
-	test   %rbx,%rbx
-	je     44a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x860>
+	je     6a20 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x25e0>
 	subq   $0x1,(%rbx)
-	jne    44a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x860>
+	jne    545a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x101a>
 	mov    %rbx,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    44a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x860>
-	nop
+	call   24b0 <_Py_Dealloc@plt>
+	test   %r13,%r13
+	jne    46a9 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x269>
+	jmp    4fd0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb90>
+	nopl   0x0(%rax,%rax,1)
+	mov    %rbp,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    50b1 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc71>
+	nopl   (%rax)
 	mov    %r15,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    470f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xacf>
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    50c0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc80>
+	nopl   (%rax)
+	mov    %r9,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    5070 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc30>
+	nopl   (%rax)
+	mov    %r13,%rdi
+	mov    %r8,0x10(%rsp)
+	mov    %r9,0x8(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x8(%rsp),%r9
+	mov    0x10(%rsp),%r8
+	jmp    5043 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc03>
+	nopl   0x0(%rax)
+	mov    %r8,%rdi
+	mov    %r9,0x8(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x8(%rsp),%r9
+	jmp    5052 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc12>
+	nop
+	mov    %rbx,%rdi
+	mov    %r9,0x8(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x8(%rsp),%r9
+	jmp    5061 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc21>
 	nopw   0x0(%rax,%rax,1)
+	xor    %ebx,%ebx
 	mov    %r14,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    46f4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xab4>
+	mov    %rbx,%r14
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    50a1 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc61>
 	nopw   0x0(%rax,%rax,1)
-	mov    0x3829(%rip),%rax        
-	mov    0x18(%rdx),%rdx
-	lea    0x1a66(%rip),%rsi        
-	mov    (%rax),%rdi
-	xor    %eax,%eax
-	call   26c0 <PyErr_Format@plt>
-	lea    0x19d5(%rip),%rax        
-	xor    %r13d,%r13d
-	xor    %r12d,%r12d
-	movl   $0x9,0x4051(%rip)        
-	mov    %rax,0x403e(%rip)        
-	mov    (%r14),%rax
-	movl   $0x4e9,0x4039(%rip)        
-	lea    -0x1(%rax),%rdx
-	jmp    457b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x93b>
-	lea    0x19a1(%rip),%rax        
-	xor    %ebx,%ebx
-	xor    %r15d,%r15d
-	movl   $0x9,0x401e(%rip)        
-	mov    %rax,0x400b(%rip)        
-	mov    0x0(%r13),%rax
-	movl   $0x4e0,0x4005(%rip)        
-	sub    $0x1,%rax
-	jmp    46d5 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xa95>
+	mov    %r8,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    4908 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x4c8>
+	nopl   (%rax)
+	mov    %r13,%rdi
+	mov    %r8,0x10(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x10(%rsp),%r8
+	jmp    48fe <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x4be>
+	nop
+	mov    %r12,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    4840 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x400>
+	nopl   (%rax)
+	mov    $0x1,%edi
+	call   25d0 <PyTuple_New@plt>
+	mov    %rax,%r12
+	test   %rax,%rax
+	je     6340 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1f00>
+	addq   $0x1,(%rbx)
+	mov    %rbx,0x18(%rax)
+	mov    0x8(%r13),%rax
+	mov    0x80(%rax),%rbp
+	test   %rbp,%rbp
+	je     70bb <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2c7b>
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x49fa(%rip),%r15        
+	mov    0x20(%rax),%ecx
+	lea    0x1(%rcx),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%r15),%edx
+	jg     70fe <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2cbe>
+	xor    %edx,%edx
+	mov    %r12,%rsi
+	mov    %r13,%rdi
+	call   *%rbp
+	mov    %rax,%rbp
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%esi
+	lea    -0x1(%rsi),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%r15),%eax
+	lea    -0x32(%rax),%ecx
+	cmp    $0xc8,%eax
+	jg     55ce <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x118e>
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%ecx
+	cmp    %ecx,%edx
+	jl     6c20 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x27e0>
+	test   %rbp,%rbp
+	je     7119 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2cd9>
+	subq   $0x1,(%r12)
+	je     6b90 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2750>
+	subq   $0x1,(%rbx)
+	jne    55f8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11b8>
+	mov    %rbx,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	test   %rbp,%rbp
+	jne    47d0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x390>
+	mov    %r13,%r12
+	jmp    5195 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd55>
 	nopl   0x0(%rax)
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%eax
+	jmp    468e <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x24e>
+	nopl   0x0(%rax,%rax,1)
+	mov    %r12,%rdi
+	mov    %r9,0x10(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x10(%rsp),%r9
+	jmp    499e <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x55e>
+	nopw   0x0(%rax,%rax,1)
+	mov    0x52f9(%rip),%rdi        
+	lea    0x522a(%rip),%rdx        
+	lea    0x522b(%rip),%rsi        
+	call   36c0 <__Pyx__GetModuleGlobalName>
+	mov    %rax,%rbp
+	test   %rbp,%rbp
+	jne    448f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x4f>
+	lea    0x2b0b(%rip),%rcx        
+	mov    $0xa,%edx
+	mov    $0x4e1,%esi
+	xor    %r14d,%r14d
+	lea    0x2b47(%rip),%rdi        
+	mov    %rcx,0x5360(%rip)        
+	movl   $0xa,0x5362(%rip)        
+	movl   $0x4e1,0x5354(%rip)        
+	call   3c50 <__Pyx_AddTraceback>
+	jmp    50c0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc80>
+	cs nopw 0x0(%rax,%rax,1)
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	jmp    4f9c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb5c>
+	xchg   %ax,%ax
+	mov    %r9,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    49c7 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x587>
+	nopl   (%rax)
+	mov    %rbx,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    496a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x52a>
+	nopl   (%rax)
 	mov    $0x1,%edi
-	call   25c0 <PyTuple_New@plt>
-	mov    %rax,%r13
+	call   25d0 <PyTuple_New@plt>
+	mov    %rax,%r12
 	test   %rax,%rax
-	je     4e30 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11f0>
-	addq   $0x1,(%r12)
-	mov    %r12,0x18(%rax)
-	mov    0x8(%rbp),%rax
-	mov    0x80(%rax),%rbx
-	test   %rbx,%rbx
-	je     5160 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1520>
-	call   25d0 <PyThreadState_Get@plt>
-	mov    0x3771(%rip),%rcx        
+	je     65e0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x21a0>
+	addq   $0x1,(%rbx)
+	mov    %rbx,0x18(%rax)
+	mov    0x8(%r13),%rax
+	mov    0x80(%rax),%r8
+	test   %r8,%r8
+	je     715a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2d1a>
+	mov    %r8,0x10(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x4865(%rip),%r15        
+	mov    0x10(%rsp),%r8
 	mov    0x20(%rax),%edi
 	lea    0x1(%rdi),%edx
+	cmp    (%r15),%edx
 	mov    %edx,0x20(%rax)
-	cmp    (%rcx),%edx
-	jg     5175 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1535>
-	mov    %rcx,(%rsp)
+	jg     71b9 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2d79>
 	xor    %edx,%edx
-	mov    %r13,%rsi
-	mov    %rbp,%rdi
-	call   *%rbx
-	mov    %rax,%rbx
-	call   25d0 <PyThreadState_Get@plt>
+	mov    %r12,%rsi
+	mov    %r13,%rdi
+	call   *%r8
+	mov    %rax,0x10(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x10(%rsp),%r8
 	mov    0x20(%rax),%ecx
 	lea    -0x1(%rcx),%edx
-	mov    (%rsp),%rcx
 	mov    %edx,0x20(%rax)
-	mov    (%rcx),%eax
-	lea    -0x32(%rax),%ecx
+	mov    (%r15),%eax
 	cmp    $0xc8,%eax
-	jg     485d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc1d>
+	lea    -0x32(%rax),%ecx
+	jg     5770 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1330>
 	sar    $0x2,%eax
 	lea    (%rax,%rax,2),%ecx
 	cmp    %ecx,%edx
-	jl     4fa1 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1361>
-	test   %rbx,%rbx
-	je     5198 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1558>
-	subq   $0x1,0x0(%r13)
-	je     4f94 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1354>
+	jl     6df7 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x29b7>
+	test   %r8,%r8
+	je     71a3 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2d63>
 	subq   $0x1,(%r12)
-	jne    4888 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc48>
-	mov    %r12,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	test   %rbx,%rbx
-	jne    405f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x41f>
-	lea    0x18b0(%rip),%rax        
-	xor    %r12d,%r12d
-	xor    %r13d,%r13d
-	mov    %rbp,%r14
-	mov    %rax,0x3f20(%rip)        
-	movl   $0x9,0x3f22(%rip)        
-	movl   $0x4fb,0x3f14(%rip)        
-	jmp    439f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x75f>
+	je     6cf6 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x28b6>
+	subq   $0x1,(%rbx)
+	jne    57a4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1364>
+	mov    %rbx,%rdi
+	mov    %r8,0x10(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x10(%rsp),%r8
+	test   %r8,%r8
+	jne    48f3 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x4b3>
+	mov    %r13,%r12
+	jmp    527c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe3c>
+	nopl   (%rax)
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%eax
+	jmp    47b5 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x375>
+	nopl   0x0(%rax,%rax,1)
+	mov    0x5171(%rip),%rdi        
+	call   3640 <__Pyx_GetBuiltinName>
+	mov    %rax,%rbp
+	jmp    565d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x121d>
 	nopl   0x0(%rax)
-	mov    0x3e49(%rip),%rdi        
-	call   3b40 <__Pyx_GetBuiltinName>
+	call   2720 <PyObject_GetAttr@plt>
+	mov    %rax,%r12
+	jmp    44b2 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x72>
+	nopl   (%rax)
+	movl   $0xa,0x51fa(%rip)        
+	lea    0x2977(%rip),%rax        
+	movl   $0x4e3,0x51e5(%rip)        
+	mov    %rax,0x51d6(%rip)        
+	xor    %eax,%eax
+	mov    %rdx,0x0(%rbp)
+	test   %rdx,%rdx
+	je     7393 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2f53>
+	mov    %rax,%rbp
+	mov    %r12,%r14
+	xor    %r15d,%r15d
+	jmp    5070 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc30>
+	nop
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%eax
+	jmp    4570 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x130>
+	nopl   0x0(%rax,%rax,1)
+	mov    0x18(%r12),%rbp
+	test   %rbp,%rbp
+	je     44e2 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xa2>
+	mov    0x10(%r12),%r13
+	addq   $0x1,0x0(%rbp)
+	addq   $0x1,0x0(%r13)
+	subq   $0x1,(%r12)
+	je     5c20 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x17e0>
+	mov    0x5109(%rip),%rdx        
+	mov    %rbp,%rsi
+	mov    %r13,%rdi
+	call   3a00 <__Pyx_PyObject_Call2Args>
+	subq   $0x1,0x0(%rbp)
+	mov    %rax,%r14
+	jne    4584 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x144>
+	mov    %rbp,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    4584 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x144>
+	nopl   (%rax)
+	mov    %r13,%rdi
+	mov    %r9,0x10(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x10(%rsp),%r9
+	jmp    498a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x54a>
+	nop
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	jmp    517b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd3b>
+	xchg   %ax,%ax
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	jmp    4696 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x256>
+	xchg   %ax,%ax
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%eax
+	jmp    48d8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x498>
+	nopl   0x0(%rax,%rax,1)
+	call   2720 <PyObject_GetAttr@plt>
 	mov    %rax,%rbp
-	jmp    469d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xa5d>
+	jmp    45bb <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x17b>
+	nopl   (%rax)
+	lea    0x2881(%rip),%rax        
+	movl   $0xb,0x50f3(%rip)        
+	mov    %rax,0x50e0(%rip)        
+	movl   $0x4ff,0x50de(%rip)        
+	mov    0x50cf(%rip),%rcx        
+	mov    0x50d5(%rip),%edx        
+	xor    %r15d,%r15d
+	lea    0x289f(%rip),%rdi        
+	mov    0x50c1(%rip),%esi        
+	call   3c50 <__Pyx_AddTraceback>
+	jmp    5094 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc54>
 	nopl   0x0(%rax)
-	call   2700 <PyObject_GetAttr@plt>
-	mov    %rax,%rbx
-	jmp    3d32 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf2>
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%eax
+	jmp    5353 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf13>
+	nopl   0x0(%rax,%rax,1)
+	mov    %r8,0x10(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	mov    0x10(%rsp),%r8
+	jmp    5262 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe22>
+	nopl   0x0(%rax,%rax,1)
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	jmp    47bd <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x37d>
+	xchg   %ax,%ax
+	mov    %r12,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    4a40 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x600>
 	nopl   (%rax)
-	lea    0x1851(%rip),%rax        
-	mov    %rbp,%r15
+	call   2720 <PyObject_GetAttr@plt>
+	mov    %rax,%r12
+	jmp    46d7 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x297>
+	nopl   (%rax)
+	lea    0x27d1(%rip),%rbx        
 	xor    %ebp,%ebp
-	movl   $0x9,0x3ece(%rip)        
-	mov    %rax,0x3ebb(%rip)        
-	mov    0x0(%r13),%rax
-	movl   $0x4ce,0x3eb5(%rip)        
-	sub    $0x1,%rax
-	jmp    46d5 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xa95>
+	movl   $0xb,0x5041(%rip)        
+	mov    %rbx,0x502e(%rip)        
+	movl   $0x510,0x502c(%rip)        
+	xor    %r15d,%r15d
+	xor    %r9d,%r9d
+	xor    %ebx,%ebx
+	xor    %r8d,%r8d
+	jmp    5036 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xbf6>
 	nopl   0x0(%rax)
-	mov    0x18(%rbx),%r12
+	mov    0x80(%rax),%r12
+	mov    0x501a(%rip),%r13        
 	test   %r12,%r12
-	je     3d57 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x117>
-	mov    0x10(%rbx),%r15
-	addq   $0x1,(%r12)
-	addq   $0x1,(%r15)
-	subq   $0x1,(%rbx)
-	je     4a98 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe58>
-	mov    0x365d(%rip),%rbx        
-	mov    0x8(%r15),%rax
-	mov    %r12,0x10(%rsp)
-	mov    %rbx,(%rsp)
-	cmp    %rbx,%rax
-	je     507f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x143f>
-	cmp    0x3680(%rip),%rax        
-	jne    4faf <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x136f>
-	mov    0x10(%r15),%rdx
-	mov    0x10(%rdx),%eax
-	test   $0x8,%al
-	je     50e9 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x14a9>
-	mov    0x8(%rdx),%rbp
-	xor    %ebx,%ebx
-	test   $0x20,%al
-	jne    4993 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd53>
-	mov    0x18(%r15),%rbx
-	call   25d0 <PyThreadState_Get@plt>
+	je     6f16 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2ad6>
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x458d(%rip),%r15        
 	mov    0x20(%rax),%ecx
 	lea    0x1(%rcx),%edx
-	mov    0x35e3(%rip),%rcx        
 	mov    %edx,0x20(%rax)
-	cmp    (%rcx),%edx
-	jg     513d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x14fd>
-	mov    %rcx,0x8(%rsp)
-	mov    %rbx,%rdi
-	mov    %r12,%rsi
-	call   *%rbp
-	mov    %rax,%rbp
-	call   25d0 <PyThreadState_Get@plt>
-	mov    0x8(%rsp),%rcx
+	cmp    (%r15),%edx
+	jg     5d1d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x18dd>
+	mov    %r13,%rsi
+	xor    %edx,%edx
+	mov    %rbp,%rdi
+	call   *%r12
+	mov    %rax,%r13
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%esi
+	lea    -0x1(%rsi),%edx
+	jmp    4f7e <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb3e>
+	nopl   0x0(%rax,%rax,1)
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	jmp    4578 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x138>
+	xchg   %ax,%ax
+	mov    0x8(%rbp),%rax
+	mov    0x4ec5(%rip),%rsi        
+	mov    %rbp,%rdi
+	mov    0x90(%rax),%rax
+	test   %rax,%rax
+	je     6f55 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2b15>
+	call   *%rax
+	mov    %rax,%r12
+	test   %r12,%r12
+	je     6f2e <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2aee>
+	mov    0x8(%r12),%rax
+	mov    0x4e48(%rip),%rbx        
+	mov    0x80(%rax),%r13
+	test   %r13,%r13
+	je     5d39 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x18f9>
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x44f4(%rip),%r15        
+	mov    0x20(%rax),%ecx
+	lea    0x1(%rcx),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%r15),%edx
+	jg     6fe4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2ba4>
+	xor    %edx,%edx
+	mov    %rbx,%rsi
+	mov    %r12,%rdi
+	call   *%r13
+	mov    %rax,%r13
+	call   25e0 <PyThreadState_Get@plt>
 	mov    0x20(%rax),%ebx
 	lea    -0x1(%rbx),%edx
 	mov    %edx,0x20(%rax)
-	mov    (%rcx),%eax
+	mov    (%r15),%eax
+	lea    -0x32(%rax),%ecx
 	cmp    $0xc8,%eax
-	jle    4ef0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x12b0>
-	sub    $0x32,%eax
-	cmp    %eax,%edx
-	jl     4f86 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1346>
-	test   %rbp,%rbp
-	je     5096 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1456>
+	jg     5ad5 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1695>
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%ecx
+	cmp    %ecx,%edx
+	jl     6970 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2530>
+	test   %r13,%r13
+	je     6f87 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2b47>
 	subq   $0x1,(%r12)
-	mov    %r15,%rbx
-	jne    3dfa <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1ba>
-	nopw   0x0(%rax,%rax,1)
+	je     6908 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x24c8>
+	mov    0x8(%r13),%rax
+	mov    0x4dec(%rip),%rsi        
+	mov    %r13,%rdi
+	mov    0x90(%rax),%rax
+	test   %rax,%rax
+	je     6fd7 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2b97>
+	call   *%rax
+	mov    %rax,%r15
+	mov    0x0(%r13),%rax
+	sub    $0x1,%rax
+	test   %r15,%r15
+	je     6fb0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2b70>
+	mov    %rax,0x0(%r13)
+	test   %rax,%rax
+	je     6a30 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x25f0>
+	mov    0x4427(%rip),%rax        
+	cmp    %rax,0x8(%r15)
+	jne    648d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x204d>
+	mov    0x18(%r15),%r13
+	test   %r13,%r13
+	je     648d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x204d>
+	mov    0x10(%r15),%r12
+	addq   $0x1,0x0(%r13)
+	addq   $0x1,(%r12)
+	subq   $0x1,(%r15)
+	je     6ba0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2760>
+	mov    %r13,%rsi
 	mov    %r12,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    4a30 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xdf0>
-	nopw   0x0(%rax,%rax,1)
-	xor    %edx,%edx
-	xor    %esi,%esi
-	mov    %rbx,%rdi
-	mov    %rbx,%r15
-	call   39d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
-	mov    %rax,%rbp
-	nopw   0x0(%rax,%rax,1)
-	mov    %r15,%rbx
-	test   %rbp,%rbp
-	jne    3dfa <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1ba>
-	nopl   0x0(%rax)
-	lea    0x1701(%rip),%rax        
+	call   3740 <__Pyx_PyObject_CallOneArg>
+	subq   $0x1,0x0(%r13)
+	mov    %rax,%rbx
+	je     6ce9 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x28a9>
+	test   %rbx,%rbx
+	je     702b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2beb>
+	subq   $0x1,(%r12)
+	je     6b58 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2718>
+	subq   $0x1,0x0(%rbp)
+	je     6b40 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2700>
+	mov    %rbx,%rbp
 	xor    %r15d,%r15d
-	xor    %ebp,%ebp
-	movl   $0x9,0x3d7e(%rip)        
-	mov    %rax,0x3d6b(%rip)        
+	addq   $0x1,0x0(%rbp)
+	mov    %rbp,%rbx
+	subq   $0x1,(%r14)
+	je     5502 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x10c2>
+	mov    %rbp,%r14
+	jmp    50a6 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc66>
+	lea    0x25b1(%rip),%rax        
+	movl   $0xa,0x4e23(%rip)        
+	mov    %rax,0x4e10(%rip)        
+	movl   $0x4f2,0x4e0e(%rip)        
 	mov    0x0(%r13),%rax
-	movl   $0x4dd,0x3d65(%rip)        
+	xor    %r15d,%r15d
+	xor    %r9d,%r9d
+	xor    %ebp,%ebp
+	xor    %r14d,%r14d
+	xor    %ebx,%ebx
+	xor    %r8d,%r8d
 	sub    $0x1,%rax
-	jmp    46d5 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xa95>
-	nopl   0x0(%rax)
+	jmp    5036 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xbf6>
+	nop
 	sar    $0x2,%eax
-	lea    (%rax,%rax,2),%eax
-	jmp    4043 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x403>
+	lea    (%rax,%rax,2),%ecx
+	jmp    4c34 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x7f4>
 	nopl   0x0(%rax,%rax,1)
-	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    460e <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x9ce>
+	mov    0x18(%r9),%r8
+	jmp    4b06 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x6c6>
+	nopl   0x0(%rax)
+	mov    %r12,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    5868 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1428>
 	nopl   (%rax)
-	mov    %rbx,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    494c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd0c>
+	lea    0x20(%rsp),%rsi
+	mov    $0x1,%edx
+	mov    %r12,%rdi
+	call   34d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
+	mov    %rax,%r14
+	jmp    4581 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x141>
+	nopw   0x0(%rax,%rax,1)
+	mov    %r8,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    4d1d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x8dd>
 	nopl   (%rax)
+	mov    $0x1,%edi
+	call   25d0 <PyTuple_New@plt>
+	mov    %rax,%rbp
+	test   %rax,%rax
+	je     6238 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1df8>
+	addq   $0x1,0x0(%r13)
+	mov    %r13,0x18(%rax)
+	mov    0x8(%r12),%rax
+	mov    0x80(%rax),%r13
+	test   %r13,%r13
+	je     70e9 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2ca9>
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x42e8(%rip),%r15        
+	mov    0x20(%rax),%ebx
+	lea    0x1(%rbx),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%r15),%edx
+	jg     7141 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2d01>
+	xor    %edx,%edx
+	mov    %rbp,%rsi
+	mov    %r12,%rdi
+	call   *%r13
+	mov    %rax,%r14
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%ebx
+	lea    -0x1(%rbx),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%r15),%eax
+	lea    -0x32(%rax),%ecx
+	cmp    $0xc8,%eax
+	jg     5ce1 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x18a1>
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%ecx
+	cmp    %ecx,%edx
+	jl     6c87 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2847>
+	test   %r14,%r14
+	je     6217 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1dd7>
+	subq   $0x1,0x0(%rbp)
+	jne    4581 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x141>
 	mov    %rbp,%rdi
-	mov    %rbx,%r12
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    439f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x75f>
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    4581 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x141>
+	nopw   0x0(%rax,%rax,1)
+	mov    %r15,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    4d52 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x912>
+	lea    0x233c(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     5a0d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x15cd>
+	mov    %rbp,%r12
+	jmp    4fd0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb90>
+	xor    %edx,%edx
+	mov    %rbx,%rsi
+	mov    %r12,%rdi
+	call   26c0 <PyObject_Call@plt>
+	mov    %rax,%r13
+	test   %rax,%rax
+	jne    5ae6 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x16a6>
+	lea    0x241f(%rip),%rax        
+	movl   $0xe,0x4c91(%rip)        
+	mov    %rax,0x4c7e(%rip)        
+	movl   $0x565,0x4c7c(%rip)        
+	mov    (%r12),%rax
+	lea    -0x1(%rax),%rdx
+	mov    %rbp,%rax
+	mov    %r12,%rbp
+	mov    %r14,%r12
+	jmp    5814 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x13d4>
+	nopw   0x0(%rax,%rax,1)
+	mov    %r8,0x10(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x10(%rsp),%r8
+	movb   $0x0,0x24(%rax)
+	jmp    48e0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x4a0>
 	nopl   0x0(%rax,%rax,1)
-	mov    %rbp,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    41f4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x5b4>
+	lea    0x23c1(%rip),%rax        
+	movl   $0xc,0x4c33(%rip)        
+	mov    %rax,0x4c20(%rip)        
+	movl   $0x52c,0x4c1e(%rip)        
+	jmp    5912 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x14d2>
+	nopw   0x0(%rax,%rax,1)
+	call   2720 <PyObject_GetAttr@plt>
+	mov    %rax,%r12
+	jmp    47fe <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x3be>
 	nopl   (%rax)
-	call   25f0 <PyErr_Occurred@plt>
-	test   %rax,%rax
-	jne    4a40 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe00>
-	mov    0x3473(%rip),%rax        
-	lea    0x16ac(%rip),%rsi        
-	mov    (%rax),%rdi
-	call   24f0 <PyErr_SetString@plt>
-	jmp    4a40 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe00>
+	mov    0x80(%rax),%rbp
+	mov    0x4c02(%rip),%r13        
+	test   %rbp,%rbp
+	je     6f6f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2b2f>
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x4175(%rip),%r15        
+	mov    0x20(%rax),%edi
+	lea    0x1(%rdi),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%r15),%edx
+	jg     7012 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2bd2>
+	xor    %edx,%edx
+	mov    %r13,%rsi
+	mov    %r12,%rdi
+	call   *%rbp
+	jmp    514f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd0f>
 	nopl   0x0(%rax)
-	mov    %r13,%rdx
-	mov    %r15,%rsi
-	mov    %r14,%rdi
-	call   26a0 <PyObject_Call@plt>
-	mov    %rax,%rbp
-	test   %rax,%rax
-	jne    3eaa <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x26a>
-	nopw   0x0(%rax,%rax,1)
-	lea    0x1621(%rip),%rax        
-	xor    %ebx,%ebx
-	xor    %r15d,%r15d
-	xor    %ebp,%ebp
-	mov    %rax,0x3c93(%rip)        
-	mov    0x0(%r13),%rax
-	movl   $0x9,0x3c91(%rip)        
-	movl   $0x4e2,0x3c83(%rip)        
-	sub    $0x1,%rax
-	jmp    46d5 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xa95>
-	cs nopw 0x0(%rax,%rax,1)
-	call   25d0 <PyThreadState_Get@plt>
+	mov    %r8,%rdi
+	mov    %r9,0x10(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x10(%rsp),%r9
+	jmp    4abd <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x67d>
+	nop
+	mov    %r9,0x10(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x10(%rsp),%r9
 	movb   $0x0,0x24(%rax)
-	jmp    435d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x71d>
-	xchg   %ax,%ax
-	lea    0x15d1(%rip),%rax        
-	movl   $0xa,0x3c53(%rip)        
-	mov    %rax,0x3c40(%rip)        
-	movl   $0x50e,0x3c3e(%rip)        
-	jmp    41e9 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x5a9>
+	jmp    535b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf1b>
+	nopl   0x0(%rax,%rax,1)
+	mov    %r9,%rdi
+	mov    %r8,0x8(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x8(%rsp),%r8
+	jmp    4b8f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x74f>
 	nopw   0x0(%rax,%rax,1)
-	cmp    0x33c9(%rip),%rdx        
-	je     5064 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1424>
-	mov    %r13,%rdi
-	call   2430 <PyNumber_Add@plt>
-	mov    %rax,%r14
-	jmp    40fa <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x4ba>
+	lea    0x22e1(%rip),%rax        
+	movl   $0xd,0x4b53(%rip)        
+	mov    %rax,0x4b40(%rip)        
+	movl   $0x546,0x4b3e(%rip)        
+	jmp    5912 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x14d2>
+	nopw   0x0(%rax,%rax,1)
+	call   2720 <PyObject_GetAttr@plt>
+	mov    %rax,%rbx
+	jmp    492b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x4eb>
 	nopl   (%rax)
-	call   2700 <PyObject_GetAttr@plt>
-	mov    %rax,%r14
-	jmp    3ee2 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2a2>
+	mov    0x80(%rax),%r13
+	mov    0x4b22(%rip),%rbx        
+	test   %r13,%r13
+	je     70a3 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2c63>
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x4095(%rip),%r15        
+	mov    0x20(%rax),%esi
+	lea    0x1(%rsi),%edx
+	mov    %edx,0x20(%rax)
+	cmp    (%r15),%edx
+	jg     70d0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2c90>
+	xor    %edx,%edx
+	mov    %rbx,%rsi
+	mov    %r12,%rdi
+	call   *%r13
+	mov    %rax,0x10(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x20(%rax),%ebx
+	lea    -0x1(%rbx),%edx
+	jmp    523f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xdff>
 	nopl   (%rax)
-	lea    0x14a9(%rip),%rdi        
-	mov    %rcx,0x8(%rsp)
-	call   25b0 <_Py_CheckRecursiveCall@plt>
-	mov    0x8(%rsp),%rcx
+	mov    %r8,0x10(%rsp)
+	mov    %r9,0x8(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	mov    0x10(%rsp),%r8
+	mov    0x8(%rsp),%r9
+	jmp    4b7c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x73c>
+	nopw   0x0(%rax,%rax,1)
+	mov    %r15,%rdi
+	mov    %r15,%r12
+	call   4240 <__Pyx_PyObject_CallNoArg>
+	mov    %rax,%r13
+	jmp    4d6a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x92a>
+	lea    0x20f6(%rip),%rdi        
+	mov    %r10,0x10(%rsp)
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	mov    0x10(%rsp),%r10
 	test   %eax,%eax
-	je     3e61 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x221>
-	jmp    4b20 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xee0>
-	nopl   0x0(%rax,%rax,1)
-	lea    0x1549(%rip),%rbx        
-	movl   $0x9,0x3bcb(%rip)        
-	mov    %rbx,0x3bb8(%rip)        
-	movl   $0x4e6,0x3bb6(%rip)        
-	xor    %r12d,%r12d
-	xor    %r13d,%r13d
-	jmp    4210 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x5d0>
+	je     617b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1d3b>
+	subq   $0x1,(%r10)
+	jne    68a8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2468>
+	mov    %r10,%rdi
+	mov    %rbx,%r12
+	call   24b0 <_Py_Dealloc@plt>
+	cs nopw 0x0(%rax,%rax,1)
+	lea    0x21d1(%rip),%rax        
+	movl   $0xd,0x4a43(%rip)        
+	mov    %rax,0x4a30(%rip)        
+	movl   $0x554,0x4a2e(%rip)        
+	jmp    4ff4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xbb4>
+	nopw   0x0(%rax,%rax,1)
+	mov    %r8,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    4bbd <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x77d>
 	nopl   (%rax)
-	call   25f0 <PyErr_Occurred@plt>
+	xor    %edx,%edx
+	xor    %esi,%esi
+	mov    %rbp,%rdi
+	mov    %rbp,%r12
+	call   34d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
+	mov    %rax,%r13
+	jmp    545a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x101a>
+	nopw   0x0(%rax,%rax,1)
+	lea    0x2171(%rip),%rax        
+	xor    %r15d,%r15d
+	xor    %r8d,%r8d
+	movl   $0xd,0x49dd(%rip)        
+	mov    %rax,0x49ca(%rip)        
+	movl   $0x557,0x49c8(%rip)        
+	subq   $0x1,(%r9)
+	jne    604c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1c0c>
+	xor    %r12d,%r12d
+	mov    %r9,%rdi
+	mov    %r8,0x8(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	test   %r12,%r12
+	mov    0x8(%rsp),%r8
+	jne    4ffa <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xbba>
+	xor    %ebx,%ebx
+	xor    %r9d,%r9d
+	test   %r8,%r8
+	jne    5048 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc08>
+	jmp    5070 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc30>
+	nop
+	mov    %r12,%rdi
+	mov    %r8,0x8(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x8(%rsp),%r8
+	jmp    4c5b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x81b>
+	nopw   0x0(%rax,%rax,1)
+	mov    %r13,%rdi
+	mov    %r8,0x8(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x8(%rsp),%r8
+	jmp    4c50 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x810>
+	nopw   0x0(%rax,%rax,1)
+	lea    0x20(%rsp),%rsi
+	mov    $0x1,%edx
+	mov    %r12,%rdi
+	call   34d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
+	mov    %rax,%r13
+	jmp    544c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x100c>
+	nopw   0x0(%rax,%rax,1)
+	mov    %r8,0x8(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x8(%rsp),%r8
+	movb   $0x0,0x24(%rax)
+	jmp    4c3c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x7fc>
+	nopl   0x0(%rax,%rax,1)
+	call   2600 <PyErr_Occurred@plt>
 	test   %rax,%rax
-	jne    4b20 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xee0>
-	mov    0x331b(%rip),%rax        
-	lea    0x1554(%rip),%rsi        
+	jne    6100 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1cc0>
+	mov    0x3e67(%rip),%rax        
+	lea    0x1f88(%rip),%rsi        
 	mov    (%rax),%rdi
-	call   24f0 <PyErr_SetString@plt>
-	jmp    4b20 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xee0>
+	call   2500 <PyErr_SetString@plt>
+	subq   $0x1,(%rbx)
+	jne    4fd0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb90>
+	mov    %rbx,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    4fd0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb90>
+	nopw   0x0(%rax,%rax,1)
+	mov    $0x1,%edi
+	call   25d0 <PyTuple_New@plt>
+	mov    %rax,%r10
+	test   %rax,%rax
+	je     68a8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2468>
+	addq   $0x1,0x0(%r13)
+	mov    %r13,0x18(%rax)
+	mov    0x8(%rbx),%rax
+	mov    0x80(%rax),%r12
+	test   %r12,%r12
+	je     71d9 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2d99>
+	mov    %r10,0x10(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x3e24(%rip),%r15        
+	mov    0x10(%rsp),%r10
+	mov    0x20(%rax),%edi
+	lea    0x1(%rdi),%edx
+	cmp    (%r15),%edx
+	mov    %edx,0x20(%rax)
+	jg     5f63 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1b23>
+	xor    %edx,%edx
+	mov    %r10,%rsi
+	mov    %r10,0x18(%rsp)
+	mov    %rbx,%rdi
+	call   *%r12
+	mov    %rax,0x10(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x10(%rsp),%r9
+	mov    0x18(%rsp),%r10
+	mov    0x20(%rax),%esi
+	lea    -0x1(%rsi),%edx
+	mov    %edx,0x20(%rax)
+	mov    (%r15),%eax
+	cmp    $0xc8,%eax
+	lea    -0x32(%rax),%ecx
+	jg     61bb <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1d7b>
+	sar    $0x2,%eax
+	lea    (%rax,%rax,2),%ecx
+	cmp    %ecx,%edx
+	jl     6ea3 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2a63>
+	test   %r9,%r9
+	je     7213 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2dd3>
+	subq   $0x1,(%r10)
+	jne    5364 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf24>
+	mov    %r10,%rdi
+	mov    %r9,0x10(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x10(%rsp),%r9
+	jmp    5364 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf24>
+	nopl   (%rax)
+	mov    %r8,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    4c9b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x85b>
+	nopl   (%rax)
+	xor    %edx,%edx
+	xor    %esi,%esi
+	mov    %r12,%rdi
+	mov    %r12,%r13
+	call   34d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
+	mov    %rax,%rbp
+	jmp    55f8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11b8>
+	call   2600 <PyErr_Occurred@plt>
+	test   %rax,%rax
+	je     7354 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2f14>
+	subq   $0x1,0x0(%rbp)
+	jne    6238 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1df8>
+	mov    %rbp,%rdi
+	call   24b0 <_Py_Dealloc@plt>
 	nopl   0x0(%rax)
-	lea    0x1421(%rip),%rdi        
-	mov    %rcx,0x8(%rsp)
-	call   25b0 <_Py_CheckRecursiveCall@plt>
-	mov    0x8(%rsp),%rcx
-	test   %eax,%eax
-	je     3db5 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x175>
-	jmp    4a40 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe00>
-	nopl   0x0(%rax,%rax,1)
-	cmp    $0xfffffffffffffffe,%rax
-	je     4e70 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1230>
-	cmp    $0x2,%rax
-	je     4e50 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1210>
-	mov    0x60(%rdx),%rax
+	lea    0x1f39(%rip),%rax        
+	mov    %r12,%r13
+	movl   $0xa,0x47a8(%rip)        
+	mov    %rax,0x4795(%rip)        
+	movl   $0x4f2,0x4793(%rip)        
+	jmp    5be2 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x17a2>
+	nopw   0x0(%rax,%rax,1)
+	mov    %r12,%rdi
+	mov    %r9,0x10(%rsp)
+	mov    %r8,0x8(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x10(%rsp),%r9
+	mov    0x8(%rsp),%r8
+	jmp    4eb2 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xa72>
+	nopl   0x0(%rax)
+	test   $0x80,%al
+	je     53b0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf70>
+	mov    0x8(%rdx),%r9
+	xor    %edi,%edi
+	test   $0x20,%al
+	jne    62a7 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1e67>
+	mov    0x18(%r12),%rdi
+	lea    0x20(%rsp),%rsi
+	test   $0x2,%al
+	jne    72f4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2eb4>
+	mov    $0x1,%edx
+	call   *%r9
+	mov    %rax,%r13
+	jmp    544c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x100c>
+	nopl   0x0(%rax)
+	lea    0x20(%rsp),%rsi
+	mov    $0x1,%edx
 	mov    %r13,%rdi
-	call   *(%rax)
-	mov    %rax,%r14
-	jmp    40fa <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x4ba>
-	nopl   (%rax)
-	mov    $0x2,%edi
-	jmp    40f2 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x4b2>
+	call   34d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
+	mov    %rax,%rbp
+	jmp    55ea <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11aa>
 	nopw   0x0(%rax,%rax,1)
-	mov    %r12,%rsi
-	mov    %rbp,%rdi
-	call   25a0 <PyList_Append@plt>
+	mov    %r12,%rdi
+	mov    %rax,0x8(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x8(%rsp),%r8
+	jmp    4cdd <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x89d>
+	nop
+	lea    0x1d59(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
 	test   %eax,%eax
-	je     4191 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x551>
-	lea    0x1476(%rip),%rax        
-	mov    %r12,%r14
-	movl   $0xa,0x3af5(%rip)        
-	mov    %rax,0x3ae2(%rip)        
-	movl   $0x513,0x3ae0(%rip)        
-	jmp    41e9 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x5a9>
-	nopl   (%rax)
-	call   25d0 <PyThreadState_Get@plt>
-	movb   $0x0,0x24(%rax)
-	jmp    404b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x40b>
-	cs nopw 0x0(%rax,%rax,1)
-	call   2700 <PyObject_GetAttr@plt>
-	mov    %rax,%r14
-	jmp    3f63 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x323>
-	nopl   (%rax)
-	lea    0x1421(%rip),%rbx        
-	movl   $0x9,0x3aa3(%rip)        
-	mov    %rbx,0x3a90(%rip)        
-	movl   $0x4ec,0x3a8e(%rip)        
-	jmp    4c1a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xfda>
+	je     4f68 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb28>
+	jmp    5d31 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x18f1>
+	nopl   0x0(%rax)
+	call   2600 <PyErr_Occurred@plt>
+	test   %rax,%rax
+	jne    6340 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1f00>
+	mov    0x3c27(%rip),%rax        
+	lea    0x1d48(%rip),%rsi        
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
+	subq   $0x1,(%rbx)
+	mov    %r13,%r12
+	jne    5195 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd55>
+	mov    %rbx,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    5195 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd55>
 	nopw   0x0(%rax,%rax,1)
-	lea    0x13f1(%rip),%rax        
-	mov    %rbx,%r12
-	movl   $0xa,0x3a70(%rip)        
-	mov    %rax,0x3a5d(%rip)        
-	movl   $0x507,0x3a5b(%rip)        
-	jmp    4498 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x858>
+	mov    %r8,%rdi
+	mov    %r9,0x8(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x8(%rsp),%r9
+	jmp    4ede <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xa9e>
 	nopw   0x0(%rax,%rax,1)
-	mov    0x80(%rax),%rbx
-	mov    0x3a52(%rip),%rbp        
-	test   %rbx,%rbx
-	je     50d1 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1491>
-	call   25d0 <PyThreadState_Get@plt>
+	lea    0x1cd9(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     4664 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x224>
+	jmp    6100 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1cc0>
+	nopl   0x0(%rax)
+	mov    %rbp,%rdi
+	mov    %r9,0x8(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x8(%rsp),%r9
+	jmp    4dce <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x98e>
+	nopw   0x0(%rax,%rax,1)
+	mov    0x4519(%rip),%rdi        
+	lea    0x449a(%rip),%rdx        
+	lea    0x449b(%rip),%rsi        
+	call   36c0 <__Pyx__GetModuleGlobalName>
+	mov    %rax,%r12
+	test   %r12,%r12
+	jne    49fe <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x5be>
+	lea    0x1d8b(%rip),%rax        
+	movl   $0x10,0x45fd(%rip)        
+	mov    %rax,0x45ea(%rip)        
+	movl   $0x58f,0x45e8(%rip)        
+	jmp    5912 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x14d2>
+	nopl   (%rax)
+	xor    %edx,%edx
+	xor    %esi,%esi
+	mov    %r12,%rdi
+	mov    %r12,%r13
+	call   34d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
+	mov    %rax,%r8
+	jmp    57a4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1364>
+	nopw   0x0(%rax,%rax,1)
+	mov    0x80(%rax),%rcx
+	mov    0x45c2(%rip),%rbx        
+	test   %rcx,%rcx
+	je     723d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2dfd>
+	mov    %rcx,0x10(%rsp)
+	mov    %r9,0x8(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x3b2b(%rip),%r15        
+	mov    0x8(%rsp),%r9
 	mov    0x20(%rax),%ecx
 	lea    0x1(%rcx),%edx
-	mov    0x31df(%rip),%rcx        
+	cmp    (%r15),%edx
+	mov    0x10(%rsp),%rcx
 	mov    %edx,0x20(%rax)
-	cmp    (%rcx),%edx
-	jg     511c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x14dc>
-	mov    %rcx,(%rsp)
-	xor    %edx,%edx
-	mov    %rbp,%rsi
-	mov    %r14,%rdi
-	call   *%rbx
-	mov    %rax,%rbx
-	call   25d0 <PyThreadState_Get@plt>
-	mov    0x20(%rax),%ecx
-	lea    -0x1(%rcx),%edx
-	jmp    433c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x6fc>
-	nopl   (%rax)
+	jg     727a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2e3a>
+	mov    %r9,0x10(%rsp)
 	xor    %edx,%edx
-	xor    %esi,%esi
-	mov    %r14,%rdi
-	mov    %r14,%rbp
-	call   39d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
+	mov    %rbx,%rsi
+	mov    %r9,%rdi
+	call   *%rcx
+	jmp    4b44 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x704>
+	mov    %r15,%rdi
+	mov    %r15,%r12
+	call   4240 <__Pyx_PyObject_CallNoArg>
 	mov    %rax,%rbx
-	jmp    4888 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc48>
-	nop
-	lea    0x10(%rsp),%rsi
+	jmp    5b81 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1741>
+	mov    %rbp,%rdi
+	mov    %rax,0x8(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x8(%rsp),%r8
+	mov    0x10(%rsp),%r9
+	jmp    4e9e <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xa5e>
+	nopl   0x0(%rax)
+	test   $0x80,%al
+	je     5550 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1110>
+	mov    0x8(%rdx),%r9
+	xor    %edi,%edi
+	test   $0x20,%al
+	jne    64d6 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2096>
+	mov    0x18(%r13),%rdi
+	lea    0x20(%rsp),%rsi
+	test   $0x2,%al
+	jne    730b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2ecb>
 	mov    $0x1,%edx
+	call   *%r9
+	mov    %rax,%rbp
+	jmp    55ea <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11aa>
+	nopl   0x0(%rax,%rax,1)
 	mov    %rbp,%rdi
-	call   39d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
-	mov    %rax,%rbx
-	jmp    4879 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc39>
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    4d89 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x949>
+	nopl   (%rax)
+	mov    %r12,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    4d7e <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x93e>
+	nopl   (%rax)
+	lea    0x20(%rsp),%rsi
+	mov    $0x1,%edx
+	mov    %r13,%rdi
+	call   34d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
+	mov    %rax,%r8
+	jmp    578c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x134c>
 	nopw   0x0(%rax,%rax,1)
-	call   25f0 <PyErr_Occurred@plt>
+	lea    0x1c39(%rip),%rax        
+	movl   $0x10,0x44ab(%rip)        
+	mov    %rax,0x4498(%rip)        
+	mov    %rbp,%rax
+	mov    %r12,%rbp
+	mov    %r14,%r12
+	movl   $0x591,0x448d(%rip)        
+	jmp    5814 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x13d4>
+	nopl   0x0(%rax,%rax,1)
+	call   2720 <PyObject_GetAttr@plt>
+	mov    %rax,%r13
+	jmp    4a22 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x5e2>
+	nopl   (%rax)
+	mov    0x4359(%rip),%rdi        
+	call   3640 <__Pyx_GetBuiltinName>
+	mov    %rax,%r12
+	jmp    63dd <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1f9d>
+	nopl   0x0(%rax)
+	lea    0x1ac1(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     5148 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd08>
+	jmp    5195 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd55>
+	nopl   0x0(%rax)
+	call   2600 <PyErr_Occurred@plt>
 	test   %rax,%rax
-	jne    4e30 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11f0>
-	mov    0x3137(%rip),%rax        
-	lea    0x1370(%rip),%rsi        
+	jne    65e0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x21a0>
+	mov    0x398f(%rip),%rax        
+	lea    0x1ab0(%rip),%rsi        
 	mov    (%rax),%rdi
-	call   24f0 <PyErr_SetString@plt>
-	subq   $0x1,(%r12)
-	mov    %rbp,%r14
-	jne    4377 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x737>
-	mov    %r12,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    4377 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x737>
+	call   2500 <PyErr_SetString@plt>
 	nopl   0x0(%rax,%rax,1)
-	mov    0x1c(%r13),%edi
-	mov    0x18(%r13),%eax
-	shl    $0x1e,%rdi
-	or     %rax,%rdi
-	add    $0x2,%rdi
-	jmp    40f2 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x4b2>
-	nopl   0x0(%rax,%rax,1)
-	mov    0x1c(%r13),%eax
-	mov    0x18(%r13),%edx
-	mov    $0x2,%edi
-	shl    $0x1e,%rax
-	or     %rdx,%rax
-	sub    %rax,%rdi
-	jmp    40f2 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x4b2>
+	subq   $0x1,(%rbx)
+	mov    %r13,%r12
+	jne    527c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe3c>
+	mov    %rbx,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    527c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe3c>
+	nopw   0x0(%rax,%rax,1)
+	test   $0x80,%al
+	je     5c60 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1820>
+	mov    0x8(%rdx),%r8
+	xor    %edi,%edi
+	test   $0x20,%al
+	jne    6617 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x21d7>
+	mov    0x18(%r12),%rdi
+	lea    0x20(%rsp),%rsi
+	test   $0x2,%al
+	jne    731d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2edd>
+	mov    $0x1,%edx
+	call   *%r8
+	mov    %rax,%r14
+	jmp    4581 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x141>
+	nopl   0x0(%rax)
+	lea    0x1a21(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     478b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x34b>
+	jmp    6340 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1f00>
+	nopl   0x0(%rax)
+	lea    0x1b19(%rip),%rax        
+	movl   $0x10,0x438b(%rip)        
+	mov    %rax,0x4378(%rip)        
+	mov    0x0(%r13),%rax
+	movl   $0x594,0x4372(%rip)        
+	sub    $0x1,%rax
+	jmp    59c4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1584>
+	nopw   0x0(%rax,%rax,1)
+	mov    0x4319(%rip),%rdi        
+	mov    %r9,%rsi
+	mov    %r9,0x8(%rsp)
+	call   2460 <PyUnicode_Join@plt>
+	mov    0x8(%rsp),%r9
+	test   %rax,%rax
+	mov    %rax,%rbp
+	je     72a7 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2e67>
+	subq   $0x1,(%r9)
+	je     6f62 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2b22>
+	subq   $0x1,0x0(%r13)
+	jne    5ba6 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1766>
+	mov    %r13,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    5ba6 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1766>
+	nopw   0x0(%rax,%rax,1)
+	lea    0x1979(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     4546 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x106>
+	jmp    6238 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1df8>
+	nopl   0x0(%rax)
+	lea    0x20(%rsp),%rsi
+	mov    $0x1,%edx
+	mov    %rbx,%rdi
+	call   34d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
+	mov    %rax,%r9
+	jmp    5364 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf24>
+	nopw   0x0(%rax,%rax,1)
+	call   2600 <PyErr_Occurred@plt>
+	test   %rax,%rax
+	jne    6238 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1df8>
+	mov    0x3823(%rip),%rax        
+	lea    0x1944(%rip),%rsi        
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
+	jmp    6238 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1df8>
 	nopl   0x0(%rax)
 	test   $0x80,%al
-	je     47d8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xb98>
+	je     56e0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x12a0>
 	mov    0x8(%rdx),%r8
 	xor    %edi,%edi
 	test   $0x20,%al
-	jne    4ea6 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1266>
-	mov    0x18(%rbp),%rdi
-	lea    0x10(%rsp),%rsi
+	jne    6766 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2326>
+	mov    0x18(%r13),%rdi
+	lea    0x20(%rsp),%rsi
 	test   $0x2,%al
-	jne    5249 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1609>
+	jne    7381 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2f41>
 	mov    $0x1,%edx
 	call   *%r8
-	mov    %rax,%rbx
-	jmp    4879 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc39>
+	mov    %rax,%r8
+	jmp    578c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x134c>
+	nopl   0x0(%rax,%rax,1)
+	mov    0x18(%rax),%rdx
+	mov    0x37ed(%rip),%rax        
+	lea    0x1a5e(%rip),%rsi        
+	mov    %r9,0x8(%rsp)
+	mov    (%rax),%rdi
+	xor    %eax,%eax
+	call   26e0 <PyErr_Format@plt>
+	mov    0x8(%rsp),%r9
+	subq   $0x1,(%r9)
+	mov    %r13,%rbp
+	lea    0x19bc(%rip),%rax        
+	mov    $0x0,%r8d
+	mov    %rax,0x421f(%rip)        
+	movl   $0x11,0x4221(%rip)        
+	movl   $0x5da,0x4213(%rip)        
+	jne    4ffa <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xbba>
+	jmp    6031 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1bf1>
 	nopl   0x0(%rax,%rax,1)
-	lea    0x11b1(%rip),%rdi        
-	mov    %rcx,(%rsp)
-	call   25b0 <_Py_CheckRecursiveCall@plt>
-	mov    (%rsp),%rcx
+	mov    0x40e9(%rip),%rdi        
+	lea    0x405a(%rip),%rdx        
+	lea    0x405b(%rip),%rsi        
+	call   36c0 <__Pyx__GetModuleGlobalName>
+	mov    %rax,%r8
+	test   %r8,%r8
+	jne    4a7d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x63d>
+	lea    0x195b(%rip),%rax        
+	xor    %r9d,%r9d
+	xor    %ebx,%ebx
+	movl   $0x10,0x41c8(%rip)        
+	mov    %rax,0x41b5(%rip)        
+	mov    (%r12),%rax
+	movl   $0x596,0x41af(%rip)        
+	sub    $0x1,%rax
+	mov    %rax,(%r12)
+	xor    %r15d,%r15d
+	test   %rax,%rax
+	jne    502e <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xbee>
+	jmp    500d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xbcd>
+	nopw   0x0(%rax,%rax,1)
+	lea    0x17f9(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
 	test   %eax,%eax
-	je     4323 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x6e3>
-	jmp    4377 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x737>
-	nopl   0x0(%rax)
-	sar    $0x2,%eax
-	lea    (%rax,%rax,2),%eax
-	jmp    49e3 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xda3>
+	je     5227 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xde7>
+	jmp    527c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe3c>
+	mov    0x36d8(%rip),%rax        
+	lea    0x17f9(%rip),%rsi        
+	mov    %r10,0x8(%rsp)
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
+	mov    0x8(%rsp),%r10
+	subq   $0x1,(%r10)
+	je     5f8b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1b4b>
+	nopl   0x0(%rax,%rax,1)
+	mov    %rbx,%r12
+	jmp    5fa0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1b60>
+	mov    0x36c9(%rip),%rax        
+	mov    0x18(%rdx),%rdx
+	lea    0x1936(%rip),%rsi        
+	mov    (%rax),%rdi
+	xor    %eax,%eax
+	call   26e0 <PyErr_Format@plt>
+	lea    0x18a5(%rip),%rax        
+	movl   $0x10,0x4117(%rip)        
+	mov    %rax,0x4104(%rip)        
+	movl   $0x5b3,0x4102(%rip)        
+	jmp    5d74 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1934>
 	nopl   0x0(%rax,%rax,1)
-	lea    0x1179(%rip),%rdi        
-	mov    %rcx,(%rsp)
-	call   25b0 <_Py_CheckRecursiveCall@plt>
-	mov    (%rsp),%rcx
-	test   %eax,%eax
-	je     4012 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x3d2>
-	jmp    4e30 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11f0>
-	mov    %r15,%rsi
-	xor    %edx,%edx
 	mov    %rbx,%rdi
-	mov    %rbx,%r15
-	call   26a0 <PyObject_Call@plt>
-	mov    %rax,%rbp
-	jmp    4a30 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xdf0>
-	lea    0x1140(%rip),%rdi        
-	mov    %rcx,0x8(%rsp)
-	call   25b0 <_Py_CheckRecursiveCall@plt>
-	mov    0x8(%rsp),%rcx
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    4d6a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x92a>
+	nopl   (%rax)
+	mov    %r12,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    5af1 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x16b1>
+	nopl   (%rax)
+	lea    0x1859(%rip),%rax        
+	xor    %r9d,%r9d
+	xor    %ebx,%ebx
+	movl   $0x10,0x40c6(%rip)        
+	mov    %rax,0x40b3(%rip)        
+	mov    (%r12),%rax
+	movl   $0x5aa,0x40ad(%rip)        
+	sub    $0x1,%rax
+	jmp    6845 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2405>
+	nopl   0x0(%rax)
+	lea    0x1709(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
 	test   %eax,%eax
-	je     429c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x65c>
-	jmp    4a40 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe00>
-	lea    0x11e5(%rip),%rax        
-	xor    %r14d,%r14d
-	movl   $0xa,0x3864(%rip)        
-	mov    %rax,0x3851(%rip)        
-	movl   $0x516,0x384f(%rip)        
-	jmp    41e9 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x5a9>
-	call   25d0 <PyThreadState_Get@plt>
-	movb   $0x0,0x24(%rax)
-	jmp    49eb <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xdab>
-	mov    %r13,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    4879 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc39>
-	call   25d0 <PyThreadState_Get@plt>
+	je     48a2 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x462>
+	jmp    65e0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x21a0>
+	nopl   0x0(%rax)
+	call   25e0 <PyThreadState_Get@plt>
 	movb   $0x0,0x24(%rax)
-	jmp    4865 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc25>
-	mov    $0x1,%edi
-	call   25c0 <PyTuple_New@plt>
-	mov    %rax,%rbx
+	jmp    5add <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x169d>
+	xchg   %ax,%ax
+	mov    0x3f59(%rip),%rdi        
+	call   3640 <__Pyx_GetBuiltinName>
+	mov    %rax,%r8
+	jmp    680d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x23cd>
+	nopl   0x0(%rax)
+	lea    0x17d9(%rip),%rax        
+	mov    %r8,%rbx
+	xor    %r8d,%r8d
+	movl   $0x10,0x4045(%rip)        
+	mov    %rax,0x4032(%rip)        
+	mov    (%r12),%rax
+	movl   $0x598,0x402c(%rip)        
+	sub    $0x1,%rax
+	jmp    6845 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2405>
+	nopl   (%rax)
+	call   2720 <PyObject_GetAttr@plt>
+	mov    0x10(%rsp),%r8
+	mov    %rax,%r9
+	jmp    4aaa <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x66a>
+	nopw   0x0(%rax,%rax,1)
+	test   $0x80,%al
+	je     6120 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1ce0>
+	mov    0x8(%rdx),%r9
+	xor    %edi,%edi
+	test   $0x20,%al
+	jne    69fe <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x25be>
+	mov    0x18(%rbx),%rdi
+	lea    0x20(%rsp),%rsi
+	test   $0x2,%al
+	jne    736f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2f2f>
+	mov    $0x1,%edx
+	call   *%r9
+	mov    %rax,%r9
+	jmp    5364 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf24>
+	nopl   0x0(%rax,%rax,1)
+	mov    %rbp,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    544c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x100c>
+	nopl   (%rax)
+	mov    %r13,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    5b32 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x16f2>
+	nopl   (%rax)
+	mov    0x18(%r9),%rbx
+	test   %rbx,%rbx
+	je     4ace <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x68e>
+	mov    0x10(%r9),%r15
+	addq   $0x1,(%rbx)
+	addq   $0x1,(%r15)
+	subq   $0x1,(%r9)
+	je     706e <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2c2e>
+	mov    %rbx,%rsi
+	mov    %r15,%rdi
+	call   3740 <__Pyx_PyObject_CallOneArg>
+	subq   $0x1,(%rbx)
+	mov    %rax,%r8
+	je     6ac0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2680>
+	mov    %r15,%r9
+	test   %r8,%r8
+	jne    4b85 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x745>
+	nopl   0x0(%rax,%rax,1)
+	lea    0x16e9(%rip),%rax        
+	xor    %ebx,%ebx
+	xor    %r8d,%r8d
+	movl   $0x10,0x3f56(%rip)        
+	mov    %rax,0x3f43(%rip)        
+	mov    (%r12),%rax
+	movl   $0x5a7,0x3f3d(%rip)        
+	sub    $0x1,%rax
+	jmp    6845 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2405>
+	nopl   0x0(%rax)
+	mov    %rbx,%rdi
+	mov    %r8,0x8(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x8(%rsp),%r8
+	jmp    6a77 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2637>
+	nopl   0x0(%rax)
+	lea    0x1581(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     531d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xedd>
+	jmp    68a8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2468>
+	nopl   0x0(%rax)
+	call   2600 <PyErr_Occurred@plt>
 	test   %rax,%rax
-	je     50b6 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1476>
-	addq   $0x1,(%r12)
-	mov    %r12,0x18(%rax)
-	mov    0x8(%r15),%rax
-	mov    0x80(%rax),%rbp
-	test   %rbp,%rbp
-	je     5234 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x15f4>
-	call   25d0 <PyThreadState_Get@plt>
-	mov    0x2f9a(%rip),%rcx        
-	mov    %rax,%rdx
-	mov    0x20(%rax),%eax
-	add    $0x1,%eax
-	mov    %eax,0x20(%rdx)
-	cmp    (%rcx),%eax
-	jg     520f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x15cf>
-	mov    %rcx,0x8(%rsp)
+	jne    68a8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2468>
+	mov    0x344b(%rip),%rax        
+	lea    0x156c(%rip),%rsi        
+	mov    %rbx,%r12
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
+	jmp    5fa0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1b60>
+	nopl   0x0(%rax)
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	jmp    5438 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xff8>
+	cs nopw 0x0(%rax,%rax,1)
+	mov    %rbp,%rdi
+	xor    %r15d,%r15d
+	mov    %rbx,%rbp
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    5ba6 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1766>
+	nopl   0x0(%rax,%rax,1)
+	mov    %r12,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    5b95 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1755>
+	nopl   (%rax)
+	mov    %r9,%rdi
 	xor    %edx,%edx
+	xor    %esi,%esi
+	mov    %r9,0x8(%rsp)
+	call   34d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
+	mov    0x8(%rsp),%r9
+	mov    %rax,%r8
+	mov    %r9,%r15
+	jmp    6a77 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2637>
+	nopl   0x0(%rax)
+	mov    %r12,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    55ea <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11aa>
+	nopl   (%rax)
 	mov    %r15,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    5b68 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1728>
+	nopl   (%rax)
+	mov    %r9,0x8(%rsp)
+	call   2600 <PyErr_Occurred@plt>
+	mov    0x8(%rsp),%r9
+	test   %rax,%rax
+	jne    6a88 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2648>
+	mov    0x3389(%rip),%rax        
+	lea    0x14aa(%rip),%rsi        
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
+	mov    0x8(%rsp),%r9
+	jmp    6a88 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2648>
+	nopl   0x0(%rax,%rax,1)
+	lea    0x1581(%rip),%rax        
+	mov    %rbp,%r15
+	xor    %r8d,%r8d
+	movl   $0x11,0x3ded(%rip)        
+	mov    %rax,0x3dda(%rip)        
+	mov    %r13,%rbp
+	movl   $0x5d4,0x3dd5(%rip)        
+	jmp    6028 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1be8>
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	jmp    55d6 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1196>
+	xchg   %ax,%ax
+	mov    %r12,%rdx
 	mov    %rbx,%rsi
-	call   *%rbp
-	mov    %rax,%rbp
-	call   25d0 <PyThreadState_Get@plt>
+	mov    %r13,%rdi
+	call   26c0 <PyObject_Call@plt>
+	mov    %rax,%r8
+	test   %rax,%rax
+	jne    4c45 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x805>
+	nopw   0x0(%rax,%rax,1)
+	lea    0x1521(%rip),%rax        
+	xor    %r9d,%r9d
+	xor    %ebx,%ebx
+	xor    %r8d,%r8d
+	mov    %rax,0x3d82(%rip)        
+	mov    (%r12),%rax
+	movl   $0x10,0x3d80(%rip)        
+	movl   $0x5ac,0x3d72(%rip)        
+	sub    $0x1,%rax
+	jmp    6845 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2405>
+	call   25e0 <PyThreadState_Get@plt>
+	movb   $0x0,0x24(%rax)
+	jmp    5ce9 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x18a9>
+	lea    0x14dc(%rip),%rax        
+	xor    %r8d,%r8d
+	mov    %r13,%rbp
+	movl   $0x11,0x3d48(%rip)        
+	mov    %rax,0x3d35(%rip)        
+	movl   $0x5d8,0x3d33(%rip)        
+	jmp    6028 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1be8>
+	cmp    0x32a7(%rip),%rdx        
+	mov    %r9,0x8(%rsp)
+	je     72d4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2e94>
+	mov    %r15,%rdi
+	call   2440 <PyNumber_Add@plt>
+	mov    0x8(%rsp),%r9
+	mov    %rax,%r12
+	jmp    4e2b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x9eb>
+	mov    %r13,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    5b81 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1741>
+	mov    %r12,%rdi
+	mov    %r8,0x10(%rsp)
+	call   24b0 <_Py_Dealloc@plt>
+	mov    0x10(%rsp),%r8
+	jmp    578c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x134c>
+	lea    0x134c(%rip),%rdi        
+	mov    %rcx,0x8(%rsp)
+	call   25c0 <_Py_CheckRecursiveCall@plt>
 	mov    0x8(%rsp),%rcx
-	mov    0x20(%rax),%edi
-	lea    -0x1(%rdi),%edx
-	mov    %edx,0x20(%rax)
-	mov    (%rcx),%eax
-	lea    -0x32(%rax),%ecx
-	cmp    $0xc8,%eax
-	jg     5039 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x13f9>
-	sar    $0x2,%eax
-	lea    (%rax,%rax,2),%ecx
-	cmp    %ecx,%edx
-	jl     51e8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x15a8>
-	test   %rbp,%rbp
-	je     51f6 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x15b6>
-	subq   $0x1,(%rbx)
-	je     51c0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1580>
-	subq   $0x1,(%r12)
-	jne    4a30 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xdf0>
-	jmp    4a08 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xdc8>
-	movsd  0x10(%r13),%xmm0
-	addsd  0x1376(%rip),%xmm0        
-	call   2570 <PyFloat_FromDouble@plt>
-	mov    %rax,%r14
-	jmp    40fa <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x4ba>
-	lea    0x10(%rsp),%rsi
-	mov    $0x1,%edx
+	test   %eax,%eax
+	je     4c00 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x7c0>
+	jmp    6c50 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2810>
+	lea    0x1441(%rip),%rax        
+	movl   $0x10,0x3cb3(%rip)        
+	mov    %rax,0x3ca0(%rip)        
+	movl   $0x5b0,0x3c9e(%rip)        
+	xor    %ebx,%ebx
+	xor    %r15d,%r15d
+	xor    %r9d,%r9d
+	jmp    5048 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc08>
+	nop
+	call   2720 <PyObject_GetAttr@plt>
+	mov    0x8(%rsp),%r8
+	mov    %rax,%r12
+	jmp    4c88 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x848>
+	call   2600 <PyErr_Occurred@plt>
+	test   %rax,%rax
+	jne    6c50 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2810>
+	mov    0x31d1(%rip),%rax        
+	lea    0x12f2(%rip),%rsi        
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
+	jmp    6c50 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2810>
+	lea    0x12be(%rip),%rdi        
+	mov    %r8,0x10(%rsp)
+	mov    %r9,0x8(%rsp)
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	mov    0x8(%rsp),%r9
+	mov    0x10(%rsp),%r8
+	test   %eax,%eax
+	je     4b38 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x6f8>
+	jmp    6a88 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2648>
+	cmp    $0xfffffffffffffffe,%rax
+	je     7187 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2d47>
+	cmp    $0x2,%rax
+	je     716f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2d2f>
+	mov    0x60(%rdx),%rax
+	mov    %r9,0x8(%rsp)
 	mov    %r15,%rdi
-	call   39d0 <__Pyx_PyFunction_FastCallDict.constprop.0>
+	call   *(%rax)
+	mov    0x8(%rsp),%r9
+	mov    %rax,%r12
+	jmp    4e2b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x9eb>
+	mov    %r8,0x10(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x10(%rsp),%r8
+	movb   $0x0,0x24(%rax)
+	jmp    5778 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1338>
+	mov    $0x2,%edi
+	jmp    4e19 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x9d9>
+	mov    %r8,%rsi
+	mov    %r9,%rdi
+	mov    %r8,0x10(%rsp)
+	mov    %r9,0x8(%rsp)
+	call   25b0 <PyList_Append@plt>
+	mov    0x8(%rsp),%r9
+	mov    0x10(%rsp),%r8
+	test   %eax,%eax
+	je     4ed4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xa94>
+	lea    0x1331(%rip),%rax        
+	mov    %r13,%rbp
+	movl   $0x11,0x3ba0(%rip)        
+	mov    %rax,0x3b8d(%rip)        
+	movl   $0x5dd,0x3b8b(%rip)        
+	jmp    6028 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1be8>
+	lea    0x1307(%rip),%rax        
+	movl   $0x10,0x3b79(%rip)        
+	mov    %rax,0x3b66(%rip)        
+	movl   $0x5b6,0x3b64(%rip)        
+	jmp    6d52 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2912>
+	call   2720 <PyObject_GetAttr@plt>
+	mov    0x8(%rsp),%r8
+	mov    %rax,%r15
+	jmp    4d0a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x8ca>
+	mov    %r10,0x18(%rsp)
+	mov    %r9,0x10(%rsp)
+	call   25e0 <PyThreadState_Get@plt>
+	mov    0x18(%rsp),%r10
+	mov    0x10(%rsp),%r9
+	movb   $0x0,0x24(%rax)
+	jmp    61c3 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1d83>
+	lea    0x12ac(%rip),%rax        
+	movl   $0x10,0x3b1e(%rip)        
+	mov    %rax,0x3b0b(%rip)        
+	movl   $0x5c5,0x3b09(%rip)        
+	jmp    4ff4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xbb4>
+	lea    0x1285(%rip),%rax        
+	mov    %r13,%rbp
+	movl   $0x11,0x3af4(%rip)        
+	mov    %rax,0x3ae1(%rip)        
+	movl   $0x5d1,0x3adf(%rip)        
+	jmp    5912 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x14d2>
+	mov    %r13,%rsi
+	xor    %edx,%edx
+	mov    %rbp,%rdi
+	mov    %rbp,%r12
+	call   26c0 <PyObject_Call@plt>
+	mov    %rax,%r13
+	jmp    545a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x101a>
+	lea    0x1243(%rip),%rax        
+	movl   $0xe,0x3ab5(%rip)        
+	mov    %rax,0x3aa2(%rip)        
+	movl   $0x563,0x3aa0(%rip)        
+	jmp    5912 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x14d2>
+	call   2720 <PyObject_GetAttr@plt>
+	mov    %rax,%r12
+	jmp    5a63 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1623>
+	mov    %r9,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    66bf <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x227f>
+	mov    %r13,%rsi
+	xor    %edx,%edx
+	mov    %r12,%rdi
+	mov    %r12,%r13
+	call   26c0 <PyObject_Call@plt>
 	mov    %rax,%rbp
-	jmp    5054 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1414>
-	call   25f0 <PyErr_Occurred@plt>
+	jmp    55f8 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11b8>
+	call   2600 <PyErr_Occurred@plt>
 	test   %rax,%rax
-	jne    50b6 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1476>
-	mov    0x2eb1(%rip),%rax        
-	lea    0x10ea(%rip),%rsi        
+	jne    5d52 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1912>
+	mov    0x2fbc(%rip),%rax        
+	lea    0x10dd(%rip),%rsi        
 	mov    (%rax),%rdi
-	call   24f0 <PyErr_SetString@plt>
-	subq   $0x1,(%r12)
-	mov    %r15,%rbx
-	jne    4a40 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe00>
-	mov    %r12,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    4a40 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe00>
+	call   2500 <PyErr_SetString@plt>
+	jmp    5d52 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1912>
+	lea    0x11c1(%rip),%rbx        
+	movl   $0xe,0x3a33(%rip)        
+	mov    %rbx,0x3a20(%rip)        
+	movl   $0x568,0x3a1e(%rip)        
+	jmp    59c4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1584>
+	call   2720 <PyObject_GetAttr@plt>
+	mov    %rax,%r15
+	jmp    5b14 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x16d4>
+	lea    0x1075(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     5aa6 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1666>
+	jmp    5d52 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1912>
+	xor    %edx,%edx
 	mov    %rbp,%rsi
+	mov    %r12,%rdi
+	call   26c0 <PyObject_Call@plt>
+	mov    %rax,%r13
+	jmp    5441 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1001>
+	lea    0x1047(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     5e25 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x19e5>
+	jmp    5195 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd55>
+	lea    0x1146(%rip),%rax        
+	movl   $0xe,0x39b8(%rip)        
+	mov    %rax,0x39a5(%rip)        
+	movl   $0x577,0x39a3(%rip)        
+	jmp    4ff4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xbb4>
+	lea    0x1007(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     5401 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xfc1>
+	xor    %r13d,%r13d
+	jmp    5441 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1001>
+	mov    %r9,%rdi
+	call   24b0 <_Py_Dealloc@plt>
+	jmp    6a63 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2623>
+	call   2600 <PyErr_Occurred@plt>
+	mov    %rax,%r13
+	test   %rax,%rax
+	jne    7066 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2c26>
+	mov    0x2ec9(%rip),%rax        
+	lea    0xfea(%rip),%rsi        
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
+	jmp    5441 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1001>
 	xor    %edx,%edx
-	mov    %r14,%rdi
-	mov    %r14,%rbp
-	call   26a0 <PyObject_Call@plt>
-	mov    %rax,%rbx
-	jmp    4888 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc48>
-	test   $0x80,%al
-	je     4faf <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x136f>
-	mov    0x8(%rdx),%r8
-	xor    %edi,%edi
-	test   $0x20,%al
-	jne    50ff <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x14bf>
-	mov    0x18(%r15),%rdi
-	lea    0x10(%rsp),%rsi
-	test   $0x2,%al
-	jne    525b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x161b>
-	mov    $0x1,%edx
-	call   *%r8
+	mov    %rbx,%rsi
+	mov    %r12,%rdi
+	mov    %r12,%r13
+	call   26c0 <PyObject_Call@plt>
+	mov    %rax,%r8
+	jmp    57a4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1364>
+	xor    %edx,%edx
+	mov    %r12,%rsi
+	mov    %r13,%rdi
+	call   26c0 <PyObject_Call@plt>
 	mov    %rax,%rbp
-	jmp    5054 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1414>
-	lea    0xf5d(%rip),%rdi        
-	mov    %rcx,(%rsp)
-	call   25b0 <_Py_CheckRecursiveCall@plt>
-	mov    (%rsp),%rcx
-	test   %eax,%eax
-	je     4db4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1174>
-	jmp    4377 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x737>
-	lea    0xf3c(%rip),%rdi        
-	mov    %rcx,0x8(%rsp)
-	call   25b0 <_Py_CheckRecursiveCall@plt>
-	mov    0x8(%rsp),%rcx
+	jmp    55df <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x119f>
+	lea    0xf89(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
 	test   %eax,%eax
-	je     49b0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd70>
-	jmp    50b6 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1476>
+	je     5f05 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1ac5>
+	jmp    527c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe3c>
 	xor    %edx,%edx
-	mov    %r13,%rsi
-	mov    %rbp,%rdi
-	call   26a0 <PyObject_Call@plt>
-	mov    %rax,%rbx
-	jmp    486e <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc2e>
-	lea    0xf04(%rip),%rdi        
-	mov    %rcx,(%rsp)
-	call   25b0 <_Py_CheckRecursiveCall@plt>
-	mov    (%rsp),%rcx
+	mov    %rbp,%rsi
+	mov    %r12,%rdi
+	call   26c0 <PyObject_Call@plt>
+	mov    %rax,%r14
+	jmp    5cf2 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x18b2>
+	lea    0xf5b(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
 	test   %eax,%eax
-	je     4828 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xbe8>
-	xor    %ebx,%ebx
-	jmp    486e <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc2e>
-	call   25f0 <PyErr_Occurred@plt>
-	mov    %rax,%rbx
+	je     55a0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1160>
+	xor    %ebp,%ebp
+	jmp    55df <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x119f>
+	call   2600 <PyErr_Occurred@plt>
+	mov    %rax,%rbp
 	test   %rax,%rax
-	jne    5191 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1551>
-	mov    0x2dac(%rip),%rax        
-	lea    0xfe5(%rip),%rsi        
+	jne    7112 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2cd2>
+	mov    0x2e2b(%rip),%rax        
+	lea    0xf4c(%rip),%rsi        
 	mov    (%rax),%rdi
-	call   24f0 <PyErr_SetString@plt>
-	jmp    486e <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc2e>
+	call   2500 <PyErr_SetString@plt>
+	jmp    55df <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x119f>
+	lea    0xf18(%rip),%rdi        
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	test   %eax,%eax
+	je     5cb2 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1872>
+	jmp    6225 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1de5>
+	xor    %edx,%edx
+	mov    %r12,%rsi
+	mov    %r13,%rdi
+	call   26c0 <PyObject_Call@plt>
+	mov    %rax,%r8
+	jmp    5781 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1341>
+	mov    0x1c(%r15),%edi
+	mov    0x18(%r15),%eax
+	shl    $0x1e,%rdi
+	or     %rax,%rdi
+	add    $0x2,%rdi
+	jmp    4e19 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x9d9>
+	mov    0x1c(%r15),%eax
+	mov    0x18(%r15),%edx
+	mov    $0x2,%edi
+	shl    $0x1e,%rax
+	or     %rdx,%rax
+	sub    %rax,%rdi
+	jmp    4e19 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x9d9>
+	call   2600 <PyErr_Occurred@plt>
+	test   %rax,%rax
+	je     732f <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2eef>
+	xor    %r8d,%r8d
+	jmp    5781 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1341>
+	lea    0xea0(%rip),%rdi        
+	mov    %r8,0x10(%rsp)
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	mov    0x10(%rsp),%r8
+	test   %eax,%eax
+	je     573a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x12fa>
+	jmp    71b1 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2d71>
+	mov    %r10,%rsi
+	xor    %edx,%edx
 	mov    %rbx,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    5054 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1414>
-	mov    0x2d84(%rip),%rax        
-	lea    0xfbd(%rip),%rsi        
+	mov    %r10,0x10(%rsp)
+	call   26c0 <PyObject_Call@plt>
+	mov    0x10(%rsp),%r10
+	mov    %rax,%r9
+	jmp    61cc <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1d8c>
+	mov    0x2d59(%rip),%rax        
+	lea    0xe7a(%rip),%rsi        
 	mov    (%rax),%rdi
-	call   24f0 <PyErr_SetString@plt>
-	jmp    4377 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x737>
-	call   25d0 <PyThreadState_Get@plt>
-	movb   $0x0,0x24(%rax)
-	jmp    5041 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1401>
-	call   25f0 <PyErr_Occurred@plt>
-	mov    %rax,%rbp
+	call   2500 <PyErr_SetString@plt>
+	jmp    5195 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xd55>
+	mov    %r10,0x8(%rsp)
+	call   2600 <PyErr_Occurred@plt>
+	mov    0x8(%rsp),%r10
 	test   %rax,%rax
-	je     526d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x162d>
-	xor    %ebp,%ebp
-	jmp    504a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x140a>
-	call   24e0 <__stack_chk_fail@plt>
-	lea    0xe6a(%rip),%rdi        
-	mov    %rcx,0x8(%rsp)
-	call   25b0 <_Py_CheckRecursiveCall@plt>
-	mov    0x8(%rsp),%rcx
-	test   %eax,%eax
-	je     5002 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x13c2>
-	xor    %ebp,%ebp
-	jmp    504a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x140a>
+	je     6879 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2439>
+	subq   $0x1,(%r10)
+	mov    %rbx,%r12
+	jne    5fa0 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1b60>
+	jmp    5f8b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1b4b>
+	mov    %r9,%rdi
 	xor    %edx,%edx
 	mov    %rbx,%rsi
-	mov    %r15,%rdi
-	call   26a0 <PyObject_Call@plt>
+	mov    %r9,0x8(%rsp)
+	call   26c0 <PyObject_Call@plt>
+	mov    0x8(%rsp),%r9
+	mov    %rax,%r8
+	mov    %r9,%r15
+	jmp    6a77 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2637>
+	mov    0x2cf2(%rip),%rax        
+	lea    0xe13(%rip),%rsi        
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
+	jmp    527c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xe3c>
+	lea    0xddf(%rip),%rdi        
+	mov    %rcx,0x10(%rsp)
+	mov    %r9,0x8(%rsp)
+	call   25c0 <_Py_CheckRecursiveCall@plt>
+	mov    0x8(%rsp),%r9
+	mov    0x10(%rsp),%rcx
+	test   %eax,%eax
+	je     6479 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2039>
+	jmp    6a88 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x2648>
+	lea    0xeca(%rip),%rax        
+	xor    %r8d,%r8d
+	mov    %r13,%rbp
+	movl   $0x11,0x3736(%rip)        
+	mov    %rax,0x3723(%rip)        
+	movl   $0x5e0,0x3721(%rip)        
+	jmp    6028 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1be8>
+	movsd  0x10(%r15),%xmm0
+	addsd  0x116e(%rip),%xmm0        
+	call   2580 <PyFloat_FromDouble@plt>
+	mov    0x8(%rsp),%r9
+	mov    %rax,%r12
+	jmp    4e2b <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x9eb>
+	xor    %ecx,%ecx
+	mov    $0x1,%edx
+	call   *%r9
+	mov    %rax,%r13
+	jmp    544c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x100c>
+	call   24f0 <__stack_chk_fail@plt>
+	xor    %ecx,%ecx
+	mov    $0x1,%edx
+	call   *%r9
 	mov    %rax,%rbp
-	jmp    504a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x140a>
+	jmp    55ea <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x11aa>
 	xor    %ecx,%ecx
 	mov    $0x1,%edx
 	call   *%r8
-	mov    %rax,%rbx
-	jmp    4879 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xc39>
+	mov    %rax,%r14
+	jmp    4581 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x141>
+	mov    %rax,0x10(%rsp)
+	mov    0x2c1d(%rip),%rax        
+	lea    0xd3e(%rip),%rsi        
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
+	mov    0x10(%rsp),%r8
+	jmp    5781 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1341>
+	mov    0x2bfd(%rip),%rax        
+	lea    0xd1e(%rip),%rsi        
+	mov    (%rax),%rdi
+	call   2500 <PyErr_SetString@plt>
+	jmp    6225 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1de5>
+	xor    %ecx,%ecx
+	mov    $0x1,%edx
+	call   *%r9
+	mov    %rax,%r9
+	jmp    5364 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xf24>
 	xor    %ecx,%ecx
 	mov    $0x1,%edx
 	call   *%r8
+	mov    %rax,%r8
+	jmp    578c <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x134c>
+	mov    %r12,%r14
+	xor    %r15d,%r15d
+	mov    %rbp,%r12
+	xor    %r9d,%r9d
 	mov    %rax,%rbp
-	jmp    5054 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x1414>
-	mov    0x2ce4(%rip),%rax        
-	lea    0xf1d(%rip),%rsi        
-	mov    (%rax),%rdi
-	call   24f0 <PyErr_SetString@plt>
-	jmp    504a <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x140a>
-	mov    %r13,%rdi
-	call   24a0 <_Py_Dealloc@plt>
-	jmp    46e2 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xaa2>
-	mov    0x352c(%rip),%rcx        
-	mov    0x3532(%rip),%edx        
-	mov    %rbx,%r12
-	lea    0xf3c(%rip),%rdi        
-	mov    0x351e(%rip),%esi        
-	call   33e0 <__Pyx_AddTraceback>
-	jmp    44c4 <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0x884>
+	xor    %r8d,%r8d
+	xor    %ebx,%ebx
+	xor    %r13d,%r13d
+	jmp    500d <__pyx_pw_10pytelerdac_5utils_12device_utils_1get_device_id+0xbcd>
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,11 +1,11 @@
 
 
 
 Disassembly of section .fini:
 
-00000000000052bc <_fini>:
+00000000000073b0 <_fini>:
 _fini():
 	endbr64
 	sub    $0x8,%rsp
 	add    $0x8,%rsp
 	ret
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,66 +1,73 @@
 
 Hex dump of section '.rodata':
-  0x00006000 70797465 6c657264 61632f75 74696c73 pytelerdac/utils
-  0x00006010 2f646576 6963655f 7574696c 732e6300 /device_utils.c.
-  0x00006020 496e7465 72707265 74657220 6368616e Interpreter chan
-  0x00006030 67652064 65746563 74656420 2d207468 ge detected - th
-  0x00006040 6973206d 6f64756c 65206361 6e206f6e is module can on
-  0x00006050 6c792062 65206c6f 61646564 20696e74 ly be loaded int
-  0x00006060 6f206f6e 6520696e 74657270 72657465 o one interprete
-  0x00006070 72207065 72207072 6f636573 732e0000 r per process...
-  0x00006080 20776869 6c652063 616c6c69 6e672061  while calling a
-  0x00006090 20507974 686f6e20 6f626a65 63740000  Python object..
-  0x000060a0 4d6f6475 6c652027 64657669 63655f75 Module 'device_u
-  0x000060b0 74696c73 27206861 7320616c 72656164 tils' has alread
-  0x000060c0 79206265 656e2069 6d706f72 7465642e y been imported.
-  0x000060d0 2052652d 696e6974 69616c69 73617469  Re-initialisati
-  0x000060e0 6f6e2069 73206e6f 74207375 70706f72 on is not suppor
-  0x000060f0 7465642e 00000000 636f6d70 696c6574 ted.....compilet
-  0x00006100 696d6520 76657273 696f6e20 2573206f ime version %s o
-  0x00006110 66206d6f 64756c65 2027252e 31303073 f module '%.100s
-  0x00006120 2720646f 6573206e 6f74206d 61746368 ' does not match
-  0x00006130 2072756e 74696d65 20766572 73696f6e  runtime version
-  0x00006140 20257300 00000000 70797465 6c657264  %s.....pytelerd
-  0x00006150 61632f75 74696c73 2f646576 6963655f ac/utils/device_
-  0x00006160 7574696c 732e7079 78000000 00000000 utils.pyx.......
-  0x00006170 696e6974 20707974 656c6572 6461632e init pytelerdac.
-  0x00006180 7574696c 732e6465 76696365 5f757469 utils.device_uti
-  0x00006190 6c730000 00000000 4e554c4c 20726573 ls......NULL res
-  0x000061a0 756c7420 77697468 6f757420 6572726f ult without erro
-  0x000061b0 7220696e 2050794f 626a6563 745f4361 r in PyObject_Ca
-  0x000061c0 6c6c0000 00000000 27252e32 30307327 ll......'%.200s'
-  0x000061d0 206f626a 65637420 69732075 6e736c69  object is unsli
-  0x000061e0 63656162 6c650000 70797465 6c657264 ceable..pytelerd
-  0x000061f0 61632e75 74696c73 2e646576 6963655f ac.utils.device_
-  0x00006200 7574696c 732e6765 745f6465 76696365 utils.get_device
-  0x00006210 5f696400 25732028 25733a25 6429006e _id.%s (%s:%d).n
-  0x00006220 616d6500 5f5f6c6f 61646572 5f5f006c ame.__loader__.l
-  0x00006230 6f616465 72005f5f 66696c65 5f5f006f oader.__file__.o
-  0x00006240 72696769 6e005f5f 7061636b 6167655f rigin.__package_
-  0x00006250 5f007061 72656e74 005f5f70 6174685f _.parent.__path_
-  0x00006260 5f007375 626d6f64 756c655f 73656172 _.submodule_sear
-  0x00006270 63685f6c 6f636174 696f6e73 006e616d ch_locations.nam
-  0x00006280 65202725 55272069 73206e6f 74206465 e '%U' is not de
-  0x00006290 66696e65 64002564 2e256400 25730070 fined.%d.%d.%s.p
-  0x000062a0 7974656c 65726461 632e7574 696c732e ytelerdac.utils.
-  0x000062b0 64657669 63655f75 74696c73 00627569 device_utils.bui
-  0x000062c0 6c74696e 73006379 74686f6e 5f72756e ltins.cython_run
-  0x000062d0 74696d65 005f5f62 75696c74 696e735f time.__builtins_
-  0x000062e0 5f006765 745f6465 76696365 5f696400 _.get_device_id.
-  0x000062f0 00000000 00000000 00000000 00000000 ................
-  0x00006300 70797465 6c657264 61632f75 74696c73 pytelerdac/utils
-  0x00006310 2f646576 6963655f 7574696c 732e7079 /device_utils.py
-  0x00006320 78000000 00000000 00000000 00000000 x...............
-  0x00006330 70797465 6c657264 61632e75 74696c73 pytelerdac.utils
-  0x00006340 2e646576 6963655f 7574696c 73000000 .device_utils...
-  0x00006350 636c696e 655f696e 5f747261 63656261 cline_in_traceba
-  0x00006360 636b0000 00000000 6765745f 64657669 ck......get_devi
-  0x00006370 63655f69 64000000 6765746e 6f646500 ce_id...getnode.
-  0x00006380 5f5f696d 706f7274 5f5f0075 70706572 __import__.upper
-  0x00006390 0072616e 67650075 75696400 00000000 .range.uuid.....
-  0x000063a0 5f5f7465 73745f5f 00000000 00000000 __test__........
-  0x000063b0 5f5f6e61 6d655f5f 00000000 00000000 __name__........
-  0x000063c0 5f5f6d61 696e5f5f 006a6f69 6e005555 __main__.join.UU
-  0x000063d0 4944006d 61630069 6e740068 6578002d ID.mac.int.hex.-
-  0x000063e0 00650000 00000000 00000000 00000040 .e.............@
+  0x00008000 496e7465 72707265 74657220 6368616e Interpreter chan
+  0x00008010 67652064 65746563 74656420 2d207468 ge detected - th
+  0x00008020 6973206d 6f64756c 65206361 6e206f6e is module can on
+  0x00008030 6c792062 65206c6f 61646564 20696e74 ly be loaded int
+  0x00008040 6f206f6e 6520696e 74657270 72657465 o one interprete
+  0x00008050 72207065 72207072 6f636573 732e0000 r per process...
+  0x00008060 20776869 6c652063 616c6c69 6e672061  while calling a
+  0x00008070 20507974 686f6e20 6f626a65 63740000  Python object..
+  0x00008080 4e554c4c 20726573 756c7420 77697468 NULL result with
+  0x00008090 6f757420 6572726f 7220696e 2050794f out error in PyO
+  0x000080a0 626a6563 745f4361 6c6c0000 00000000 bject_Call......
+  0x000080b0 70797465 6c657264 61632f75 74696c73 pytelerdac/utils
+  0x000080c0 2f646576 6963655f 7574696c 732e6300 /device_utils.c.
+  0x000080d0 4d6f6475 6c652027 64657669 63655f75 Module 'device_u
+  0x000080e0 74696c73 27206861 7320616c 72656164 tils' has alread
+  0x000080f0 79206265 656e2069 6d706f72 7465642e y been imported.
+  0x00008100 2052652d 696e6974 69616c69 73617469  Re-initialisati
+  0x00008110 6f6e2069 73206e6f 74207375 70706f72 on is not suppor
+  0x00008120 7465642e 00000000 636f6d70 696c6574 ted.....compilet
+  0x00008130 696d6520 76657273 696f6e20 2573206f ime version %s o
+  0x00008140 66206d6f 64756c65 2027252e 31303073 f module '%.100s
+  0x00008150 2720646f 6573206e 6f74206d 61746368 ' does not match
+  0x00008160 2072756e 74696d65 20766572 73696f6e  runtime version
+  0x00008170 20257300 00000000 70797465 6c657264  %s.....pytelerd
+  0x00008180 61632f75 74696c73 2f646576 6963655f ac/utils/device_
+  0x00008190 7574696c 732e7079 78000000 00000000 utils.pyx.......
+  0x000081a0 696e6974 20707974 656c6572 6461632e init pytelerdac.
+  0x000081b0 7574696c 732e6465 76696365 5f757469 utils.device_uti
+  0x000081c0 6c730000 00000000 70797465 6c657264 ls......pytelerd
+  0x000081d0 61632e75 74696c73 2e646576 6963655f ac.utils.device_
+  0x000081e0 7574696c 732e6765 745f6465 76696365 utils.get_device
+  0x000081f0 5f696400 00000000 27252e32 30307327 _id.....'%.200s'
+  0x00008200 206f626a 65637420 69732075 6e736c69  object is unsli
+  0x00008210 63656162 6c65006e 616d6500 5f5f6c6f ceable.name.__lo
+  0x00008220 61646572 5f5f006c 6f616465 72005f5f ader__.loader.__
+  0x00008230 66696c65 5f5f006f 72696769 6e005f5f file__.origin.__
+  0x00008240 7061636b 6167655f 5f007061 72656e74 package__.parent
+  0x00008250 005f5f70 6174685f 5f007375 626d6f64 .__path__.submod
+  0x00008260 756c655f 73656172 63685f6c 6f636174 ule_search_locat
+  0x00008270 696f6e73 006e616d 65202725 55272069 ions.name '%U' i
+  0x00008280 73206e6f 74206465 66696e65 64002573 s not defined.%s
+  0x00008290 20282573 3a256429 0025642e 25640025  (%s:%d).%d.%d.%
+  0x000082a0 73007079 74656c65 72646163 2e757469 s.pytelerdac.uti
+  0x000082b0 6c732e64 65766963 655f7574 696c7300 ls.device_utils.
+  0x000082c0 6275696c 74696e73 00637974 686f6e5f builtins.cython_
+  0x000082d0 72756e74 696d6500 5f5f6275 696c7469 runtime.__builti
+  0x000082e0 6e735f5f 00676574 5f646576 6963655f ns__.get_device_
+  0x000082f0 69640000 00000000 00000000 00000000 id..............
+  0x00008300 70797465 6c657264 61632f75 74696c73 pytelerdac/utils
+  0x00008310 2f646576 6963655f 7574696c 732e7079 /device_utils.py
+  0x00008320 78000000 00000000 00000000 00000000 x...............
+  0x00008330 00000000 00000000 00000000 00000000 ................
+  0x00008340 6966636f 6e666967 206d6c61 6e30207c ifconfig mlan0 |
+  0x00008350 20677265 70206574 68657220 7c206177  grep ether | aw
+  0x00008360 6b20277b 7072696e 74202432 7d270000 k '{print $2}'..
+  0x00008370 70797465 6c657264 61632e75 74696c73 pytelerdac.utils
+  0x00008380 2e646576 6963655f 7574696c 73000000 .device_utils...
+  0x00008390 636c696e 655f696e 5f747261 63656261 cline_in_traceba
+  0x000083a0 636b0000 00000000 6765745f 64657669 ck......get_devi
+  0x000083b0 63655f69 64000000 7265706c 61636500 ce_id...replace.
+  0x000083c0 6765746e 6f646500 72657375 6c740000 getnode.result..
+  0x000083d0 5f5f696d 706f7274 5f5f0075 70706572 __import__.upper
+  0x000083e0 00737472 69700073 706c6974 0072616e .strip.split.ran
+  0x000083f0 67650070 6f70656e 00636c6f 73650075 ge.popen.close.u
+  0x00008400 75696400 00000000 5f5f7465 73745f5f uid.....__test__
+  0x00008410 00726561 64000000 5f5f6e61 6d655f5f .read...__name__
+  0x00008420 00000000 00000000 5f5f6d61 696e5f5f ........__main__
+  0x00008430 006a6f69 6e005555 4944006d 61630069 .join.UUID.mac.i
+  0x00008440 6e740068 6578006f 73002d00 65003a00 nt.hex.os.-.e.:.
+  0x00008450 00000000 00000040                   .......@
```

### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,11 +1,13 @@
 
 Hex dump of section '.eh_frame_hdr':
-  0x000063f0 011b033b 7c000000 0e000000 30bcffff ...;|.......0...
-  0x00006400 98000000 c0bfffff c0000000 d0bfffff ................
-  0x00006410 d8000000 50c3ffff d4010000 cec3ffff ....P...........
-  0x00006420 10020000 32c5ffff 2c030000 e8cdffff ....2...,.......
-  0x00006430 f0030000 c0ceffff f0000000 40cfffff ............@...
-  0x00006440 04010000 f0cfffff 44010000 e0d5ffff ........D.......
-  0x00006450 4c020000 50d7ffff ac020000 d0d7ffff L...P...........
-  0x00006460 e0020000 50d8ffff a4030000          ....P.......
+  0x00008458 011b033b 9c000000 12000000 c89bffff ...;............
+  0x00008468 b8000000 689fffff e0000000 789fffff ....h.......x...
+  0x00008478 f8000000 08a3ffff 64010000 86a3ffff ........d.......
+  0x00008488 a0010000 eaa4ffff dc010000 b0a5ffff ................
+  0x00008498 08040000 70aeffff 1c050000 48afffff ....p.......H...
+  0x000084a8 10010000 c8afffff 24010000 78b0ffff ........$...x...
+  0x000084b8 18020000 e8b1ffff 78020000 68b2ffff ........x...h...
+  0x000084c8 ac020000 e8b2ffff f8020000 a8b5ffff ................
+  0x000084d8 3c030000 f8b7ffff 78030000 e8bdffff <.......x.......
+  0x000084e8 70040000 e8bfffff d0040000          p...........
```

### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,60 +1,77 @@
 
 Hex dump of section '.eh_frame':
-  0x00006470 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x00006480 1b0c0708 90010000 24000000 1c000000 ........$.......
-  0x00006490 90bbffff 90030000 000e1046 0e184a0f ...........F..J.
-  0x000064a0 0b770880 003f1a3a 2a332422 00000000 .w...?.:*3$"....
-  0x000064b0 14000000 44000000 f8beffff 10000000 ....D...........
-  0x000064c0 00000000 00000000 14000000 5c000000 ............\...
-  0x000064d0 f0beffff 80030000 00000000 00000000 ................
-  0x000064e0 10000000 74000000 c8cdffff 77000000 ....t.......w...
-  0x000064f0 00000000 3c000000 88000000 34ceffff ....<.......4...
-  0x00006500 a6000000 00420e10 8e02450e 188d0342 .....B....E....B
-  0x00006510 0e208c04 440e2886 05440e30 83060271 . ..D.(..D.0...q
-  0x00006520 0a0e2844 0e20420e 18420e10 420e0844 ..(D. B..B..B..D
-  0x00006530 0b000000 8c000000 c8000000 a4ceffff ................
-  0x00006540 ec050000 00420e10 8f02420e 188e0342 .....B....B....B
-  0x00006550 0e208d04 450e288c 05440e30 8606440e . ..E.(..D.0..D.
-  0x00006560 38830746 0e6002a5 0a0e3841 0e30410e 8..F.`....8A.0A.
-  0x00006570 28420e20 420e1842 0e10420e 08480b56 (B. B..B..B..H.V
-  0x00006580 0a0e3841 0e30410e 28420e20 420e1842 ..8A.0A.(B. B..B
-  0x00006590 0e10420e 08480b03 77010e68 540e7041 ..B..H..w..hT.pA
-  0x000065a0 0e78420e 8001410e 8801410e 9001410e .xB...A...A...A.
-  0x000065b0 9801410e a001410e a801410e b001490e ..A...A...A...I.
-  0x000065c0 60000000 38000000 58010000 74c1ffff `...8...X...t...
-  0x000065d0 7e000000 00420e10 8e02450e 188d0348 ~....B....E....H
-  0x000065e0 0e208c04 410e2886 05410e30 83060262 . ..A.(..A.0...b
-  0x000065f0 0e28440e 20420e18 420e1042 0e080000 .(D. B..B..B....
-  0x00006600 38000000 94010000 b6c1ffff 64010000 8...........d...
-  0x00006610 00460e10 8e02420e 188d0345 0e208c04 .F....B....E. ..
-  0x00006620 410e2886 05410e30 034a010e 28440e20 A.(..A.0.J..(D. 
-  0x00006630 420e1842 0e10420e 08000000 5c000000 B..B..B.....\...
-  0x00006640 d0010000 8cd3ffff 65010000 00420e10 ........e....B..
-  0x00006650 8f02420e 188e0342 0e208d04 420e288c ..B....B. ..B.(.
-  0x00006660 05440e30 8606430e 38830747 0e400257 .D.0..C.8..G.@.W
-  0x00006670 0e484a0e 50470e58 430e6042 0e68420e .HJ.PG.XC.`B.hB.
-  0x00006680 70490e40 6f0a0e38 440e3041 0e28420e pI.@o..8D.0A.(B.
-  0x00006690 20420e18 420e1042 0e08460b 30000000  B..B..B..F.0...
-  0x000066a0 30020000 9cd4ffff 74000000 00420e10 0.......t....B..
-  0x000066b0 8d02450e 188c0347 0e20650a 0e18450e ..E....G. e...E.
-  0x000066c0 10420e08 460b6c0e 18450e10 420e0800 .B..F.l..E..B...
-  0x000066d0 48000000 64020000 e8d4ffff 74000000 H...d.......t...
-  0x000066e0 00420e10 8d02480e 188c0341 0e208604 .B....H....A. ..
-  0x000066f0 440e2883 05470e30 730a0e28 440e2041 D.(..G.0s..(D. A
-  0x00006700 0e18420e 10420e08 460b4e0e 28440e20 ..B..B..F.N.(D. 
-  0x00006710 410e1842 0e10420e 08000000 74000000 A..B..B.....t...
-  0x00006720 b0020000 fec1ffff b6080000 00460e10 .............F..
-  0x00006730 8f02420e 188e0342 0e208d04 420e288c ..B....B. ..B.(.
-  0x00006740 05410e30 8606440e 38830747 0ea00203 .A.0..D.8..G....
-  0x00006750 bc050ea8 024e0eb0 02420eb8 02460ec0 .....N...B...F..
-  0x00006760 02460ec8 02410ed0 02410ed8 02410ee0 .F...A...A...A..
-  0x00006770 02410ee8 02410ef0 024e0ea0 0203a802 .A...A...N......
-  0x00006780 0e38410e 30410e28 420e2042 0e18420e .8A.0A.(B. B..B.
-  0x00006790 10420e08 48000000 28030000 a4d4ffff .B..H...(.......
-  0x000067a0 7c160000 00460e10 8f02420e 188e0342 |....F....B....B
-  0x000067b0 0e208d04 420e288c 05410e30 8606410e . ..B.(..A.0..A.
-  0x000067c0 38830744 0e6003a0 080a0e38 440e3041 8..D.`.....8D.0A
-  0x000067d0 0e28420e 20420e18 420e1042 0e08410b .(B. B..B..B..A.
-  0x000067e0 10000000 74030000 f0c9ffff 10000000 ....t...........
-  0x000067f0 00000000 00000000                   ........
+  0x000084f8 14000000 00000000 017a5200 01781001 .........zR..x..
+  0x00008508 1b0c0708 90010000 24000000 1c000000 ........$.......
+  0x00008518 089bffff a0030000 000e1046 0e184a0f ...........F..J.
+  0x00008528 0b770880 003f1a3a 2a332422 00000000 .w...?.:*3$"....
+  0x00008538 14000000 44000000 809effff 10000000 ....D...........
+  0x00008548 00000000 00000000 14000000 5c000000 ............\...
+  0x00008558 789effff 90030000 00000000 00000000 x...............
+  0x00008568 10000000 74000000 30aeffff 77000000 ....t...0...w...
+  0x00008578 00000000 3c000000 88000000 9caeffff ....<...........
+  0x00008588 a6000000 00420e10 8e02450e 188d0342 .....B....E....B
+  0x00008598 0e208c04 440e2886 05440e30 83060271 . ..D.(..D.0...q
+  0x000085a8 0a0e2844 0e20420e 18420e10 420e0844 ..(D. B..B..B..D
+  0x000085b8 0b000000 38000000 c8000000 9ca1ffff ....8...........
+  0x000085c8 7e000000 00420e10 8e02450e 188d0348 ~....B....E....H
+  0x000085d8 0e208c04 410e2886 05410e30 83060262 . ..A.(..A.0...b
+  0x000085e8 0e28440e 20420e18 420e1042 0e080000 .(D. B..B..B....
+  0x000085f8 38000000 04010000 dea1ffff 64010000 8...........d...
+  0x00008608 00460e10 8e02420e 188d0345 0e208c04 .F....B....E. ..
+  0x00008618 410e2886 05410e30 034a010e 28440e20 A.(..A.0.J..(D. 
+  0x00008628 420e1842 0e10420e 08000000 38000000 B..B..B.....8...
+  0x00008638 40010000 06a3ffff c6000000 00420e10 @............B..
+  0x00008648 8f02470e 188e0342 0e208d04 420e288c ..G....B. ..B.(.
+  0x00008658 05440e30 860602a9 0e28450e 20420e18 .D.0.....(E. B..
+  0x00008668 420e1042 0e080000 5c000000 7c010000 B..B....\...|...
+  0x00008678 58aeffff 65010000 00420e10 8f02420e X...e....B....B.
+  0x00008688 188e0342 0e208d04 420e288c 05440e30 ...B. ..B.(..D.0
+  0x00008698 8606430e 38830747 0e400257 0e484a0e ..C.8..G.@.W.HJ.
+  0x000086a8 50470e58 430e6042 0e68420e 70490e40 PG.XC.`B.hB.pI.@
+  0x000086b8 6f0a0e38 440e3041 0e28420e 20420e18 o..8D.0A.(B. B..
+  0x000086c8 420e1042 0e08460b 30000000 dc010000 B..B..F.0.......
+  0x000086d8 68afffff 74000000 00420e10 8d02450e h...t....B....E.
+  0x000086e8 188c0347 0e20650a 0e18450e 10420e08 ...G. e...E..B..
+  0x000086f8 460b6c0e 18450e10 420e0800 48000000 F.l..E..B...H...
+  0x00008708 10020000 b4afffff 74000000 00420e10 ........t....B..
+  0x00008718 8d02480e 188c0341 0e208604 440e2883 ..H....A. ..D.(.
+  0x00008728 05470e30 730a0e28 440e2041 0e18420e .G.0s..(D. A..B.
+  0x00008738 10420e08 460b4e0e 28440e20 410e1842 .B..F.N.(D. A..B
+  0x00008748 0e10420e 08000000 40000000 5c020000 ..B.....@...\...
+  0x00008758 e8afffff ba020000 00420e10 8e02420e .........B....B.
+  0x00008768 188d0342 0e208c04 410e2886 05440e30 ...B. ..A.(..D.0
+  0x00008778 8306440e 4002960a 0e30440e 28410e20 ..D.@....0D.(A. 
+  0x00008788 420e1842 0e10420e 08480b00 38000000 B..B..B..H..8...
+  0x00008798 a0020000 64b2ffff 4f020000 00420e10 ....d...O....B..
+  0x000087a8 8d02450e 188c0341 0e208604 440e2883 ..E....A. ..D.(.
+  0x000087b8 05470e50 02f60a0e 28440e20 410e1842 .G.P....(D. A..B
+  0x000087c8 0e10420e 08460b00 8c000000 dc020000 ..B..F..........
+  0x000087d8 78b4ffff ec050000 00420e10 8f02420e x........B....B.
+  0x000087e8 188e0342 0e208d04 450e288c 05440e30 ...B. ..E.(..D.0
+  0x000087f8 8606440e 38830746 0e6002a5 0a0e3841 ..D.8..F.`....8A
+  0x00008808 0e30410e 28420e20 420e1842 0e10420e .0A.(B. B..B..B.
+  0x00008818 08480b56 0a0e3841 0e30410e 28420e20 .H.V..8A.0A.(B. 
+  0x00008828 420e1842 0e10420e 08480b03 77010e68 B..B..B..H..w..h
+  0x00008838 540e7041 0e78420e 8001410e 8801410e T.pA.xB...A...A.
+  0x00008848 9001410e 9801410e a001410e a801410e ..A...A...A...A.
+  0x00008858 b001490e 60000000 64000000 6c030000 ..I.`...d...l...
+  0x00008868 a0a1ffff c0080000 00460e10 8d02420e .........F....B.
+  0x00008878 188c0341 0e208604 440e2883 05470e90 ...A. ..D.(..G..
+  0x00008888 0203e405 0e98024e 0ea00242 0ea80246 .......N...B...F
+  0x00008898 0eb00246 0eb80241 0ec00241 0ec80241 ...F...A...A...A
+  0x000088a8 0ed00241 0ed80241 0ee0024e 0e900203 ...A...A...N....
+  0x000088b8 92020e28 410e2041 0e18420e 10420e08 ...(A. A..B..B..
+  0x000088c8 5c000000 d4030000 70b9ffff f1010000 \.......p.......
+  0x000088d8 00420e10 8d02420e 188c0341 0e208604 .B....B....A. ..
+  0x000088e8 440e2883 05440e30 02920a0e 28440e20 D.(..D.0....(D. 
+  0x000088f8 410e1842 0e10420e 08480b02 a40a0e28 A..B..B..H.....(
+  0x00008908 450e2041 0e18420e 10420e08 4a0b7c0a E. A..B..B..J.|.
+  0x00008918 0e28490e 20410e18 420e1042 0e084e0b .(I. A..B..B..N.
+  0x00008928 48000000 34040000 10bbffff 6f2f0000 H...4.......o/..
+  0x00008938 00460e10 8f02420e 188e0342 0e208d04 .F....B....B. ..
+  0x00008948 420e288c 05410e30 8606410e 38830744 B.(..A.0..A.8..D
+  0x00008958 0e700386 0c0a0e38 440e3041 0e28420e .p.....8D.0A.(B.
+  0x00008968 20420e18 420e1042 0e084b0b 10000000  B..B..B..K.....
+  0x00008978 80040000 4ca9ffff 10000000 00000000 ....L...........
+  0x00008988 00000000                            ....
```

### readelf --wide --decompress --hex-dump=.init_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.init_array':
-  0x00007d78 a0320000 00000000                   .2......
+  0x00009d78 90330000 00000000                   .3......
```

### readelf --wide --decompress --hex-dump=.fini_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.fini_array':
-  0x00007d80 60320000 00000000                   `2......
+  0x00009d80 50330000 00000000                   P3......
```

### readelf --wide --decompress --hex-dump=.got {}

```diff
@@ -1,14 +1,14 @@
 
 Hex dump of section '.got':
-  0x00007f58 00000000 00000000 00000000 00000000 ................
-  0x00007f68 00000000 00000000 00000000 00000000 ................
-  0x00007f78 00000000 00000000 00000000 00000000 ................
-  0x00007f88 00000000 00000000 00000000 00000000 ................
-  0x00007f98 00000000 00000000 00000000 00000000 ................
-  0x00007fa8 00000000 00000000 00000000 00000000 ................
-  0x00007fb8 00000000 00000000 00000000 00000000 ................
-  0x00007fc8 00000000 00000000 00000000 00000000 ................
-  0x00007fd8 00000000 00000000 00000000 00000000 ................
-  0x00007fe8 00000000 00000000 00000000 00000000 ................
-  0x00007ff8 00000000 00000000                   ........
+  0x00009f58 00000000 00000000 00000000 00000000 ................
+  0x00009f68 00000000 00000000 00000000 00000000 ................
+  0x00009f78 00000000 00000000 00000000 00000000 ................
+  0x00009f88 00000000 00000000 00000000 00000000 ................
+  0x00009f98 00000000 00000000 00000000 00000000 ................
+  0x00009fa8 00000000 00000000 00000000 00000000 ................
+  0x00009fb8 00000000 00000000 00000000 00000000 ................
+  0x00009fc8 00000000 00000000 00000000 00000000 ................
+  0x00009fd8 00000000 00000000 00000000 00000000 ................
+  0x00009fe8 00000000 00000000 00000000 00000000 ................
+  0x00009ff8 00000000 00000000                   ........
```

### readelf --wide --decompress --hex-dump=.got.plt {}

```diff
@@ -1,34 +1,34 @@
 
 Hex dump of section '.got.plt':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
-  0x00008000 887d0000 00000000 00000000 00000000 .}..............
-  0x00008010 00000000 00000000 30200000 00000000 ........0 ......
-  0x00008020 40200000 00000000 50200000 00000000 @ ......P ......
-  0x00008030 60200000 00000000 70200000 00000000 ` ......p ......
-  0x00008040 80200000 00000000 90200000 00000000 . ....... ......
-  0x00008050 a0200000 00000000 b0200000 00000000 . ....... ......
-  0x00008060 c0200000 00000000 d0200000 00000000 . ....... ......
-  0x00008070 e0200000 00000000 f0200000 00000000 . ....... ......
-  0x00008080 00210000 00000000 10210000 00000000 .!.......!......
-  0x00008090 20210000 00000000 30210000 00000000  !......0!......
-  0x000080a0 40210000 00000000 50210000 00000000 @!......P!......
-  0x000080b0 60210000 00000000 70210000 00000000 `!......p!......
-  0x000080c0 80210000 00000000 90210000 00000000 .!.......!......
-  0x000080d0 a0210000 00000000 b0210000 00000000 .!.......!......
-  0x000080e0 c0210000 00000000 d0210000 00000000 .!.......!......
-  0x000080f0 e0210000 00000000 f0210000 00000000 .!.......!......
-  0x00008100 00220000 00000000 10220000 00000000 ."......."......
-  0x00008110 20220000 00000000 30220000 00000000  "......0"......
-  0x00008120 40220000 00000000 50220000 00000000 @"......P"......
-  0x00008130 60220000 00000000 70220000 00000000 `"......p"......
-  0x00008140 80220000 00000000 90220000 00000000 ."......."......
-  0x00008150 a0220000 00000000 b0220000 00000000 ."......."......
-  0x00008160 c0220000 00000000 d0220000 00000000 ."......."......
-  0x00008170 e0220000 00000000 f0220000 00000000 ."......."......
-  0x00008180 00230000 00000000 10230000 00000000 .#.......#......
-  0x00008190 20230000 00000000 30230000 00000000  #......0#......
-  0x000081a0 40230000 00000000 50230000 00000000 @#......P#......
-  0x000081b0 60230000 00000000 70230000 00000000 `#......p#......
-  0x000081c0 80230000 00000000 90230000 00000000 .#.......#......
-  0x000081d0 a0230000 00000000                   .#......
+  0x0000a000 889d0000 00000000 00000000 00000000 ................
+  0x0000a010 00000000 00000000 30200000 00000000 ........0 ......
+  0x0000a020 40200000 00000000 50200000 00000000 @ ......P ......
+  0x0000a030 60200000 00000000 70200000 00000000 ` ......p ......
+  0x0000a040 80200000 00000000 90200000 00000000 . ....... ......
+  0x0000a050 a0200000 00000000 b0200000 00000000 . ....... ......
+  0x0000a060 c0200000 00000000 d0200000 00000000 . ....... ......
+  0x0000a070 e0200000 00000000 f0200000 00000000 . ....... ......
+  0x0000a080 00210000 00000000 10210000 00000000 .!.......!......
+  0x0000a090 20210000 00000000 30210000 00000000  !......0!......
+  0x0000a0a0 40210000 00000000 50210000 00000000 @!......P!......
+  0x0000a0b0 60210000 00000000 70210000 00000000 `!......p!......
+  0x0000a0c0 80210000 00000000 90210000 00000000 .!.......!......
+  0x0000a0d0 a0210000 00000000 b0210000 00000000 .!.......!......
+  0x0000a0e0 c0210000 00000000 d0210000 00000000 .!.......!......
+  0x0000a0f0 e0210000 00000000 f0210000 00000000 .!.......!......
+  0x0000a100 00220000 00000000 10220000 00000000 ."......."......
+  0x0000a110 20220000 00000000 30220000 00000000  "......0"......
+  0x0000a120 40220000 00000000 50220000 00000000 @"......P"......
+  0x0000a130 60220000 00000000 70220000 00000000 `"......p"......
+  0x0000a140 80220000 00000000 90220000 00000000 ."......."......
+  0x0000a150 a0220000 00000000 b0220000 00000000 ."......."......
+  0x0000a160 c0220000 00000000 d0220000 00000000 ."......."......
+  0x0000a170 e0220000 00000000 f0220000 00000000 ."......."......
+  0x0000a180 00230000 00000000 10230000 00000000 .#.......#......
+  0x0000a190 20230000 00000000 30230000 00000000  #......0#......
+  0x0000a1a0 40230000 00000000 50230000 00000000 @#......P#......
+  0x0000a1b0 60230000 00000000 70230000 00000000 `#......p#......
+  0x0000a1c0 80230000 00000000 90230000 00000000 .#.......#......
+  0x0000a1d0 a0230000 00000000 b0230000 00000000 .#.......#......
```

### readelf --wide --decompress --hex-dump=.data {}

```diff
@@ -1,77 +1,103 @@
 
 Hex dump of section '.data':
-  0x000081e0 e0810000 00000000 00000000 00000000 ................
-  0x000081f0 00000000 00000000 00000000 00000000 ................
-  0x00008200 ffffffff ffffffff 00000000 00000000 ................
-  0x00008210 00000000 00000000 00000000 00000000 ................
-  0x00008220 0a202020 20e88eb7 e58f96e6 9cace69c .    ...........
-  0x00008230 bae789a9 e79086e5 9cb0e59d 802c20e8 ............., .
-  0x00008240 8eb7e58f 96e69cac e69cba6d 6163e59c ...........mac..
-  0x00008250 b0e59d80 0a202020 203a7265 7475726e .....    :return
-  0x00008260 3a0a2020 20200000 00000000 00000000 :.    ..........
-  0x00008270 00000000 00000000 00000000 00000000 ................
-  0x00008280 a8870000 00000000 ce630000 00000000 .........c......
-  0x00008290 05000000 00000000 00000000 00000000 ................
-  0x000082a0 00010100 00000000 a0870000 00000000 ................
-  0x000082b0 df630000 00000000 02000000 00000000 .c..............
-  0x000082c0 00000000 00000000 00010000 00000000 ................
-  0x000082d0 98870000 00000000 50630000 00000000 ........Pc......
-  0x000082e0 13000000 00000000 00000000 00000000 ................
-  0x000082f0 00010100 00000000 90870000 00000000 ................
-  0x00008300 e1630000 00000000 02000000 00000000 .c..............
-  0x00008310 00000000 00000000 00010100 00000000 ................
-  0x00008320 88870000 00000000 68630000 00000000 ........hc......
-  0x00008330 0e000000 00000000 00000000 00000000 ................
-  0x00008340 00010100 00000000 80870000 00000000 ................
-  0x00008350 78630000 00000000 08000000 00000000 xc..............
-  0x00008360 00000000 00000000 00010100 00000000 ................
-  0x00008370 78870000 00000000 db630000 00000000 x........c......
-  0x00008380 04000000 00000000 00000000 00000000 ................
-  0x00008390 00010100 00000000 70870000 00000000 ........p.......
-  0x000083a0 80630000 00000000 0b000000 00000000 .c..............
-  0x000083b0 00000000 00000000 00010100 00000000 ................
-  0x000083c0 68870000 00000000 d7630000 00000000 h........c......
-  0x000083d0 04000000 00000000 00000000 00000000 ................
-  0x000083e0 00010100 00000000 60870000 00000000 ........`.......
-  0x000083f0 c9630000 00000000 05000000 00000000 .c..............
-  0x00008400 00000000 00000000 00010100 00000000 ................
-  0x00008410 58870000 00000000 d3630000 00000000 X........c......
-  0x00008420 04000000 00000000 00000000 00000000 ................
-  0x00008430 00010100 00000000 50870000 00000000 ........P.......
-  0x00008440 c0630000 00000000 09000000 00000000 .c..............
-  0x00008450 00000000 00000000 00010100 00000000 ................
-  0x00008460 48870000 00000000 b0630000 00000000 H........c......
-  0x00008470 09000000 00000000 00000000 00000000 ................
-  0x00008480 00010100 00000000 40870000 00000000 ........@.......
-  0x00008490 30630000 00000000 1e000000 00000000 0c..............
-  0x000084a0 00000000 00000000 00010100 00000000 ................
-  0x000084b0 38870000 00000000 00630000 00000000 8........c......
-  0x000084c0 22000000 00000000 00000000 00000000 "...............
-  0x000084d0 00010000 00000000 30870000 00000000 ........0.......
-  0x000084e0 91630000 00000000 06000000 00000000 .c..............
-  0x000084f0 00000000 00000000 00010100 00000000 ................
-  0x00008500 28870000 00000000 a0630000 00000000 (........c......
-  0x00008510 09000000 00000000 00000000 00000000 ................
-  0x00008520 00010100 00000000 20870000 00000000 ........ .......
-  0x00008530 8b630000 00000000 06000000 00000000 .c..............
-  0x00008540 00000000 00000000 00010100 00000000 ................
-  0x00008550 18870000 00000000 97630000 00000000 .........c......
-  0x00008560 05000000 00000000 00000000 00000000 ................
-  0x00008570 00010100 00000000 00000000 00000000 ................
-  0x00008580 00000000 00000000 00000000 00000000 ................
-  0x00008590 00000000 00000000 00000000 00000000 ................
-  0x000085a0 01000000 00000000 00000000 00000000 ................
-  0x000085b0 00000000 00000000 00000000 00000000 ................
-  0x000085c0 00000000 00000000 b0620000 00000000 .........b......
-  0x000085d0 00000000 00000000 00000000 00000000 ................
-  0x000085e0 e0860000 00000000 20860000 00000000 ........ .......
-  0x000085f0 00000000 00000000 00000000 00000000 ................
-  0x00008600 00000000 00000000 00000000 00000000 ................
-  0x00008610 00000000 00000000 00000000 00000000 ................
-  0x00008620 01000000 00000000 be270000 00000000 .........'......
-  0x00008630 02000000 00000000 22290000 00000000 ........")......
-  0x00008640 00000000 00000000 00000000 00000000 ................
-  0x00008650 00000000 00000000 00000000 00000000 ................
-  0x00008660 e2620000 00000000 403c0000 00000000 .b......@<......
-  0x00008670 04000000 00000000 20820000 00000000 ........ .......
+  0x0000a1e0 e0a10000 00000000 00000000 00000000 ................
+  0x0000a1f0 00000000 00000000 00000000 00000000 ................
+  0x0000a200 ffffffff ffffffff 00000000 00000000 ................
+  0x0000a210 00000000 00000000 00000000 00000000 ................
+  0x0000a220 0a202020 20e88eb7 e58f96e6 9cace69c .    ...........
+  0x0000a230 bae789a9 e79086e5 9cb0e59d 802c20e8 ............., .
+  0x0000a240 8eb7e58f 96e69cac e69cba6d 6163e59c ...........mac..
+  0x0000a250 b0e59d80 0a202020 203a7265 7475726e .....    :return
+  0x0000a260 3a0a2020 20200000 00000000 00000000 :.    ..........
+  0x0000a270 00000000 00000000 00000000 00000000 ................
+  0x0000a280 c0a90000 00000000 4e840000 00000000 ........N.......
+  0x0000a290 02000000 00000000 00000000 00000000 ................
+  0x0000a2a0 00010000 00000000 b8a90000 00000000 ................
+  0x0000a2b0 36840000 00000000 05000000 00000000 6...............
+  0x0000a2c0 00000000 00000000 00010100 00000000 ................
+  0x0000a2d0 b0a90000 00000000 4a840000 00000000 ........J.......
+  0x0000a2e0 02000000 00000000 00000000 00000000 ................
+  0x0000a2f0 00010000 00000000 a8a90000 00000000 ................
+  0x0000a300 90830000 00000000 13000000 00000000 ................
+  0x0000a310 00000000 00000000 00010100 00000000 ................
+  0x0000a320 a0a90000 00000000 f9830000 00000000 ................
+  0x0000a330 06000000 00000000 00000000 00000000 ................
+  0x0000a340 00010100 00000000 98a90000 00000000 ................
+  0x0000a350 4c840000 00000000 02000000 00000000 L...............
+  0x0000a360 00000000 00000000 00010100 00000000 ................
+  0x0000a370 90a90000 00000000 a8830000 00000000 ................
+  0x0000a380 0e000000 00000000 00000000 00000000 ................
+  0x0000a390 00010100 00000000 88a90000 00000000 ................
+  0x0000a3a0 c0830000 00000000 08000000 00000000 ................
+  0x0000a3b0 00000000 00000000 00010100 00000000 ................
+  0x0000a3c0 80a90000 00000000 43840000 00000000 ........C.......
+  0x0000a3d0 04000000 00000000 00000000 00000000 ................
+  0x0000a3e0 00010100 00000000 78a90000 00000000 ........x.......
+  0x0000a3f0 40830000 00000000 2f000000 00000000 @......./.......
+  0x0000a400 00000000 00000000 00010000 00000000 ................
+  0x0000a410 70a90000 00000000 d0830000 00000000 p...............
+  0x0000a420 0b000000 00000000 00000000 00000000 ................
+  0x0000a430 00010100 00000000 68a90000 00000000 ........h.......
+  0x0000a440 3f840000 00000000 04000000 00000000 ?...............
+  0x0000a450 00000000 00000000 00010100 00000000 ................
+  0x0000a460 60a90000 00000000 31840000 00000000 `.......1.......
+  0x0000a470 05000000 00000000 00000000 00000000 ................
+  0x0000a480 00010100 00000000 58a90000 00000000 ........X.......
+  0x0000a490 3b840000 00000000 04000000 00000000 ;...............
+  0x0000a4a0 00000000 00000000 00010100 00000000 ................
+  0x0000a4b0 50a90000 00000000 28840000 00000000 P.......(.......
+  0x0000a4c0 09000000 00000000 00000000 00000000 ................
+  0x0000a4d0 00010100 00000000 48a90000 00000000 ........H.......
+  0x0000a4e0 18840000 00000000 09000000 00000000 ................
+  0x0000a4f0 00000000 00000000 00010100 00000000 ................
+  0x0000a500 40a90000 00000000 47840000 00000000 @.......G.......
+  0x0000a510 03000000 00000000 00000000 00000000 ................
+  0x0000a520 00010100 00000000 38a90000 00000000 ........8.......
+  0x0000a530 f3830000 00000000 06000000 00000000 ................
+  0x0000a540 00000000 00000000 00010100 00000000 ................
+  0x0000a550 30a90000 00000000 70830000 00000000 0.......p.......
+  0x0000a560 1e000000 00000000 00000000 00000000 ................
+  0x0000a570 00010100 00000000 28a90000 00000000 ........(.......
+  0x0000a580 00830000 00000000 22000000 00000000 ........".......
+  0x0000a590 00000000 00000000 00010000 00000000 ................
+  0x0000a5a0 20a90000 00000000 ed830000 00000000  ...............
+  0x0000a5b0 06000000 00000000 00000000 00000000 ................
+  0x0000a5c0 00010100 00000000 18a90000 00000000 ................
+  0x0000a5d0 11840000 00000000 05000000 00000000 ................
+  0x0000a5e0 00000000 00000000 00010100 00000000 ................
+  0x0000a5f0 10a90000 00000000 b8830000 00000000 ................
+  0x0000a600 08000000 00000000 00000000 00000000 ................
+  0x0000a610 00010100 00000000 08a90000 00000000 ................
+  0x0000a620 c8830000 00000000 07000000 00000000 ................
+  0x0000a630 00000000 00000000 00010100 00000000 ................
+  0x0000a640 00a90000 00000000 e7830000 00000000 ................
+  0x0000a650 06000000 00000000 00000000 00000000 ................
+  0x0000a660 00010100 00000000 f8a80000 00000000 ................
+  0x0000a670 e1830000 00000000 06000000 00000000 ................
+  0x0000a680 00000000 00000000 00010100 00000000 ................
+  0x0000a690 f0a80000 00000000 08840000 00000000 ................
+  0x0000a6a0 09000000 00000000 00000000 00000000 ................
+  0x0000a6b0 00010100 00000000 e8a80000 00000000 ................
+  0x0000a6c0 db830000 00000000 06000000 00000000 ................
+  0x0000a6d0 00000000 00000000 00010100 00000000 ................
+  0x0000a6e0 e0a80000 00000000 ff830000 00000000 ................
+  0x0000a6f0 05000000 00000000 00000000 00000000 ................
+  0x0000a700 00010100 00000000 00000000 00000000 ................
+  0x0000a710 00000000 00000000 00000000 00000000 ................
+  0x0000a720 00000000 00000000 00000000 00000000 ................
+  0x0000a730 00000000 00000000 00000000 00000000 ................
+  0x0000a740 01000000 00000000 00000000 00000000 ................
+  0x0000a750 00000000 00000000 00000000 00000000 ................
+  0x0000a760 00000000 00000000 b3820000 00000000 ................
+  0x0000a770 00000000 00000000 00000000 00000000 ................
+  0x0000a780 a0a80000 00000000 c0a70000 00000000 ................
+  0x0000a790 00000000 00000000 00000000 00000000 ................
+  0x0000a7a0 00000000 00000000 00000000 00000000 ................
+  0x0000a7b0 00000000 00000000 00000000 00000000 ................
+  0x0000a7c0 01000000 00000000 de270000 00000000 .........'......
+  0x0000a7d0 02000000 00000000 082a0000 00000000 .........*......
+  0x0000a7e0 00000000 00000000 00000000 00000000 ................
+  0x0000a7f0 00000000 00000000 00000000 00000000 ................
+  0x0000a800 e5820000 00000000 40440000 00000000 ........@D......
+  0x0000a810 04000000 00000000 20a20000 00000000 ........ .......
```

### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -2,208 +2,241 @@
 Hex dump of section '.strtab':
   0x00000000 00646576 6963655f 7574696c 732e6300 .device_utils.c.
   0x00000010 5f5f7079 785f6269 73656374 5f636f64 __pyx_bisect_cod
   0x00000020 655f6f62 6a656374 73005f5f 5079785f e_objects.__Pyx_
   0x00000030 50794675 6e637469 6f6e5f46 61737443 PyFunction_FastC
   0x00000040 616c6c4e 6f4b7700 5f5f7079 785f7079 allNoKw.__pyx_py
   0x00000050 6672616d 655f6c6f 63616c73 706c7573 frame_localsplus
-  0x00000060 5f6f6666 73657400 5f5f5079 785f4164 _offset.__Pyx_Ad
-  0x00000070 64547261 63656261 636b005f 5f707978 dTraceback.__pyx
-  0x00000080 5f636f64 655f6361 63686500 5f5f7079 _code_cache.__py
-  0x00000090 785f6400 5f5f7079 785f6379 74686f6e x_d.__pyx_cython
-  0x000000a0 5f72756e 74696d65 005f5f70 79785f64 _runtime.__pyx_d
-  0x000000b0 6963745f 76657273 696f6e2e 31353836 ict_version.1586
-  0x000000c0 36005f5f 7079785f 64696374 5f636163 6.__pyx_dict_cac
-  0x000000d0 6865645f 76616c75 652e3135 38363700 hed_value.15867.
-  0x000000e0 5f5f7079 785f6e5f 735f636c 696e655f __pyx_n_s_cline_
-  0x000000f0 696e5f74 72616365 6261636b 005f5f70 in_traceback.__p
-  0x00000100 79785f65 6d707479 5f747570 6c65005f yx_empty_tuple._
-  0x00000110 5f707978 5f656d70 74795f62 79746573 _pyx_empty_bytes
-  0x00000120 005f5f50 79785f63 6f70795f 73706563 .__Pyx_copy_spec
-  0x00000130 5f746f5f 6d6f6475 6c65005f 5f707978 _to_module.__pyx
-  0x00000140 5f70796d 6f645f63 72656174 65006d61 _pymod_create.ma
-  0x00000150 696e5f69 6e746572 70726574 65725f69 in_interpreter_i
-  0x00000160 642e3135 36373000 5f5f7079 785f6d00 d.15670.__pyx_m.
-  0x00000170 5f5f5079 785f5079 46756e63 74696f6e __Pyx_PyFunction
-  0x00000180 5f466173 7443616c 6c446963 742e636f _FastCallDict.co
-  0x00000190 6e737470 726f702e 30005f5f 5079785f nstprop.0.__Pyx_
-  0x000001a0 47657442 75696c74 696e4e61 6d65005f GetBuiltinName._
-  0x000001b0 5f707978 5f62005f 5f507978 5f5f4765 _pyx_b.__Pyx__Ge
-  0x000001c0 744d6f64 756c6547 6c6f6261 6c4e616d tModuleGlobalNam
-  0x000001d0 65005f5f 7079785f 70796d6f 645f6578 e.__pyx_pymod_ex
-  0x000001e0 65635f64 65766963 655f7574 696c7300 ec_device_utils.
-  0x000001f0 5f5f7079 785f6c69 6e656e6f 005f5f70 __pyx_lineno.__p
-  0x00000200 79785f66 696c656e 616d6500 5f5f7079 yx_filename.__py
-  0x00000210 785f636c 696e656e 6f005f5f 7079785f x_clineno.__pyx_
-  0x00000220 73747269 6e675f74 6162005f 5f707978 string_tab.__pyx
-  0x00000230 5f696e74 5f32005f 5f707978 5f696e74 _int_2.__pyx_int
-  0x00000240 5f6e6567 5f313200 5f5f7079 785f6e5f _neg_12.__pyx_n_
-  0x00000250 735f6d61 696e005f 5f707978 5f6e5f73 s_main.__pyx_n_s
-  0x00000260 5f6e616d 65005f5f 7079785f 6e5f735f _name.__pyx_n_s_
-  0x00000270 72616e67 65005f5f 7079785f 736c6963 range.__pyx_slic
-  0x00000280 655f005f 5f707978 5f6e5f73 5f65005f e_.__pyx_n_s_e._
-  0x00000290 5f707978 5f6e5f73 5f6d6163 005f5f70 _pyx_n_s_mac.__p
-  0x000002a0 79785f6e 5f735f67 65745f64 65766963 yx_n_s_get_devic
-  0x000002b0 655f6964 005f5f70 79785f6b 705f735f e_id.__pyx_kp_s_
-  0x000002c0 70797465 6c657264 61635f75 74696c73 pytelerdac_utils
-  0x000002d0 5f646576 6963655f 7574696c 735f7079 _device_utils_py
-  0x000002e0 005f5f70 79785f6e 5f735f75 75696400 .__pyx_n_s_uuid.
-  0x000002f0 5f5f7079 785f6e5f 735f7079 74656c65 __pyx_n_s_pytele
-  0x00000300 72646163 5f757469 6c735f64 65766963 rdac_utils_devic
-  0x00000310 655f7574 696c7300 5f5f7079 785f6d64 e_utils.__pyx_md
-  0x00000320 65665f31 30707974 656c6572 6461635f ef_10pytelerdac_
-  0x00000330 35757469 6c735f31 32646576 6963655f 5utils_12device_
-  0x00000340 7574696c 735f3167 65745f64 65766963 utils_1get_devic
-  0x00000350 655f6964 005f5f70 79785f6e 5f735f74 e_id.__pyx_n_s_t
-  0x00000360 65737400 5f5f7079 785f7077 5f313070 est.__pyx_pw_10p
-  0x00000370 7974656c 65726461 635f3575 74696c73 ytelerdac_5utils
-  0x00000380 5f313264 65766963 655f7574 696c735f _12device_utils_
-  0x00000390 31676574 5f646576 6963655f 6964005f 1get_device_id._
-  0x000003a0 5f707978 5f646963 745f7665 7273696f _pyx_dict_versio
-  0x000003b0 6e2e3135 35393200 5f5f7079 785f6469 n.15592.__pyx_di
-  0x000003c0 63745f63 61636865 645f7661 6c75652e ct_cached_value.
-  0x000003d0 31353539 33005f5f 7079785f 6e5f735f 15593.__pyx_n_s_
-  0x000003e0 55554944 005f5f70 79785f64 6963745f UUID.__pyx_dict_
-  0x000003f0 76657273 696f6e2e 31353539 35005f5f version.15595.__
-  0x00000400 7079785f 64696374 5f636163 6865645f pyx_dict_cached_
-  0x00000410 76616c75 652e3135 35393600 5f5f7079 value.15596.__py
-  0x00000420 785f6e5f 735f6765 746e6f64 65005f5f x_n_s_getnode.__
-  0x00000430 7079785f 6e5f735f 696e7400 5f5f7079 pyx_n_s_int.__py
-  0x00000440 785f6e5f 735f6865 78005f5f 7079785f x_n_s_hex.__pyx_
-  0x00000450 6e5f735f 75707065 72005f5f 7079785f n_s_upper.__pyx_
-  0x00000460 6b705f73 5f5f3200 5f5f7079 785f6d6f kp_s__2.__pyx_mo
-  0x00000470 64756c65 64656600 5f5f7079 785f6b5f duledef.__pyx_k_
-  0x00000480 55554944 005f5f70 79785f6b 5f5f3200 UUID.__pyx_k__2.
-  0x00000490 5f5f7079 785f6b5f 636c696e 655f696e __pyx_k_cline_in
-  0x000004a0 5f747261 63656261 636b005f 5f707978 _traceback.__pyx
-  0x000004b0 5f6b5f65 005f5f70 79785f6b 5f676574 _k_e.__pyx_k_get
-  0x000004c0 5f646576 6963655f 6964005f 5f707978 _device_id.__pyx
-  0x000004d0 5f6b5f67 65746e6f 6465005f 5f707978 _k_getnode.__pyx
-  0x000004e0 5f6b5f68 6578005f 5f707978 5f6e5f73 _k_hex.__pyx_n_s
-  0x000004f0 5f696d70 6f727400 5f5f7079 785f6b5f _import.__pyx_k_
-  0x00000500 696d706f 7274005f 5f707978 5f6b5f69 import.__pyx_k_i
-  0x00000510 6e74005f 5f707978 5f6e5f73 5f6a6f69 nt.__pyx_n_s_joi
-  0x00000520 6e005f5f 7079785f 6b5f6a6f 696e005f n.__pyx_k_join._
-  0x00000530 5f707978 5f6b5f6d 6163005f 5f707978 _pyx_k_mac.__pyx
-  0x00000540 5f6b5f6d 61696e00 5f5f7079 785f6b5f _k_main.__pyx_k_
-  0x00000550 6e616d65 005f5f70 79785f6b 5f707974 name.__pyx_k_pyt
-  0x00000560 656c6572 6461635f 7574696c 735f6465 elerdac_utils_de
-  0x00000570 76696365 5f757469 6c73005f 5f707978 vice_utils.__pyx
-  0x00000580 5f6b5f70 7974656c 65726461 635f7574 _k_pytelerdac_ut
-  0x00000590 696c735f 64657669 63655f75 74696c73 ils_device_utils
-  0x000005a0 5f707900 5f5f7079 785f6b5f 72616e67 _py.__pyx_k_rang
-  0x000005b0 65005f5f 7079785f 6b5f7465 7374005f e.__pyx_k_test._
-  0x000005c0 5f707978 5f6b5f75 70706572 005f5f70 _pyx_k_upper.__p
-  0x000005d0 79785f6b 5f757569 64005f5f 7079785f yx_k_uuid.__pyx_
-  0x000005e0 6d657468 6f647300 5f5f7079 785f6d6f methods.__pyx_mo
-  0x000005f0 64756c65 6465665f 736c6f74 73005f5f duledef_slots.__
-  0x00000600 7079785f 646f635f 31307079 74656c65 pyx_doc_10pytele
-  0x00000610 72646163 5f357574 696c735f 31326465 rdac_5utils_12de
-  0x00000620 76696365 5f757469 6c735f67 65745f64 vice_utils_get_d
-  0x00000630 65766963 655f6964 00637274 73747566 evice_id.crtstuf
-  0x00000640 662e6300 64657265 67697374 65725f74 f.c.deregister_t
-  0x00000650 6d5f636c 6f6e6573 005f5f64 6f5f676c m_clones.__do_gl
-  0x00000660 6f62616c 5f64746f 72735f61 75780063 obal_dtors_aux.c
-  0x00000670 6f6d706c 65746564 2e383036 31005f5f ompleted.8061.__
-  0x00000680 646f5f67 6c6f6261 6c5f6474 6f72735f do_global_dtors_
-  0x00000690 6175785f 66696e69 5f617272 61795f65 aux_fini_array_e
-  0x000006a0 6e747279 00667261 6d655f64 756d6d79 ntry.frame_dummy
-  0x000006b0 005f5f66 72616d65 5f64756d 6d795f69 .__frame_dummy_i
-  0x000006c0 6e69745f 61727261 795f656e 74727900 nit_array_entry.
-  0x000006d0 5f5f4652 414d455f 454e445f 5f005f66 __FRAME_END__._f
-  0x000006e0 696e6900 5f5f6473 6f5f6861 6e646c65 ini.__dso_handle
-  0x000006f0 005f4459 4e414d49 43005f5f 474e555f ._DYNAMIC.__GNU_
-  0x00000700 45485f46 52414d45 5f484452 005f5f54 EH_FRAME_HDR.__T
-  0x00000710 4d435f45 4e445f5f 005f474c 4f42414c MC_END__._GLOBAL
-  0x00000720 5f4f4646 5345545f 5441424c 455f005f _OFFSET_TABLE_._
-  0x00000730 696e6974 00507955 6e69636f 64655f46 init.PyUnicode_F
-  0x00000740 726f6d46 6f726d61 74005079 4c697374 romFormat.PyList
-  0x00000750 5f4e6577 00507945 78635f53 79737465 _New.PyExc_Syste
-  0x00000760 6d457272 6f720050 79446963 745f5365 mError.PyDict_Se
-  0x00000770 74497465 6d537472 696e6700 50794d65 tItemString.PyMe
-  0x00000780 74686f64 5f547970 65005f49 544d5f64 thod_Type._ITM_d
-  0x00000790 65726567 69737465 72544d43 6c6f6e65 eregisterTMClone
-  0x000007a0 5461626c 65005079 466c6f61 745f5479 Table.PyFloat_Ty
-  0x000007b0 7065005f 50795468 72656164 53746174 pe._PyThreadStat
-  0x000007c0 655f556e 63686563 6b656447 65740050 e_UncheckedGet.P
-  0x000007d0 794d6f64 756c6544 65665f49 6e697400 yModuleDef_Init.
-  0x000007e0 50794672 616d655f 4e657700 50794346 PyFrame_New.PyCF
-  0x000007f0 756e6374 696f6e5f 4e657745 78005079 unction_NewEx.Py
-  0x00000800 4e756d62 65725f41 64640050 794f626a Number_Add.PyObj
-  0x00000810 6563745f 47657441 74747253 7472696e ect_GetAttrStrin
-  0x00000820 67005079 556e6963 6f64655f 4a6f696e g.PyUnicode_Join
-  0x00000830 00507949 6d706f72 745f4164 644d6f64 .PyImport_AddMod
-  0x00000840 756c6500 50794279 7465735f 46726f6d ule.PyBytes_From
-  0x00000850 53747269 6e67416e 6453697a 65005079 StringAndSize.Py
-  0x00000860 4f626a65 63745f53 65744174 74725374 Object_SetAttrSt
-  0x00000870 72696e67 00507945 72725f57 61726e45 ring.PyErr_WarnE
-  0x00000880 78005f50 795f4465 616c6c6f 63005079 x._Py_Dealloc.Py
-  0x00000890 4d6f6475 6c655f4e 65774f62 6a656374 Module_NewObject
-  0x000008a0 00507943 6f64655f 4e657700 5079496d .PyCode_New.PyIm
-  0x000008b0 706f7274 5f476574 4d6f6475 6c654469 port_GetModuleDi
-  0x000008c0 6374005f 5f737461 636b5f63 686b5f66 ct.__stack_chk_f
-  0x000008d0 61696c40 474c4942 435f322e 34005079 ail@GLIBC_2.4.Py
-  0x000008e0 4578635f 52756e74 696d6545 72726f72 Exc_RuntimeError
-  0x000008f0 00507945 72725f53 65745374 72696e67 .PyErr_SetString
-  0x00000900 00507945 78635f54 79706545 72726f72 .PyExc_TypeError
-  0x00000910 00507949 6e746572 70726574 65725374 .PyInterpreterSt
-  0x00000920 6174655f 47657449 44005079 4576616c ate_GetID.PyEval
-  0x00000930 5f457661 6c467261 6d654578 0050794d _EvalFrameEx.PyM
-  0x00000940 656d5f52 65616c6c 6f630050 79457272 em_Realloc.PyErr
-  0x00000950 5f457863 65707469 6f6e4d61 74636865 _ExceptionMatche
-  0x00000960 73005079 4f535f73 6e707269 6e746600 s.PyOS_snprintf.
-  0x00000970 50795472 61636542 61636b5f 48657265 PyTraceBack_Here
-  0x00000980 0050794f 626a6563 745f4e6f 74005079 .PyObject_Not.Py
-  0x00000990 466c6f61 745f4672 6f6d446f 75626c65 Float_FromDouble
-  0x000009a0 0050794c 6f6e675f 46726f6d 4c6f6e67 .PyLong_FromLong
-  0x000009b0 00507949 6e69745f 64657669 63655f75 .PyInit_device_u
-  0x000009c0 74696c73 00507945 72725f43 6c656172 tils.PyErr_Clear
-  0x000009d0 0050794c 6973745f 41707065 6e64005f .PyList_Append._
-  0x000009e0 50795f43 6865636b 52656375 72736976 Py_CheckRecursiv
-  0x000009f0 6543616c 6c005f50 795f4368 65636b52 eCall._Py_CheckR
-  0x00000a00 65637572 73696f6e 4c696d69 74005f50 ecursionLimit._P
-  0x00000a10 795f4661 6c736553 74727563 74005f5f y_FalseStruct.__
-  0x00000a20 676d6f6e 5f737461 72745f5f 00507954 gmon_start__.PyT
-  0x00000a30 75706c65 5f4e6577 00507954 68726561 uple_New.PyThrea
-  0x00000a40 64537461 74655f47 65740050 794f626a dState_Get.PyObj
-  0x00000a50 6563745f 53657441 74747200 50794572 ect_SetAttr.PyEr
-  0x00000a60 725f4f63 63757272 6564005f 50794469 r_Occurred._PyDi
-  0x00000a70 63745f47 65744974 656d5f4b 6e6f776e ct_GetItem_Known
-  0x00000a80 48617368 00507944 6963745f 47657449 Hash.PyDict_GetI
-  0x00000a90 74656d53 7472696e 67005079 4576616c temString.PyEval
-  0x00000aa0 5f457661 6c436f64 65457800 5f50795f _EvalCodeEx._Py_
-  0x00000ab0 4e6f6e65 53747275 63740050 79496d70 NoneStruct.PyImp
-  0x00000ac0 6f72745f 496d706f 72744d6f 64756c65 ort_ImportModule
-  0x00000ad0 4c657665 6c4f626a 65637400 50794f62 LevelObject.PyOb
-  0x00000ae0 6a656374 5f486173 68005f50 795f5472 ject_Hash._Py_Tr
-  0x00000af0 75655374 72756374 00507946 756e6374 ueStruct.PyFunct
-  0x00000b00 696f6e5f 54797065 00507944 6963745f ion_Type.PyDict_
-  0x00000b10 4e657700 50794c6f 6e675f54 79706500 New.PyLong_Type.
-  0x00000b20 50794672 616d655f 54797065 005f5079 PyFrame_Type._Py
-  0x00000b30 4f626a65 63745f47 65744469 63745074 Object_GetDictPt
-  0x00000b40 72005079 556e6963 6f64655f 46726f6d r.PyUnicode_From
-  0x00000b50 53747269 6e670050 79556e69 636f6465 String.PyUnicode
-  0x00000b60 5f496e74 65726e46 726f6d53 7472696e _InternFromStrin
-  0x00000b70 67005079 4578635f 496d706f 72744572 g.PyExc_ImportEr
-  0x00000b80 726f7200 50794469 63745f53 65744974 ror.PyDict_SetIt
-  0x00000b90 656d0050 79457863 5f417474 72696275 em.PyExc_Attribu
-  0x00000ba0 74654572 726f7200 50794f62 6a656374 teError.PyObject
-  0x00000bb0 5f43616c 6c005f5f 7079785f 6d6f6475 _Call.__pyx_modu
-  0x00000bc0 6c655f69 735f6d61 696e5f70 7974656c le_is_main_pytel
-  0x00000bd0 65726461 635f5f75 74696c73 5f5f6465 erdac__utils__de
-  0x00000be0 76696365 5f757469 6c730050 79556e69 vice_utils.PyUni
-  0x00000bf0 636f6465 5f446563 6f646500 50794572 code_Decode.PyEr
-  0x00000c00 725f466f 726d6174 00507953 6c696365 r_Format.PySlice
-  0x00000c10 5f4e6577 00507945 78635f4e 616d6545 _New.PyExc_NameE
-  0x00000c20 72726f72 00507955 6e69636f 64655f46 rror.PyUnicode_F
-  0x00000c30 726f6d53 7472696e 67416e64 53697a65 romStringAndSize
-  0x00000c40 0050794d 6f64756c 655f4765 74446963 .PyModule_GetDic
-  0x00000c50 74005f49 544d5f72 65676973 74657254 t._ITM_registerT
-  0x00000c60 4d436c6f 6e655461 626c6500 50794f62 MCloneTable.PyOb
-  0x00000c70 6a656374 5f476574 41747472 00507943 ject_GetAttr.PyC
-  0x00000c80 46756e63 74696f6e 5f547970 65005079 Function_Type.Py
-  0x00000c90 4d656d5f 4d616c6c 6f63005f 5f637861 Mem_Malloc.__cxa
-  0x00000ca0 5f66696e 616c697a 6540474c 4942435f _finalize@GLIBC_
-  0x00000cb0 322e322e 35005079 5475706c 655f5061 2.2.5.PyTuple_Pa
-  0x00000cc0 636b0050 795f4765 74566572 73696f6e ck.Py_GetVersion
-  0x00000cd0 00                                  .
+  0x00000060 5f6f6666 73657400 5f5f5079 785f636f _offset.__Pyx_co
+  0x00000070 70795f73 7065635f 746f5f6d 6f64756c py_spec_to_modul
+  0x00000080 65005f5f 7079785f 70796d6f 645f6372 e.__pyx_pymod_cr
+  0x00000090 65617465 006d6169 6e5f696e 74657270 eate.main_interp
+  0x000000a0 72657465 725f6964 2e313537 3136005f reter_id.15716._
+  0x000000b0 5f707978 5f6d005f 5f507978 5f496d70 _pyx_m.__Pyx_Imp
+  0x000000c0 6f72742e 636f6e73 7470726f 702e3000 ort.constprop.0.
+  0x000000d0 5f5f5079 785f5079 46756e63 74696f6e __Pyx_PyFunction
+  0x000000e0 5f466173 7443616c 6c446963 742e636f _FastCallDict.co
+  0x000000f0 6e737470 726f702e 30005f5f 5079785f nstprop.0.__Pyx_
+  0x00000100 47657442 75696c74 696e4e61 6d65005f GetBuiltinName._
+  0x00000110 5f707978 5f62005f 5f507978 5f5f4765 _pyx_b.__Pyx__Ge
+  0x00000120 744d6f64 756c6547 6c6f6261 6c4e616d tModuleGlobalNam
+  0x00000130 65005f5f 7079785f 64005f5f 5079785f e.__pyx_d.__Pyx_
+  0x00000140 50794f62 6a656374 5f43616c 6c4f6e65 PyObject_CallOne
+  0x00000150 41726700 5f5f5079 785f5079 4f626a65 Arg.__Pyx_PyObje
+  0x00000160 63745f43 616c6c32 41726773 005f5f50 ct_Call2Args.__P
+  0x00000170 79785f41 64645472 61636562 61636b00 yx_AddTraceback.
+  0x00000180 5f5f7079 785f636f 64655f63 61636865 __pyx_code_cache
+  0x00000190 005f5f70 79785f63 7974686f 6e5f7275 .__pyx_cython_ru
+  0x000001a0 6e74696d 65005f5f 7079785f 64696374 ntime.__pyx_dict
+  0x000001b0 5f766572 73696f6e 2e313539 3232005f _version.15922._
+  0x000001c0 5f707978 5f646963 745f6361 63686564 _pyx_dict_cached
+  0x000001d0 5f76616c 75652e31 35393233 005f5f70 _value.15923.__p
+  0x000001e0 79785f6e 5f735f63 6c696e65 5f696e5f yx_n_s_cline_in_
+  0x000001f0 74726163 65626163 6b005f5f 7079785f traceback.__pyx_
+  0x00000200 656d7074 795f7475 706c6500 5f5f7079 empty_tuple.__py
+  0x00000210 785f656d 7074795f 62797465 73005f5f x_empty_bytes.__
+  0x00000220 7079785f 70796d6f 645f6578 65635f64 pyx_pymod_exec_d
+  0x00000230 65766963 655f7574 696c7300 5f5f7079 evice_utils.__py
+  0x00000240 785f6c69 6e656e6f 005f5f70 79785f66 x_lineno.__pyx_f
+  0x00000250 696c656e 616d6500 5f5f7079 785f636c ilename.__pyx_cl
+  0x00000260 696e656e 6f005f5f 7079785f 73747269 ineno.__pyx_stri
+  0x00000270 6e675f74 6162005f 5f707978 5f696e74 ng_tab.__pyx_int
+  0x00000280 5f32005f 5f707978 5f696e74 5f6e6567 _2.__pyx_int_neg
+  0x00000290 5f313200 5f5f7079 785f6e5f 735f6d61 _12.__pyx_n_s_ma
+  0x000002a0 696e005f 5f707978 5f6e5f73 5f6e616d in.__pyx_n_s_nam
+  0x000002b0 65005f5f 7079785f 6e5f735f 72616e67 e.__pyx_n_s_rang
+  0x000002c0 65005f5f 7079785f 6b705f73 5f5f3200 e.__pyx_kp_s__2.
+  0x000002d0 5f5f7079 785f6b70 5f735f00 5f5f7079 __pyx_kp_s_.__py
+  0x000002e0 785f7475 706c655f 5f33005f 5f707978 x_tuple__3.__pyx
+  0x000002f0 5f736c69 63655f5f 34005f5f 7079785f _slice__4.__pyx_
+  0x00000300 6e5f735f 65005f5f 7079785f 6e5f735f n_s_e.__pyx_n_s_
+  0x00000310 6d616300 5f5f7079 785f6e5f 735f7265 mac.__pyx_n_s_re
+  0x00000320 73756c74 005f5f70 79785f6e 5f735f67 sult.__pyx_n_s_g
+  0x00000330 65745f64 65766963 655f6964 005f5f70 et_device_id.__p
+  0x00000340 79785f6b 705f735f 70797465 6c657264 yx_kp_s_pytelerd
+  0x00000350 61635f75 74696c73 5f646576 6963655f ac_utils_device_
+  0x00000360 7574696c 735f7079 005f5f70 79785f6e utils_py.__pyx_n
+  0x00000370 5f735f6f 73005f5f 7079785f 6e5f735f _s_os.__pyx_n_s_
+  0x00000380 75756964 005f5f70 79785f6e 5f735f70 uuid.__pyx_n_s_p
+  0x00000390 7974656c 65726461 635f7574 696c735f ytelerdac_utils_
+  0x000003a0 64657669 63655f75 74696c73 005f5f70 device_utils.__p
+  0x000003b0 79785f6d 6465665f 31307079 74656c65 yx_mdef_10pytele
+  0x000003c0 72646163 5f357574 696c735f 31326465 rdac_5utils_12de
+  0x000003d0 76696365 5f757469 6c735f31 6765745f vice_utils_1get_
+  0x000003e0 64657669 63655f69 64005f5f 7079785f device_id.__pyx_
+  0x000003f0 6e5f735f 74657374 005f5f50 79785f50 n_s_test.__Pyx_P
+  0x00000400 794f626a 6563745f 43616c6c 4e6f4172 yObject_CallNoAr
+  0x00000410 67005f5f 7079785f 70775f31 30707974 g.__pyx_pw_10pyt
+  0x00000420 656c6572 6461635f 35757469 6c735f31 elerdac_5utils_1
+  0x00000430 32646576 6963655f 7574696c 735f3167 2device_utils_1g
+  0x00000440 65745f64 65766963 655f6964 005f5f70 et_device_id.__p
+  0x00000450 79785f64 6963745f 76657273 696f6e2e yx_dict_version.
+  0x00000460 31353632 30005f5f 7079785f 64696374 15620.__pyx_dict
+  0x00000470 5f636163 6865645f 76616c75 652e3135 _cached_value.15
+  0x00000480 36323100 5f5f7079 785f6e5f 735f706f 621.__pyx_n_s_po
+  0x00000490 70656e00 5f5f7079 785f6b70 5f735f69 pen.__pyx_kp_s_i
+  0x000004a0 66636f6e 6669675f 6d6c616e 305f6772 fconfig_mlan0_gr
+  0x000004b0 65705f65 74686572 5f61776b 5f707200 ep_ether_awk_pr.
+  0x000004c0 5f5f7079 785f6e5f 735f7265 6164005f __pyx_n_s_read._
+  0x000004d0 5f707978 5f6e5f73 5f737472 6970005f _pyx_n_s_strip._
+  0x000004e0 5f707978 5f6e5f73 5f636c6f 7365005f _pyx_n_s_close._
+  0x000004f0 5f707978 5f6e5f73 5f73706c 6974005f _pyx_n_s_split._
+  0x00000500 5f707978 5f646963 745f7665 7273696f _pyx_dict_versio
+  0x00000510 6e2e3135 36333700 5f5f7079 785f6469 n.15637.__pyx_di
+  0x00000520 63745f63 61636865 645f7661 6c75652e ct_cached_value.
+  0x00000530 31353633 38005f5f 7079785f 6e5f735f 15638.__pyx_n_s_
+  0x00000540 55554944 005f5f70 79785f64 6963745f UUID.__pyx_dict_
+  0x00000550 76657273 696f6e2e 31353633 39005f5f version.15639.__
+  0x00000560 7079785f 64696374 5f636163 6865645f pyx_dict_cached_
+  0x00000570 76616c75 652e3135 36343000 5f5f7079 value.15640.__py
+  0x00000580 785f6e5f 735f6765 746e6f64 65005f5f x_n_s_getnode.__
+  0x00000590 7079785f 6e5f735f 696e7400 5f5f7079 pyx_n_s_int.__py
+  0x000005a0 785f6e5f 735f6865 78005f5f 7079785f x_n_s_hex.__pyx_
+  0x000005b0 6e5f735f 75707065 72005f5f 7079785f n_s_upper.__pyx_
+  0x000005c0 6e5f735f 7265706c 61636500 5f5f7079 n_s_replace.__py
+  0x000005d0 785f6d6f 64756c65 64656600 5f5f7079 x_moduledef.__py
+  0x000005e0 785f6b5f 005f5f70 79785f6b 5f555549 x_k_.__pyx_k_UUI
+  0x000005f0 44005f5f 7079785f 6b5f5f32 005f5f70 D.__pyx_k__2.__p
+  0x00000600 79785f6b 5f636c69 6e655f69 6e5f7472 yx_k_cline_in_tr
+  0x00000610 61636562 61636b00 5f5f7079 785f6b5f aceback.__pyx_k_
+  0x00000620 636c6f73 65005f5f 7079785f 6b5f6500 close.__pyx_k_e.
+  0x00000630 5f5f7079 785f6b5f 6765745f 64657669 __pyx_k_get_devi
+  0x00000640 63655f69 64005f5f 7079785f 6b5f6765 ce_id.__pyx_k_ge
+  0x00000650 746e6f64 65005f5f 7079785f 6b5f6865 tnode.__pyx_k_he
+  0x00000660 78005f5f 7079785f 6b5f6966 636f6e66 x.__pyx_k_ifconf
+  0x00000670 69675f6d 6c616e30 5f677265 705f6574 ig_mlan0_grep_et
+  0x00000680 6865725f 61776b5f 7072005f 5f707978 her_awk_pr.__pyx
+  0x00000690 5f6e5f73 5f696d70 6f727400 5f5f7079 _n_s_import.__py
+  0x000006a0 785f6b5f 696d706f 7274005f 5f707978 x_k_import.__pyx
+  0x000006b0 5f6b5f69 6e74005f 5f707978 5f6e5f73 _k_int.__pyx_n_s
+  0x000006c0 5f6a6f69 6e005f5f 7079785f 6b5f6a6f _join.__pyx_k_jo
+  0x000006d0 696e005f 5f707978 5f6b5f6d 6163005f in.__pyx_k_mac._
+  0x000006e0 5f707978 5f6b5f6d 61696e00 5f5f7079 _pyx_k_main.__py
+  0x000006f0 785f6b5f 6e616d65 005f5f70 79785f6b x_k_name.__pyx_k
+  0x00000700 5f6f7300 5f5f7079 785f6b5f 706f7065 _os.__pyx_k_pope
+  0x00000710 6e005f5f 7079785f 6b5f7079 74656c65 n.__pyx_k_pytele
+  0x00000720 72646163 5f757469 6c735f64 65766963 rdac_utils_devic
+  0x00000730 655f7574 696c7300 5f5f7079 785f6b5f e_utils.__pyx_k_
+  0x00000740 70797465 6c657264 61635f75 74696c73 pytelerdac_utils
+  0x00000750 5f646576 6963655f 7574696c 735f7079 _device_utils_py
+  0x00000760 005f5f70 79785f6b 5f72616e 6765005f .__pyx_k_range._
+  0x00000770 5f707978 5f6b5f72 65616400 5f5f7079 _pyx_k_read.__py
+  0x00000780 785f6b5f 7265706c 61636500 5f5f7079 x_k_replace.__py
+  0x00000790 785f6b5f 72657375 6c74005f 5f707978 x_k_result.__pyx
+  0x000007a0 5f6b5f73 706c6974 005f5f70 79785f6b _k_split.__pyx_k
+  0x000007b0 5f737472 6970005f 5f707978 5f6b5f74 _strip.__pyx_k_t
+  0x000007c0 65737400 5f5f7079 785f6b5f 75707065 est.__pyx_k_uppe
+  0x000007d0 72005f5f 7079785f 6b5f7575 6964005f r.__pyx_k_uuid._
+  0x000007e0 5f707978 5f6d6574 686f6473 005f5f70 _pyx_methods.__p
+  0x000007f0 79785f6d 6f64756c 65646566 5f736c6f yx_moduledef_slo
+  0x00000800 7473005f 5f707978 5f646f63 5f313070 ts.__pyx_doc_10p
+  0x00000810 7974656c 65726461 635f3575 74696c73 ytelerdac_5utils
+  0x00000820 5f313264 65766963 655f7574 696c735f _12device_utils_
+  0x00000830 6765745f 64657669 63655f69 64006372 get_device_id.cr
+  0x00000840 74737475 66662e63 00646572 65676973 tstuff.c.deregis
+  0x00000850 7465725f 746d5f63 6c6f6e65 73005f5f ter_tm_clones.__
+  0x00000860 646f5f67 6c6f6261 6c5f6474 6f72735f do_global_dtors_
+  0x00000870 61757800 636f6d70 6c657465 642e3830 aux.completed.80
+  0x00000880 3631005f 5f646f5f 676c6f62 616c5f64 61.__do_global_d
+  0x00000890 746f7273 5f617578 5f66696e 695f6172 tors_aux_fini_ar
+  0x000008a0 7261795f 656e7472 79006672 616d655f ray_entry.frame_
+  0x000008b0 64756d6d 79005f5f 6672616d 655f6475 dummy.__frame_du
+  0x000008c0 6d6d795f 696e6974 5f617272 61795f65 mmy_init_array_e
+  0x000008d0 6e747279 005f5f46 52414d45 5f454e44 ntry.__FRAME_END
+  0x000008e0 5f5f005f 66696e69 005f5f64 736f5f68 __._fini.__dso_h
+  0x000008f0 616e646c 65005f44 594e414d 4943005f andle._DYNAMIC._
+  0x00000900 5f474e55 5f45485f 4652414d 455f4844 _GNU_EH_FRAME_HD
+  0x00000910 52005f5f 544d435f 454e445f 5f005f47 R.__TMC_END__._G
+  0x00000920 4c4f4241 4c5f4f46 46534554 5f544142 LOBAL_OFFSET_TAB
+  0x00000930 4c455f00 5f696e69 74005079 556e6963 LE_._init.PyUnic
+  0x00000940 6f64655f 46726f6d 466f726d 61740050 ode_FromFormat.P
+  0x00000950 794c6973 745f4e65 77005079 4578635f yList_New.PyExc_
+  0x00000960 53797374 656d4572 726f7200 50794469 SystemError.PyDi
+  0x00000970 63745f53 65744974 656d5374 72696e67 ct_SetItemString
+  0x00000980 0050794d 6574686f 645f5479 7065005f .PyMethod_Type._
+  0x00000990 49544d5f 64657265 67697374 6572544d ITM_deregisterTM
+  0x000009a0 436c6f6e 65546162 6c650050 79466c6f CloneTable.PyFlo
+  0x000009b0 61745f54 79706500 5f507954 68726561 at_Type._PyThrea
+  0x000009c0 64537461 74655f55 6e636865 636b6564 dState_Unchecked
+  0x000009d0 47657400 50794d6f 64756c65 4465665f Get.PyModuleDef_
+  0x000009e0 496e6974 00507946 72616d65 5f4e6577 Init.PyFrame_New
+  0x000009f0 00507943 46756e63 74696f6e 5f4e6577 .PyCFunction_New
+  0x00000a00 45780050 794e756d 6265725f 41646400 Ex.PyNumber_Add.
+  0x00000a10 50794f62 6a656374 5f476574 41747472 PyObject_GetAttr
+  0x00000a20 53747269 6e670050 79556e69 636f6465 String.PyUnicode
+  0x00000a30 5f4a6f69 6e005079 496d706f 72745f41 _Join.PyImport_A
+  0x00000a40 64644d6f 64756c65 00507942 79746573 ddModule.PyBytes
+  0x00000a50 5f46726f 6d537472 696e6741 6e645369 _FromStringAndSi
+  0x00000a60 7a650050 794f626a 6563745f 53657441 ze.PyObject_SetA
+  0x00000a70 74747253 7472696e 67005079 4572725f ttrString.PyErr_
+  0x00000a80 5761726e 4578005f 50795f44 65616c6c WarnEx._Py_Deall
+  0x00000a90 6f630050 794d6f64 756c655f 4e65774f oc.PyModule_NewO
+  0x00000aa0 626a6563 74005079 436f6465 5f4e6577 bject.PyCode_New
+  0x00000ab0 00507949 6d706f72 745f4765 744d6f64 .PyImport_GetMod
+  0x00000ac0 756c6544 69637400 5f5f7374 61636b5f uleDict.__stack_
+  0x00000ad0 63686b5f 6661696c 40474c49 42435f32 chk_fail@GLIBC_2
+  0x00000ae0 2e340050 79457863 5f52756e 74696d65 .4.PyExc_Runtime
+  0x00000af0 4572726f 72005079 4572725f 53657453 Error.PyErr_SetS
+  0x00000b00 7472696e 67005079 4578635f 54797065 tring.PyExc_Type
+  0x00000b10 4572726f 72005079 496e7465 72707265 Error.PyInterpre
+  0x00000b20 74657253 74617465 5f476574 49440050 terState_GetID.P
+  0x00000b30 79457661 6c5f4576 616c4672 616d6545 yEval_EvalFrameE
+  0x00000b40 78005079 4d656d5f 5265616c 6c6f6300 x.PyMem_Realloc.
+  0x00000b50 50794572 725f4578 63657074 696f6e4d PyErr_ExceptionM
+  0x00000b60 61746368 65730050 794f535f 736e7072 atches.PyOS_snpr
+  0x00000b70 696e7466 00507954 72616365 4261636b intf.PyTraceBack
+  0x00000b80 5f486572 65005079 4f626a65 63745f4e _Here.PyObject_N
+  0x00000b90 6f740050 79466c6f 61745f46 726f6d44 ot.PyFloat_FromD
+  0x00000ba0 6f75626c 65005079 4c6f6e67 5f46726f ouble.PyLong_Fro
+  0x00000bb0 6d4c6f6e 67005079 496e6974 5f646576 mLong.PyInit_dev
+  0x00000bc0 6963655f 7574696c 73005079 4572725f ice_utils.PyErr_
+  0x00000bd0 436c6561 72005079 4c697374 5f417070 Clear.PyList_App
+  0x00000be0 656e6400 5f50795f 43686563 6b526563 end._Py_CheckRec
+  0x00000bf0 75727369 76654361 6c6c005f 50795f43 ursiveCall._Py_C
+  0x00000c00 6865636b 52656375 7273696f 6e4c696d heckRecursionLim
+  0x00000c10 6974005f 50795f46 616c7365 53747275 it._Py_FalseStru
+  0x00000c20 6374005f 5f676d6f 6e5f7374 6172745f ct.__gmon_start_
+  0x00000c30 5f005079 5475706c 655f4e65 77005079 _.PyTuple_New.Py
+  0x00000c40 54687265 61645374 6174655f 47657400 ThreadState_Get.
+  0x00000c50 50794f62 6a656374 5f536574 41747472 PyObject_SetAttr
+  0x00000c60 00507945 72725f4f 63637572 72656400 .PyErr_Occurred.
+  0x00000c70 5f507944 6963745f 47657449 74656d5f _PyDict_GetItem_
+  0x00000c80 4b6e6f77 6e486173 68005079 44696374 KnownHash.PyDict
+  0x00000c90 5f476574 4974656d 53747269 6e670050 _GetItemString.P
+  0x00000ca0 79457661 6c5f4576 616c436f 64654578 yEval_EvalCodeEx
+  0x00000cb0 0050794f 626a6563 745f5369 7a65005f .PyObject_Size._
+  0x00000cc0 50795f4e 6f6e6553 74727563 74005079 Py_NoneStruct.Py
+  0x00000cd0 496d706f 72745f49 6d706f72 744d6f64 Import_ImportMod
+  0x00000ce0 756c654c 6576656c 4f626a65 63740050 uleLevelObject.P
+  0x00000cf0 794f626a 6563745f 48617368 005f5079 yObject_Hash._Py
+  0x00000d00 5f547275 65537472 75637400 50794675 _TrueStruct.PyFu
+  0x00000d10 6e637469 6f6e5f54 79706500 50794469 nction_Type.PyDi
+  0x00000d20 63745f4e 65770050 794c6f6e 675f5479 ct_New.PyLong_Ty
+  0x00000d30 70650050 79467261 6d655f54 79706500 pe.PyFrame_Type.
+  0x00000d40 5f50794f 626a6563 745f4765 74446963 _PyObject_GetDic
+  0x00000d50 74507472 00507955 6e69636f 64655f46 tPtr.PyUnicode_F
+  0x00000d60 726f6d53 7472696e 67005079 556e6963 romString.PyUnic
+  0x00000d70 6f64655f 496e7465 726e4672 6f6d5374 ode_InternFromSt
+  0x00000d80 72696e67 00507945 78635f49 6d706f72 ring.PyExc_Impor
+  0x00000d90 74457272 6f720050 79446963 745f5365 tError.PyDict_Se
+  0x00000da0 74497465 6d005079 4578635f 41747472 tItem.PyExc_Attr
+  0x00000db0 69627574 65457272 6f720050 794f626a ibuteError.PyObj
+  0x00000dc0 6563745f 43616c6c 005f5f70 79785f6d ect_Call.__pyx_m
+  0x00000dd0 6f64756c 655f6973 5f6d6169 6e5f7079 odule_is_main_py
+  0x00000de0 74656c65 72646163 5f5f7574 696c735f telerdac__utils_
+  0x00000df0 5f646576 6963655f 7574696c 73005079 _device_utils.Py
+  0x00000e00 556e6963 6f64655f 4465636f 64650050 Unicode_Decode.P
+  0x00000e10 79457272 5f466f72 6d617400 5079536c yErr_Format.PySl
+  0x00000e20 6963655f 4e657700 50794578 635f4e61 ice_New.PyExc_Na
+  0x00000e30 6d654572 726f7200 5079556e 69636f64 meError.PyUnicod
+  0x00000e40 655f4672 6f6d5374 72696e67 416e6453 e_FromStringAndS
+  0x00000e50 697a6500 50794d6f 64756c65 5f476574 ize.PyModule_Get
+  0x00000e60 44696374 005f4954 4d5f7265 67697374 Dict._ITM_regist
+  0x00000e70 6572544d 436c6f6e 65546162 6c650050 erTMCloneTable.P
+  0x00000e80 794f626a 6563745f 47657441 74747200 yObject_GetAttr.
+  0x00000e90 50794346 756e6374 696f6e5f 54797065 PyCFunction_Type
+  0x00000ea0 0050794d 656d5f4d 616c6c6f 63005f5f .PyMem_Malloc.__
+  0x00000eb0 6378615f 66696e61 6c697a65 40474c49 cxa_finalize@GLI
+  0x00000ec0 42435f32 2e322e35 00507954 75706c65 BC_2.2.5.PyTuple
+  0x00000ed0 5f506163 6b005079 5f476574 56657273 _Pack.Py_GetVers
+  0x00000ee0 696f6e00                            ion.
```

## Comparing `pytelerdac-0.2.0.dist-info/METADATA` & `pytelerdac-0.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytelerdac
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python Package for tele rdac client
 Author: imason
 Author-email: moy7@chinatelecom.cn
 Keywords: pytelerdac
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `pytelerdac-0.2.0.dist-info/RECORD` & `pytelerdac-0.3.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pytelerdac/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytelerdac/rdac.cpython-38-x86_64-linux-gnu.so,sha256=jdIiVNRLVco2iJGKHTP9octRcTd920pik2bi1EkrI-8,114776
 pytelerdac/client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytelerdac/client/http_client.cpython-38-x86_64-linux-gnu.so,sha256=nkTFoomEmoE2qiCFCQZ9wkugWfnV3YrFYGSBP7p3MbM,91800
 pytelerdac/const/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytelerdac/const/public.cpython-38-x86_64-linux-gnu.so,sha256=nCeBaJx5cdbdFQxsuMMDM0MWQn2i3HqsEAAdUhvc-_k,28032
 pytelerdac/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pytelerdac/utils/device_utils.cpython-38-x86_64-linux-gnu.so,sha256=CkeP8IYi-IIqzk9TN91D-ixRg_thtUfvu7rhE0fQQj8,40008
+pytelerdac/utils/device_utils.cpython-38-x86_64-linux-gnu.so,sha256=uF3toB9rE2hGRbJMq3tlQmYbjgRethnUfnPZFcFKvUw,49824
 pytelerdac/utils/license_utils.cpython-38-x86_64-linux-gnu.so,sha256=h7yy2wKpN6JgQ9nu_lLxZLyt5wZsL1v57rftQYXLYG8,153112
-pytelerdac-0.2.0.dist-info/METADATA,sha256=Dm7N2xdrS4JYi8urXVsZ369PC6vzsQ-I1Kcgzxi5Ep4,531
-pytelerdac-0.2.0.dist-info/WHEEL,sha256=w1d_q2QQYYWFjc1BOr71GnX8BifSnUvEochN_fqB7tA,108
-pytelerdac-0.2.0.dist-info/top_level.txt,sha256=GGNlG_2NZi0eb98LT66rSRZgIW8h9OJfX-vBlOMuOZQ,11
-pytelerdac-0.2.0.dist-info/RECORD,,
+pytelerdac-0.3.0.dist-info/METADATA,sha256=gV9mecGnPBKRAz9ixKgA5S54fMb1n37ZoKTvZjxc4yE,531
+pytelerdac-0.3.0.dist-info/WHEEL,sha256=w1d_q2QQYYWFjc1BOr71GnX8BifSnUvEochN_fqB7tA,108
+pytelerdac-0.3.0.dist-info/top_level.txt,sha256=GGNlG_2NZi0eb98LT66rSRZgIW8h9OJfX-vBlOMuOZQ,11
+pytelerdac-0.3.0.dist-info/RECORD,,
```

