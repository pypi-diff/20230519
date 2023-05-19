# Comparing `tmp/character-encoding-utils-0.0.2.tar.gz` & `tmp/character-encoding-utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "character-encoding-utils-0.0.2.tar", last modified: Tue May 16 10:36:05 2023, max compression
+gzip compressed data, was "character-encoding-utils-0.0.3.tar", last modified: Fri May 19 13:00:43 2023, max compression
```

## Comparing `character-encoding-utils-0.0.2.tar` & `character-encoding-utils-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:36:05.112311 character-encoding-utils-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-16 10:36:05.112311 character-encoding-utils-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:36:05.112311 character-encoding-utils-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:36:05.108311 character-encoding-utils-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:36:05.108311 character-encoding-utils-0.0.2/src/character_encoding_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/src/character_encoding_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/src/character_encoding_utils/big5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/src/character_encoding_utils/gb2312.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/src/character_encoding_utils/ksx1001.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/src/character_encoding_utils/shiftjis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:36:05.108311 character-encoding-utils-0.0.2/src/character_encoding_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-16 10:36:05.000000 character-encoding-utils-0.0.2/src/character_encoding_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-16 10:36:05.000000 character-encoding-utils-0.0.2/src/character_encoding_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:36:05.000000 character-encoding-utils-0.0.2/src/character_encoding_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 10:36:05.000000 character-encoding-utils-0.0.2/src/character_encoding_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:36:05.112311 character-encoding-utils-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/tests/test_big5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/tests/test_gb2312.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/tests/test_ksx1001.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-16 10:35:50.000000 character-encoding-utils-0.0.2/tests/test_shiftjis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:00:43.790450 character-encoding-utils-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-19 13:00:43.790450 character-encoding-utils-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 13:00:43.790450 character-encoding-utils-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:00:43.790450 character-encoding-utils-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:00:43.790450 character-encoding-utils-0.0.3/src/character_encoding_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/src/character_encoding_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/src/character_encoding_utils/big5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/src/character_encoding_utils/gb2312.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/src/character_encoding_utils/ksx1001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/src/character_encoding_utils/shiftjis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:00:43.790450 character-encoding-utils-0.0.3/src/character_encoding_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-19 13:00:43.000000 character-encoding-utils-0.0.3/src/character_encoding_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-19 13:00:43.000000 character-encoding-utils-0.0.3/src/character_encoding_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:00:43.000000 character-encoding-utils-0.0.3/src/character_encoding_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 13:00:43.000000 character-encoding-utils-0.0.3/src/character_encoding_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:00:43.790450 character-encoding-utils-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/tests/test_big5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/tests/test_gb2312.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/tests/test_ksx1001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/tests/test_shiftjis.py
```

### Comparing `character-encoding-utils-0.0.2/LICENSE` & `character-encoding-utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.2/PKG-INFO` & `character-encoding-utils-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: character-encoding-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Some character encoding utils.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/character-encoding-utils
 Project-URL: source, https://github.com/TakWolf/character-encoding-utils
 Project-URL: issues, https://github.com/TakWolf/character-encoding-utils/issues
-Keywords: encoding
+Keywords: encoding,gb2312,big5,shift-jis,ksx1001
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -56,15 +56,15 @@
 ```
 
 ### Shift-JIS
 
 ```python
 from character_encoding_utils import shiftjis
 
-bs =  shiftjis.encode('abc日本')
+bs = shiftjis.encode('abc日本')
 assert shiftjis.decode(bs) == 'abc日本'
 ```
 
 ### KS-X-1001
 
 ```python
 from character_encoding_utils import ksx1001
```

### Comparing `character-encoding-utils-0.0.2/README.md` & `character-encoding-utils-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ```
 
 ### Shift-JIS
 
 ```python
 from character_encoding_utils import shiftjis
 
-bs =  shiftjis.encode('abc日本')
+bs = shiftjis.encode('abc日本')
 assert shiftjis.decode(bs) == 'abc日本'
 ```
 
 ### KS-X-1001
 
 ```python
 from character_encoding_utils import ksx1001
```

### Comparing `character-encoding-utils-0.0.2/pyproject.toml` & `character-encoding-utils-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "character-encoding-utils"
-version = "0.0.2"
+version = "0.0.3"
 description = "Some character encoding utils."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
 maintainers = [
     { name = "TakWolf" },
 ]
-keywords = ["encoding"]
+keywords = ["encoding", "gb2312", "big5", "shift-jis", "ksx1001"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `character-encoding-utils-0.0.2/src/character_encoding_utils/big5.py` & `character-encoding-utils-0.0.3/src/character_encoding_utils/big5.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,90 +12,91 @@
 
 
 class Big5DecodeError(Big5Exception):
     def __init__(self, obj: bytes, position: int, reason: str):
         self.object = obj
         self.position = position
         self.reason = reason
-        super().__init__(f"'big5' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
+        if len(obj) <= 1:
+            super().__init__(f"'big5' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
+        else:
+            super().__init__(f"'big5' codec can't decode bytes in position {position}-{position + len(obj) - 1}: {reason}")
 
 
 def encode(cs: str) -> bytes:
     bs = bytearray()
     for position, c in enumerate(cs):
-        # 此处默认编码器映射错误
         if c == '〸':  # 0x3038
             bs.extend(b'\xa2\xcc')
-            continue
         elif c == '〹':  # 0x3039
             bs.extend(b'\xa2\xcd')
-            continue
         elif c == '〺':  # 0x303A
             bs.extend(b'\xa2\xce')
-            continue
         elif c == '十':  # 0x5341
             bs.extend(b'\xa4\x51')
-            continue
         elif c == '卄':  # 0x5344
             # Big5 不包含汉字的 '卄'
             raise Big5EncodeError(c, position, 'illegal multibyte sequence')
         elif c == '卅':  # 0x5345
             bs.extend(b'\xa4\xca')
-            continue
-
-        try:
-            bs.extend(c.encode('big5'))
-        except UnicodeEncodeError as e:
-            raise Big5EncodeError(c, position, e.reason) from e
+        elif c == '／':  # 0xFF0F
+            bs.extend(b'\xa1\xfe')
+        elif c == '＼':  # 0xFF3C
+            bs.extend(b'\xa2\x40')
+        elif c == '∕':  # 0x2215
+            bs.extend(b'\xa2\x41')
+        elif c == '﹨':  # 0xFE68
+            bs.extend(b'\xa2\x42')
+        else:
+            try:
+                bs.extend(c.encode('big5'))
+            except UnicodeEncodeError as e:
+                raise Big5EncodeError(c, position, e.reason) from e
     return bytes(bs)
 
 
-def decode(bs: bytes) -> str:
+def decode(bs: bytes | bytearray) -> str:
     cs = []
-    bs = iter(bs)
-    position = -1
+    cursor = 0
+    passed = 0
     while True:
-        try:
-            b1 = next(bs)
-            position += 1
-        except StopIteration:
+        if cursor >= len(bs):
             break
-        b2 = None
-        if b1 > 0x7F:
-            try:
-                b2 = next(bs)
-                position += 1
-            except StopIteration:
-                pass
-        if b2 is None:
-            bc = bytes([b1])
-        else:
-            bc = bytes([b1, b2])
+        bc = bytearray([bs[cursor]])
+        cursor += 1
+
+        if bc[0] > 0x7F:
+            if cursor < len(bs):
+                bc.append(bs[cursor])
+                cursor += 1
 
-        # 此处默认编码器映射错误
         if bc == b'\xa2\xcc':
             cs.append('〸')  # 0x3038
-            continue
         elif bc == b'\xa2\xcd':
             cs.append('〹')  # 0x3039
-            continue
         elif bc == b'\xa2\xce':
             cs.append('〺')  # 0x303A
-            continue
         elif bc == b'\xa4\x51':
             cs.append('十')  # 0x5341
-            continue
         elif bc == b'\xa4\xca':
             cs.append('卅')  # 0x5345
-            continue
-
-        try:
-            cs.append(bc.decode('big5'))
-        except UnicodeDecodeError as e:
-            raise Big5DecodeError(bc, position, e.reason) from e
+        elif bc == b'\xa1\xfe':
+            cs.append('／')  # 0xFF0F
+        elif bc == b'\xa2\x40':
+            cs.append('＼')  # 0xFF3C
+        elif bc == b'\xa2\x41':
+            cs.append('∕')  # 0x2215
+        elif bc == b'\xa2\x42':
+            cs.append('﹨')  # 0xFE68
+        else:
+            try:
+                cs.append(bc.decode('big5'))
+            except UnicodeDecodeError as e:
+                raise Big5DecodeError(bc, passed, e.reason) from e
+        passed += len(bc)
     return ''.join(cs)
 
 
 def query_code(c: str) -> int:
     if len(c) != 1:
         raise Big5Exception('must be one character')
     try:
```

### Comparing `character-encoding-utils-0.0.2/src/character_encoding_utils/gb2312.py` & `character-encoding-utils-0.0.3/src/character_encoding_utils/gb2312.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,52 +15,50 @@
 
 
 class GB2312DecodeError(GB2312Exception):
     def __init__(self, obj: bytes, position: int, reason: str):
         self.object = obj
         self.position = position
         self.reason = reason
-        super().__init__(f"'gb2312' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
+        if len(obj) <= 1:
+            super().__init__(f"'gb2312' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
+        else:
+            super().__init__(f"'gb2312' codec can't decode bytes in position {position}-{position + len(obj) - 1}: {reason}")
 
 
 def encode(cs: str) -> bytes:
     bs = bytearray()
     for position, c in enumerate(cs):
         try:
             bs.extend(c.encode('gb2312'))
         except UnicodeEncodeError as e:
             raise GB2312EncodeError(c, position, e.reason) from e
     return bytes(bs)
 
 
-def decode(bs: bytes) -> str:
+def decode(bs: bytes | bytearray) -> str:
     cs = []
-    bs = iter(bs)
-    position = -1
+    cursor = 0
+    passed = 0
     while True:
-        try:
-            b1 = next(bs)
-            position += 1
-        except StopIteration:
+        if cursor >= len(bs):
             break
-        b2 = None
-        if b1 > 0x7F:
-            try:
-                b2 = next(bs)
-                position += 1
-            except StopIteration:
-                pass
-        if b2 is None:
-            bc = bytes([b1])
-        else:
-            bc = bytes([b1, b2])
+        bc = bytearray([bs[cursor]])
+        cursor += 1
+
+        if bc[0] > 0x7F:
+            if cursor < len(bs):
+                bc.append(bs[cursor])
+                cursor += 1
+
         try:
             cs.append(bc.decode('gb2312'))
         except UnicodeDecodeError as e:
-            raise GB2312DecodeError(bc, position, e.reason) from e
+            raise GB2312DecodeError(bc, passed, e.reason) from e
+        passed += len(bc)
     return ''.join(cs)
 
 
 def query_coord(c: str) -> tuple[int, int]:
     if len(c) != 1:
         raise GB2312Exception('must be one character')
     try:
```

### Comparing `character-encoding-utils-0.0.2/src/character_encoding_utils/shiftjis.py` & `character-encoding-utils-0.0.3/src/character_encoding_utils/shiftjis.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,65 +14,60 @@
 
 
 class ShiftJISDecodeError(ShiftJISException):
     def __init__(self, obj: bytes, position: int, reason: str):
         self.object = obj
         self.position = position
         self.reason = reason
-        super().__init__(f"'shift-jis' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
+        if len(obj) <= 1:
+            super().__init__(f"'shift-jis' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
+        else:
+            super().__init__(f"'shift-jis' codec can't decode bytes in position {position}-{position + len(obj) - 1}: {reason}")
 
 
 def encode(cs: str) -> bytes:
     bs = bytearray()
     for position, c in enumerate(cs):
         if c == '\\':
             raise ShiftJISEncodeError(c, position, f"in 'shift-jis' the character '\\' is replaced with '¥'")
         elif c == '~':
             raise ShiftJISEncodeError(c, position, f"in 'shift-jis' the character '~' is replaced with '‾'")
-
-        try:
-            bs.extend(c.encode('shift-jis'))
-        except UnicodeEncodeError as e:
-            raise ShiftJISEncodeError(c, position, e.reason) from e
+        else:
+            try:
+                bs.extend(c.encode('shift-jis'))
+            except UnicodeEncodeError as e:
+                raise ShiftJISEncodeError(c, position, e.reason) from e
     return bytes(bs)
 
 
-def decode(bs: bytes) -> str:
+def decode(bs: bytes | bytearray) -> str:
     cs = []
-    bs = iter(bs)
-    position = -1
+    cursor = 0
+    passed = 0
     while True:
-        try:
-            b1 = next(bs)
-            position += 1
-        except StopIteration:
+        if cursor >= len(bs):
             break
-        b2 = None
-        if not (b1 <= 0x7F or 0xA1 <= b1 <= 0xDF):
-            try:
-                b2 = next(bs)
-                position += 1
-            except StopIteration:
-                pass
-        if b2 is None:
-            bc = bytes([b1])
-        else:
-            bc = bytes([b1, b2])
+        bc = bytearray([bs[cursor]])
+        cursor += 1
+
+        if not (bc[0] <= 0x7F or 0xA1 <= bc[0] <= 0xDF):
+            if cursor < len(bs):
+                bc.append(bs[cursor])
+                cursor += 1
 
         if bc == b'\\':
             cs.append('¥')
-            continue
         elif bc == b'~':
             cs.append('‾')
-            continue
-
-        try:
-            cs.append(bc.decode('shift-jis'))
-        except UnicodeDecodeError as e:
-            raise ShiftJISDecodeError(bc, position, e.reason) from e
+        else:
+            try:
+                cs.append(bc.decode('shift-jis'))
+            except UnicodeDecodeError as e:
+                raise ShiftJISDecodeError(bc, passed, e.reason) from e
+        passed += len(bc)
     return ''.join(cs)
 
 
 def get_categories() -> list[str]:
     return [
         'single-byte-ascii-control',
         'single-byte-ascii-printable',
```

### Comparing `character-encoding-utils-0.0.2/src/character_encoding_utils.egg-info/PKG-INFO` & `character-encoding-utils-0.0.3/src/character_encoding_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: character-encoding-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Some character encoding utils.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/character-encoding-utils
 Project-URL: source, https://github.com/TakWolf/character-encoding-utils
 Project-URL: issues, https://github.com/TakWolf/character-encoding-utils/issues
-Keywords: encoding
+Keywords: encoding,gb2312,big5,shift-jis,ksx1001
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -56,15 +56,15 @@
 ```
 
 ### Shift-JIS
 
 ```python
 from character_encoding_utils import shiftjis
 
-bs =  shiftjis.encode('abc日本')
+bs = shiftjis.encode('abc日本')
 assert shiftjis.decode(bs) == 'abc日本'
 ```
 
 ### KS-X-1001
 
 ```python
 from character_encoding_utils import ksx1001
```

### Comparing `character-encoding-utils-0.0.2/src/character_encoding_utils.egg-info/SOURCES.txt` & `character-encoding-utils-0.0.3/src/character_encoding_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.2/tests/test_big5.py` & `character-encoding-utils-0.0.3/tests/test_big5.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,14 +41,30 @@
     with pytest.raises(Big5EncodeError):
         big5.encode(c)
 
     c = '卅'
     assert ord(c) == 0x5345
     assert big5.decode(big5.encode(c)) == c
 
+    c = '／'
+    assert ord(c) == 0xFF0F
+    assert big5.decode(big5.encode(c)) == c
+
+    c = '＼'
+    assert ord(c) == 0xFF3C
+    assert big5.decode(big5.encode(c)) == c
+
+    c = '∕'
+    assert ord(c) == 0x2215
+    assert big5.decode(big5.encode(c)) == c
+
+    c = '﹨'
+    assert ord(c) == 0xFE68
+    assert big5.decode(big5.encode(c)) == c
+
 
 def test_query_code():
     assert big5.query_code('　') == 0xA140
     assert big5.query_code('¢') == 0xA246
     assert big5.query_code('一') == 0xA440
     assert big5.query_code('訐') == 0xB050
     assert big5.query_code('乂') == 0xC940
@@ -125,7 +141,33 @@
 
 
 def test_count():
     assert big5.get_other_count() == 408
     assert big5.get_level_1_count() == 5401
     assert big5.get_level_2_count() == 7652
     assert big5.get_count() == 13461
+
+
+def test_unicode():
+    alphabet_other = []
+    alphabet_level_1 = []
+    alphabet_level_2 = []
+    alphabet = []
+
+    for code_point in range(0, 0x10FFFF + 1):
+        c = chr(code_point)
+        category = big5.query_category(c)
+
+        if category == 'other':
+            alphabet_other.append(c)
+        elif category == 'level-1':
+            alphabet_level_1.append(c)
+        elif category == 'level-2':
+            alphabet_level_2.append(c)
+
+        if category is not None:
+            alphabet.append(c)
+
+    assert len(alphabet_other) == big5.get_other_count()
+    assert len(alphabet_level_1) == big5.get_level_1_count()
+    assert len(alphabet_level_2) == big5.get_level_2_count()
+    assert len(alphabet) == big5.get_count()
```

### Comparing `character-encoding-utils-0.0.2/tests/test_shiftjis.py` & `character-encoding-utils-0.0.3/tests/test_shiftjis.py`

 * *Files 24% similar despite different names*

```diff
@@ -90,7 +90,41 @@
 def test_count():
     assert shiftjis.get_single_byte_ascii_control_count() == 33
     assert shiftjis.get_single_byte_ascii_printable_count() == 95
     assert shiftjis.get_single_byte_half_width_katakana_count() == 63
     assert shiftjis.get_double_byte_other_count() == 524
     assert shiftjis.get_double_byte_kanji_count() == 6355
     assert shiftjis.get_count() == 7070
+
+
+def test_unicode():
+    alphabet_single_byte_ascii_control = []
+    alphabet_single_byte_ascii_printable = []
+    alphabet_single_byte_half_width_katakana = []
+    alphabet_double_byte_other = []
+    alphabet_double_byte_kanji = []
+    alphabet = []
+
+    for code_point in range(0, 0x10FFFF + 1):
+        c = chr(code_point)
+        category = shiftjis.query_category(c)
+
+        if category == 'single-byte-ascii-control':
+            alphabet_single_byte_ascii_control.append(c)
+        elif category == 'single-byte-ascii-printable':
+            alphabet_single_byte_ascii_printable.append(c)
+        elif category == 'single-byte-half-width-katakana':
+            alphabet_single_byte_half_width_katakana.append(c)
+        elif category == 'double-byte-other':
+            alphabet_double_byte_other.append(c)
+        elif category == 'double-byte-kanji':
+            alphabet_double_byte_kanji.append(c)
+
+        if category is not None:
+            alphabet.append(c)
+
+    assert len(alphabet_single_byte_ascii_control) == shiftjis.get_single_byte_ascii_control_count()
+    assert len(alphabet_single_byte_ascii_printable) == shiftjis.get_single_byte_ascii_printable_count()
+    assert len(alphabet_single_byte_half_width_katakana) == shiftjis.get_single_byte_half_width_katakana_count()
+    assert len(alphabet_double_byte_other) == shiftjis.get_double_byte_other_count()
+    assert len(alphabet_double_byte_kanji) == shiftjis.get_double_byte_kanji_count()
+    assert len(alphabet) == shiftjis.get_count()
```

