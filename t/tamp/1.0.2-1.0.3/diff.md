# Comparing `tmp/tamp-1.0.2.tar.gz` & `tmp/tamp-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamp-1.0.2.tar", max compression
+gzip compressed data, was "tamp-1.0.3.tar", max compression
```

## Comparing `tamp-1.0.2.tar` & `tamp-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-04-29 16:23:57.808892 tamp-1.0.2/LICENSE
--rw-r--r--   0        0        0    14325 2023-04-29 16:23:57.808892 tamp-1.0.2/README.rst
--rw-r--r--   0        0        0     4891 2023-04-29 16:24:20.810662 tamp-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2497 2023-04-29 16:24:20.810662 tamp-1.0.2/tamp/__init__.py
--rw-r--r--   0        0        0     1619 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/__init__.pyi
--rw-r--r--   0        0        0       57 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/__main__.py
--rw-r--r--   0        0        0        0 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/cli/__init__.py
--rw-r--r--   0        0        0     2665 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/cli/main.py
--rw-r--r--   0        0        0     8237 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/compressor.py
--rw-r--r--   0        0        0     7136 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/compressor_viper.py
--rw-r--r--   0        0        0     6530 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/decompressor.py
--rw-r--r--   0        0        0     9951 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/decompressor_viper.py
--rw-r--r--   0        0        0        0 2023-04-29 16:23:57.812893 tamp-1.0.2/tamp/py.typed
--rw-r--r--   0        0        0    14944 1970-01-01 00:00:00.000000 tamp-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-19 18:43:33.846204 tamp-1.0.3/LICENSE
+-rw-r--r--   0        0        0    14800 2023-05-19 18:43:33.846204 tamp-1.0.3/README.rst
+-rw-r--r--   0        0        0     4891 2023-05-19 18:43:54.087338 tamp-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2497 2023-05-19 18:43:54.091338 tamp-1.0.3/tamp/__init__.py
+-rw-r--r--   0        0        0     1619 2023-05-19 18:43:33.850204 tamp-1.0.3/tamp/__init__.pyi
+-rw-r--r--   0        0        0       57 2023-05-19 18:43:33.850204 tamp-1.0.3/tamp/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:43:33.850204 tamp-1.0.3/tamp/cli/__init__.py
+-rw-r--r--   0        0        0     2665 2023-05-19 18:43:33.850204 tamp-1.0.3/tamp/cli/main.py
+-rw-r--r--   0        0        0     8237 2023-05-19 18:43:33.850204 tamp-1.0.3/tamp/compressor.py
+-rw-r--r--   0        0        0     7136 2023-05-19 18:43:33.850204 tamp-1.0.3/tamp/compressor_viper.py
+-rw-r--r--   0        0        0     6530 2023-05-19 18:43:33.850204 tamp-1.0.3/tamp/decompressor.py
+-rw-r--r--   0        0        0     9275 2023-05-19 18:43:33.850204 tamp-1.0.3/tamp/decompressor_viper.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:43:33.850204 tamp-1.0.3/tamp/py.typed
+-rw-r--r--   0        0        0    15419 1970-01-01 00:00:00.000000 tamp-1.0.3/PKG-INFO
```

### Comparing `tamp-1.0.2/LICENSE` & `tamp-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tamp-1.0.2/README.rst` & `tamp-1.0.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,22 @@
 2. ``tamp/decompressor_viper.py`` - Required for on-device decompression.
 
 3. ``tamp/compressor_viper.py`` - Required for on-device compression.
 
 For example, if on-device decompression isn't used, then do not include ``decompressor_viper.py``.
 If manually installing, just copy these files to your microcontroller's ``/lib/tamp`` folder.
 
+If using `mip`_, tamp can be installed by specifying the appropriate ``package-*.json`` file.
+
+.. code-block:: bash
+
+   mip install github:brianpugh/tamp  # Defaults to package.json: Compressor & Decompressor
+   mip install github:brianpugh/tamp/package-compressor.json  # Compressor only
+   mip install github:brianpugh/tamp/package-decompressor.json  # Decompressor only
+
 If using `Belay`_, tamp can be installed by adding the following to ``pyproject.toml``.
 
 .. code-block:: toml
 
    [tool.belay.dependencies]
    tamp = [
       "https://github.com/BrianPugh/tamp/blob/main/tamp/__init__.py",
@@ -269,7 +277,8 @@
 .. |PyPi| image:: https://img.shields.io/pypi/v/tamp.svg
         :target: https://pypi.python.org/pypi/tamp
 .. _Belay: https://github.com/BrianPugh/belay
 .. _zlib:  https://docs.python.org/3/library/zlib.html
 .. _heatshrink: https://github.com/atomicobject/heatshrink
 .. _Silesia Corpus: https://sun.aei.polsl.pl//~sdeor/index.php?page=silesia
 .. _Enwik8: https://mattmahoney.net/dc/textdata.html
+.. _mip: https://docs.micropython.org/en/latest/reference/packages.html#installing-packages-with-mip
```

### Comparing `tamp-1.0.2/pyproject.toml` & `tamp-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "semver"
 
 [tool.poetry]
 name = "tamp"
-version = "1.0.2"  # Do not change, let poetry-dynamic-versioning handle it.
+version = "1.0.3"  # Do not change, let poetry-dynamic-versioning handle it.
 homepage = "https://github.com/BrianPugh/tamp"
 repository = "https://github.com/BrianPugh/tamp"
 license = "Apache-2.0"
 description = ""
 authors = ["Brian Pugh"]
 readme = "README.rst"
 packages = [{include = "tamp"}]
```

### Comparing `tamp-1.0.2/tamp/__init__.py` & `tamp-1.0.3/tamp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Don't manually change, let poetry-dynamic-versioning-plugin handle it.
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 
 class ExcessBitsError(Exception):
     """Provided data has more bits than expected ``literal`` bits."""
 
 
 def bit_size(value):
```

### Comparing `tamp-1.0.2/tamp/__init__.pyi` & `tamp-1.0.3/tamp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tamp-1.0.2/tamp/cli/main.py` & `tamp-1.0.3/tamp/cli/main.py`

 * *Files identical despite different names*

### Comparing `tamp-1.0.2/tamp/compressor.py` & `tamp-1.0.3/tamp/compressor.py`

 * *Files identical despite different names*

### Comparing `tamp-1.0.2/tamp/compressor_viper.py` & `tamp-1.0.3/tamp/compressor_viper.py`

 * *Files identical despite different names*

### Comparing `tamp-1.0.2/tamp/decompressor.py` & `tamp-1.0.3/tamp/decompressor.py`

 * *Files identical despite different names*

### Comparing `tamp-1.0.2/tamp/decompressor_viper.py` & `tamp-1.0.3/tamp/decompressor_viper.py`

 * *Files 10% similar despite different names*

```diff
@@ -104,74 +104,67 @@
                     w_buf[w_pos] = c
                 else:
                     # Read and decode Huffman
                     # always read; we'll need the bits regardless
                     f_buf |= int(f.read(1)[0]) << (22 - f_pos)
                     f_pos += 8
 
-                    proposed_code = f_buf >> 29
-                    f_buf = (f_buf << 1) & full_mask
-                    f_pos -= 1
-                    if proposed_code:  # 0b1
-                        proposed_code = (proposed_code << 1) | (f_buf >> 29)
-                        f_buf = (f_buf << 1) & full_mask
-                        f_pos -= 1
-                        if proposed_code == 0b11:
+                    if f_buf >> 29:
+                        if (f_buf >> 28) == 0b11:
                             match_size = 1
+                            delta = 2
                         else:
-                            proposed_code = (proposed_code << 2) | (f_buf >> 28)
-                            f_buf = (f_buf << 2) & full_mask
-                            f_pos -= 2
+                            proposed_code = f_buf >> 26
+                            delta = 4
                             if proposed_code == 0b1000:
                                 match_size = 2
                             elif proposed_code == 0b1011:
                                 match_size = 3
                             else:
-                                proposed_code = (proposed_code << 1) | (f_buf >> 29)
-                                f_buf = (f_buf << 1) & full_mask
-                                f_pos -= 1
-                                if proposed_code == 0b10100:
+                                if (f_buf >> 25) == 0b10100:
                                     match_size = 4
+                                    delta = 5
                                 else:
-                                    proposed_code = (proposed_code << 1) | (f_buf >> 29)
-                                    f_buf = (f_buf << 1) & full_mask
-                                    f_pos -= 1
+                                    proposed_code = f_buf >> 24
+                                    delta = 6
                                     if proposed_code == 0b100100:
                                         match_size = 5
                                     elif proposed_code == 0b100110:
                                         match_size = 6
                                     elif proposed_code == 0b101011:
                                         match_size = 7
                                     elif proposed_code == 0b100111:
                                         match_size = 13
                                     else:
-                                        proposed_code = (proposed_code << 1) | (f_buf >> 29)
-                                        f_buf = (f_buf << 1) & full_mask
-                                        f_pos -= 1
+                                        proposed_code = f_buf >> 23
+                                        delta = 7
                                         if proposed_code == 0b1001011:
                                             match_size = 8
                                         elif proposed_code == 0b1010100:
                                             match_size = 9
                                         else:
-                                            proposed_code = (proposed_code << 1) | (f_buf >> 29)
-                                            f_buf = (f_buf << 1) & full_mask
-                                            f_pos -= 1
+                                            proposed_code = f_buf >> 22
+                                            delta = 8
                                             if proposed_code == 0b10010100:
                                                 match_size = 10
                                             elif proposed_code == 0b10010101:
                                                 match_size = 11
                                             elif proposed_code == 0b10101010:
                                                 match_size = 12
                                             elif proposed_code == 0b10101011:
                                                 f_pos = f_buf = 0  # FLUSH
                                                 continue
                                             else:
                                                 break  # no valid code detected
                     else:  # 0b0
                         match_size = 0
+                        delta = 1
+
+                    f_buf = (f_buf << delta) & full_mask
+                    f_pos -= delta
 
                     match_size += min_pattern_size
                     while f_pos < w_bits:
                         f_buf |= int(f.read(1)[0]) << (22 - f_pos)
                         f_pos += 8
 
                     index = f_buf >> (30 - w_bits)
```

### Comparing `tamp-1.0.2/PKG-INFO` & `tamp-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tamp
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Home-page: https://github.com/BrianPugh/tamp
 License: Apache-2.0
 Author: Brian Pugh
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -68,14 +68,22 @@
 2. ``tamp/decompressor_viper.py`` - Required for on-device decompression.
 
 3. ``tamp/compressor_viper.py`` - Required for on-device compression.
 
 For example, if on-device decompression isn't used, then do not include ``decompressor_viper.py``.
 If manually installing, just copy these files to your microcontroller's ``/lib/tamp`` folder.
 
+If using `mip`_, tamp can be installed by specifying the appropriate ``package-*.json`` file.
+
+.. code-block:: bash
+
+   mip install github:brianpugh/tamp  # Defaults to package.json: Compressor & Decompressor
+   mip install github:brianpugh/tamp/package-compressor.json  # Compressor only
+   mip install github:brianpugh/tamp/package-decompressor.json  # Decompressor only
+
 If using `Belay`_, tamp can be installed by adding the following to ``pyproject.toml``.
 
 .. code-block:: toml
 
    [tool.belay.dependencies]
    tamp = [
       "https://github.com/BrianPugh/tamp/blob/main/tamp/__init__.py",
@@ -287,8 +295,9 @@
 .. |PyPi| image:: https://img.shields.io/pypi/v/tamp.svg
         :target: https://pypi.python.org/pypi/tamp
 .. _Belay: https://github.com/BrianPugh/belay
 .. _zlib:  https://docs.python.org/3/library/zlib.html
 .. _heatshrink: https://github.com/atomicobject/heatshrink
 .. _Silesia Corpus: https://sun.aei.polsl.pl//~sdeor/index.php?page=silesia
 .. _Enwik8: https://mattmahoney.net/dc/textdata.html
+.. _mip: https://docs.micropython.org/en/latest/reference/packages.html#installing-packages-with-mip
```

