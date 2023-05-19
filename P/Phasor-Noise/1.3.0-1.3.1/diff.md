# Comparing `tmp/Phasor Noise-1.3.0.tar.gz` & `tmp/Phasor Noise-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Phasor Noise-1.3.0.tar", last modified: Thu May 18 19:41:37 2023, max compression
+gzip compressed data, was "Phasor Noise-1.3.1.tar", last modified: Fri May 19 19:59:19 2023, max compression
```

## Comparing `Phasor Noise-1.3.0.tar` & `Phasor Noise-1.3.1.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.659980 Phasor Noise-1.3.0/
--rw-rw-rw-   0        0        0      284 2023-05-18 19:41:37.000000 Phasor Noise-1.3.0/AUTHORS
--rw-rw-rw-   0        0        0    35869 2023-05-16 20:15:41.000000 Phasor Noise-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      157 2023-05-18 19:39:39.000000 Phasor Noise-1.3.0/Makefile
--rw-rw-rw-   0        0        0     1119 2023-05-18 19:41:37.659980 Phasor Noise-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-05-18 19:41:02.000000 Phasor Noise-1.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.611051 Phasor Noise-1.3.0/docs/
--rw-rw-rw-   0        0        0      603 2023-05-17 18:17:17.000000 Phasor Noise-1.3.0/docs/Makefile
--rw-rw-rw-   0        0        0        0 2023-05-17 13:34:47.000000 Phasor Noise-1.3.0/docs/README.rst
--rwxrwxrwx   0        0        0      827 2023-05-17 18:16:47.000000 Phasor Noise-1.3.0/docs/make.bat
--rw-rw-rw-   0        0        0       24 2023-05-17 18:51:28.000000 Phasor Noise-1.3.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.626747 Phasor Noise-1.3.0/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.626747 Phasor Noise-1.3.0/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.626747 Phasor Noise-1.3.0/docs/source/api/GUI/
--rw-rw-rw-   0        0        0      131 2023-05-17 20:04:06.000000 Phasor Noise-1.3.0/docs/source/api/GUI/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.626747 Phasor Noise-1.3.0/docs/source/api/analysis/
--rw-rw-rw-   0        0        0      175 2023-05-17 20:03:35.000000 Phasor Noise-1.3.0/docs/source/api/analysis/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.626747 Phasor Noise-1.3.0/docs/source/api/generator/
--rw-rw-rw-   0        0        0      203 2023-05-17 20:03:35.000000 Phasor Noise-1.3.0/docs/source/api/generator/index.rst
--rw-rw-rw-   0        0        0      248 2023-05-17 20:58:47.000000 Phasor Noise-1.3.0/docs/source/api/index.rst
--rw-rw-rw-   0        0        0     9189 2023-05-18 16:10:27.000000 Phasor Noise-1.3.0/docs/source/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.626747 Phasor Noise-1.3.0/docs/source/getting_started/
--rw-rw-rw-   0        0        0      196 2023-05-17 18:55:41.000000 Phasor Noise-1.3.0/docs/source/getting_started/index.rst
--rw-rw-rw-   0        0        0      193 2023-05-17 20:58:03.000000 Phasor Noise-1.3.0/docs/source/getting_started/installation.rst
--rw-rw-rw-   0        0        0      668 2023-05-18 15:29:52.000000 Phasor Noise-1.3.0/docs/source/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.626747 Phasor Noise-1.3.0/docs/source/user_guide/
--rw-rw-rw-   0        0        0       99 2023-05-17 14:58:13.000000 Phasor Noise-1.3.0/docs/source/user_guide/index.rst
--rw-rw-rw-   0        0        0       89 2023-05-17 19:39:21.000000 Phasor Noise-1.3.0/requirements.txt
--rw-rw-rw-   0        0        0      652 2023-05-18 19:41:37.659980 Phasor Noise-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      181 2023-05-17 18:14:41.000000 Phasor Noise-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.595433 Phasor Noise-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.659980 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/
--rw-rw-rw-   0        0        0     1119 2023-05-18 19:41:37.000000 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1115 2023-05-18 19:41:37.000000 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 19:41:37.000000 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 21:01:55.000000 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-05-18 19:41:37.000000 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/pbr.json
--rw-rw-rw-   0        0        0       86 2023-05-18 19:41:37.000000 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-18 19:41:37.000000 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.642369 Phasor Noise-1.3.0/src/phasor_noise/
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.642369 Phasor Noise-1.3.0/src/phasor_noise/GUI/
--rw-rw-rw-   0        0        0    22725 2023-05-18 16:04:17.000000 Phasor Noise-1.3.0/src/phasor_noise/GUI/__init__.py
--rw-rw-rw-   0        0        0     1436 2023-05-18 16:04:17.000000 Phasor Noise-1.3.0/src/phasor_noise/GUI/menu.py
--rw-rw-rw-   0        0        0      535 2023-05-18 16:04:17.000000 Phasor Noise-1.3.0/src/phasor_noise/GUI/platform_specific.py
--rw-rw-rw-   0        0        0      546 2023-05-18 16:04:17.000000 Phasor Noise-1.3.0/src/phasor_noise/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.642369 Phasor Noise-1.3.0/src/phasor_noise/analysis/
--rw-rw-rw-   0        0        0      777 2023-05-18 15:41:41.000000 Phasor Noise-1.3.0/src/phasor_noise/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.642369 Phasor Noise-1.3.0/src/phasor_noise/generator/
--rw-rw-rw-   0        0        0     5325 2023-05-18 15:37:46.000000 Phasor Noise-1.3.0/src/phasor_noise/generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.372633 Phasor Noise-1.3.1/
+-rw-rw-rw-   0        0        0      284 2023-05-19 19:59:18.000000 Phasor Noise-1.3.1/AUTHORS
+-rw-rw-rw-   0        0        0    35869 2023-05-16 20:15:41.000000 Phasor Noise-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0      147 2023-05-18 19:46:50.000000 Phasor Noise-1.3.1/Makefile
+-rw-rw-rw-   0        0        0     1119 2023-05-19 19:59:19.372633 Phasor Noise-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2023-05-18 19:48:23.000000 Phasor Noise-1.3.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.328262 Phasor Noise-1.3.1/docs/
+-rw-rw-rw-   0        0        0      603 2023-05-17 18:17:17.000000 Phasor Noise-1.3.1/docs/Makefile
+-rw-rw-rw-   0        0        0        0 2023-05-17 13:34:47.000000 Phasor Noise-1.3.1/docs/README.rst
+-rwxrwxrwx   0        0        0      827 2023-05-17 18:16:47.000000 Phasor Noise-1.3.1/docs/make.bat
+-rw-rw-rw-   0        0        0       24 2023-05-17 18:51:28.000000 Phasor Noise-1.3.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.332261 Phasor Noise-1.3.1/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.332261 Phasor Noise-1.3.1/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.336257 Phasor Noise-1.3.1/docs/source/api/GUI/
+-rw-rw-rw-   0        0        0      128 2023-05-18 20:12:40.000000 Phasor Noise-1.3.1/docs/source/api/GUI/index.rst
+-rw-rw-rw-   0        0        0      125 2023-05-18 20:08:51.000000 Phasor Noise-1.3.1/docs/source/api/GUI/menu.rst
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.340257 Phasor Noise-1.3.1/docs/source/api/analysis/
+-rw-rw-rw-   0        0        0      174 2023-05-18 20:11:22.000000 Phasor Noise-1.3.1/docs/source/api/analysis/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.340257 Phasor Noise-1.3.1/docs/source/api/generator/
+-rw-rw-rw-   0        0        0      190 2023-05-18 20:08:29.000000 Phasor Noise-1.3.1/docs/source/api/generator/index.rst
+-rw-rw-rw-   0        0        0      248 2023-05-17 20:58:47.000000 Phasor Noise-1.3.1/docs/source/api/index.rst
+-rw-rw-rw-   0        0        0     9191 2023-05-19 19:58:11.000000 Phasor Noise-1.3.1/docs/source/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.344256 Phasor Noise-1.3.1/docs/source/getting_started/
+-rw-rw-rw-   0        0        0      196 2023-05-19 07:43:30.000000 Phasor Noise-1.3.1/docs/source/getting_started/index.rst
+-rw-rw-rw-   0        0        0      193 2023-05-17 20:58:03.000000 Phasor Noise-1.3.1/docs/source/getting_started/installation.rst
+-rw-rw-rw-   0        0        0      668 2023-05-18 15:29:52.000000 Phasor Noise-1.3.1/docs/source/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.344256 Phasor Noise-1.3.1/docs/source/user_guide/
+-rw-rw-rw-   0        0        0       99 2023-05-17 14:58:13.000000 Phasor Noise-1.3.1/docs/source/user_guide/index.rst
+-rw-rw-rw-   0        0        0       89 2023-05-17 19:39:21.000000 Phasor Noise-1.3.1/requirements.txt
+-rw-rw-rw-   0        0        0      654 2023-05-19 19:59:19.376647 Phasor Noise-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      181 2023-05-17 18:14:41.000000 Phasor Noise-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.303974 Phasor Noise-1.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.372633 Phasor Noise-1.3.1/src/Phasor_Noise.egg-info/
+-rw-rw-rw-   0        0        0     1119 2023-05-19 19:59:19.000000 Phasor Noise-1.3.1/src/Phasor_Noise.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1144 2023-05-19 19:59:19.000000 Phasor Noise-1.3.1/src/Phasor_Noise.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 19:59:19.000000 Phasor Noise-1.3.1/src/Phasor_Noise.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 21:01:55.000000 Phasor Noise-1.3.1/src/Phasor_Noise.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-05-19 19:59:19.000000 Phasor Noise-1.3.1/src/Phasor_Noise.egg-info/pbr.json
+-rw-rw-rw-   0        0        0       86 2023-05-19 19:59:19.000000 Phasor Noise-1.3.1/src/Phasor_Noise.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-19 19:59:19.000000 Phasor Noise-1.3.1/src/Phasor_Noise.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.348261 Phasor Noise-1.3.1/src/phasor_noise/
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.355412 Phasor Noise-1.3.1/src/phasor_noise/GUI/
+-rw-rw-rw-   0        0        0    22675 2023-05-19 19:55:04.000000 Phasor Noise-1.3.1/src/phasor_noise/GUI/__init__.py
+-rw-rw-rw-   0        0        0     1436 2023-05-18 16:04:17.000000 Phasor Noise-1.3.1/src/phasor_noise/GUI/menu.py
+-rw-rw-rw-   0        0        0      552 2023-05-19 19:55:04.000000 Phasor Noise-1.3.1/src/phasor_noise/GUI/platform_specific.py
+-rw-rw-rw-   0        0        0      532 2023-05-19 07:41:06.000000 Phasor Noise-1.3.1/src/phasor_noise/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.356419 Phasor Noise-1.3.1/src/phasor_noise/analysis/
+-rw-rw-rw-   0        0        0      777 2023-05-18 15:41:41.000000 Phasor Noise-1.3.1/src/phasor_noise/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 19:59:19.356419 Phasor Noise-1.3.1/src/phasor_noise/generator/
+-rw-rw-rw-   0        0        0     5325 2023-05-18 15:37:46.000000 Phasor Noise-1.3.1/src/phasor_noise/generator/__init__.py
```

### Comparing `Phasor Noise-1.3.0/LICENSE` & `Phasor Noise-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Phasor Noise-1.3.0/PKG-INFO` & `Phasor Noise-1.3.1/src/Phasor_Noise.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Phasor Noise
-Version: 1.3.0
+Name: Phasor-Noise
+Version: 1.3.1
 Home-page: https://github.com/etachouzin/phasor_noise
 Author: Alexis Le Meur, Etienne Tachouzin, Paul Martin, Guillaume Hisleur, Paul Bedrossian
 Author-email: phasor_noise_dev@outlook.fr
 Maintainer: Alexis Le Meur, Etienne Tachouzin, Paul Martin, Guillaume Hisleur, Paul Bedrossian
 Maintainer-email: phasor_noise_dev@outlook.fr
 License: GNU
 Keywords: phasor_noise,generator
```

### Comparing `Phasor Noise-1.3.0/README.rst` & `Phasor Noise-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `Phasor Noise-1.3.0/docs/Makefile` & `Phasor Noise-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Phasor Noise-1.3.0/docs/make.bat` & `Phasor Noise-1.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Phasor Noise-1.3.0/docs/source/conf.py` & `Phasor Noise-1.3.1/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 author = 'Alexis Le Meur, Etienne Tachouzin, Paul Martin, Guillaume Hisleur, Paul Bedrossian'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = release = "1.3"
+version = release = "1.3.1"
 # The full version, including alpha/beta/rc tags.
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
```

### Comparing `Phasor Noise-1.3.0/docs/source/index.rst` & `Phasor Noise-1.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `Phasor Noise-1.3.0/setup.cfg` & `Phasor Noise-1.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 00000130: 7574 6c6f 6f6b 2e66 720d 0a64 6573 6372  utlook.fr..descr
 00000140: 6970 7469 6f6e 5f66 696c 6520 3d20 5245  iption_file = RE
 00000150: 4144 4d45 2e72 7374 0d0a 686f 6d65 5f70  ADME.rst..home_p
 00000160: 6167 6520 3d20 6874 7470 733a 2f2f 6769  age = https://gi
 00000170: 7468 7562 2e63 6f6d 2f65 7461 6368 6f75  thub.com/etachou
 00000180: 7a69 6e2f 7068 6173 6f72 5f6e 6f69 7365  zin/phasor_noise
 00000190: 0d0a 6c69 6365 6e73 6520 3d20 474e 550d  ..license = GNU.
-000001a0: 0a76 6572 7369 6f6e 203d 2031 2e33 0d0a  .version = 1.3..
-000001b0: 6b65 7977 6f72 6473 203d 200d 0a09 7068  keywords = ...ph
-000001c0: 6173 6f72 5f6e 6f69 7365 0d0a 0967 656e  asor_noise...gen
-000001d0: 6572 6174 6f72 0d0a 0d0a 5b6f 7074 696f  erator....[optio
-000001e0: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
-000001f0: 203d 200d 0a09 3d73 7263 0d0a 0d0a 5b66   = ...=src....[f
-00000200: 696c 6573 5d0d 0a70 6163 6b61 6765 7320  iles]..packages 
-00000210: 3d20 0d0a 0970 6861 736f 725f 6e6f 6973  = ...phasor_nois
-00000220: 650d 0a0d 0a5b 7062 725d 0d0a 736b 6970  e....[pbr]..skip
-00000230: 5f63 6861 6e67 656c 6f67 203d 2031 0d0a  _changelog = 1..
-00000240: 0d0a 5b73 6469 7374 5f77 6865 656c 5d0d  ..[sdist_wheel].
-00000250: 0a75 6e69 7665 7273 616c 203d 2031 0d0a  .universal = 1..
-00000260: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000270: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000280: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+000001a0: 0a76 6572 7369 6f6e 203d 2031 2e33 2e31  .version = 1.3.1
+000001b0: 0d0a 6b65 7977 6f72 6473 203d 200d 0a09  ..keywords = ...
+000001c0: 7068 6173 6f72 5f6e 6f69 7365 0d0a 0967  phasor_noise...g
+000001d0: 656e 6572 6174 6f72 0d0a 0d0a 5b6f 7074  enerator....[opt
+000001e0: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
+000001f0: 6972 203d 200d 0a09 3d73 7263 0d0a 0d0a  ir = ...=src....
+00000200: 5b66 696c 6573 5d0d 0a70 6163 6b61 6765  [files]..package
+00000210: 7320 3d20 0d0a 0970 6861 736f 725f 6e6f  s = ...phasor_no
+00000220: 6973 650d 0a0d 0a5b 7062 725d 0d0a 736b  ise....[pbr]..sk
+00000230: 6970 5f63 6861 6e67 656c 6f67 203d 2031  ip_changelog = 1
+00000240: 0d0a 0d0a 5b73 6469 7374 5f77 6865 656c  ....[sdist_wheel
+00000250: 5d0d 0a75 6e69 7665 7273 616c 203d 2031  ]..universal = 1
+00000260: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000270: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000280: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/PKG-INFO` & `Phasor Noise-1.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Phasor-Noise
-Version: 1.3.0
+Name: Phasor Noise
+Version: 1.3.1
 Home-page: https://github.com/etachouzin/phasor_noise
 Author: Alexis Le Meur, Etienne Tachouzin, Paul Martin, Guillaume Hisleur, Paul Bedrossian
 Author-email: phasor_noise_dev@outlook.fr
 Maintainer: Alexis Le Meur, Etienne Tachouzin, Paul Martin, Guillaume Hisleur, Paul Bedrossian
 Maintainer-email: phasor_noise_dev@outlook.fr
 License: GNU
 Keywords: phasor_noise,generator
```

### Comparing `Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/SOURCES.txt` & `Phasor Noise-1.3.1/src/Phasor_Noise.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 docs/README.rst
 docs/make.bat
 docs/requirements.txt
 docs/source/conf.py
 docs/source/index.rst
 docs/source/api/index.rst
 docs/source/api/GUI/index.rst
+docs/source/api/GUI/menu.rst
 docs/source/api/analysis/index.rst
 docs/source/api/generator/index.rst
 docs/source/getting_started/index.rst
 docs/source/getting_started/installation.rst
 docs/source/user_guide/index.rst
 src/phasor_noise/__init__.py
 src/phasor_noise/GUI/__init__.py
```

### Comparing `Phasor Noise-1.3.0/src/phasor_noise/GUI/__init__.py` & `Phasor Noise-1.3.1/src/phasor_noise/GUI/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import phasor_noise.GUI.menu
-import phasor_noise.phasor_noise_generator
+import phasor_noise.GUI.menu as menu
+import phasor_noise.generator as generator
 import phasor_noise.analysis as analysis
 import tkinter as tk
 import random as rd
 import numpy as np
 import matplotlib.pyplot as plt
 from PIL import Image
 from PIL import ImageTk
 import json
 from skimage import exposure
 from copy import deepcopy
 from phasor_noise.GUI.platform_specific import *
+import os
 
 
 class Window:
     """
     Window GUI to manipulate the phasor noise and analyse it
     """
     def __init__(self, master, version="Python") -> None:
@@ -26,15 +27,15 @@
         self.visualize = tk.BooleanVar()
         self.master.resizable(height=False, width=False)
         self.master.title("Générateur de bruit Phasor - Version : " + version)
         self.master.geometry("1090x720")
         self.currentPage = 0
         self.gen_mode = version
         self.load_page()
-        self.menu = phasor_noise.GUI.menu.Menu(self)
+        self.menu = menu.Menu(self)
 
     def save(self):
         """
         Save current configuration
         """
         new_config = {
             "x": self.img_size_x.get(),
@@ -387,15 +388,15 @@
         self.kernels = kernels
 
     def gen_noise(self):
         if self.gen_mode == "Python":
             X = np.arange(0, self.size[0])
             Y = np.arange(0, self.size[1])
             X, Y = np.meshgrid(X, Y)
-            self.results = phasor_noise.phasor_noise_generator.apply_noise_python(X, Y, self.kernels)
+            self.results = generator.apply_noise_python(X, Y, self.kernels)
             plt.contourf(X, Y, self.results[0], cmap='Greys')
             plt.colorbar()
             plt.axis('off')
             if self.visualize.get() == 1:
                 for kernel in self.kernels:
                     plt.plot(kernel[0][0], kernel[0][1], color="green", marker="o")
                     plt.arrow(kernel[0][0], kernel[0][1], kernel[1][0] * 5, kernel[1][1] * 5, width=1, head_width=2,
@@ -423,15 +424,15 @@
             plt.savefig(f"{images_directory()}/noise_hist.png", bbox_inches='tight')
             self.visu_mode_img()
 
         elif self.gen_mode == "Numpy":
             X = np.arange(0, self.size[0])
             Y = np.arange(0, self.size[1])
             X, Y = np.meshgrid(X, Y)
-            self.results = phasor_noise.phasor_noise_generator.apply_noise_numpy(X, Y, deepcopy(self.kernels),
+            self.results = generator.apply_noise_numpy(X, Y, deepcopy(self.kernels),
                                                                                  self.size)
             plt.contourf(X, Y, self.results[0], cmap='Greys')
             plt.axis('off')
             plt.colorbar()
             if self.visualize.get() == 1:
                 for kernel in self.kernels:
                     plt.plot(kernel[0][0], kernel[0][1], color="green", marker="o")
```

### Comparing `Phasor Noise-1.3.0/src/phasor_noise/GUI/menu.py` & `Phasor Noise-1.3.1/src/phasor_noise/GUI/menu.py`

 * *Files identical despite different names*

### Comparing `Phasor Noise-1.3.0/src/phasor_noise/analysis/__init__.py` & `Phasor Noise-1.3.1/src/phasor_noise/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `Phasor Noise-1.3.0/src/phasor_noise/generator/__init__.py` & `Phasor Noise-1.3.1/src/phasor_noise/generator/__init__.py`

 * *Files identical despite different names*

