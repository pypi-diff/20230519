# Comparing `tmp/tankioapi-1.0.0.tar.gz` & `tmp/tankioapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tankioapi-1.0.0.tar", last modified: Tue May 16 18:16:14 2023, max compression
+gzip compressed data, was "tankioapi-1.0.1.tar", last modified: Fri May 19 17:53:47 2023, max compression
```

## Comparing `tankioapi-1.0.0.tar` & `tankioapi-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 18:16:14.822874 tankioapi-1.0.0/
--rw-rw-rw-   0        0        0     1072 2023-05-13 16:20:18.000000 tankioapi-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      116 2023-05-15 17:49:50.000000 tankioapi-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4577 2023-05-16 18:16:14.821874 tankioapi-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3196 2023-05-16 18:15:16.000000 tankioapi-1.0.0/README.md
--rw-rw-rw-   0        0        0     1977 2023-05-16 18:08:50.000000 tankioapi-1.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-16 18:16:14.632872 tankioapi-1.0.0/requirements/
--rw-rw-rw-   0        0        0       29 2023-05-14 11:20:40.000000 tankioapi-1.0.0/requirements/dev.txt
--rw-rw-rw-   0        0        0       24 2023-05-13 16:18:41.000000 tankioapi-1.0.0/requirements/speedup.txt
--rw-rw-rw-   0        0        0        7 2023-05-13 16:15:33.000000 tankioapi-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 18:16:14.822874 tankioapi-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     3776 2023-05-16 17:56:05.000000 tankioapi-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 18:16:14.552872 tankioapi-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 18:16:14.745872 tankioapi-1.0.0/src/tankioapi.egg-info/
--rw-rw-rw-   0        0        0     4577 2023-05-16 18:16:14.000000 tankioapi-1.0.0/src/tankioapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-05-16 18:16:14.000000 tankioapi-1.0.0/src/tankioapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 18:16:14.000000 tankioapi-1.0.0/src/tankioapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-16 18:16:14.000000 tankioapi-1.0.0/src/tankioapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-16 18:16:14.000000 tankioapi-1.0.0/src/tankioapi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 18:16:14.758871 tankioapi-1.0.0/src/toapi/
--rw-rw-rw-   0        0        0     1303 2023-05-16 18:09:30.000000 tankioapi-1.0.0/src/toapi/__init__.py
--rw-rw-rw-   0        0        0     3674 2023-05-16 18:07:42.000000 tankioapi-1.0.0/src/toapi/client.py
-drwxrwxrwx   0        0        0        0 2023-05-16 18:16:14.779873 tankioapi-1.0.0/src/toapi/data/
--rw-rw-rw-   0        0        0     1132 2023-05-16 17:39:09.000000 tankioapi-1.0.0/src/toapi/data/__init__.py
--rw-rw-rw-   0        0        0     3272 2023-05-15 19:06:28.000000 tankioapi-1.0.0/src/toapi/data/ranks.py
--rw-rw-rw-   0        0        0     2524 2023-05-16 17:38:18.000000 tankioapi-1.0.0/src/toapi/data/test_server.py
--rw-rw-rw-   0        0        0     1609 2023-05-13 18:17:03.000000 tankioapi-1.0.0/src/toapi/errors.py
--rw-rw-rw-   0        0        0     2577 2023-05-16 17:56:05.000000 tankioapi-1.0.0/src/toapi/http.py
--rw-rw-rw-   0        0        0        0 2023-05-15 17:51:02.000000 tankioapi-1.0.0/src/toapi/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-16 18:16:14.817871 tankioapi-1.0.0/src/toapi/types/
--rw-rw-rw-   0        0        0     1239 2023-05-15 20:04:05.000000 tankioapi-1.0.0/src/toapi/types/__init__.py
--rw-rw-rw-   0        0        0     5845 2023-05-16 17:56:05.000000 tankioapi-1.0.0/src/toapi/types/game_object.py
--rw-rw-rw-   0        0        0     2910 2023-05-16 17:56:05.000000 tankioapi-1.0.0/src/toapi/types/mode.py
--rw-rw-rw-   0        0        0     2567 2023-05-16 17:56:05.000000 tankioapi-1.0.0/src/toapi/types/rank.py
--rw-rw-rw-   0        0        0     3148 2023-05-15 19:06:18.000000 tankioapi-1.0.0/src/toapi/types/rating.py
--rw-rw-rw-   0        0        0     7032 2023-05-16 17:56:05.000000 tankioapi-1.0.0/src/toapi/types/status.py
--rw-rw-rw-   0        0        0     3523 2023-05-15 19:23:46.000000 tankioapi-1.0.0/src/toapi/types/top.py
--rw-rw-rw-   0        0        0     8211 2023-05-15 19:36:53.000000 tankioapi-1.0.0/src/toapi/types/user.py
+drwxrwxrwx   0        0        0        0 2023-05-19 17:53:47.749008 tankioapi-1.0.1/
+-rw-rw-rw-   0        0        0     1072 2023-05-13 16:20:18.000000 tankioapi-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      116 2023-05-15 17:49:50.000000 tankioapi-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4982 2023-05-19 17:53:47.748007 tankioapi-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3535 2023-05-18 18:29:42.000000 tankioapi-1.0.1/README.md
+-rw-rw-rw-   0        0        0     2046 2023-05-19 17:22:34.000000 tankioapi-1.0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-19 17:53:47.605006 tankioapi-1.0.1/requirements/
+-rw-rw-rw-   0        0        0       29 2023-05-14 11:20:40.000000 tankioapi-1.0.1/requirements/dev.txt
+-rw-rw-rw-   0        0        0       34 2023-05-19 17:18:08.000000 tankioapi-1.0.1/requirements/docs.txt
+-rw-rw-rw-   0        0        0       24 2023-05-13 16:18:41.000000 tankioapi-1.0.1/requirements/speedup.txt
+-rw-rw-rw-   0        0        0        7 2023-05-13 16:15:33.000000 tankioapi-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 17:53:47.750006 tankioapi-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     3898 2023-05-19 17:23:50.000000 tankioapi-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 17:53:47.545005 tankioapi-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 17:53:47.680008 tankioapi-1.0.1/src/tankioapi.egg-info/
+-rw-rw-rw-   0        0        0     4982 2023-05-19 17:53:47.000000 tankioapi-1.0.1/src/tankioapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2023-05-19 17:53:47.000000 tankioapi-1.0.1/src/tankioapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 17:53:47.000000 tankioapi-1.0.1/src/tankioapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-19 17:53:47.000000 tankioapi-1.0.1/src/tankioapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-19 17:53:47.000000 tankioapi-1.0.1/src/tankioapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 17:53:47.701006 tankioapi-1.0.1/src/toapi/
+-rw-rw-rw-   0        0        0     1303 2023-05-19 17:53:21.000000 tankioapi-1.0.1/src/toapi/__init__.py
+-rw-rw-rw-   0        0        0     3676 2023-05-18 17:19:18.000000 tankioapi-1.0.1/src/toapi/client.py
+drwxrwxrwx   0        0        0        0 2023-05-19 17:53:47.710006 tankioapi-1.0.1/src/toapi/data/
+-rw-rw-rw-   0        0        0     1132 2023-05-16 17:39:09.000000 tankioapi-1.0.1/src/toapi/data/__init__.py
+-rw-rw-rw-   0        0        0     3272 2023-05-15 19:06:28.000000 tankioapi-1.0.1/src/toapi/data/ranks.py
+-rw-rw-rw-   0        0        0     2524 2023-05-16 17:38:18.000000 tankioapi-1.0.1/src/toapi/data/test_server.py
+-rw-rw-rw-   0        0        0     1609 2023-05-13 18:17:03.000000 tankioapi-1.0.1/src/toapi/errors.py
+-rw-rw-rw-   0        0        0     2291 2023-05-19 17:51:05.000000 tankioapi-1.0.1/src/toapi/http.py
+-rw-rw-rw-   0        0        0        0 2023-05-15 17:51:02.000000 tankioapi-1.0.1/src/toapi/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-19 17:53:47.746007 tankioapi-1.0.1/src/toapi/types/
+-rw-rw-rw-   0        0        0     1239 2023-05-15 20:04:05.000000 tankioapi-1.0.1/src/toapi/types/__init__.py
+-rw-rw-rw-   0        0        0     5850 2023-05-19 17:51:29.000000 tankioapi-1.0.1/src/toapi/types/game_object.py
+-rw-rw-rw-   0        0        0     2910 2023-05-16 17:56:05.000000 tankioapi-1.0.1/src/toapi/types/mode.py
+-rw-rw-rw-   0        0        0     2453 2023-05-18 19:11:20.000000 tankioapi-1.0.1/src/toapi/types/rank.py
+-rw-rw-rw-   0        0        0     3148 2023-05-15 19:06:18.000000 tankioapi-1.0.1/src/toapi/types/rating.py
+-rw-rw-rw-   0        0        0     7032 2023-05-16 17:56:05.000000 tankioapi-1.0.1/src/toapi/types/status.py
+-rw-rw-rw-   0        0        0     3523 2023-05-15 19:23:46.000000 tankioapi-1.0.1/src/toapi/types/top.py
+-rw-rw-rw-   0        0        0     8211 2023-05-15 19:36:53.000000 tankioapi-1.0.1/src/toapi/types/user.py
```

### Comparing `tankioapi-1.0.0/LICENSE` & `tankioapi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tankioapi-1.0.0/PKG-INFO` & `tankioapi-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,287 +1,312 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2074 616e  : 2.1..Name: tan
 00000020: 6b69 6f61 7069 0d0a 5665 7273 696f 6e3a  kioapi..Version:
-00000030: 2031 2e30 2e30 0d0a 5375 6d6d 6172 793a   1.0.0..Summary:
+00000030: 2031 2e30 2e31 0d0a 5375 6d6d 6172 793a   1.0.1..Summary:
 00000040: 2041 2050 7974 686f 6e20 7772 6974 7465   A Python writte
 00000050: 6e20 7772 6170 7065 7220 666f 7220 7468  n wrapper for th
 00000060: 6520 5461 6e6b 6920 4f6e 6c69 6e65 2067  e Tanki Online g
 00000070: 616d 6520 4150 490d 0a48 6f6d 652d 7061  ame API..Home-pa
 00000080: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
 00000090: 7562 2e63 6f6d 2f73 746e 6775 6c61 7269  ub.com/stngulari
-000000a0: 7479 2f74 616e 6b69 6f61 7069 2e70 790d  ty/tankioapi.py.
-000000b0: 0a41 7574 686f 723a 2073 746e 6775 6c61  .Author: stngula
-000000c0: 7269 7479 0d0a 4175 7468 6f72 2d65 6d61  rity..Author-ema
-000000d0: 696c 3a20 7374 6e67 756c 6172 6974 7920  il: stngularity 
-000000e0: 3c73 746e 6775 6c61 7269 7479 4067 6d61  <stngularity@gma
-000000f0: 696c 2e63 6f6d 3e0d 0a4c 6963 656e 7365  il.com>..License
-00000100: 3a20 4d49 5420 4c69 6365 6e73 650d 0a50  : MIT License..P
-00000110: 726f 6a65 6374 2d55 524c 3a20 486f 6d65  roject-URL: Home
-00000120: 7061 6765 2c20 6874 7470 733a 2f2f 6769  page, https://gi
-00000130: 7468 7562 2e63 6f6d 2f73 746e 6775 6c61  thub.com/stngula
-00000140: 7269 7479 2f74 616e 6b69 6f61 7069 0d0a  rity/tankioapi..
-00000150: 5072 6f6a 6563 742d 5552 4c3a 2053 6f75  Project-URL: Sou
-00000160: 7263 6520 436f 6465 2c20 6874 7470 733a  rce Code, https:
-00000170: 2f2f 6769 7468 7562 2e63 6f6d 2f73 746e  //github.com/stn
-00000180: 6775 6c61 7269 7479 2f74 616e 6b69 6f61  gularity/tankioa
-00000190: 7069 0d0a 5072 6f6a 6563 742d 5552 4c3a  pi..Project-URL:
-000001a0: 2043 6861 6e67 656c 6f67 2c20 6874 7470   Changelog, http
+000000a0: 7479 2f74 616e 6b69 6f61 7069 0d0a 4175  ty/tankioapi..Au
+000000b0: 7468 6f72 3a20 7374 6e67 756c 6172 6974  thor: stngularit
+000000c0: 790d 0a41 7574 686f 722d 656d 6169 6c3a  y..Author-email:
+000000d0: 2073 746e 6775 6c61 7269 7479 203c 7374   stngularity <st
+000000e0: 6e67 756c 6172 6974 7940 676d 6169 6c2e  ngularity@gmail.
+000000f0: 636f 6d3e 0d0a 4c69 6365 6e73 653a 204d  com>..License: M
+00000100: 4954 204c 6963 656e 7365 0d0a 5072 6f6a  IT License..Proj
+00000110: 6563 742d 5552 4c3a 2044 6f63 756d 656e  ect-URL: Documen
+00000120: 7461 7469 6f6e 2c20 6874 7470 733a 2f2f  tation, https://
+00000130: 7374 6e67 756c 6172 6974 792e 6769 7468  stngularity.gith
+00000140: 7562 2e69 6f2f 7461 6e6b 696f 6170 690d  ub.io/tankioapi.
+00000150: 0a50 726f 6a65 6374 2d55 524c 3a20 486f  .Project-URL: Ho
+00000160: 6d65 7061 6765 2c20 6874 7470 733a 2f2f  mepage, https://
+00000170: 6769 7468 7562 2e63 6f6d 2f73 746e 6775  github.com/stngu
+00000180: 6c61 7269 7479 2f74 616e 6b69 6f61 7069  larity/tankioapi
+00000190: 0d0a 5072 6f6a 6563 742d 5552 4c3a 2053  ..Project-URL: S
+000001a0: 6f75 7263 6520 436f 6465 2c20 6874 7470  ource Code, http
 000001b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
 000001c0: 746e 6775 6c61 7269 7479 2f74 616e 6b69  tngularity/tanki
-000001d0: 6f61 7069 2f62 6c6f 622f 6d61 696e 2f43  oapi/blob/main/C
-000001e0: 4841 4e47 454c 4f47 2e6d 640d 0a50 726f  HANGELOG.md..Pro
-000001f0: 6a65 6374 2d55 524c 3a20 4275 6720 5472  ject-URL: Bug Tr
-00000200: 6163 6b65 722c 2068 7474 7073 3a2f 2f67  acker, https://g
-00000210: 6974 6875 622e 636f 6d2f 7374 6e67 756c  ithub.com/stngul
-00000220: 6172 6974 792f 7461 6e6b 696f 6170 692f  arity/tankioapi/
-00000230: 6973 7375 6573 0d0a 4b65 7977 6f72 6473  issues..Keywords
-00000240: 3a20 6761 6d65 2c61 7069 2c74 6f2c 7461  : game,api,to,ta
-00000250: 6e6b 6920 6f6e 6c69 6e65 0d0a 436c 6173  nki online..Clas
-00000260: 7369 6669 6572 3a20 4465 7665 6c6f 706d  sifier: Developm
-00000270: 656e 7420 5374 6174 7573 203a 3a20 3520  ent Status :: 5 
-00000280: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
-00000290: 626c 650d 0a43 6c61 7373 6966 6965 723a  ble..Classifier:
-000002a0: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
-000002b0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-000002c0: 4c69 6365 6e73 650d 0a43 6c61 7373 6966  License..Classif
-000002d0: 6965 723a 204e 6174 7572 616c 204c 616e  ier: Natural Lan
-000002e0: 6775 6167 6520 3a3a 2045 6e67 6c69 7368  guage :: English
-000002f0: 0d0a 436c 6173 7369 6669 6572 3a20 4f70  ..Classifier: Op
-00000300: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-00000310: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-00000320: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
-00000330: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000340: 6765 203a 3a20 5079 7468 6f6e 0d0a 436c  ge :: Python..Cl
-00000350: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000360: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000370: 3a20 5079 7468 6f6e 203a 3a20 3320 3a3a  : Python :: 3 ::
-00000380: 204f 6e6c 790d 0a43 6c61 7373 6966 6965   Only..Classifie
-00000390: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-000003a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000003b0: 6e20 3a3a 2033 2e38 0d0a 436c 6173 7369  n :: 3.8..Classi
-000003c0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000003d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000003e0: 7468 6f6e 203a 3a20 332e 390d 0a43 6c61  thon :: 3.9..Cla
-000003f0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000400: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000410: 2050 7974 686f 6e20 3a3a 2033 2e31 300d   Python :: 3.10.
-00000420: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000430: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000440: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000450: 2e31 310d 0a43 6c61 7373 6966 6965 723a  .11..Classifier:
-00000460: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000470: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000480: 3a3a 2049 6d70 6c65 6d65 6e74 6174 696f  :: Implementatio
-00000490: 6e20 3a3a 2043 5079 7468 6f6e 0d0a 436c  n :: CPython..Cl
-000004a0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-000004b0: 3a3a 2055 7469 6c69 7469 6573 0d0a 436c  :: Utilities..Cl
-000004c0: 6173 7369 6669 6572 3a20 5479 7069 6e67  assifier: Typing
-000004d0: 203a 3a20 5479 7065 640d 0a52 6571 7569   :: Typed..Requi
-000004e0: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
-000004f0: 380d 0a44 6573 6372 6970 7469 6f6e 2d43  8..Description-C
-00000500: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000510: 742f 6d61 726b 646f 776e 0d0a 5072 6f76  t/markdown..Prov
-00000520: 6964 6573 2d45 7874 7261 3a20 7370 6565  ides-Extra: spee
-00000530: 6475 700d 0a50 726f 7669 6465 732d 4578  dup..Provides-Ex
-00000540: 7472 613a 2064 6576 0d0a 4c69 6365 6e73  tra: dev..Licens
-00000550: 652d 4669 6c65 3a20 4c49 4345 4e53 450d  e-File: LICENSE.
-00000560: 0a0d 0a3c 7020 616c 6967 6e3d 6365 6e74  ...<p align=cent
-00000570: 6572 3e0d 0a20 2020 203c 696d 6720 7372  er>..    <img sr
-00000580: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000590: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-000005a0: 2d73 746e 6775 6c61 7269 7479 2773 2532  -stngularity's%2
-000005b0: 3077 6f72 6b2d 2532 3334 3664 6631 3122  0work-%2346df11"
-000005c0: 3e0d 0a20 2020 203c 696d 6720 7372 633d  >..    <img src=
-000005d0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-000005e0: 656c 6473 2e69 6f2f 7079 7069 2f76 2f74  elds.io/pypi/v/t
-000005f0: 616e 6b69 6f61 7069 3f63 6f6c 6f72 3d25  ankioapi?color=%
-00000600: 3233 3436 6466 3131 266c 6162 656c 3d56  2346df11&label=V
-00000610: 6572 7369 6f6e 223e 0d0a 2020 2020 3c69  ersion">..    <i
-00000620: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000630: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-00000640: 7970 692f 6464 2f74 616e 6b69 6f61 7069  ypi/dd/tankioapi
-00000650: 3f63 6f6c 6f72 3d25 3233 3436 6466 3131  ?color=%2346df11
-00000660: 266c 6162 656c 3d44 6f77 6e6c 6f61 6473  &label=Downloads
-00000670: 223e 0d0a 3c2f 703e 0d0a 3c70 2061 6c69  ">..</p>..<p ali
-00000680: 676e 3d63 656e 7465 723e 0d0a 2020 2020  gn=center>..    
-00000690: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000006a0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000006b0: 2f67 6974 6875 622f 6973 7375 6573 2f73  /github/issues/s
-000006c0: 746e 6775 6c61 7269 7479 2f74 616e 6b69  tngularity/tanki
-000006d0: 6f61 7069 3f63 6f6c 6f72 3d25 3233 3436  oapi?color=%2346
-000006e0: 6466 3131 266c 6162 656c 3d49 7373 7565  df11&label=Issue
-000006f0: 7322 3e0d 0a20 2020 203c 696d 6720 7372  s">..    <img sr
-00000700: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000710: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00000720: 2f6c 6963 656e 7365 2f73 746e 6775 6c61  /license/stngula
-00000730: 7269 7479 2f74 616e 6b69 6f61 7069 3f63  rity/tankioapi?c
-00000740: 6f6c 6f72 3d25 3233 3436 6466 3131 266c  olor=%2346df11&l
-00000750: 6162 656c 3d4c 6963 656e 7365 223e 0d0a  abel=License">..
-00000760: 3c2f 703e 0d0a 0d0a 2323 204e 6f74 6966  </p>....## Notif
-00000770: 6963 6174 696f 6e0d 0a54 6869 7320 7072  ication..This pr
-00000780: 6f6a 6563 7420 7761 7320 6372 6561 7465  oject was create
-00000790: 6420 6a75 7374 2074 6f20 6578 6973 742e  d just to exist.
-000007a0: 204f 6620 636f 7572 7365 2c20 4920 7769   Of course, I wi
-000007b0: 6c6c 2075 7064 6174 6520 6974 2077 6865  ll update it whe
-000007c0: 6e20 7468 6520 4150 4920 6974 7365 6c66  n the API itself
-000007d0: 2063 6861 6e67 6573 2c20 6275 7420 6e6f   changes, but no
-000007e0: 7420 696d 6d65 6469 6174 656c 792e 2057  t immediately. W
-000007f0: 656c 6c2c 2069 6620 596f 7520 7761 6e74  ell, if You want
-00000800: 2074 6f20 7375 7070 6f72 7420 7468 6973   to support this
-00000810: 2070 726f 6a65 6374 2c20 596f 7520 6361   project, You ca
-00000820: 6e20 6769 7665 2069 7420 6120 7374 6172  n give it a star
-00000830: 2e0d 0a0d 0a23 2320 496e 666f 726d 6174  .....## Informat
-00000840: 696f 6e0d 0a41 7320 6d65 6e74 696f 6e65  ion..As mentione
-00000850: 6420 6561 726c 6965 722c 2074 6869 7320  d earlier, this 
-00000860: 7072 6f6a 6563 7420 6973 2063 7265 6174  project is creat
-00000870: 6564 206a 7573 7420 746f 2065 7869 7374  ed just to exist
-00000880: 2e20 416e 6420 736f 2c20 7468 6520 6d6f  . And so, the mo
-00000890: 6475 6c65 2069 7473 656c 6620 6973 206e  dule itself is n
-000008a0: 6565 6465 6420 746f 2067 6574 2074 6865  eeded to get the
-000008b0: 2074 6f70 206f 6620 706c 6179 6572 7320   top of players 
-000008c0: 616e 6420 6765 7420 696e 666f 726d 6174  and get informat
-000008d0: 696f 6e20 6162 6f75 7420 7468 6520 706c  ion about the pl
-000008e0: 6179 6572 2073 6570 6172 6174 656c 792e  ayer separately.
-000008f0: 2049 6620 596f 7520 6b6e 6f77 206d 6f72   If You know mor
-00000900: 6520 6675 6e63 7469 6f6e 616c 6974 7920  e functionality 
-00000910: 6f66 2074 6865 2041 5049 206f 6620 7468  of the API of th
-00000920: 6520 6761 6d65 2060 5461 6e6b 6920 4f6e  e game `Tanki On
-00000930: 6c69 6e65 602c 2074 6865 6e20 706c 6561  line`, then plea
-00000940: 7365 2072 6570 6f72 7420 7468 6973 2066  se report this f
-00000950: 756e 6374 696f 6e61 6c69 7479 2069 6e20  unctionality in 
-00000960: 7468 6520 5b60 4973 7375 6573 605d 2868  the [`Issues`](h
-00000970: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000980: 6d2f 7374 6e67 756c 6172 6974 792f 7461  m/stngularity/ta
-00000990: 6e6b 696f 6170 692f 6973 7375 6573 292e  nkioapi/issues).
-000009a0: 0d0a 0d0a 2323 2323 2323 2046 6561 7475  ....###### Featu
-000009b0: 7265 730d 0a2d 2046 756c 6c79 2060 6173  res..- Fully `as
-000009c0: 796e 6360 2f60 6177 6169 7460 0d0a 2d20  ync`/`await`..- 
-000009d0: 4765 7474 696e 6720 746f 7020 6f66 2070  Getting top of p
-000009e0: 6c61 7965 7273 0d0a 2d20 4765 7474 696e  layers..- Gettin
-000009f0: 6720 696e 666f 726d 6174 696f 6e20 6f66  g information of
-00000a00: 2061 6e79 2070 6c61 7965 7220 6279 2068   any player by h
-00000a10: 696d 206e 616d 650d 0a2d 2047 6574 7469  im name..- Getti
-00000a20: 6e67 2073 7461 7475 7320 6f66 2073 7461  ng status of sta
-00000a30: 626c 6520 7365 7276 6572 2060 4d61 7962  ble server `Mayb
-00000a40: 6520 6465 7072 6563 6174 6564 600d 0a2d  e deprecated`..-
-00000a50: 2047 6574 7469 6e67 2073 7461 7475 7320   Getting status 
-00000a60: 6f66 2074 6573 7420 7365 7276 6572 730d  of test servers.
-00000a70: 0a0d 0a23 2320 496e 7374 616c 6c69 6e67  ...## Installing
-00000a80: 0d0a 2a2a 5b50 7974 686f 6e20 332e 385d  ..**[Python 3.8]
-00000a90: 2868 7474 7073 3a2f 2f77 7777 2e70 7974  (https://www.pyt
-00000aa0: 686f 6e2e 6f72 672f 646f 776e 6c6f 6164  hon.org/download
-00000ab0: 732f 2920 6f72 2068 6967 6865 7220 6973  s/) or higher is
-00000ac0: 2072 6571 7569 7265 642a 2a0d 0a0d 0a54   required**....T
-00000ad0: 6f20 696e 7374 616c 6c20 6120 6e6f 6e2d  o install a non-
-00000ae0: 6073 7065 6564 7570 6020 7665 7273 696f  `speedup` versio
-00000af0: 6e20 6f66 2074 6865 206c 6962 7261 7279  n of the library
-00000b00: 2c20 646f 2074 6865 2066 6f6c 6c6f 7769  , do the followi
-00000b10: 6e67 3a0d 0a3e 2060 6060 7368 0d0a 3e20  ng:..> ```sh..> 
-00000b20: 2320 4c69 6e75 782f 6d61 634f 530d 0a3e  # Linux/macOS..>
-00000b30: 2070 7974 686f 6e33 202d 6d20 7069 7020   python3 -m pip 
-00000b40: 696e 7374 616c 6c20 2d55 2074 616e 6b69  install -U tanki
-00000b50: 6f61 7069 0d0a 3e0d 0a3e 2023 2057 696e  oapi..>..> # Win
-00000b60: 646f 7773 0d0a 3e20 7079 202d 3320 2d6d  dows..> py -3 -m
-00000b70: 2070 6970 2069 6e73 7461 6c6c 202d 5520   pip install -U 
-00000b80: 7461 6e6b 696f 6170 690d 0a3e 2060 6060  tankioapi..> ```
-00000b90: 0d0a 0d0a 4f72 2c20 746f 2069 6e73 7461  ....Or, to insta
-00000ba0: 6c6c 2074 6865 2060 7370 6565 6475 7060  ll the `speedup`
-00000bb0: 2076 6572 7369 6f6e 2c20 646f 2074 6865   version, do the
-00000bc0: 2066 6f6c 6c6f 7769 6e67 3a0d 0a3e 2060   following:..> `
-00000bd0: 6060 7368 0d0a 3e20 2320 4c69 6e75 782f  ``sh..> # Linux/
-00000be0: 6d61 634f 530d 0a3e 2070 7974 686f 6e33  macOS..> python3
-00000bf0: 202d 6d20 7069 7020 696e 7374 616c 6c20   -m pip install 
-00000c00: 2d55 2022 7461 6e6b 696f 6170 695b 7370  -U "tankioapi[sp
-00000c10: 6565 6475 705d 220d 0a3e 0d0a 3e20 2320  eedup]"..>..> # 
-00000c20: 5769 6e64 6f77 730d 0a3e 2070 7920 2d33  Windows..> py -3
-00000c30: 202d 6d20 7069 7020 696e 7374 616c 6c20   -m pip install 
-00000c40: 2d55 2074 616e 6b69 6f61 7069 5b73 7065  -U tankioapi[spe
-00000c50: 6564 7570 5d0d 0a3e 2060 6060 0d0a 0d0a  edup]..> ```....
-00000c60: 416e 642c 2074 6f20 696e 7374 616c 6c20  And, to install 
-00000c70: 7468 6520 6465 7665 6c6f 706d 656e 7420  the development 
-00000c80: 7665 7273 696f 6e2c 2064 6f20 7468 6520  version, do the 
-00000c90: 666f 6c6c 6f77 696e 673a 0d0a 3e20 6060  following:..> ``
-00000ca0: 6073 680d 0a3e 2024 2067 6974 2063 6c6f  `sh..> $ git clo
-00000cb0: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
-00000cc0: 622e 636f 6d2f 7374 6e67 756c 6172 6974  b.com/stngularit
-00000cd0: 792f 7461 6e6b 696f 6170 690d 0a3e 2024  y/tankioapi..> $
-00000ce0: 2063 6420 7461 6e6b 696f 6170 690d 0a3e   cd tankioapi..>
-00000cf0: 2024 2070 7974 686f 6e33 202d 6d20 7069   $ python3 -m pi
-00000d00: 7020 696e 7374 616c 6c20 2d55 202e 5b73  p install -U .[s
-00000d10: 7065 6564 7570 5d0d 0a3e 2060 6060 0d0a  peedup]..> ```..
-00000d20: 0d0a 2323 2045 7861 6d70 6c65 730d 0a48  ..## Examples..H
-00000d30: 6572 6520 6172 6520 6578 616d 706c 6573  ere are examples
-00000d40: 206f 6620 736f 6d65 206f 6620 7468 6520   of some of the 
-00000d50: 6665 6174 7572 6573 206f 6620 7468 6520  features of the 
-00000d60: 6c69 6272 6172 792e 204d 6f72 6520 6578  library. More ex
-00000d70: 616d 706c 6573 2069 6e20 5b60 6578 616d  amples in [`exam
-00000d80: 706c 6573 2f60 5d28 2f65 7861 6d70 6c65  ples/`](/example
-00000d90: 7329 0d0a 0d0a 2323 2323 2323 2047 6574  s)....###### Get
-00000da0: 7469 6e67 2061 6c6c 2074 6f70 7320 6f66  ting all tops of
-00000db0: 2070 6c61 7965 7273 0d0a 6060 6070 790d   players..```py.
-00000dc0: 0a69 6d70 6f72 7420 6173 796e 6369 6f0d  .import asyncio.
-00000dd0: 0a66 726f 6d20 746f 6170 6920 696d 706f  .from toapi impo
-00000de0: 7274 2054 6f70 2c20 546f 704c 6973 7473  rt Top, TopLists
-00000df0: 2c20 6765 745f 746f 7073 0d0a 0d0a 0d0a  , get_tops......
-00000e00: 746f 7073 3a20 546f 704c 6973 7473 203d  tops: TopLists =
-00000e10: 2061 7379 6e63 696f 2e72 756e 2867 6574   asyncio.run(get
-00000e20: 5f74 6f70 7328 2929 0d0a 6566 6669 6369  _tops())..effici
-00000e30: 656e 6379 5f74 6f70 3a20 546f 7020 3d20  ency_top: Top = 
-00000e40: 746f 7073 2e65 6666 6963 6965 6e63 790d  tops.efficiency.
-00000e50: 0a70 7269 6e74 2822 2d2d 2d2d 2d20 4566  .print("----- Ef
-00000e60: 6669 6369 656e 6379 2074 6f70 202d 2d2d  ficiency top ---
-00000e70: 2d2d 2229 0d0a 666f 7220 6e75 6d62 6572  --")..for number
-00000e80: 2c20 7573 6572 2069 6e20 656e 756d 6572  , user in enumer
-00000e90: 6174 6528 6566 6669 6369 656e 6379 5f74  ate(efficiency_t
-00000ea0: 6f70 2e75 7365 7273 293a 0d0a 2020 2020  op.users):..    
-00000eb0: 7072 696e 7428 6622 237b 6e75 6d62 6572  print(f"#{number
-00000ec0: 2b31 7d20 2020 7b75 7365 722e 6e61 6d65  +1}   {user.name
-00000ed0: 7d20 287b 7573 6572 2e74 6f70 5f76 616c  } ({user.top_val
-00000ee0: 7565 7d29 2229 0d0a 6060 600d 0a0d 0a23  ue})")..```....#
-00000ef0: 2323 2323 2320 4765 7474 696e 6720 696e  ##### Getting in
-00000f00: 666f 726d 6174 696f 6e20 6f66 2070 6c61  formation of pla
-00000f10: 7965 720d 0a60 6060 7079 0d0a 696d 706f  yer..```py..impo
-00000f20: 7274 2061 7379 6e63 696f 0d0a 6672 6f6d  rt asyncio..from
-00000f30: 2074 6f61 7069 2069 6d70 6f72 7420 5573   toapi import Us
-00000f40: 6572 2c20 6765 745f 7573 6572 0d0a 0d0a  er, get_user....
-00000f50: 7573 6572 203d 2061 7379 6e63 696f 2e72  user = asyncio.r
-00000f60: 756e 2867 6574 5f75 7365 7228 2273 7479  un(get_user("sty
-00000f70: 2229 290d 0a23 2061 6e64 2059 6f75 2063  "))..# and You c
-00000f80: 616e 2073 7065 6369 6679 206c 616e 6775  an specify langu
-00000f90: 6167 650d 0a23 2075 7365 7220 3d20 6173  age..# user = as
-00000fa0: 796e 6369 6f2e 7275 6e28 6765 745f 7573  yncio.run(get_us
-00000fb0: 6572 2822 7374 7922 2c20 6c61 6e67 3d22  er("sty", lang="
-00000fc0: 7275 2229 290d 0a0d 0a70 7269 6e74 2866  ru"))....print(f
-00000fd0: 224e 616d 653a 207b 7573 6572 2e6e 616d  "Name: {user.nam
-00000fe0: 657d 2229 0d0a 7261 6e6b 3a20 7374 7220  e}")..rank: str 
-00000ff0: 3d20 7573 6572 2e72 616e 6b2e 6e61 6d65  = user.rank.name
-00001000: 2e74 6974 6c65 2829 0d0a 7072 696e 7428  .title()..print(
-00001010: 6622 5261 6e6b 3a20 7b72 616e 6b7d 2028  f"Rank: {rank} (
-00001020: 7b75 7365 722e 7363 6f72 657d 2f7b 7573  {user.score}/{us
-00001030: 6572 2e73 636f 7265 5f6e 6578 747d 207b  er.score_next} {
-00001040: 726f 756e 6428 7573 6572 2e73 636f 7265  round(user.score
-00001050: 2f75 7365 722e 7363 6f72 655f 6e65 7874  /user.score_next
-00001060: 2a31 3030 297d 2529 2229 0d0a 7072 696e  *100)}%)")..prin
-00001070: 7428 6622 4861 7320 7072 656d 6975 6d3a  t(f"Has premium:
-00001080: 207b 2759 6573 2720 6966 2075 7365 722e   {'Yes' if user.
-00001090: 7072 656d 6975 6d20 656c 7365 2027 4e6f  premium else 'No
-000010a0: 277d 2229 0d0a 7072 696e 7428 290d 0a70  '}")..print()..p
-000010b0: 7269 6e74 2866 224b 443a 207b 7573 6572  rint(f"KD: {user
-000010c0: 2e6b 696c 6c73 7d2f 7b75 7365 722e 6465  .kills}/{user.de
-000010d0: 6174 6873 7d20 287b 7573 6572 2e6b 645f  aths} ({user.kd_
-000010e0: 7261 7469 6f7d 2922 290d 0a70 7269 6e74  ratio})")..print
-000010f0: 2866 2243 6175 6768 7420 676f 6c64 733a  (f"Caught golds:
-00001100: 207b 7573 6572 2e63 6175 6768 745f 676f   {user.caught_go
-00001110: 6c64 737d 2229 0d0a 7072 696e 7428 6622  lds}")..print(f"
-00001120: 4372 7973 7461 6c73 3a20 7b75 7365 722e  Crystals: {user.
-00001130: 6372 7973 7461 6c73 7d22 290d 0a70 7269  crystals}")..pri
-00001140: 6e74 2866 2247 533a 207b 7573 6572 2e67  nt(f"GS: {user.g
-00001150: 6561 725f 7363 6f72 657d 2229 0d0a 6060  ear_score}")..``
-00001160: 600d 0a0d 0a23 2320 4c69 6365 6e73 650d  `....## License.
-00001170: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
-00001180: 2064 6973 7472 6962 7574 6564 2075 6e64   distributed und
-00001190: 6572 2074 6865 2060 4d49 5460 206c 6963  er the `MIT` lic
-000011a0: 656e 7365 2e20 596f 7520 6361 6e20 6c65  ense. You can le
-000011b0: 6172 6e20 6d6f 7265 2066 726f 6d20 7468  arn more from th
-000011c0: 6520 5b2a 2a4c 4943 454e 5345 2a2a 5d28  e [**LICENSE**](
-000011d0: 2f4c 4943 454e 5345 2920 6669 6c65 2e0d  /LICENSE) file..
-000011e0: 0a                                       .
+000001d0: 6f61 7069 0d0a 5072 6f6a 6563 742d 5552  oapi..Project-UR
+000001e0: 4c3a 2043 6861 6e67 656c 6f67 2c20 6874  L: Changelog, ht
+000001f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000200: 2f73 746e 6775 6c61 7269 7479 2f74 616e  /stngularity/tan
+00000210: 6b69 6f61 7069 2f62 6c6f 622f 6d61 696e  kioapi/blob/main
+00000220: 2f43 4841 4e47 454c 4f47 2e6d 640d 0a50  /CHANGELOG.md..P
+00000230: 726f 6a65 6374 2d55 524c 3a20 4275 6720  roject-URL: Bug 
+00000240: 5472 6163 6b65 722c 2068 7474 7073 3a2f  Tracker, https:/
+00000250: 2f67 6974 6875 622e 636f 6d2f 7374 6e67  /github.com/stng
+00000260: 756c 6172 6974 792f 7461 6e6b 696f 6170  ularity/tankioap
+00000270: 692f 6973 7375 6573 0d0a 4b65 7977 6f72  i/issues..Keywor
+00000280: 6473 3a20 6761 6d65 2c61 7069 2c74 6f2c  ds: game,api,to,
+00000290: 7461 6e6b 6920 6f6e 6c69 6e65 0d0a 436c  tanki online..Cl
+000002a0: 6173 7369 6669 6572 3a20 4465 7665 6c6f  assifier: Develo
+000002b0: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+000002c0: 3520 2d20 5072 6f64 7563 7469 6f6e 2f53  5 - Production/S
+000002d0: 7461 626c 650d 0a43 6c61 7373 6966 6965  table..Classifie
+000002e0: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
+000002f0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+00000300: 5420 4c69 6365 6e73 650d 0a43 6c61 7373  T License..Class
+00000310: 6966 6965 723a 204e 6174 7572 616c 204c  ifier: Natural L
+00000320: 616e 6775 6167 6520 3a3a 2045 6e67 6c69  anguage :: Engli
+00000330: 7368 0d0a 436c 6173 7369 6669 6572 3a20  sh..Classifier: 
+00000340: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000350: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+00000360: 6e74 0d0a 436c 6173 7369 6669 6572 3a20  nt..Classifier: 
+00000370: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000380: 7561 6765 203a 3a20 5079 7468 6f6e 0d0a  uage :: Python..
+00000390: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000003a0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000003b0: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
+000003c0: 3a3a 204f 6e6c 790d 0a43 6c61 7373 6966  :: Only..Classif
+000003d0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000003e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000003f0: 686f 6e20 3a3a 2033 2e38 0d0a 436c 6173  hon :: 3.8..Clas
+00000400: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000410: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000420: 5079 7468 6f6e 203a 3a20 332e 390d 0a43  Python :: 3.9..C
+00000430: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000440: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000450: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000460: 300d 0a43 6c61 7373 6966 6965 723a 2050  0..Classifier: P
+00000470: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000480: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000490: 2033 2e31 310d 0a43 6c61 7373 6966 6965   3.11..Classifie
+000004a0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000004b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000004c0: 6e20 3a3a 2049 6d70 6c65 6d65 6e74 6174  n :: Implementat
+000004d0: 696f 6e20 3a3a 2043 5079 7468 6f6e 0d0a  ion :: CPython..
+000004e0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+000004f0: 6320 3a3a 2055 7469 6c69 7469 6573 0d0a  c :: Utilities..
+00000500: 436c 6173 7369 6669 6572 3a20 5479 7069  Classifier: Typi
+00000510: 6e67 203a 3a20 5479 7065 640d 0a52 6571  ng :: Typed..Req
+00000520: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
+00000530: 332e 380d 0a44 6573 6372 6970 7469 6f6e  3.8..Description
+00000540: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+00000550: 6578 742f 6d61 726b 646f 776e 0d0a 5072  ext/markdown..Pr
+00000560: 6f76 6964 6573 2d45 7874 7261 3a20 7370  ovides-Extra: sp
+00000570: 6565 6475 700d 0a50 726f 7669 6465 732d  eedup..Provides-
+00000580: 4578 7472 613a 2064 6576 0d0a 4c69 6365  Extra: dev..Lice
+00000590: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
+000005a0: 450d 0a0d 0a3c 7020 616c 6967 6e3d 6365  E....<p align=ce
+000005b0: 6e74 6572 3e0d 0a20 2020 203c 6120 6872  nter>..    <a hr
+000005c0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000005d0: 7562 2e63 6f6d 2f73 746e 6775 6c61 7269  ub.com/stngulari
+000005e0: 7479 223e 3c69 6d67 2073 7263 3d22 6874  ty"><img src="ht
+000005f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000600: 732e 696f 2f62 6164 6765 2f2d 7374 6e67  s.io/badge/-stng
+00000610: 756c 6172 6974 7927 7325 3230 7072 6f6a  ularity's%20proj
+00000620: 6563 742d 2532 3334 3664 6631 3122 3e3c  ect-%2346df11"><
+00000630: 2f61 3e0d 0a20 2020 203c 6120 6872 6566  /a>..    <a href
+00000640: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
+00000650: 7267 2f70 726f 6a65 6374 2f74 616e 6b69  rg/project/tanki
+00000660: 6f61 7069 2f22 3e3c 696d 6720 7372 633d  oapi/"><img src=
+00000670: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000680: 656c 6473 2e69 6f2f 7079 7069 2f76 2f74  elds.io/pypi/v/t
+00000690: 616e 6b69 6f61 7069 3f63 6f6c 6f72 3d25  ankioapi?color=%
+000006a0: 3233 3436 6466 3131 266c 6162 656c 3d56  2346df11&label=V
+000006b0: 6572 7369 6f6e 223e 3c2f 613e 0d0a 2020  ersion"></a>..  
+000006c0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000006d0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000006e0: 6563 742f 7461 6e6b 696f 6170 692f 223e  ect/tankioapi/">
+000006f0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000700: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000710: 2f70 7970 692f 6464 2f74 616e 6b69 6f61  /pypi/dd/tankioa
+00000720: 7069 3f63 6f6c 6f72 3d25 3233 3436 6466  pi?color=%2346df
+00000730: 3131 266c 6162 656c 3d44 6f77 6e6c 6f61  11&label=Downloa
+00000740: 6473 223e 3c2f 613e 0d0a 3c2f 703e 0d0a  ds"></a>..</p>..
+00000750: 3c70 2061 6c69 676e 3d63 656e 7465 723e  <p align=center>
+00000760: 0d0a 2020 2020 3c61 2068 7265 663d 2268  ..    <a href="h
+00000770: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000780: 6d2f 7374 6e67 756c 6172 6974 792f 7461  m/stngularity/ta
+00000790: 6e6b 696f 6170 692f 6973 7375 6573 223e  nkioapi/issues">
+000007a0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000007b0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000007c0: 2f67 6974 6875 622f 6973 7375 6573 2f73  /github/issues/s
+000007d0: 746e 6775 6c61 7269 7479 2f74 616e 6b69  tngularity/tanki
+000007e0: 6f61 7069 3f63 6f6c 6f72 3d25 3233 3436  oapi?color=%2346
+000007f0: 6466 3131 266c 6162 656c 3d49 7373 7565  df11&label=Issue
+00000800: 7322 3e3c 2f61 3e0d 0a20 2020 203c 6120  s"></a>..    <a 
+00000810: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000820: 7468 7562 2e63 6f6d 2f73 746e 6775 6c61  thub.com/stngula
+00000830: 7269 7479 2f74 616e 6b69 6f61 7069 223e  rity/tankioapi">
+00000840: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000850: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000860: 2f67 6974 6875 622f 6c69 6365 6e73 652f  /github/license/
+00000870: 7374 6e67 756c 6172 6974 792f 7461 6e6b  stngularity/tank
+00000880: 696f 6170 693f 636f 6c6f 723d 2532 3334  ioapi?color=%234
+00000890: 3664 6631 3126 6c61 6265 6c3d 4c69 6365  6df11&label=Lice
+000008a0: 6e73 6522 3e3c 2f61 3e0d 0a3c 2f70 3e0d  nse"></a>..</p>.
+000008b0: 0a0d 0a23 2320 4e6f 7469 6669 6361 7469  ...## Notificati
+000008c0: 6f6e 0d0a 5468 6973 2070 726f 6a65 6374  on..This project
+000008d0: 2077 6173 2063 7265 6174 6564 206a 7573   was created jus
+000008e0: 7420 746f 2065 7869 7374 2e20 4f66 2063  t to exist. Of c
+000008f0: 6f75 7273 652c 2049 2077 696c 6c20 7570  ourse, I will up
+00000900: 6461 7465 2069 7420 7768 656e 2074 6865  date it when the
+00000910: 2041 5049 2069 7473 656c 6620 6368 616e   API itself chan
+00000920: 6765 732c 2062 7574 206e 6f74 2069 6d6d  ges, but not imm
+00000930: 6564 6961 7465 6c79 2e20 5765 6c6c 2c20  ediately. Well, 
+00000940: 6966 2059 6f75 2077 616e 7420 746f 2073  if You want to s
+00000950: 7570 706f 7274 2074 6869 7320 7072 6f6a  upport this proj
+00000960: 6563 742c 2059 6f75 2063 616e 2067 6976  ect, You can giv
+00000970: 6520 6974 2061 2073 7461 722e 0d0a 0d0a  e it a star.....
+00000980: 2323 2049 6e66 6f72 6d61 7469 6f6e 0d0a  ## Information..
+00000990: 4173 206d 656e 7469 6f6e 6564 2065 6172  As mentioned ear
+000009a0: 6c69 6572 2c20 7468 6973 2070 726f 6a65  lier, this proje
+000009b0: 6374 2069 7320 6372 6561 7465 6420 6a75  ct is created ju
+000009c0: 7374 2074 6f20 6578 6973 742e 2041 6e64  st to exist. And
+000009d0: 2073 6f2c 2074 6865 206d 6f64 756c 6520   so, the module 
+000009e0: 6974 7365 6c66 2069 7320 6e65 6564 6564  itself is needed
+000009f0: 2074 6f20 6765 7420 7468 6520 746f 7020   to get the top 
+00000a00: 6f66 2070 6c61 7965 7273 2061 6e64 2067  of players and g
+00000a10: 6574 2069 6e66 6f72 6d61 7469 6f6e 2061  et information a
+00000a20: 626f 7574 2074 6865 2070 6c61 7965 7220  bout the player 
+00000a30: 7365 7061 7261 7465 6c79 2e20 4966 2059  separately. If Y
+00000a40: 6f75 206b 6e6f 7720 6d6f 7265 2066 756e  ou know more fun
+00000a50: 6374 696f 6e61 6c69 7479 206f 6620 7468  ctionality of th
+00000a60: 6520 4150 4920 6f66 2074 6865 2067 616d  e API of the gam
+00000a70: 6520 6054 616e 6b69 204f 6e6c 696e 6560  e `Tanki Online`
+00000a80: 2c20 7468 656e 2070 6c65 6173 6520 7265  , then please re
+00000a90: 706f 7274 2074 6869 7320 6675 6e63 7469  port this functi
+00000aa0: 6f6e 616c 6974 7920 696e 2074 6865 205b  onality in the [
+00000ab0: 6049 7373 7565 7360 5d28 6874 7470 733a  `Issues`](https:
+00000ac0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 746e  //github.com/stn
+00000ad0: 6775 6c61 7269 7479 2f74 616e 6b69 6f61  gularity/tankioa
+00000ae0: 7069 2f69 7373 7565 7329 2e0d 0a0d 0a23  pi/issues).....#
+00000af0: 2323 2323 2320 4665 6174 7572 6573 0d0a  ##### Features..
+00000b00: 2d20 4675 6c6c 7920 6061 7379 6e63 602f  - Fully `async`/
+00000b10: 6061 7761 6974 600d 0a2d 2047 6574 7469  `await`..- Getti
+00000b20: 6e67 2074 6f70 206f 6620 706c 6179 6572  ng top of player
+00000b30: 730d 0a2d 2047 6574 7469 6e67 2069 6e66  s..- Getting inf
+00000b40: 6f72 6d61 7469 6f6e 206f 6620 616e 7920  ormation of any 
+00000b50: 706c 6179 6572 2062 7920 6869 6d20 6e61  player by him na
+00000b60: 6d65 0d0a 2d20 4765 7474 696e 6720 7374  me..- Getting st
+00000b70: 6174 7573 206f 6620 7374 6162 6c65 2073  atus of stable s
+00000b80: 6572 7665 7220 604d 6179 6265 2064 6570  erver `Maybe dep
+00000b90: 7265 6361 7465 6460 0d0a 2d20 4765 7474  recated`..- Gett
+00000ba0: 696e 6720 7374 6174 7573 206f 6620 7465  ing status of te
+00000bb0: 7374 2073 6572 7665 7273 0d0a 0d0a 2323  st servers....##
+00000bc0: 2049 6e73 7461 6c6c 696e 670d 0a2a 2a5b   Installing..**[
+00000bd0: 5079 7468 6f6e 2033 2e38 5d28 6874 7470  Python 3.8](http
+00000be0: 733a 2f2f 7777 772e 7079 7468 6f6e 2e6f  s://www.python.o
+00000bf0: 7267 2f64 6f77 6e6c 6f61 6473 2f29 206f  rg/downloads/) o
+00000c00: 7220 6869 6768 6572 2069 7320 7265 7175  r higher is requ
+00000c10: 6972 6564 2a2a 0d0a 0d0a 546f 2069 6e73  ired**....To ins
+00000c20: 7461 6c6c 2061 206e 6f6e 2d60 7370 6565  tall a non-`spee
+00000c30: 6475 7060 2076 6572 7369 6f6e 206f 6620  dup` version of 
+00000c40: 7468 6520 6c69 6272 6172 792c 2064 6f20  the library, do 
+00000c50: 7468 6520 666f 6c6c 6f77 696e 673a 0d0a  the following:..
+00000c60: 3e20 6060 6073 680d 0a3e 2023 204c 696e  > ```sh..> # Lin
+00000c70: 7578 2f6d 6163 4f53 0d0a 3e20 7079 7468  ux/macOS..> pyth
+00000c80: 6f6e 3320 2d6d 2070 6970 2069 6e73 7461  on3 -m pip insta
+00000c90: 6c6c 202d 5520 7461 6e6b 696f 6170 690d  ll -U tankioapi.
+00000ca0: 0a3e 0d0a 3e20 2320 5769 6e64 6f77 730d  .>..> # Windows.
+00000cb0: 0a3e 2070 7920 2d33 202d 6d20 7069 7020  .> py -3 -m pip 
+00000cc0: 696e 7374 616c 6c20 2d55 2074 616e 6b69  install -U tanki
+00000cd0: 6f61 7069 0d0a 3e20 6060 600d 0a0d 0a4f  oapi..> ```....O
+00000ce0: 722c 2074 6f20 696e 7374 616c 6c20 7468  r, to install th
+00000cf0: 6520 6073 7065 6564 7570 6020 7665 7273  e `speedup` vers
+00000d00: 696f 6e2c 2064 6f20 7468 6520 666f 6c6c  ion, do the foll
+00000d10: 6f77 696e 673a 0d0a 3e20 6060 6073 680d  owing:..> ```sh.
+00000d20: 0a3e 2023 204c 696e 7578 2f6d 6163 4f53  .> # Linux/macOS
+00000d30: 0d0a 3e20 7079 7468 6f6e 3320 2d6d 2070  ..> python3 -m p
+00000d40: 6970 2069 6e73 7461 6c6c 202d 5520 2274  ip install -U "t
+00000d50: 616e 6b69 6f61 7069 5b73 7065 6564 7570  ankioapi[speedup
+00000d60: 5d22 0d0a 3e0d 0a3e 2023 2057 696e 646f  ]"..>..> # Windo
+00000d70: 7773 0d0a 3e20 7079 202d 3320 2d6d 2070  ws..> py -3 -m p
+00000d80: 6970 2069 6e73 7461 6c6c 202d 5520 7461  ip install -U ta
+00000d90: 6e6b 696f 6170 695b 7370 6565 6475 705d  nkioapi[speedup]
+00000da0: 0d0a 3e20 6060 600d 0a0d 0a41 6e64 2c20  ..> ```....And, 
+00000db0: 746f 2069 6e73 7461 6c6c 2074 6865 2064  to install the d
+00000dc0: 6576 656c 6f70 6d65 6e74 2076 6572 7369  evelopment versi
+00000dd0: 6f6e 2c20 646f 2074 6865 2066 6f6c 6c6f  on, do the follo
+00000de0: 7769 6e67 3a0d 0a3e 2060 6060 7368 0d0a  wing:..> ```sh..
+00000df0: 3e20 2420 6769 7420 636c 6f6e 6520 6874  > $ git clone ht
+00000e00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000e10: 2f73 746e 6775 6c61 7269 7479 2f74 616e  /stngularity/tan
+00000e20: 6b69 6f61 7069 0d0a 3e20 2420 6364 2074  kioapi..> $ cd t
+00000e30: 616e 6b69 6f61 7069 0d0a 3e20 2420 7079  ankioapi..> $ py
+00000e40: 7468 6f6e 3320 2d6d 2070 6970 2069 6e73  thon3 -m pip ins
+00000e50: 7461 6c6c 202d 5520 2e5b 7370 6565 6475  tall -U .[speedu
+00000e60: 705d 0d0a 3e20 6060 600d 0a0d 0a23 2320  p]..> ```....## 
+00000e70: 4578 616d 706c 6573 0d0a 4865 7265 2061  Examples..Here a
+00000e80: 7265 2065 7861 6d70 6c65 7320 6f66 2073  re examples of s
+00000e90: 6f6d 6520 6f66 2074 6865 2066 6561 7475  ome of the featu
+00000ea0: 7265 7320 6f66 2074 6865 206c 6962 7261  res of the libra
+00000eb0: 7279 2e20 4d6f 7265 2065 7861 6d70 6c65  ry. More example
+00000ec0: 7320 696e 205b 6065 7861 6d70 6c65 732f  s in [`examples/
+00000ed0: 605d 282f 6578 616d 706c 6573 290d 0a0d  `](/examples)...
+00000ee0: 0a23 2323 2323 2320 4765 7474 696e 6720  .###### Getting 
+00000ef0: 616c 6c20 746f 7073 206f 6620 706c 6179  all tops of play
+00000f00: 6572 730d 0a60 6060 7079 0d0a 696d 706f  ers..```py..impo
+00000f10: 7274 2061 7379 6e63 696f 0d0a 6672 6f6d  rt asyncio..from
+00000f20: 2074 6f61 7069 2069 6d70 6f72 7420 546f   toapi import To
+00000f30: 702c 2054 6f70 4c69 7374 732c 2067 6574  p, TopLists, get
+00000f40: 5f74 6f70 730d 0a0d 0a74 6f70 733a 2054  _tops....tops: T
+00000f50: 6f70 4c69 7374 7320 3d20 6173 796e 6369  opLists = asynci
+00000f60: 6f2e 7275 6e28 6765 745f 746f 7073 2829  o.run(get_tops()
+00000f70: 290d 0a65 6666 6963 6965 6e63 795f 746f  )..efficiency_to
+00000f80: 703a 2054 6f70 203d 2074 6f70 732e 6566  p: Top = tops.ef
+00000f90: 6669 6369 656e 6379 0d0a 7072 696e 7428  ficiency..print(
+00000fa0: 222d 2d2d 2d2d 2045 6666 6963 6965 6e63  "----- Efficienc
+00000fb0: 7920 746f 7020 2d2d 2d2d 2d22 290d 0a66  y top -----")..f
+00000fc0: 6f72 206e 756d 6265 722c 2075 7365 7220  or number, user 
+00000fd0: 696e 2065 6e75 6d65 7261 7465 2865 6666  in enumerate(eff
+00000fe0: 6963 6965 6e63 795f 746f 702e 7573 6572  iciency_top.user
+00000ff0: 7329 3a0d 0a20 2020 2070 7269 6e74 2866  s):..    print(f
+00001000: 2223 7b6e 756d 6265 722b 317d 2020 207b  "#{number+1}   {
+00001010: 7573 6572 2e6e 616d 657d 2028 7b75 7365  user.name} ({use
+00001020: 722e 746f 705f 7661 6c75 657d 2922 290d  r.top_value})").
+00001030: 0a60 6060 0d0a 0d0a 2323 2323 2323 2047  .```....###### G
+00001040: 6574 7469 6e67 2069 6e66 6f72 6d61 7469  etting informati
+00001050: 6f6e 206f 6620 706c 6179 6572 0d0a 6060  on of player..``
+00001060: 6070 790d 0a69 6d70 6f72 7420 6173 796e  `py..import asyn
+00001070: 6369 6f0d 0a66 726f 6d20 746f 6170 6920  cio..from toapi 
+00001080: 696d 706f 7274 2055 7365 722c 2067 6574  import User, get
+00001090: 5f75 7365 720d 0a0d 0a75 7365 723a 2055  _user....user: U
+000010a0: 7365 7220 3d20 6173 796e 6369 6f2e 7275  ser = asyncio.ru
+000010b0: 6e28 6765 745f 7573 6572 2822 7374 7922  n(get_user("sty"
+000010c0: 2929 0d0a 2320 616e 6420 596f 7520 6361  ))..# and You ca
+000010d0: 6e20 7370 6563 6966 7920 6c61 6e67 7561  n specify langua
+000010e0: 6765 0d0a 2320 7573 6572 3a20 5573 6572  ge..# user: User
+000010f0: 203d 2061 7379 6e63 696f 2e72 756e 2867   = asyncio.run(g
+00001100: 6574 5f75 7365 7228 2273 7479 222c 206c  et_user("sty", l
+00001110: 616e 673d 2272 7522 2929 0d0a 0d0a 7072  ang="ru"))....pr
+00001120: 696e 7428 6622 4e61 6d65 3a20 7b75 7365  int(f"Name: {use
+00001130: 722e 6e61 6d65 7d22 290d 0a72 616e 6b3a  r.name}")..rank:
+00001140: 2073 7472 203d 2075 7365 722e 7261 6e6b   str = user.rank
+00001150: 2e6e 616d 652e 7469 746c 6528 290d 0a70  .name.title()..p
+00001160: 7269 6e74 2866 2252 616e 6b3a 207b 7261  rint(f"Rank: {ra
+00001170: 6e6b 7d20 287b 7573 6572 2e73 636f 7265  nk} ({user.score
+00001180: 7d2f 7b75 7365 722e 7363 6f72 655f 6e65  }/{user.score_ne
+00001190: 7874 7d20 7b72 6f75 6e64 2875 7365 722e  xt} {round(user.
+000011a0: 7363 6f72 652f 7573 6572 2e73 636f 7265  score/user.score
+000011b0: 5f6e 6578 742a 3130 3029 7d25 2922 290d  _next*100)}%)").
+000011c0: 0a70 7269 6e74 2866 2248 6173 2070 7265  .print(f"Has pre
+000011d0: 6d69 756d 3a20 7b27 5965 7327 2069 6620  mium: {'Yes' if 
+000011e0: 7573 6572 2e70 7265 6d69 756d 2065 6c73  user.premium els
+000011f0: 6520 274e 6f27 7d22 290d 0a70 7269 6e74  e 'No'}")..print
+00001200: 2829 0d0a 7072 696e 7428 6622 4b44 3a20  ()..print(f"KD: 
+00001210: 7b75 7365 722e 6b69 6c6c 737d 2f7b 7573  {user.kills}/{us
+00001220: 6572 2e64 6561 7468 737d 2028 7b75 7365  er.deaths} ({use
+00001230: 722e 6b64 5f72 6174 696f 7d29 2229 0d0a  r.kd_ratio})")..
+00001240: 7072 696e 7428 6622 4361 7567 6874 2067  print(f"Caught g
+00001250: 6f6c 6473 3a20 7b75 7365 722e 6361 7567  olds: {user.caug
+00001260: 6874 5f67 6f6c 6473 7d22 290d 0a70 7269  ht_golds}")..pri
+00001270: 6e74 2866 2243 7279 7374 616c 733a 207b  nt(f"Crystals: {
+00001280: 7573 6572 2e63 7279 7374 616c 737d 2229  user.crystals}")
+00001290: 0d0a 7072 696e 7428 6622 4753 3a20 7b75  ..print(f"GS: {u
+000012a0: 7365 722e 6765 6172 5f73 636f 7265 7d22  ser.gear_score}"
+000012b0: 290d 0a60 6060 0d0a 0d0a 2323 204c 6963  )..```....## Lic
+000012c0: 656e 7365 0d0a 5468 6973 2070 726f 6a65  ense..This proje
+000012d0: 6374 2069 7320 6469 7374 7269 6275 7465  ct is distribute
+000012e0: 6420 756e 6465 7220 7468 6520 604d 4954  d under the `MIT
+000012f0: 6020 6c69 6365 6e73 652e 2059 6f75 2063  ` license. You c
+00001300: 616e 206c 6561 726e 206d 6f72 6520 6672  an learn more fr
+00001310: 6f6d 2074 6865 205b 2a2a 4c49 4345 4e53  om the [**LICENS
+00001320: 452a 2a5d 282f 4c49 4345 4e53 4529 2066  E**](/LICENSE) f
+00001330: 696c 652e 0d0a 0d0a 6060 600d 0a4d 6164  ile.....```..Mad
+00001340: 6520 7769 7468 20e2 9da4 2061 6e64 20f0  e with ... and .
+00001350: 9f8d b520 6279 2073 746e 6775 6c61 7269  ... by stngulari
+00001360: 7479 2066 6f72 2065 7665 7279 6f6e 650d  ty for everyone.
+00001370: 0a60 6060 0d0a                           .```..
```

### Comparing `tankioapi-1.0.0/README.md` & `tankioapi-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,200 +1,221 @@
 00000000: 3c70 2061 6c69 676e 3d63 656e 7465 723e  <p align=center>
-00000010: 0d0a 2020 2020 3c69 6d67 2073 7263 3d22  ..    <img src="
-00000020: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000030: 6c64 732e 696f 2f62 6164 6765 2f2d 7374  lds.io/badge/-st
-00000040: 6e67 756c 6172 6974 7927 7325 3230 776f  ngularity's%20wo
-00000050: 726b 2d25 3233 3436 6466 3131 223e 0d0a  rk-%2346df11">..
-00000060: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-00000070: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000080: 732e 696f 2f70 7970 692f 762f 7461 6e6b  s.io/pypi/v/tank
-00000090: 696f 6170 693f 636f 6c6f 723d 2532 3334  ioapi?color=%234
-000000a0: 3664 6631 3126 6c61 6265 6c3d 5665 7273  6df11&label=Vers
-000000b0: 696f 6e22 3e0d 0a20 2020 203c 696d 6720  ion">..    <img 
-000000c0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000000d0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-000000e0: 2f64 642f 7461 6e6b 696f 6170 693f 636f  /dd/tankioapi?co
-000000f0: 6c6f 723d 2532 3334 3664 6631 3126 6c61  lor=%2346df11&la
-00000100: 6265 6c3d 446f 776e 6c6f 6164 7322 3e0d  bel=Downloads">.
-00000110: 0a3c 2f70 3e0d 0a3c 7020 616c 6967 6e3d  .</p>..<p align=
-00000120: 6365 6e74 6572 3e0d 0a20 2020 203c 696d  center>..    <im
-00000130: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-00000140: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-00000150: 7468 7562 2f69 7373 7565 732f 7374 6e67  thub/issues/stng
-00000160: 756c 6172 6974 792f 7461 6e6b 696f 6170  ularity/tankioap
-00000170: 693f 636f 6c6f 723d 2532 3334 3664 6631  i?color=%2346df1
-00000180: 3126 6c61 6265 6c3d 4973 7375 6573 223e  1&label=Issues">
-00000190: 0d0a 2020 2020 3c69 6d67 2073 7263 3d22  ..    <img src="
-000001a0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000001b0: 6c64 732e 696f 2f67 6974 6875 622f 6c69  lds.io/github/li
-000001c0: 6365 6e73 652f 7374 6e67 756c 6172 6974  cense/stngularit
-000001d0: 792f 7461 6e6b 696f 6170 693f 636f 6c6f  y/tankioapi?colo
-000001e0: 723d 2532 3334 3664 6631 3126 6c61 6265  r=%2346df11&labe
-000001f0: 6c3d 4c69 6365 6e73 6522 3e0d 0a3c 2f70  l=License">..</p
-00000200: 3e0d 0a0d 0a23 2320 4e6f 7469 6669 6361  >....## Notifica
-00000210: 7469 6f6e 0d0a 5468 6973 2070 726f 6a65  tion..This proje
-00000220: 6374 2077 6173 2063 7265 6174 6564 206a  ct was created j
-00000230: 7573 7420 746f 2065 7869 7374 2e20 4f66  ust to exist. Of
-00000240: 2063 6f75 7273 652c 2049 2077 696c 6c20   course, I will 
-00000250: 7570 6461 7465 2069 7420 7768 656e 2074  update it when t
-00000260: 6865 2041 5049 2069 7473 656c 6620 6368  he API itself ch
-00000270: 616e 6765 732c 2062 7574 206e 6f74 2069  anges, but not i
-00000280: 6d6d 6564 6961 7465 6c79 2e20 5765 6c6c  mmediately. Well
-00000290: 2c20 6966 2059 6f75 2077 616e 7420 746f  , if You want to
-000002a0: 2073 7570 706f 7274 2074 6869 7320 7072   support this pr
-000002b0: 6f6a 6563 742c 2059 6f75 2063 616e 2067  oject, You can g
-000002c0: 6976 6520 6974 2061 2073 7461 722e 0d0a  ive it a star...
-000002d0: 0d0a 2323 2049 6e66 6f72 6d61 7469 6f6e  ..## Information
-000002e0: 0d0a 4173 206d 656e 7469 6f6e 6564 2065  ..As mentioned e
-000002f0: 6172 6c69 6572 2c20 7468 6973 2070 726f  arlier, this pro
-00000300: 6a65 6374 2069 7320 6372 6561 7465 6420  ject is created 
-00000310: 6a75 7374 2074 6f20 6578 6973 742e 2041  just to exist. A
-00000320: 6e64 2073 6f2c 2074 6865 206d 6f64 756c  nd so, the modul
-00000330: 6520 6974 7365 6c66 2069 7320 6e65 6564  e itself is need
-00000340: 6564 2074 6f20 6765 7420 7468 6520 746f  ed to get the to
-00000350: 7020 6f66 2070 6c61 7965 7273 2061 6e64  p of players and
-00000360: 2067 6574 2069 6e66 6f72 6d61 7469 6f6e   get information
-00000370: 2061 626f 7574 2074 6865 2070 6c61 7965   about the playe
-00000380: 7220 7365 7061 7261 7465 6c79 2e20 4966  r separately. If
-00000390: 2059 6f75 206b 6e6f 7720 6d6f 7265 2066   You know more f
-000003a0: 756e 6374 696f 6e61 6c69 7479 206f 6620  unctionality of 
-000003b0: 7468 6520 4150 4920 6f66 2074 6865 2067  the API of the g
-000003c0: 616d 6520 6054 616e 6b69 204f 6e6c 696e  ame `Tanki Onlin
-000003d0: 6560 2c20 7468 656e 2070 6c65 6173 6520  e`, then please 
-000003e0: 7265 706f 7274 2074 6869 7320 6675 6e63  report this func
-000003f0: 7469 6f6e 616c 6974 7920 696e 2074 6865  tionality in the
-00000400: 205b 6049 7373 7565 7360 5d28 6874 7470   [`Issues`](http
-00000410: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00000420: 746e 6775 6c61 7269 7479 2f74 616e 6b69  tngularity/tanki
-00000430: 6f61 7069 2f69 7373 7565 7329 2e0d 0a0d  oapi/issues)....
-00000440: 0a23 2323 2323 2320 4665 6174 7572 6573  .###### Features
-00000450: 0d0a 2d20 4675 6c6c 7920 6061 7379 6e63  ..- Fully `async
-00000460: 602f 6061 7761 6974 600d 0a2d 2047 6574  `/`await`..- Get
-00000470: 7469 6e67 2074 6f70 206f 6620 706c 6179  ting top of play
-00000480: 6572 730d 0a2d 2047 6574 7469 6e67 2069  ers..- Getting i
-00000490: 6e66 6f72 6d61 7469 6f6e 206f 6620 616e  nformation of an
-000004a0: 7920 706c 6179 6572 2062 7920 6869 6d20  y player by him 
-000004b0: 6e61 6d65 0d0a 2d20 4765 7474 696e 6720  name..- Getting 
-000004c0: 7374 6174 7573 206f 6620 7374 6162 6c65  status of stable
-000004d0: 2073 6572 7665 7220 604d 6179 6265 2064   server `Maybe d
-000004e0: 6570 7265 6361 7465 6460 0d0a 2d20 4765  eprecated`..- Ge
-000004f0: 7474 696e 6720 7374 6174 7573 206f 6620  tting status of 
-00000500: 7465 7374 2073 6572 7665 7273 0d0a 0d0a  test servers....
-00000510: 2323 2049 6e73 7461 6c6c 696e 670d 0a2a  ## Installing..*
-00000520: 2a5b 5079 7468 6f6e 2033 2e38 5d28 6874  *[Python 3.8](ht
-00000530: 7470 733a 2f2f 7777 772e 7079 7468 6f6e  tps://www.python
-00000540: 2e6f 7267 2f64 6f77 6e6c 6f61 6473 2f29  .org/downloads/)
-00000550: 206f 7220 6869 6768 6572 2069 7320 7265   or higher is re
-00000560: 7175 6972 6564 2a2a 0d0a 0d0a 546f 2069  quired**....To i
-00000570: 6e73 7461 6c6c 2061 206e 6f6e 2d60 7370  nstall a non-`sp
-00000580: 6565 6475 7060 2076 6572 7369 6f6e 206f  eedup` version o
-00000590: 6620 7468 6520 6c69 6272 6172 792c 2064  f the library, d
-000005a0: 6f20 7468 6520 666f 6c6c 6f77 696e 673a  o the following:
-000005b0: 0d0a 3e20 6060 6073 680d 0a3e 2023 204c  ..> ```sh..> # L
-000005c0: 696e 7578 2f6d 6163 4f53 0d0a 3e20 7079  inux/macOS..> py
-000005d0: 7468 6f6e 3320 2d6d 2070 6970 2069 6e73  thon3 -m pip ins
-000005e0: 7461 6c6c 202d 5520 7461 6e6b 696f 6170  tall -U tankioap
-000005f0: 690d 0a3e 0d0a 3e20 2320 5769 6e64 6f77  i..>..> # Window
-00000600: 730d 0a3e 2070 7920 2d33 202d 6d20 7069  s..> py -3 -m pi
-00000610: 7020 696e 7374 616c 6c20 2d55 2074 616e  p install -U tan
-00000620: 6b69 6f61 7069 0d0a 3e20 6060 600d 0a0d  kioapi..> ```...
-00000630: 0a4f 722c 2074 6f20 696e 7374 616c 6c20  .Or, to install 
-00000640: 7468 6520 6073 7065 6564 7570 6020 7665  the `speedup` ve
-00000650: 7273 696f 6e2c 2064 6f20 7468 6520 666f  rsion, do the fo
-00000660: 6c6c 6f77 696e 673a 0d0a 3e20 6060 6073  llowing:..> ```s
-00000670: 680d 0a3e 2023 204c 696e 7578 2f6d 6163  h..> # Linux/mac
-00000680: 4f53 0d0a 3e20 7079 7468 6f6e 3320 2d6d  OS..> python3 -m
-00000690: 2070 6970 2069 6e73 7461 6c6c 202d 5520   pip install -U 
-000006a0: 2274 616e 6b69 6f61 7069 5b73 7065 6564  "tankioapi[speed
-000006b0: 7570 5d22 0d0a 3e0d 0a3e 2023 2057 696e  up]"..>..> # Win
-000006c0: 646f 7773 0d0a 3e20 7079 202d 3320 2d6d  dows..> py -3 -m
-000006d0: 2070 6970 2069 6e73 7461 6c6c 202d 5520   pip install -U 
-000006e0: 7461 6e6b 696f 6170 695b 7370 6565 6475  tankioapi[speedu
-000006f0: 705d 0d0a 3e20 6060 600d 0a0d 0a41 6e64  p]..> ```....And
-00000700: 2c20 746f 2069 6e73 7461 6c6c 2074 6865  , to install the
-00000710: 2064 6576 656c 6f70 6d65 6e74 2076 6572   development ver
-00000720: 7369 6f6e 2c20 646f 2074 6865 2066 6f6c  sion, do the fol
-00000730: 6c6f 7769 6e67 3a0d 0a3e 2060 6060 7368  lowing:..> ```sh
-00000740: 0d0a 3e20 2420 6769 7420 636c 6f6e 6520  ..> $ git clone 
-00000750: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000760: 6f6d 2f73 746e 6775 6c61 7269 7479 2f74  om/stngularity/t
-00000770: 616e 6b69 6f61 7069 0d0a 3e20 2420 6364  ankioapi..> $ cd
-00000780: 2074 616e 6b69 6f61 7069 0d0a 3e20 2420   tankioapi..> $ 
-00000790: 7079 7468 6f6e 3320 2d6d 2070 6970 2069  python3 -m pip i
-000007a0: 6e73 7461 6c6c 202d 5520 2e5b 7370 6565  nstall -U .[spee
-000007b0: 6475 705d 0d0a 3e20 6060 600d 0a0d 0a23  dup]..> ```....#
-000007c0: 2320 4578 616d 706c 6573 0d0a 4865 7265  # Examples..Here
-000007d0: 2061 7265 2065 7861 6d70 6c65 7320 6f66   are examples of
-000007e0: 2073 6f6d 6520 6f66 2074 6865 2066 6561   some of the fea
-000007f0: 7475 7265 7320 6f66 2074 6865 206c 6962  tures of the lib
-00000800: 7261 7279 2e20 4d6f 7265 2065 7861 6d70  rary. More examp
-00000810: 6c65 7320 696e 205b 6065 7861 6d70 6c65  les in [`example
-00000820: 732f 605d 282f 6578 616d 706c 6573 290d  s/`](/examples).
-00000830: 0a0d 0a23 2323 2323 2320 4765 7474 696e  ...###### Gettin
-00000840: 6720 616c 6c20 746f 7073 206f 6620 706c  g all tops of pl
-00000850: 6179 6572 730d 0a60 6060 7079 0d0a 696d  ayers..```py..im
-00000860: 706f 7274 2061 7379 6e63 696f 0d0a 6672  port asyncio..fr
-00000870: 6f6d 2074 6f61 7069 2069 6d70 6f72 7420  om toapi import 
-00000880: 546f 702c 2054 6f70 4c69 7374 732c 2067  Top, TopLists, g
-00000890: 6574 5f74 6f70 730d 0a0d 0a0d 0a74 6f70  et_tops......top
-000008a0: 733a 2054 6f70 4c69 7374 7320 3d20 6173  s: TopLists = as
-000008b0: 796e 6369 6f2e 7275 6e28 6765 745f 746f  yncio.run(get_to
-000008c0: 7073 2829 290d 0a65 6666 6963 6965 6e63  ps())..efficienc
-000008d0: 795f 746f 703a 2054 6f70 203d 2074 6f70  y_top: Top = top
-000008e0: 732e 6566 6669 6369 656e 6379 0d0a 7072  s.efficiency..pr
-000008f0: 696e 7428 222d 2d2d 2d2d 2045 6666 6963  int("----- Effic
-00000900: 6965 6e63 7920 746f 7020 2d2d 2d2d 2d22  iency top -----"
-00000910: 290d 0a66 6f72 206e 756d 6265 722c 2075  )..for number, u
-00000920: 7365 7220 696e 2065 6e75 6d65 7261 7465  ser in enumerate
-00000930: 2865 6666 6963 6965 6e63 795f 746f 702e  (efficiency_top.
-00000940: 7573 6572 7329 3a0d 0a20 2020 2070 7269  users):..    pri
-00000950: 6e74 2866 2223 7b6e 756d 6265 722b 317d  nt(f"#{number+1}
-00000960: 2020 207b 7573 6572 2e6e 616d 657d 2028     {user.name} (
-00000970: 7b75 7365 722e 746f 705f 7661 6c75 657d  {user.top_value}
-00000980: 2922 290d 0a60 6060 0d0a 0d0a 2323 2323  )")..```....####
-00000990: 2323 2047 6574 7469 6e67 2069 6e66 6f72  ## Getting infor
-000009a0: 6d61 7469 6f6e 206f 6620 706c 6179 6572  mation of player
-000009b0: 0d0a 6060 6070 790d 0a69 6d70 6f72 7420  ..```py..import 
-000009c0: 6173 796e 6369 6f0d 0a66 726f 6d20 746f  asyncio..from to
-000009d0: 6170 6920 696d 706f 7274 2055 7365 722c  api import User,
-000009e0: 2067 6574 5f75 7365 720d 0a0d 0a75 7365   get_user....use
-000009f0: 7220 3d20 6173 796e 6369 6f2e 7275 6e28  r = asyncio.run(
-00000a00: 6765 745f 7573 6572 2822 7374 7922 2929  get_user("sty"))
-00000a10: 0d0a 2320 616e 6420 596f 7520 6361 6e20  ..# and You can 
-00000a20: 7370 6563 6966 7920 6c61 6e67 7561 6765  specify language
-00000a30: 0d0a 2320 7573 6572 203d 2061 7379 6e63  ..# user = async
-00000a40: 696f 2e72 756e 2867 6574 5f75 7365 7228  io.run(get_user(
-00000a50: 2273 7479 222c 206c 616e 673d 2272 7522  "sty", lang="ru"
-00000a60: 2929 0d0a 0d0a 7072 696e 7428 6622 4e61  ))....print(f"Na
-00000a70: 6d65 3a20 7b75 7365 722e 6e61 6d65 7d22  me: {user.name}"
-00000a80: 290d 0a72 616e 6b3a 2073 7472 203d 2075  )..rank: str = u
-00000a90: 7365 722e 7261 6e6b 2e6e 616d 652e 7469  ser.rank.name.ti
-00000aa0: 746c 6528 290d 0a70 7269 6e74 2866 2252  tle()..print(f"R
-00000ab0: 616e 6b3a 207b 7261 6e6b 7d20 287b 7573  ank: {rank} ({us
-00000ac0: 6572 2e73 636f 7265 7d2f 7b75 7365 722e  er.score}/{user.
-00000ad0: 7363 6f72 655f 6e65 7874 7d20 7b72 6f75  score_next} {rou
-00000ae0: 6e64 2875 7365 722e 7363 6f72 652f 7573  nd(user.score/us
-00000af0: 6572 2e73 636f 7265 5f6e 6578 742a 3130  er.score_next*10
-00000b00: 3029 7d25 2922 290d 0a70 7269 6e74 2866  0)}%)")..print(f
-00000b10: 2248 6173 2070 7265 6d69 756d 3a20 7b27  "Has premium: {'
-00000b20: 5965 7327 2069 6620 7573 6572 2e70 7265  Yes' if user.pre
-00000b30: 6d69 756d 2065 6c73 6520 274e 6f27 7d22  mium else 'No'}"
-00000b40: 290d 0a70 7269 6e74 2829 0d0a 7072 696e  )..print()..prin
-00000b50: 7428 6622 4b44 3a20 7b75 7365 722e 6b69  t(f"KD: {user.ki
-00000b60: 6c6c 737d 2f7b 7573 6572 2e64 6561 7468  lls}/{user.death
-00000b70: 737d 2028 7b75 7365 722e 6b64 5f72 6174  s} ({user.kd_rat
-00000b80: 696f 7d29 2229 0d0a 7072 696e 7428 6622  io})")..print(f"
-00000b90: 4361 7567 6874 2067 6f6c 6473 3a20 7b75  Caught golds: {u
-00000ba0: 7365 722e 6361 7567 6874 5f67 6f6c 6473  ser.caught_golds
-00000bb0: 7d22 290d 0a70 7269 6e74 2866 2243 7279  }")..print(f"Cry
-00000bc0: 7374 616c 733a 207b 7573 6572 2e63 7279  stals: {user.cry
-00000bd0: 7374 616c 737d 2229 0d0a 7072 696e 7428  stals}")..print(
-00000be0: 6622 4753 3a20 7b75 7365 722e 6765 6172  f"GS: {user.gear
-00000bf0: 5f73 636f 7265 7d22 290d 0a60 6060 0d0a  _score}")..```..
-00000c00: 0d0a 2323 204c 6963 656e 7365 0d0a 5468  ..## License..Th
-00000c10: 6973 2070 726f 6a65 6374 2069 7320 6469  is project is di
-00000c20: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
-00000c30: 7468 6520 604d 4954 6020 6c69 6365 6e73  the `MIT` licens
-00000c40: 652e 2059 6f75 2063 616e 206c 6561 726e  e. You can learn
-00000c50: 206d 6f72 6520 6672 6f6d 2074 6865 205b   more from the [
-00000c60: 2a2a 4c49 4345 4e53 452a 2a5d 282f 4c49  **LICENSE**](/LI
-00000c70: 4345 4e53 4529 2066 696c 652e            CENSE) file.
+00000010: 0d0a 2020 2020 3c61 2068 7265 663d 2268  ..    <a href="h
+00000020: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000030: 6d2f 7374 6e67 756c 6172 6974 7922 3e3c  m/stngularity"><
+00000040: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000050: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000060: 6261 6467 652f 2d73 746e 6775 6c61 7269  badge/-stngulari
+00000070: 7479 2773 2532 3070 726f 6a65 6374 2d25  ty's%20project-%
+00000080: 3233 3436 6466 3131 223e 3c2f 613e 0d0a  2346df11"></a>..
+00000090: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+000000a0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+000000b0: 6f6a 6563 742f 7461 6e6b 696f 6170 692f  oject/tankioapi/
+000000c0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+000000d0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000000e0: 696f 2f70 7970 692f 762f 7461 6e6b 696f  io/pypi/v/tankio
+000000f0: 6170 693f 636f 6c6f 723d 2532 3334 3664  api?color=%2346d
+00000100: 6631 3126 6c61 6265 6c3d 5665 7273 696f  f11&label=Versio
+00000110: 6e22 3e3c 2f61 3e0d 0a20 2020 203c 6120  n"></a>..    <a 
+00000120: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00000130: 7069 2e6f 7267 2f70 726f 6a65 6374 2f74  pi.org/project/t
+00000140: 616e 6b69 6f61 7069 2f22 3e3c 696d 6720  ankioapi/"><img 
+00000150: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000160: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000170: 2f64 642f 7461 6e6b 696f 6170 693f 636f  /dd/tankioapi?co
+00000180: 6c6f 723d 2532 3334 3664 6631 3126 6c61  lor=%2346df11&la
+00000190: 6265 6c3d 446f 776e 6c6f 6164 7322 3e3c  bel=Downloads"><
+000001a0: 2f61 3e0d 0a3c 2f70 3e0d 0a3c 7020 616c  /a>..</p>..<p al
+000001b0: 6967 6e3d 6365 6e74 6572 3e0d 0a20 2020  ign=center>..   
+000001c0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000001d0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 746e  //github.com/stn
+000001e0: 6775 6c61 7269 7479 2f74 616e 6b69 6f61  gularity/tankioa
+000001f0: 7069 2f69 7373 7565 7322 3e3c 696d 6720  pi/issues"><img 
+00000200: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000210: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000220: 7562 2f69 7373 7565 732f 7374 6e67 756c  ub/issues/stngul
+00000230: 6172 6974 792f 7461 6e6b 696f 6170 693f  arity/tankioapi?
+00000240: 636f 6c6f 723d 2532 3334 3664 6631 3126  color=%2346df11&
+00000250: 6c61 6265 6c3d 4973 7375 6573 223e 3c2f  label=Issues"></
+00000260: 613e 0d0a 2020 2020 3c61 2068 7265 663d  a>..    <a href=
+00000270: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000280: 636f 6d2f 7374 6e67 756c 6172 6974 792f  com/stngularity/
+00000290: 7461 6e6b 696f 6170 6922 3e3c 696d 6720  tankioapi"><img 
+000002a0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000002b0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+000002c0: 7562 2f6c 6963 656e 7365 2f73 746e 6775  ub/license/stngu
+000002d0: 6c61 7269 7479 2f74 616e 6b69 6f61 7069  larity/tankioapi
+000002e0: 3f63 6f6c 6f72 3d25 3233 3436 6466 3131  ?color=%2346df11
+000002f0: 266c 6162 656c 3d4c 6963 656e 7365 223e  &label=License">
+00000300: 3c2f 613e 0d0a 3c2f 703e 0d0a 0d0a 2323  </a>..</p>....##
+00000310: 204e 6f74 6966 6963 6174 696f 6e0d 0a54   Notification..T
+00000320: 6869 7320 7072 6f6a 6563 7420 7761 7320  his project was 
+00000330: 6372 6561 7465 6420 6a75 7374 2074 6f20  created just to 
+00000340: 6578 6973 742e 204f 6620 636f 7572 7365  exist. Of course
+00000350: 2c20 4920 7769 6c6c 2075 7064 6174 6520  , I will update 
+00000360: 6974 2077 6865 6e20 7468 6520 4150 4920  it when the API 
+00000370: 6974 7365 6c66 2063 6861 6e67 6573 2c20  itself changes, 
+00000380: 6275 7420 6e6f 7420 696d 6d65 6469 6174  but not immediat
+00000390: 656c 792e 2057 656c 6c2c 2069 6620 596f  ely. Well, if Yo
+000003a0: 7520 7761 6e74 2074 6f20 7375 7070 6f72  u want to suppor
+000003b0: 7420 7468 6973 2070 726f 6a65 6374 2c20  t this project, 
+000003c0: 596f 7520 6361 6e20 6769 7665 2069 7420  You can give it 
+000003d0: 6120 7374 6172 2e0d 0a0d 0a23 2320 496e  a star.....## In
+000003e0: 666f 726d 6174 696f 6e0d 0a41 7320 6d65  formation..As me
+000003f0: 6e74 696f 6e65 6420 6561 726c 6965 722c  ntioned earlier,
+00000400: 2074 6869 7320 7072 6f6a 6563 7420 6973   this project is
+00000410: 2063 7265 6174 6564 206a 7573 7420 746f   created just to
+00000420: 2065 7869 7374 2e20 416e 6420 736f 2c20   exist. And so, 
+00000430: 7468 6520 6d6f 6475 6c65 2069 7473 656c  the module itsel
+00000440: 6620 6973 206e 6565 6465 6420 746f 2067  f is needed to g
+00000450: 6574 2074 6865 2074 6f70 206f 6620 706c  et the top of pl
+00000460: 6179 6572 7320 616e 6420 6765 7420 696e  ayers and get in
+00000470: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+00000480: 7468 6520 706c 6179 6572 2073 6570 6172  the player separ
+00000490: 6174 656c 792e 2049 6620 596f 7520 6b6e  ately. If You kn
+000004a0: 6f77 206d 6f72 6520 6675 6e63 7469 6f6e  ow more function
+000004b0: 616c 6974 7920 6f66 2074 6865 2041 5049  ality of the API
+000004c0: 206f 6620 7468 6520 6761 6d65 2060 5461   of the game `Ta
+000004d0: 6e6b 6920 4f6e 6c69 6e65 602c 2074 6865  nki Online`, the
+000004e0: 6e20 706c 6561 7365 2072 6570 6f72 7420  n please report 
+000004f0: 7468 6973 2066 756e 6374 696f 6e61 6c69  this functionali
+00000500: 7479 2069 6e20 7468 6520 5b60 4973 7375  ty in the [`Issu
+00000510: 6573 605d 2868 7474 7073 3a2f 2f67 6974  es`](https://git
+00000520: 6875 622e 636f 6d2f 7374 6e67 756c 6172  hub.com/stngular
+00000530: 6974 792f 7461 6e6b 696f 6170 692f 6973  ity/tankioapi/is
+00000540: 7375 6573 292e 0d0a 0d0a 2323 2323 2323  sues).....######
+00000550: 2046 6561 7475 7265 730d 0a2d 2046 756c   Features..- Ful
+00000560: 6c79 2060 6173 796e 6360 2f60 6177 6169  ly `async`/`awai
+00000570: 7460 0d0a 2d20 4765 7474 696e 6720 746f  t`..- Getting to
+00000580: 7020 6f66 2070 6c61 7965 7273 0d0a 2d20  p of players..- 
+00000590: 4765 7474 696e 6720 696e 666f 726d 6174  Getting informat
+000005a0: 696f 6e20 6f66 2061 6e79 2070 6c61 7965  ion of any playe
+000005b0: 7220 6279 2068 696d 206e 616d 650d 0a2d  r by him name..-
+000005c0: 2047 6574 7469 6e67 2073 7461 7475 7320   Getting status 
+000005d0: 6f66 2073 7461 626c 6520 7365 7276 6572  of stable server
+000005e0: 2060 4d61 7962 6520 6465 7072 6563 6174   `Maybe deprecat
+000005f0: 6564 600d 0a2d 2047 6574 7469 6e67 2073  ed`..- Getting s
+00000600: 7461 7475 7320 6f66 2074 6573 7420 7365  tatus of test se
+00000610: 7276 6572 730d 0a0d 0a23 2320 496e 7374  rvers....## Inst
+00000620: 616c 6c69 6e67 0d0a 2a2a 5b50 7974 686f  alling..**[Pytho
+00000630: 6e20 332e 385d 2868 7474 7073 3a2f 2f77  n 3.8](https://w
+00000640: 7777 2e70 7974 686f 6e2e 6f72 672f 646f  ww.python.org/do
+00000650: 776e 6c6f 6164 732f 2920 6f72 2068 6967  wnloads/) or hig
+00000660: 6865 7220 6973 2072 6571 7569 7265 642a  her is required*
+00000670: 2a0d 0a0d 0a54 6f20 696e 7374 616c 6c20  *....To install 
+00000680: 6120 6e6f 6e2d 6073 7065 6564 7570 6020  a non-`speedup` 
+00000690: 7665 7273 696f 6e20 6f66 2074 6865 206c  version of the l
+000006a0: 6962 7261 7279 2c20 646f 2074 6865 2066  ibrary, do the f
+000006b0: 6f6c 6c6f 7769 6e67 3a0d 0a3e 2060 6060  ollowing:..> ```
+000006c0: 7368 0d0a 3e20 2320 4c69 6e75 782f 6d61  sh..> # Linux/ma
+000006d0: 634f 530d 0a3e 2070 7974 686f 6e33 202d  cOS..> python3 -
+000006e0: 6d20 7069 7020 696e 7374 616c 6c20 2d55  m pip install -U
+000006f0: 2074 616e 6b69 6f61 7069 0d0a 3e0d 0a3e   tankioapi..>..>
+00000700: 2023 2057 696e 646f 7773 0d0a 3e20 7079   # Windows..> py
+00000710: 202d 3320 2d6d 2070 6970 2069 6e73 7461   -3 -m pip insta
+00000720: 6c6c 202d 5520 7461 6e6b 696f 6170 690d  ll -U tankioapi.
+00000730: 0a3e 2060 6060 0d0a 0d0a 4f72 2c20 746f  .> ```....Or, to
+00000740: 2069 6e73 7461 6c6c 2074 6865 2060 7370   install the `sp
+00000750: 6565 6475 7060 2076 6572 7369 6f6e 2c20  eedup` version, 
+00000760: 646f 2074 6865 2066 6f6c 6c6f 7769 6e67  do the following
+00000770: 3a0d 0a3e 2060 6060 7368 0d0a 3e20 2320  :..> ```sh..> # 
+00000780: 4c69 6e75 782f 6d61 634f 530d 0a3e 2070  Linux/macOS..> p
+00000790: 7974 686f 6e33 202d 6d20 7069 7020 696e  ython3 -m pip in
+000007a0: 7374 616c 6c20 2d55 2022 7461 6e6b 696f  stall -U "tankio
+000007b0: 6170 695b 7370 6565 6475 705d 220d 0a3e  api[speedup]"..>
+000007c0: 0d0a 3e20 2320 5769 6e64 6f77 730d 0a3e  ..> # Windows..>
+000007d0: 2070 7920 2d33 202d 6d20 7069 7020 696e   py -3 -m pip in
+000007e0: 7374 616c 6c20 2d55 2074 616e 6b69 6f61  stall -U tankioa
+000007f0: 7069 5b73 7065 6564 7570 5d0d 0a3e 2060  pi[speedup]..> `
+00000800: 6060 0d0a 0d0a 416e 642c 2074 6f20 696e  ``....And, to in
+00000810: 7374 616c 6c20 7468 6520 6465 7665 6c6f  stall the develo
+00000820: 706d 656e 7420 7665 7273 696f 6e2c 2064  pment version, d
+00000830: 6f20 7468 6520 666f 6c6c 6f77 696e 673a  o the following:
+00000840: 0d0a 3e20 6060 6073 680d 0a3e 2024 2067  ..> ```sh..> $ g
+00000850: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
+00000860: 2f67 6974 6875 622e 636f 6d2f 7374 6e67  /github.com/stng
+00000870: 756c 6172 6974 792f 7461 6e6b 696f 6170  ularity/tankioap
+00000880: 690d 0a3e 2024 2063 6420 7461 6e6b 696f  i..> $ cd tankio
+00000890: 6170 690d 0a3e 2024 2070 7974 686f 6e33  api..> $ python3
+000008a0: 202d 6d20 7069 7020 696e 7374 616c 6c20   -m pip install 
+000008b0: 2d55 202e 5b73 7065 6564 7570 5d0d 0a3e  -U .[speedup]..>
+000008c0: 2060 6060 0d0a 0d0a 2323 2045 7861 6d70   ```....## Examp
+000008d0: 6c65 730d 0a48 6572 6520 6172 6520 6578  les..Here are ex
+000008e0: 616d 706c 6573 206f 6620 736f 6d65 206f  amples of some o
+000008f0: 6620 7468 6520 6665 6174 7572 6573 206f  f the features o
+00000900: 6620 7468 6520 6c69 6272 6172 792e 204d  f the library. M
+00000910: 6f72 6520 6578 616d 706c 6573 2069 6e20  ore examples in 
+00000920: 5b60 6578 616d 706c 6573 2f60 5d28 2f65  [`examples/`](/e
+00000930: 7861 6d70 6c65 7329 0d0a 0d0a 2323 2323  xamples)....####
+00000940: 2323 2047 6574 7469 6e67 2061 6c6c 2074  ## Getting all t
+00000950: 6f70 7320 6f66 2070 6c61 7965 7273 0d0a  ops of players..
+00000960: 6060 6070 790d 0a69 6d70 6f72 7420 6173  ```py..import as
+00000970: 796e 6369 6f0d 0a66 726f 6d20 746f 6170  yncio..from toap
+00000980: 6920 696d 706f 7274 2054 6f70 2c20 546f  i import Top, To
+00000990: 704c 6973 7473 2c20 6765 745f 746f 7073  pLists, get_tops
+000009a0: 0d0a 0d0a 746f 7073 3a20 546f 704c 6973  ....tops: TopLis
+000009b0: 7473 203d 2061 7379 6e63 696f 2e72 756e  ts = asyncio.run
+000009c0: 2867 6574 5f74 6f70 7328 2929 0d0a 6566  (get_tops())..ef
+000009d0: 6669 6369 656e 6379 5f74 6f70 3a20 546f  ficiency_top: To
+000009e0: 7020 3d20 746f 7073 2e65 6666 6963 6965  p = tops.efficie
+000009f0: 6e63 790d 0a70 7269 6e74 2822 2d2d 2d2d  ncy..print("----
+00000a00: 2d20 4566 6669 6369 656e 6379 2074 6f70  - Efficiency top
+00000a10: 202d 2d2d 2d2d 2229 0d0a 666f 7220 6e75   -----")..for nu
+00000a20: 6d62 6572 2c20 7573 6572 2069 6e20 656e  mber, user in en
+00000a30: 756d 6572 6174 6528 6566 6669 6369 656e  umerate(efficien
+00000a40: 6379 5f74 6f70 2e75 7365 7273 293a 0d0a  cy_top.users):..
+00000a50: 2020 2020 7072 696e 7428 6622 237b 6e75      print(f"#{nu
+00000a60: 6d62 6572 2b31 7d20 2020 7b75 7365 722e  mber+1}   {user.
+00000a70: 6e61 6d65 7d20 287b 7573 6572 2e74 6f70  name} ({user.top
+00000a80: 5f76 616c 7565 7d29 2229 0d0a 6060 600d  _value})")..```.
+00000a90: 0a0d 0a23 2323 2323 2320 4765 7474 696e  ...###### Gettin
+00000aa0: 6720 696e 666f 726d 6174 696f 6e20 6f66  g information of
+00000ab0: 2070 6c61 7965 720d 0a60 6060 7079 0d0a   player..```py..
+00000ac0: 696d 706f 7274 2061 7379 6e63 696f 0d0a  import asyncio..
+00000ad0: 6672 6f6d 2074 6f61 7069 2069 6d70 6f72  from toapi impor
+00000ae0: 7420 5573 6572 2c20 6765 745f 7573 6572  t User, get_user
+00000af0: 0d0a 0d0a 7573 6572 3a20 5573 6572 203d  ....user: User =
+00000b00: 2061 7379 6e63 696f 2e72 756e 2867 6574   asyncio.run(get
+00000b10: 5f75 7365 7228 2273 7479 2229 290d 0a23  _user("sty"))..#
+00000b20: 2061 6e64 2059 6f75 2063 616e 2073 7065   and You can spe
+00000b30: 6369 6679 206c 616e 6775 6167 650d 0a23  cify language..#
+00000b40: 2075 7365 723a 2055 7365 7220 3d20 6173   user: User = as
+00000b50: 796e 6369 6f2e 7275 6e28 6765 745f 7573  yncio.run(get_us
+00000b60: 6572 2822 7374 7922 2c20 6c61 6e67 3d22  er("sty", lang="
+00000b70: 7275 2229 290d 0a0d 0a70 7269 6e74 2866  ru"))....print(f
+00000b80: 224e 616d 653a 207b 7573 6572 2e6e 616d  "Name: {user.nam
+00000b90: 657d 2229 0d0a 7261 6e6b 3a20 7374 7220  e}")..rank: str 
+00000ba0: 3d20 7573 6572 2e72 616e 6b2e 6e61 6d65  = user.rank.name
+00000bb0: 2e74 6974 6c65 2829 0d0a 7072 696e 7428  .title()..print(
+00000bc0: 6622 5261 6e6b 3a20 7b72 616e 6b7d 2028  f"Rank: {rank} (
+00000bd0: 7b75 7365 722e 7363 6f72 657d 2f7b 7573  {user.score}/{us
+00000be0: 6572 2e73 636f 7265 5f6e 6578 747d 207b  er.score_next} {
+00000bf0: 726f 756e 6428 7573 6572 2e73 636f 7265  round(user.score
+00000c00: 2f75 7365 722e 7363 6f72 655f 6e65 7874  /user.score_next
+00000c10: 2a31 3030 297d 2529 2229 0d0a 7072 696e  *100)}%)")..prin
+00000c20: 7428 6622 4861 7320 7072 656d 6975 6d3a  t(f"Has premium:
+00000c30: 207b 2759 6573 2720 6966 2075 7365 722e   {'Yes' if user.
+00000c40: 7072 656d 6975 6d20 656c 7365 2027 4e6f  premium else 'No
+00000c50: 277d 2229 0d0a 7072 696e 7428 290d 0a70  '}")..print()..p
+00000c60: 7269 6e74 2866 224b 443a 207b 7573 6572  rint(f"KD: {user
+00000c70: 2e6b 696c 6c73 7d2f 7b75 7365 722e 6465  .kills}/{user.de
+00000c80: 6174 6873 7d20 287b 7573 6572 2e6b 645f  aths} ({user.kd_
+00000c90: 7261 7469 6f7d 2922 290d 0a70 7269 6e74  ratio})")..print
+00000ca0: 2866 2243 6175 6768 7420 676f 6c64 733a  (f"Caught golds:
+00000cb0: 207b 7573 6572 2e63 6175 6768 745f 676f   {user.caught_go
+00000cc0: 6c64 737d 2229 0d0a 7072 696e 7428 6622  lds}")..print(f"
+00000cd0: 4372 7973 7461 6c73 3a20 7b75 7365 722e  Crystals: {user.
+00000ce0: 6372 7973 7461 6c73 7d22 290d 0a70 7269  crystals}")..pri
+00000cf0: 6e74 2866 2247 533a 207b 7573 6572 2e67  nt(f"GS: {user.g
+00000d00: 6561 725f 7363 6f72 657d 2229 0d0a 6060  ear_score}")..``
+00000d10: 600d 0a0d 0a23 2320 4c69 6365 6e73 650d  `....## License.
+00000d20: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
+00000d30: 2064 6973 7472 6962 7574 6564 2075 6e64   distributed und
+00000d40: 6572 2074 6865 2060 4d49 5460 206c 6963  er the `MIT` lic
+00000d50: 656e 7365 2e20 596f 7520 6361 6e20 6c65  ense. You can le
+00000d60: 6172 6e20 6d6f 7265 2066 726f 6d20 7468  arn more from th
+00000d70: 6520 5b2a 2a4c 4943 454e 5345 2a2a 5d28  e [**LICENSE**](
+00000d80: 2f4c 4943 454e 5345 2920 6669 6c65 2e0d  /LICENSE) file..
+00000d90: 0a0d 0a60 6060 0d0a 4d61 6465 2077 6974  ...```..Made wit
+00000da0: 6820 e29d a420 616e 6420 f09f 8db5 2062  h ... and .... b
+00000db0: 7920 7374 6e67 756c 6172 6974 7920 666f  y stngularity fo
+00000dc0: 7220 6576 6572 796f 6e65 0d0a 6060 60    r everyone..```
```

### Comparing `tankioapi-1.0.0/pyproject.toml` & `tankioapi-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,18 +25,19 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Utilities",
     "Typing :: Typed"
 ]
 
 [project.urls]
-"Homepage"    = "https://github.com/stngularity/tankioapi"
-"Source Code" = "https://github.com/stngularity/tankioapi"
-"Changelog"   = "https://github.com/stngularity/tankioapi/blob/main/CHANGELOG.md"
-"Bug Tracker" = "https://github.com/stngularity/tankioapi/issues"
+"Documentation" = "https://stngularity.github.io/tankioapi"
+"Homepage"      = "https://github.com/stngularity/tankioapi"
+"Source Code"   = "https://github.com/stngularity/tankioapi"
+"Changelog"     = "https://github.com/stngularity/tankioapi/blob/main/CHANGELOG.md"
+"Bug Tracker"   = "https://github.com/stngularity/tankioapi/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["toapi*"]
 namespaces = false
 
 # The configuration for "iSort" tool
```

### Comparing `tankioapi-1.0.0/setup.py` & `tankioapi-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,17 @@
         license="MIT",
         packages=find_packages("src", include=["toapi*"]),
 
         description="A Python written wrapper for the Tanki Online game API",
         long_description=README,
         long_description_content_type="text/markdown",
 
-        url="https://github.com/stngularity/tankioapi.py",
+        url="https://github.com/stngularity/tankioapi",
         project_urls={
+            "Documentation": "https://stngularity.github.io/tankioapi",
             "Homepage": "https://github.com/stngularity/tankioapi",
             "Source Code": "https://github.com/stngularity/tankioapi",
             "Changelog": "https://github.com/stngularity/tankioapi/blob/main/CHANGELOG.md",
             "Bug Tracker": "https://github.com/stngularity/tankioapi/issues"
         },
 
         python_requires=">=3.8",
@@ -64,14 +65,15 @@
 
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "License :: OSI Approved :: MIT License",
             "Natural Language :: English",
             "Operating System :: OS Independent",
             "Programming Language :: Python",
+            "Programming Language :: Python :: 3",
             "Programming Language :: Python :: 3 :: Only",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
             "Programming Language :: Python :: Implementation :: CPython",
             "Topic :: Utilities",
```

### Comparing `tankioapi-1.0.0/src/tankioapi.egg-info/PKG-INFO` & `tankioapi-1.0.1/src/tankioapi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,287 +1,312 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2074 616e  : 2.1..Name: tan
 00000020: 6b69 6f61 7069 0d0a 5665 7273 696f 6e3a  kioapi..Version:
-00000030: 2031 2e30 2e30 0d0a 5375 6d6d 6172 793a   1.0.0..Summary:
+00000030: 2031 2e30 2e31 0d0a 5375 6d6d 6172 793a   1.0.1..Summary:
 00000040: 2041 2050 7974 686f 6e20 7772 6974 7465   A Python writte
 00000050: 6e20 7772 6170 7065 7220 666f 7220 7468  n wrapper for th
 00000060: 6520 5461 6e6b 6920 4f6e 6c69 6e65 2067  e Tanki Online g
 00000070: 616d 6520 4150 490d 0a48 6f6d 652d 7061  ame API..Home-pa
 00000080: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
 00000090: 7562 2e63 6f6d 2f73 746e 6775 6c61 7269  ub.com/stngulari
-000000a0: 7479 2f74 616e 6b69 6f61 7069 2e70 790d  ty/tankioapi.py.
-000000b0: 0a41 7574 686f 723a 2073 746e 6775 6c61  .Author: stngula
-000000c0: 7269 7479 0d0a 4175 7468 6f72 2d65 6d61  rity..Author-ema
-000000d0: 696c 3a20 7374 6e67 756c 6172 6974 7920  il: stngularity 
-000000e0: 3c73 746e 6775 6c61 7269 7479 4067 6d61  <stngularity@gma
-000000f0: 696c 2e63 6f6d 3e0d 0a4c 6963 656e 7365  il.com>..License
-00000100: 3a20 4d49 5420 4c69 6365 6e73 650d 0a50  : MIT License..P
-00000110: 726f 6a65 6374 2d55 524c 3a20 486f 6d65  roject-URL: Home
-00000120: 7061 6765 2c20 6874 7470 733a 2f2f 6769  page, https://gi
-00000130: 7468 7562 2e63 6f6d 2f73 746e 6775 6c61  thub.com/stngula
-00000140: 7269 7479 2f74 616e 6b69 6f61 7069 0d0a  rity/tankioapi..
-00000150: 5072 6f6a 6563 742d 5552 4c3a 2053 6f75  Project-URL: Sou
-00000160: 7263 6520 436f 6465 2c20 6874 7470 733a  rce Code, https:
-00000170: 2f2f 6769 7468 7562 2e63 6f6d 2f73 746e  //github.com/stn
-00000180: 6775 6c61 7269 7479 2f74 616e 6b69 6f61  gularity/tankioa
-00000190: 7069 0d0a 5072 6f6a 6563 742d 5552 4c3a  pi..Project-URL:
-000001a0: 2043 6861 6e67 656c 6f67 2c20 6874 7470   Changelog, http
+000000a0: 7479 2f74 616e 6b69 6f61 7069 0d0a 4175  ty/tankioapi..Au
+000000b0: 7468 6f72 3a20 7374 6e67 756c 6172 6974  thor: stngularit
+000000c0: 790d 0a41 7574 686f 722d 656d 6169 6c3a  y..Author-email:
+000000d0: 2073 746e 6775 6c61 7269 7479 203c 7374   stngularity <st
+000000e0: 6e67 756c 6172 6974 7940 676d 6169 6c2e  ngularity@gmail.
+000000f0: 636f 6d3e 0d0a 4c69 6365 6e73 653a 204d  com>..License: M
+00000100: 4954 204c 6963 656e 7365 0d0a 5072 6f6a  IT License..Proj
+00000110: 6563 742d 5552 4c3a 2044 6f63 756d 656e  ect-URL: Documen
+00000120: 7461 7469 6f6e 2c20 6874 7470 733a 2f2f  tation, https://
+00000130: 7374 6e67 756c 6172 6974 792e 6769 7468  stngularity.gith
+00000140: 7562 2e69 6f2f 7461 6e6b 696f 6170 690d  ub.io/tankioapi.
+00000150: 0a50 726f 6a65 6374 2d55 524c 3a20 486f  .Project-URL: Ho
+00000160: 6d65 7061 6765 2c20 6874 7470 733a 2f2f  mepage, https://
+00000170: 6769 7468 7562 2e63 6f6d 2f73 746e 6775  github.com/stngu
+00000180: 6c61 7269 7479 2f74 616e 6b69 6f61 7069  larity/tankioapi
+00000190: 0d0a 5072 6f6a 6563 742d 5552 4c3a 2053  ..Project-URL: S
+000001a0: 6f75 7263 6520 436f 6465 2c20 6874 7470  ource Code, http
 000001b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
 000001c0: 746e 6775 6c61 7269 7479 2f74 616e 6b69  tngularity/tanki
-000001d0: 6f61 7069 2f62 6c6f 622f 6d61 696e 2f43  oapi/blob/main/C
-000001e0: 4841 4e47 454c 4f47 2e6d 640d 0a50 726f  HANGELOG.md..Pro
-000001f0: 6a65 6374 2d55 524c 3a20 4275 6720 5472  ject-URL: Bug Tr
-00000200: 6163 6b65 722c 2068 7474 7073 3a2f 2f67  acker, https://g
-00000210: 6974 6875 622e 636f 6d2f 7374 6e67 756c  ithub.com/stngul
-00000220: 6172 6974 792f 7461 6e6b 696f 6170 692f  arity/tankioapi/
-00000230: 6973 7375 6573 0d0a 4b65 7977 6f72 6473  issues..Keywords
-00000240: 3a20 6761 6d65 2c61 7069 2c74 6f2c 7461  : game,api,to,ta
-00000250: 6e6b 6920 6f6e 6c69 6e65 0d0a 436c 6173  nki online..Clas
-00000260: 7369 6669 6572 3a20 4465 7665 6c6f 706d  sifier: Developm
-00000270: 656e 7420 5374 6174 7573 203a 3a20 3520  ent Status :: 5 
-00000280: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
-00000290: 626c 650d 0a43 6c61 7373 6966 6965 723a  ble..Classifier:
-000002a0: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
-000002b0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-000002c0: 4c69 6365 6e73 650d 0a43 6c61 7373 6966  License..Classif
-000002d0: 6965 723a 204e 6174 7572 616c 204c 616e  ier: Natural Lan
-000002e0: 6775 6167 6520 3a3a 2045 6e67 6c69 7368  guage :: English
-000002f0: 0d0a 436c 6173 7369 6669 6572 3a20 4f70  ..Classifier: Op
-00000300: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-00000310: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-00000320: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
-00000330: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000340: 6765 203a 3a20 5079 7468 6f6e 0d0a 436c  ge :: Python..Cl
-00000350: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000360: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000370: 3a20 5079 7468 6f6e 203a 3a20 3320 3a3a  : Python :: 3 ::
-00000380: 204f 6e6c 790d 0a43 6c61 7373 6966 6965   Only..Classifie
-00000390: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-000003a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000003b0: 6e20 3a3a 2033 2e38 0d0a 436c 6173 7369  n :: 3.8..Classi
-000003c0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000003d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000003e0: 7468 6f6e 203a 3a20 332e 390d 0a43 6c61  thon :: 3.9..Cla
-000003f0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000400: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000410: 2050 7974 686f 6e20 3a3a 2033 2e31 300d   Python :: 3.10.
-00000420: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000430: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000440: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000450: 2e31 310d 0a43 6c61 7373 6966 6965 723a  .11..Classifier:
-00000460: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000470: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000480: 3a3a 2049 6d70 6c65 6d65 6e74 6174 696f  :: Implementatio
-00000490: 6e20 3a3a 2043 5079 7468 6f6e 0d0a 436c  n :: CPython..Cl
-000004a0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-000004b0: 3a3a 2055 7469 6c69 7469 6573 0d0a 436c  :: Utilities..Cl
-000004c0: 6173 7369 6669 6572 3a20 5479 7069 6e67  assifier: Typing
-000004d0: 203a 3a20 5479 7065 640d 0a52 6571 7569   :: Typed..Requi
-000004e0: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
-000004f0: 380d 0a44 6573 6372 6970 7469 6f6e 2d43  8..Description-C
-00000500: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000510: 742f 6d61 726b 646f 776e 0d0a 5072 6f76  t/markdown..Prov
-00000520: 6964 6573 2d45 7874 7261 3a20 7370 6565  ides-Extra: spee
-00000530: 6475 700d 0a50 726f 7669 6465 732d 4578  dup..Provides-Ex
-00000540: 7472 613a 2064 6576 0d0a 4c69 6365 6e73  tra: dev..Licens
-00000550: 652d 4669 6c65 3a20 4c49 4345 4e53 450d  e-File: LICENSE.
-00000560: 0a0d 0a3c 7020 616c 6967 6e3d 6365 6e74  ...<p align=cent
-00000570: 6572 3e0d 0a20 2020 203c 696d 6720 7372  er>..    <img sr
-00000580: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000590: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-000005a0: 2d73 746e 6775 6c61 7269 7479 2773 2532  -stngularity's%2
-000005b0: 3077 6f72 6b2d 2532 3334 3664 6631 3122  0work-%2346df11"
-000005c0: 3e0d 0a20 2020 203c 696d 6720 7372 633d  >..    <img src=
-000005d0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-000005e0: 656c 6473 2e69 6f2f 7079 7069 2f76 2f74  elds.io/pypi/v/t
-000005f0: 616e 6b69 6f61 7069 3f63 6f6c 6f72 3d25  ankioapi?color=%
-00000600: 3233 3436 6466 3131 266c 6162 656c 3d56  2346df11&label=V
-00000610: 6572 7369 6f6e 223e 0d0a 2020 2020 3c69  ersion">..    <i
-00000620: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000630: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-00000640: 7970 692f 6464 2f74 616e 6b69 6f61 7069  ypi/dd/tankioapi
-00000650: 3f63 6f6c 6f72 3d25 3233 3436 6466 3131  ?color=%2346df11
-00000660: 266c 6162 656c 3d44 6f77 6e6c 6f61 6473  &label=Downloads
-00000670: 223e 0d0a 3c2f 703e 0d0a 3c70 2061 6c69  ">..</p>..<p ali
-00000680: 676e 3d63 656e 7465 723e 0d0a 2020 2020  gn=center>..    
-00000690: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000006a0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000006b0: 2f67 6974 6875 622f 6973 7375 6573 2f73  /github/issues/s
-000006c0: 746e 6775 6c61 7269 7479 2f74 616e 6b69  tngularity/tanki
-000006d0: 6f61 7069 3f63 6f6c 6f72 3d25 3233 3436  oapi?color=%2346
-000006e0: 6466 3131 266c 6162 656c 3d49 7373 7565  df11&label=Issue
-000006f0: 7322 3e0d 0a20 2020 203c 696d 6720 7372  s">..    <img sr
-00000700: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000710: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00000720: 2f6c 6963 656e 7365 2f73 746e 6775 6c61  /license/stngula
-00000730: 7269 7479 2f74 616e 6b69 6f61 7069 3f63  rity/tankioapi?c
-00000740: 6f6c 6f72 3d25 3233 3436 6466 3131 266c  olor=%2346df11&l
-00000750: 6162 656c 3d4c 6963 656e 7365 223e 0d0a  abel=License">..
-00000760: 3c2f 703e 0d0a 0d0a 2323 204e 6f74 6966  </p>....## Notif
-00000770: 6963 6174 696f 6e0d 0a54 6869 7320 7072  ication..This pr
-00000780: 6f6a 6563 7420 7761 7320 6372 6561 7465  oject was create
-00000790: 6420 6a75 7374 2074 6f20 6578 6973 742e  d just to exist.
-000007a0: 204f 6620 636f 7572 7365 2c20 4920 7769   Of course, I wi
-000007b0: 6c6c 2075 7064 6174 6520 6974 2077 6865  ll update it whe
-000007c0: 6e20 7468 6520 4150 4920 6974 7365 6c66  n the API itself
-000007d0: 2063 6861 6e67 6573 2c20 6275 7420 6e6f   changes, but no
-000007e0: 7420 696d 6d65 6469 6174 656c 792e 2057  t immediately. W
-000007f0: 656c 6c2c 2069 6620 596f 7520 7761 6e74  ell, if You want
-00000800: 2074 6f20 7375 7070 6f72 7420 7468 6973   to support this
-00000810: 2070 726f 6a65 6374 2c20 596f 7520 6361   project, You ca
-00000820: 6e20 6769 7665 2069 7420 6120 7374 6172  n give it a star
-00000830: 2e0d 0a0d 0a23 2320 496e 666f 726d 6174  .....## Informat
-00000840: 696f 6e0d 0a41 7320 6d65 6e74 696f 6e65  ion..As mentione
-00000850: 6420 6561 726c 6965 722c 2074 6869 7320  d earlier, this 
-00000860: 7072 6f6a 6563 7420 6973 2063 7265 6174  project is creat
-00000870: 6564 206a 7573 7420 746f 2065 7869 7374  ed just to exist
-00000880: 2e20 416e 6420 736f 2c20 7468 6520 6d6f  . And so, the mo
-00000890: 6475 6c65 2069 7473 656c 6620 6973 206e  dule itself is n
-000008a0: 6565 6465 6420 746f 2067 6574 2074 6865  eeded to get the
-000008b0: 2074 6f70 206f 6620 706c 6179 6572 7320   top of players 
-000008c0: 616e 6420 6765 7420 696e 666f 726d 6174  and get informat
-000008d0: 696f 6e20 6162 6f75 7420 7468 6520 706c  ion about the pl
-000008e0: 6179 6572 2073 6570 6172 6174 656c 792e  ayer separately.
-000008f0: 2049 6620 596f 7520 6b6e 6f77 206d 6f72   If You know mor
-00000900: 6520 6675 6e63 7469 6f6e 616c 6974 7920  e functionality 
-00000910: 6f66 2074 6865 2041 5049 206f 6620 7468  of the API of th
-00000920: 6520 6761 6d65 2060 5461 6e6b 6920 4f6e  e game `Tanki On
-00000930: 6c69 6e65 602c 2074 6865 6e20 706c 6561  line`, then plea
-00000940: 7365 2072 6570 6f72 7420 7468 6973 2066  se report this f
-00000950: 756e 6374 696f 6e61 6c69 7479 2069 6e20  unctionality in 
-00000960: 7468 6520 5b60 4973 7375 6573 605d 2868  the [`Issues`](h
-00000970: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000980: 6d2f 7374 6e67 756c 6172 6974 792f 7461  m/stngularity/ta
-00000990: 6e6b 696f 6170 692f 6973 7375 6573 292e  nkioapi/issues).
-000009a0: 0d0a 0d0a 2323 2323 2323 2046 6561 7475  ....###### Featu
-000009b0: 7265 730d 0a2d 2046 756c 6c79 2060 6173  res..- Fully `as
-000009c0: 796e 6360 2f60 6177 6169 7460 0d0a 2d20  ync`/`await`..- 
-000009d0: 4765 7474 696e 6720 746f 7020 6f66 2070  Getting top of p
-000009e0: 6c61 7965 7273 0d0a 2d20 4765 7474 696e  layers..- Gettin
-000009f0: 6720 696e 666f 726d 6174 696f 6e20 6f66  g information of
-00000a00: 2061 6e79 2070 6c61 7965 7220 6279 2068   any player by h
-00000a10: 696d 206e 616d 650d 0a2d 2047 6574 7469  im name..- Getti
-00000a20: 6e67 2073 7461 7475 7320 6f66 2073 7461  ng status of sta
-00000a30: 626c 6520 7365 7276 6572 2060 4d61 7962  ble server `Mayb
-00000a40: 6520 6465 7072 6563 6174 6564 600d 0a2d  e deprecated`..-
-00000a50: 2047 6574 7469 6e67 2073 7461 7475 7320   Getting status 
-00000a60: 6f66 2074 6573 7420 7365 7276 6572 730d  of test servers.
-00000a70: 0a0d 0a23 2320 496e 7374 616c 6c69 6e67  ...## Installing
-00000a80: 0d0a 2a2a 5b50 7974 686f 6e20 332e 385d  ..**[Python 3.8]
-00000a90: 2868 7474 7073 3a2f 2f77 7777 2e70 7974  (https://www.pyt
-00000aa0: 686f 6e2e 6f72 672f 646f 776e 6c6f 6164  hon.org/download
-00000ab0: 732f 2920 6f72 2068 6967 6865 7220 6973  s/) or higher is
-00000ac0: 2072 6571 7569 7265 642a 2a0d 0a0d 0a54   required**....T
-00000ad0: 6f20 696e 7374 616c 6c20 6120 6e6f 6e2d  o install a non-
-00000ae0: 6073 7065 6564 7570 6020 7665 7273 696f  `speedup` versio
-00000af0: 6e20 6f66 2074 6865 206c 6962 7261 7279  n of the library
-00000b00: 2c20 646f 2074 6865 2066 6f6c 6c6f 7769  , do the followi
-00000b10: 6e67 3a0d 0a3e 2060 6060 7368 0d0a 3e20  ng:..> ```sh..> 
-00000b20: 2320 4c69 6e75 782f 6d61 634f 530d 0a3e  # Linux/macOS..>
-00000b30: 2070 7974 686f 6e33 202d 6d20 7069 7020   python3 -m pip 
-00000b40: 696e 7374 616c 6c20 2d55 2074 616e 6b69  install -U tanki
-00000b50: 6f61 7069 0d0a 3e0d 0a3e 2023 2057 696e  oapi..>..> # Win
-00000b60: 646f 7773 0d0a 3e20 7079 202d 3320 2d6d  dows..> py -3 -m
-00000b70: 2070 6970 2069 6e73 7461 6c6c 202d 5520   pip install -U 
-00000b80: 7461 6e6b 696f 6170 690d 0a3e 2060 6060  tankioapi..> ```
-00000b90: 0d0a 0d0a 4f72 2c20 746f 2069 6e73 7461  ....Or, to insta
-00000ba0: 6c6c 2074 6865 2060 7370 6565 6475 7060  ll the `speedup`
-00000bb0: 2076 6572 7369 6f6e 2c20 646f 2074 6865   version, do the
-00000bc0: 2066 6f6c 6c6f 7769 6e67 3a0d 0a3e 2060   following:..> `
-00000bd0: 6060 7368 0d0a 3e20 2320 4c69 6e75 782f  ``sh..> # Linux/
-00000be0: 6d61 634f 530d 0a3e 2070 7974 686f 6e33  macOS..> python3
-00000bf0: 202d 6d20 7069 7020 696e 7374 616c 6c20   -m pip install 
-00000c00: 2d55 2022 7461 6e6b 696f 6170 695b 7370  -U "tankioapi[sp
-00000c10: 6565 6475 705d 220d 0a3e 0d0a 3e20 2320  eedup]"..>..> # 
-00000c20: 5769 6e64 6f77 730d 0a3e 2070 7920 2d33  Windows..> py -3
-00000c30: 202d 6d20 7069 7020 696e 7374 616c 6c20   -m pip install 
-00000c40: 2d55 2074 616e 6b69 6f61 7069 5b73 7065  -U tankioapi[spe
-00000c50: 6564 7570 5d0d 0a3e 2060 6060 0d0a 0d0a  edup]..> ```....
-00000c60: 416e 642c 2074 6f20 696e 7374 616c 6c20  And, to install 
-00000c70: 7468 6520 6465 7665 6c6f 706d 656e 7420  the development 
-00000c80: 7665 7273 696f 6e2c 2064 6f20 7468 6520  version, do the 
-00000c90: 666f 6c6c 6f77 696e 673a 0d0a 3e20 6060  following:..> ``
-00000ca0: 6073 680d 0a3e 2024 2067 6974 2063 6c6f  `sh..> $ git clo
-00000cb0: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
-00000cc0: 622e 636f 6d2f 7374 6e67 756c 6172 6974  b.com/stngularit
-00000cd0: 792f 7461 6e6b 696f 6170 690d 0a3e 2024  y/tankioapi..> $
-00000ce0: 2063 6420 7461 6e6b 696f 6170 690d 0a3e   cd tankioapi..>
-00000cf0: 2024 2070 7974 686f 6e33 202d 6d20 7069   $ python3 -m pi
-00000d00: 7020 696e 7374 616c 6c20 2d55 202e 5b73  p install -U .[s
-00000d10: 7065 6564 7570 5d0d 0a3e 2060 6060 0d0a  peedup]..> ```..
-00000d20: 0d0a 2323 2045 7861 6d70 6c65 730d 0a48  ..## Examples..H
-00000d30: 6572 6520 6172 6520 6578 616d 706c 6573  ere are examples
-00000d40: 206f 6620 736f 6d65 206f 6620 7468 6520   of some of the 
-00000d50: 6665 6174 7572 6573 206f 6620 7468 6520  features of the 
-00000d60: 6c69 6272 6172 792e 204d 6f72 6520 6578  library. More ex
-00000d70: 616d 706c 6573 2069 6e20 5b60 6578 616d  amples in [`exam
-00000d80: 706c 6573 2f60 5d28 2f65 7861 6d70 6c65  ples/`](/example
-00000d90: 7329 0d0a 0d0a 2323 2323 2323 2047 6574  s)....###### Get
-00000da0: 7469 6e67 2061 6c6c 2074 6f70 7320 6f66  ting all tops of
-00000db0: 2070 6c61 7965 7273 0d0a 6060 6070 790d   players..```py.
-00000dc0: 0a69 6d70 6f72 7420 6173 796e 6369 6f0d  .import asyncio.
-00000dd0: 0a66 726f 6d20 746f 6170 6920 696d 706f  .from toapi impo
-00000de0: 7274 2054 6f70 2c20 546f 704c 6973 7473  rt Top, TopLists
-00000df0: 2c20 6765 745f 746f 7073 0d0a 0d0a 0d0a  , get_tops......
-00000e00: 746f 7073 3a20 546f 704c 6973 7473 203d  tops: TopLists =
-00000e10: 2061 7379 6e63 696f 2e72 756e 2867 6574   asyncio.run(get
-00000e20: 5f74 6f70 7328 2929 0d0a 6566 6669 6369  _tops())..effici
-00000e30: 656e 6379 5f74 6f70 3a20 546f 7020 3d20  ency_top: Top = 
-00000e40: 746f 7073 2e65 6666 6963 6965 6e63 790d  tops.efficiency.
-00000e50: 0a70 7269 6e74 2822 2d2d 2d2d 2d20 4566  .print("----- Ef
-00000e60: 6669 6369 656e 6379 2074 6f70 202d 2d2d  ficiency top ---
-00000e70: 2d2d 2229 0d0a 666f 7220 6e75 6d62 6572  --")..for number
-00000e80: 2c20 7573 6572 2069 6e20 656e 756d 6572  , user in enumer
-00000e90: 6174 6528 6566 6669 6369 656e 6379 5f74  ate(efficiency_t
-00000ea0: 6f70 2e75 7365 7273 293a 0d0a 2020 2020  op.users):..    
-00000eb0: 7072 696e 7428 6622 237b 6e75 6d62 6572  print(f"#{number
-00000ec0: 2b31 7d20 2020 7b75 7365 722e 6e61 6d65  +1}   {user.name
-00000ed0: 7d20 287b 7573 6572 2e74 6f70 5f76 616c  } ({user.top_val
-00000ee0: 7565 7d29 2229 0d0a 6060 600d 0a0d 0a23  ue})")..```....#
-00000ef0: 2323 2323 2320 4765 7474 696e 6720 696e  ##### Getting in
-00000f00: 666f 726d 6174 696f 6e20 6f66 2070 6c61  formation of pla
-00000f10: 7965 720d 0a60 6060 7079 0d0a 696d 706f  yer..```py..impo
-00000f20: 7274 2061 7379 6e63 696f 0d0a 6672 6f6d  rt asyncio..from
-00000f30: 2074 6f61 7069 2069 6d70 6f72 7420 5573   toapi import Us
-00000f40: 6572 2c20 6765 745f 7573 6572 0d0a 0d0a  er, get_user....
-00000f50: 7573 6572 203d 2061 7379 6e63 696f 2e72  user = asyncio.r
-00000f60: 756e 2867 6574 5f75 7365 7228 2273 7479  un(get_user("sty
-00000f70: 2229 290d 0a23 2061 6e64 2059 6f75 2063  "))..# and You c
-00000f80: 616e 2073 7065 6369 6679 206c 616e 6775  an specify langu
-00000f90: 6167 650d 0a23 2075 7365 7220 3d20 6173  age..# user = as
-00000fa0: 796e 6369 6f2e 7275 6e28 6765 745f 7573  yncio.run(get_us
-00000fb0: 6572 2822 7374 7922 2c20 6c61 6e67 3d22  er("sty", lang="
-00000fc0: 7275 2229 290d 0a0d 0a70 7269 6e74 2866  ru"))....print(f
-00000fd0: 224e 616d 653a 207b 7573 6572 2e6e 616d  "Name: {user.nam
-00000fe0: 657d 2229 0d0a 7261 6e6b 3a20 7374 7220  e}")..rank: str 
-00000ff0: 3d20 7573 6572 2e72 616e 6b2e 6e61 6d65  = user.rank.name
-00001000: 2e74 6974 6c65 2829 0d0a 7072 696e 7428  .title()..print(
-00001010: 6622 5261 6e6b 3a20 7b72 616e 6b7d 2028  f"Rank: {rank} (
-00001020: 7b75 7365 722e 7363 6f72 657d 2f7b 7573  {user.score}/{us
-00001030: 6572 2e73 636f 7265 5f6e 6578 747d 207b  er.score_next} {
-00001040: 726f 756e 6428 7573 6572 2e73 636f 7265  round(user.score
-00001050: 2f75 7365 722e 7363 6f72 655f 6e65 7874  /user.score_next
-00001060: 2a31 3030 297d 2529 2229 0d0a 7072 696e  *100)}%)")..prin
-00001070: 7428 6622 4861 7320 7072 656d 6975 6d3a  t(f"Has premium:
-00001080: 207b 2759 6573 2720 6966 2075 7365 722e   {'Yes' if user.
-00001090: 7072 656d 6975 6d20 656c 7365 2027 4e6f  premium else 'No
-000010a0: 277d 2229 0d0a 7072 696e 7428 290d 0a70  '}")..print()..p
-000010b0: 7269 6e74 2866 224b 443a 207b 7573 6572  rint(f"KD: {user
-000010c0: 2e6b 696c 6c73 7d2f 7b75 7365 722e 6465  .kills}/{user.de
-000010d0: 6174 6873 7d20 287b 7573 6572 2e6b 645f  aths} ({user.kd_
-000010e0: 7261 7469 6f7d 2922 290d 0a70 7269 6e74  ratio})")..print
-000010f0: 2866 2243 6175 6768 7420 676f 6c64 733a  (f"Caught golds:
-00001100: 207b 7573 6572 2e63 6175 6768 745f 676f   {user.caught_go
-00001110: 6c64 737d 2229 0d0a 7072 696e 7428 6622  lds}")..print(f"
-00001120: 4372 7973 7461 6c73 3a20 7b75 7365 722e  Crystals: {user.
-00001130: 6372 7973 7461 6c73 7d22 290d 0a70 7269  crystals}")..pri
-00001140: 6e74 2866 2247 533a 207b 7573 6572 2e67  nt(f"GS: {user.g
-00001150: 6561 725f 7363 6f72 657d 2229 0d0a 6060  ear_score}")..``
-00001160: 600d 0a0d 0a23 2320 4c69 6365 6e73 650d  `....## License.
-00001170: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
-00001180: 2064 6973 7472 6962 7574 6564 2075 6e64   distributed und
-00001190: 6572 2074 6865 2060 4d49 5460 206c 6963  er the `MIT` lic
-000011a0: 656e 7365 2e20 596f 7520 6361 6e20 6c65  ense. You can le
-000011b0: 6172 6e20 6d6f 7265 2066 726f 6d20 7468  arn more from th
-000011c0: 6520 5b2a 2a4c 4943 454e 5345 2a2a 5d28  e [**LICENSE**](
-000011d0: 2f4c 4943 454e 5345 2920 6669 6c65 2e0d  /LICENSE) file..
-000011e0: 0a                                       .
+000001d0: 6f61 7069 0d0a 5072 6f6a 6563 742d 5552  oapi..Project-UR
+000001e0: 4c3a 2043 6861 6e67 656c 6f67 2c20 6874  L: Changelog, ht
+000001f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000200: 2f73 746e 6775 6c61 7269 7479 2f74 616e  /stngularity/tan
+00000210: 6b69 6f61 7069 2f62 6c6f 622f 6d61 696e  kioapi/blob/main
+00000220: 2f43 4841 4e47 454c 4f47 2e6d 640d 0a50  /CHANGELOG.md..P
+00000230: 726f 6a65 6374 2d55 524c 3a20 4275 6720  roject-URL: Bug 
+00000240: 5472 6163 6b65 722c 2068 7474 7073 3a2f  Tracker, https:/
+00000250: 2f67 6974 6875 622e 636f 6d2f 7374 6e67  /github.com/stng
+00000260: 756c 6172 6974 792f 7461 6e6b 696f 6170  ularity/tankioap
+00000270: 692f 6973 7375 6573 0d0a 4b65 7977 6f72  i/issues..Keywor
+00000280: 6473 3a20 6761 6d65 2c61 7069 2c74 6f2c  ds: game,api,to,
+00000290: 7461 6e6b 6920 6f6e 6c69 6e65 0d0a 436c  tanki online..Cl
+000002a0: 6173 7369 6669 6572 3a20 4465 7665 6c6f  assifier: Develo
+000002b0: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+000002c0: 3520 2d20 5072 6f64 7563 7469 6f6e 2f53  5 - Production/S
+000002d0: 7461 626c 650d 0a43 6c61 7373 6966 6965  table..Classifie
+000002e0: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
+000002f0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+00000300: 5420 4c69 6365 6e73 650d 0a43 6c61 7373  T License..Class
+00000310: 6966 6965 723a 204e 6174 7572 616c 204c  ifier: Natural L
+00000320: 616e 6775 6167 6520 3a3a 2045 6e67 6c69  anguage :: Engli
+00000330: 7368 0d0a 436c 6173 7369 6669 6572 3a20  sh..Classifier: 
+00000340: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000350: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+00000360: 6e74 0d0a 436c 6173 7369 6669 6572 3a20  nt..Classifier: 
+00000370: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000380: 7561 6765 203a 3a20 5079 7468 6f6e 0d0a  uage :: Python..
+00000390: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000003a0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000003b0: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
+000003c0: 3a3a 204f 6e6c 790d 0a43 6c61 7373 6966  :: Only..Classif
+000003d0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000003e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000003f0: 686f 6e20 3a3a 2033 2e38 0d0a 436c 6173  hon :: 3.8..Clas
+00000400: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000410: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000420: 5079 7468 6f6e 203a 3a20 332e 390d 0a43  Python :: 3.9..C
+00000430: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000440: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000450: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000460: 300d 0a43 6c61 7373 6966 6965 723a 2050  0..Classifier: P
+00000470: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000480: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000490: 2033 2e31 310d 0a43 6c61 7373 6966 6965   3.11..Classifie
+000004a0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000004b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000004c0: 6e20 3a3a 2049 6d70 6c65 6d65 6e74 6174  n :: Implementat
+000004d0: 696f 6e20 3a3a 2043 5079 7468 6f6e 0d0a  ion :: CPython..
+000004e0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+000004f0: 6320 3a3a 2055 7469 6c69 7469 6573 0d0a  c :: Utilities..
+00000500: 436c 6173 7369 6669 6572 3a20 5479 7069  Classifier: Typi
+00000510: 6e67 203a 3a20 5479 7065 640d 0a52 6571  ng :: Typed..Req
+00000520: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
+00000530: 332e 380d 0a44 6573 6372 6970 7469 6f6e  3.8..Description
+00000540: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+00000550: 6578 742f 6d61 726b 646f 776e 0d0a 5072  ext/markdown..Pr
+00000560: 6f76 6964 6573 2d45 7874 7261 3a20 7370  ovides-Extra: sp
+00000570: 6565 6475 700d 0a50 726f 7669 6465 732d  eedup..Provides-
+00000580: 4578 7472 613a 2064 6576 0d0a 4c69 6365  Extra: dev..Lice
+00000590: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
+000005a0: 450d 0a0d 0a3c 7020 616c 6967 6e3d 6365  E....<p align=ce
+000005b0: 6e74 6572 3e0d 0a20 2020 203c 6120 6872  nter>..    <a hr
+000005c0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000005d0: 7562 2e63 6f6d 2f73 746e 6775 6c61 7269  ub.com/stngulari
+000005e0: 7479 223e 3c69 6d67 2073 7263 3d22 6874  ty"><img src="ht
+000005f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000600: 732e 696f 2f62 6164 6765 2f2d 7374 6e67  s.io/badge/-stng
+00000610: 756c 6172 6974 7927 7325 3230 7072 6f6a  ularity's%20proj
+00000620: 6563 742d 2532 3334 3664 6631 3122 3e3c  ect-%2346df11"><
+00000630: 2f61 3e0d 0a20 2020 203c 6120 6872 6566  /a>..    <a href
+00000640: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
+00000650: 7267 2f70 726f 6a65 6374 2f74 616e 6b69  rg/project/tanki
+00000660: 6f61 7069 2f22 3e3c 696d 6720 7372 633d  oapi/"><img src=
+00000670: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000680: 656c 6473 2e69 6f2f 7079 7069 2f76 2f74  elds.io/pypi/v/t
+00000690: 616e 6b69 6f61 7069 3f63 6f6c 6f72 3d25  ankioapi?color=%
+000006a0: 3233 3436 6466 3131 266c 6162 656c 3d56  2346df11&label=V
+000006b0: 6572 7369 6f6e 223e 3c2f 613e 0d0a 2020  ersion"></a>..  
+000006c0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000006d0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000006e0: 6563 742f 7461 6e6b 696f 6170 692f 223e  ect/tankioapi/">
+000006f0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000700: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000710: 2f70 7970 692f 6464 2f74 616e 6b69 6f61  /pypi/dd/tankioa
+00000720: 7069 3f63 6f6c 6f72 3d25 3233 3436 6466  pi?color=%2346df
+00000730: 3131 266c 6162 656c 3d44 6f77 6e6c 6f61  11&label=Downloa
+00000740: 6473 223e 3c2f 613e 0d0a 3c2f 703e 0d0a  ds"></a>..</p>..
+00000750: 3c70 2061 6c69 676e 3d63 656e 7465 723e  <p align=center>
+00000760: 0d0a 2020 2020 3c61 2068 7265 663d 2268  ..    <a href="h
+00000770: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000780: 6d2f 7374 6e67 756c 6172 6974 792f 7461  m/stngularity/ta
+00000790: 6e6b 696f 6170 692f 6973 7375 6573 223e  nkioapi/issues">
+000007a0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000007b0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000007c0: 2f67 6974 6875 622f 6973 7375 6573 2f73  /github/issues/s
+000007d0: 746e 6775 6c61 7269 7479 2f74 616e 6b69  tngularity/tanki
+000007e0: 6f61 7069 3f63 6f6c 6f72 3d25 3233 3436  oapi?color=%2346
+000007f0: 6466 3131 266c 6162 656c 3d49 7373 7565  df11&label=Issue
+00000800: 7322 3e3c 2f61 3e0d 0a20 2020 203c 6120  s"></a>..    <a 
+00000810: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000820: 7468 7562 2e63 6f6d 2f73 746e 6775 6c61  thub.com/stngula
+00000830: 7269 7479 2f74 616e 6b69 6f61 7069 223e  rity/tankioapi">
+00000840: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000850: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000860: 2f67 6974 6875 622f 6c69 6365 6e73 652f  /github/license/
+00000870: 7374 6e67 756c 6172 6974 792f 7461 6e6b  stngularity/tank
+00000880: 696f 6170 693f 636f 6c6f 723d 2532 3334  ioapi?color=%234
+00000890: 3664 6631 3126 6c61 6265 6c3d 4c69 6365  6df11&label=Lice
+000008a0: 6e73 6522 3e3c 2f61 3e0d 0a3c 2f70 3e0d  nse"></a>..</p>.
+000008b0: 0a0d 0a23 2320 4e6f 7469 6669 6361 7469  ...## Notificati
+000008c0: 6f6e 0d0a 5468 6973 2070 726f 6a65 6374  on..This project
+000008d0: 2077 6173 2063 7265 6174 6564 206a 7573   was created jus
+000008e0: 7420 746f 2065 7869 7374 2e20 4f66 2063  t to exist. Of c
+000008f0: 6f75 7273 652c 2049 2077 696c 6c20 7570  ourse, I will up
+00000900: 6461 7465 2069 7420 7768 656e 2074 6865  date it when the
+00000910: 2041 5049 2069 7473 656c 6620 6368 616e   API itself chan
+00000920: 6765 732c 2062 7574 206e 6f74 2069 6d6d  ges, but not imm
+00000930: 6564 6961 7465 6c79 2e20 5765 6c6c 2c20  ediately. Well, 
+00000940: 6966 2059 6f75 2077 616e 7420 746f 2073  if You want to s
+00000950: 7570 706f 7274 2074 6869 7320 7072 6f6a  upport this proj
+00000960: 6563 742c 2059 6f75 2063 616e 2067 6976  ect, You can giv
+00000970: 6520 6974 2061 2073 7461 722e 0d0a 0d0a  e it a star.....
+00000980: 2323 2049 6e66 6f72 6d61 7469 6f6e 0d0a  ## Information..
+00000990: 4173 206d 656e 7469 6f6e 6564 2065 6172  As mentioned ear
+000009a0: 6c69 6572 2c20 7468 6973 2070 726f 6a65  lier, this proje
+000009b0: 6374 2069 7320 6372 6561 7465 6420 6a75  ct is created ju
+000009c0: 7374 2074 6f20 6578 6973 742e 2041 6e64  st to exist. And
+000009d0: 2073 6f2c 2074 6865 206d 6f64 756c 6520   so, the module 
+000009e0: 6974 7365 6c66 2069 7320 6e65 6564 6564  itself is needed
+000009f0: 2074 6f20 6765 7420 7468 6520 746f 7020   to get the top 
+00000a00: 6f66 2070 6c61 7965 7273 2061 6e64 2067  of players and g
+00000a10: 6574 2069 6e66 6f72 6d61 7469 6f6e 2061  et information a
+00000a20: 626f 7574 2074 6865 2070 6c61 7965 7220  bout the player 
+00000a30: 7365 7061 7261 7465 6c79 2e20 4966 2059  separately. If Y
+00000a40: 6f75 206b 6e6f 7720 6d6f 7265 2066 756e  ou know more fun
+00000a50: 6374 696f 6e61 6c69 7479 206f 6620 7468  ctionality of th
+00000a60: 6520 4150 4920 6f66 2074 6865 2067 616d  e API of the gam
+00000a70: 6520 6054 616e 6b69 204f 6e6c 696e 6560  e `Tanki Online`
+00000a80: 2c20 7468 656e 2070 6c65 6173 6520 7265  , then please re
+00000a90: 706f 7274 2074 6869 7320 6675 6e63 7469  port this functi
+00000aa0: 6f6e 616c 6974 7920 696e 2074 6865 205b  onality in the [
+00000ab0: 6049 7373 7565 7360 5d28 6874 7470 733a  `Issues`](https:
+00000ac0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 746e  //github.com/stn
+00000ad0: 6775 6c61 7269 7479 2f74 616e 6b69 6f61  gularity/tankioa
+00000ae0: 7069 2f69 7373 7565 7329 2e0d 0a0d 0a23  pi/issues).....#
+00000af0: 2323 2323 2320 4665 6174 7572 6573 0d0a  ##### Features..
+00000b00: 2d20 4675 6c6c 7920 6061 7379 6e63 602f  - Fully `async`/
+00000b10: 6061 7761 6974 600d 0a2d 2047 6574 7469  `await`..- Getti
+00000b20: 6e67 2074 6f70 206f 6620 706c 6179 6572  ng top of player
+00000b30: 730d 0a2d 2047 6574 7469 6e67 2069 6e66  s..- Getting inf
+00000b40: 6f72 6d61 7469 6f6e 206f 6620 616e 7920  ormation of any 
+00000b50: 706c 6179 6572 2062 7920 6869 6d20 6e61  player by him na
+00000b60: 6d65 0d0a 2d20 4765 7474 696e 6720 7374  me..- Getting st
+00000b70: 6174 7573 206f 6620 7374 6162 6c65 2073  atus of stable s
+00000b80: 6572 7665 7220 604d 6179 6265 2064 6570  erver `Maybe dep
+00000b90: 7265 6361 7465 6460 0d0a 2d20 4765 7474  recated`..- Gett
+00000ba0: 696e 6720 7374 6174 7573 206f 6620 7465  ing status of te
+00000bb0: 7374 2073 6572 7665 7273 0d0a 0d0a 2323  st servers....##
+00000bc0: 2049 6e73 7461 6c6c 696e 670d 0a2a 2a5b   Installing..**[
+00000bd0: 5079 7468 6f6e 2033 2e38 5d28 6874 7470  Python 3.8](http
+00000be0: 733a 2f2f 7777 772e 7079 7468 6f6e 2e6f  s://www.python.o
+00000bf0: 7267 2f64 6f77 6e6c 6f61 6473 2f29 206f  rg/downloads/) o
+00000c00: 7220 6869 6768 6572 2069 7320 7265 7175  r higher is requ
+00000c10: 6972 6564 2a2a 0d0a 0d0a 546f 2069 6e73  ired**....To ins
+00000c20: 7461 6c6c 2061 206e 6f6e 2d60 7370 6565  tall a non-`spee
+00000c30: 6475 7060 2076 6572 7369 6f6e 206f 6620  dup` version of 
+00000c40: 7468 6520 6c69 6272 6172 792c 2064 6f20  the library, do 
+00000c50: 7468 6520 666f 6c6c 6f77 696e 673a 0d0a  the following:..
+00000c60: 3e20 6060 6073 680d 0a3e 2023 204c 696e  > ```sh..> # Lin
+00000c70: 7578 2f6d 6163 4f53 0d0a 3e20 7079 7468  ux/macOS..> pyth
+00000c80: 6f6e 3320 2d6d 2070 6970 2069 6e73 7461  on3 -m pip insta
+00000c90: 6c6c 202d 5520 7461 6e6b 696f 6170 690d  ll -U tankioapi.
+00000ca0: 0a3e 0d0a 3e20 2320 5769 6e64 6f77 730d  .>..> # Windows.
+00000cb0: 0a3e 2070 7920 2d33 202d 6d20 7069 7020  .> py -3 -m pip 
+00000cc0: 696e 7374 616c 6c20 2d55 2074 616e 6b69  install -U tanki
+00000cd0: 6f61 7069 0d0a 3e20 6060 600d 0a0d 0a4f  oapi..> ```....O
+00000ce0: 722c 2074 6f20 696e 7374 616c 6c20 7468  r, to install th
+00000cf0: 6520 6073 7065 6564 7570 6020 7665 7273  e `speedup` vers
+00000d00: 696f 6e2c 2064 6f20 7468 6520 666f 6c6c  ion, do the foll
+00000d10: 6f77 696e 673a 0d0a 3e20 6060 6073 680d  owing:..> ```sh.
+00000d20: 0a3e 2023 204c 696e 7578 2f6d 6163 4f53  .> # Linux/macOS
+00000d30: 0d0a 3e20 7079 7468 6f6e 3320 2d6d 2070  ..> python3 -m p
+00000d40: 6970 2069 6e73 7461 6c6c 202d 5520 2274  ip install -U "t
+00000d50: 616e 6b69 6f61 7069 5b73 7065 6564 7570  ankioapi[speedup
+00000d60: 5d22 0d0a 3e0d 0a3e 2023 2057 696e 646f  ]"..>..> # Windo
+00000d70: 7773 0d0a 3e20 7079 202d 3320 2d6d 2070  ws..> py -3 -m p
+00000d80: 6970 2069 6e73 7461 6c6c 202d 5520 7461  ip install -U ta
+00000d90: 6e6b 696f 6170 695b 7370 6565 6475 705d  nkioapi[speedup]
+00000da0: 0d0a 3e20 6060 600d 0a0d 0a41 6e64 2c20  ..> ```....And, 
+00000db0: 746f 2069 6e73 7461 6c6c 2074 6865 2064  to install the d
+00000dc0: 6576 656c 6f70 6d65 6e74 2076 6572 7369  evelopment versi
+00000dd0: 6f6e 2c20 646f 2074 6865 2066 6f6c 6c6f  on, do the follo
+00000de0: 7769 6e67 3a0d 0a3e 2060 6060 7368 0d0a  wing:..> ```sh..
+00000df0: 3e20 2420 6769 7420 636c 6f6e 6520 6874  > $ git clone ht
+00000e00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000e10: 2f73 746e 6775 6c61 7269 7479 2f74 616e  /stngularity/tan
+00000e20: 6b69 6f61 7069 0d0a 3e20 2420 6364 2074  kioapi..> $ cd t
+00000e30: 616e 6b69 6f61 7069 0d0a 3e20 2420 7079  ankioapi..> $ py
+00000e40: 7468 6f6e 3320 2d6d 2070 6970 2069 6e73  thon3 -m pip ins
+00000e50: 7461 6c6c 202d 5520 2e5b 7370 6565 6475  tall -U .[speedu
+00000e60: 705d 0d0a 3e20 6060 600d 0a0d 0a23 2320  p]..> ```....## 
+00000e70: 4578 616d 706c 6573 0d0a 4865 7265 2061  Examples..Here a
+00000e80: 7265 2065 7861 6d70 6c65 7320 6f66 2073  re examples of s
+00000e90: 6f6d 6520 6f66 2074 6865 2066 6561 7475  ome of the featu
+00000ea0: 7265 7320 6f66 2074 6865 206c 6962 7261  res of the libra
+00000eb0: 7279 2e20 4d6f 7265 2065 7861 6d70 6c65  ry. More example
+00000ec0: 7320 696e 205b 6065 7861 6d70 6c65 732f  s in [`examples/
+00000ed0: 605d 282f 6578 616d 706c 6573 290d 0a0d  `](/examples)...
+00000ee0: 0a23 2323 2323 2320 4765 7474 696e 6720  .###### Getting 
+00000ef0: 616c 6c20 746f 7073 206f 6620 706c 6179  all tops of play
+00000f00: 6572 730d 0a60 6060 7079 0d0a 696d 706f  ers..```py..impo
+00000f10: 7274 2061 7379 6e63 696f 0d0a 6672 6f6d  rt asyncio..from
+00000f20: 2074 6f61 7069 2069 6d70 6f72 7420 546f   toapi import To
+00000f30: 702c 2054 6f70 4c69 7374 732c 2067 6574  p, TopLists, get
+00000f40: 5f74 6f70 730d 0a0d 0a74 6f70 733a 2054  _tops....tops: T
+00000f50: 6f70 4c69 7374 7320 3d20 6173 796e 6369  opLists = asynci
+00000f60: 6f2e 7275 6e28 6765 745f 746f 7073 2829  o.run(get_tops()
+00000f70: 290d 0a65 6666 6963 6965 6e63 795f 746f  )..efficiency_to
+00000f80: 703a 2054 6f70 203d 2074 6f70 732e 6566  p: Top = tops.ef
+00000f90: 6669 6369 656e 6379 0d0a 7072 696e 7428  ficiency..print(
+00000fa0: 222d 2d2d 2d2d 2045 6666 6963 6965 6e63  "----- Efficienc
+00000fb0: 7920 746f 7020 2d2d 2d2d 2d22 290d 0a66  y top -----")..f
+00000fc0: 6f72 206e 756d 6265 722c 2075 7365 7220  or number, user 
+00000fd0: 696e 2065 6e75 6d65 7261 7465 2865 6666  in enumerate(eff
+00000fe0: 6963 6965 6e63 795f 746f 702e 7573 6572  iciency_top.user
+00000ff0: 7329 3a0d 0a20 2020 2070 7269 6e74 2866  s):..    print(f
+00001000: 2223 7b6e 756d 6265 722b 317d 2020 207b  "#{number+1}   {
+00001010: 7573 6572 2e6e 616d 657d 2028 7b75 7365  user.name} ({use
+00001020: 722e 746f 705f 7661 6c75 657d 2922 290d  r.top_value})").
+00001030: 0a60 6060 0d0a 0d0a 2323 2323 2323 2047  .```....###### G
+00001040: 6574 7469 6e67 2069 6e66 6f72 6d61 7469  etting informati
+00001050: 6f6e 206f 6620 706c 6179 6572 0d0a 6060  on of player..``
+00001060: 6070 790d 0a69 6d70 6f72 7420 6173 796e  `py..import asyn
+00001070: 6369 6f0d 0a66 726f 6d20 746f 6170 6920  cio..from toapi 
+00001080: 696d 706f 7274 2055 7365 722c 2067 6574  import User, get
+00001090: 5f75 7365 720d 0a0d 0a75 7365 723a 2055  _user....user: U
+000010a0: 7365 7220 3d20 6173 796e 6369 6f2e 7275  ser = asyncio.ru
+000010b0: 6e28 6765 745f 7573 6572 2822 7374 7922  n(get_user("sty"
+000010c0: 2929 0d0a 2320 616e 6420 596f 7520 6361  ))..# and You ca
+000010d0: 6e20 7370 6563 6966 7920 6c61 6e67 7561  n specify langua
+000010e0: 6765 0d0a 2320 7573 6572 3a20 5573 6572  ge..# user: User
+000010f0: 203d 2061 7379 6e63 696f 2e72 756e 2867   = asyncio.run(g
+00001100: 6574 5f75 7365 7228 2273 7479 222c 206c  et_user("sty", l
+00001110: 616e 673d 2272 7522 2929 0d0a 0d0a 7072  ang="ru"))....pr
+00001120: 696e 7428 6622 4e61 6d65 3a20 7b75 7365  int(f"Name: {use
+00001130: 722e 6e61 6d65 7d22 290d 0a72 616e 6b3a  r.name}")..rank:
+00001140: 2073 7472 203d 2075 7365 722e 7261 6e6b   str = user.rank
+00001150: 2e6e 616d 652e 7469 746c 6528 290d 0a70  .name.title()..p
+00001160: 7269 6e74 2866 2252 616e 6b3a 207b 7261  rint(f"Rank: {ra
+00001170: 6e6b 7d20 287b 7573 6572 2e73 636f 7265  nk} ({user.score
+00001180: 7d2f 7b75 7365 722e 7363 6f72 655f 6e65  }/{user.score_ne
+00001190: 7874 7d20 7b72 6f75 6e64 2875 7365 722e  xt} {round(user.
+000011a0: 7363 6f72 652f 7573 6572 2e73 636f 7265  score/user.score
+000011b0: 5f6e 6578 742a 3130 3029 7d25 2922 290d  _next*100)}%)").
+000011c0: 0a70 7269 6e74 2866 2248 6173 2070 7265  .print(f"Has pre
+000011d0: 6d69 756d 3a20 7b27 5965 7327 2069 6620  mium: {'Yes' if 
+000011e0: 7573 6572 2e70 7265 6d69 756d 2065 6c73  user.premium els
+000011f0: 6520 274e 6f27 7d22 290d 0a70 7269 6e74  e 'No'}")..print
+00001200: 2829 0d0a 7072 696e 7428 6622 4b44 3a20  ()..print(f"KD: 
+00001210: 7b75 7365 722e 6b69 6c6c 737d 2f7b 7573  {user.kills}/{us
+00001220: 6572 2e64 6561 7468 737d 2028 7b75 7365  er.deaths} ({use
+00001230: 722e 6b64 5f72 6174 696f 7d29 2229 0d0a  r.kd_ratio})")..
+00001240: 7072 696e 7428 6622 4361 7567 6874 2067  print(f"Caught g
+00001250: 6f6c 6473 3a20 7b75 7365 722e 6361 7567  olds: {user.caug
+00001260: 6874 5f67 6f6c 6473 7d22 290d 0a70 7269  ht_golds}")..pri
+00001270: 6e74 2866 2243 7279 7374 616c 733a 207b  nt(f"Crystals: {
+00001280: 7573 6572 2e63 7279 7374 616c 737d 2229  user.crystals}")
+00001290: 0d0a 7072 696e 7428 6622 4753 3a20 7b75  ..print(f"GS: {u
+000012a0: 7365 722e 6765 6172 5f73 636f 7265 7d22  ser.gear_score}"
+000012b0: 290d 0a60 6060 0d0a 0d0a 2323 204c 6963  )..```....## Lic
+000012c0: 656e 7365 0d0a 5468 6973 2070 726f 6a65  ense..This proje
+000012d0: 6374 2069 7320 6469 7374 7269 6275 7465  ct is distribute
+000012e0: 6420 756e 6465 7220 7468 6520 604d 4954  d under the `MIT
+000012f0: 6020 6c69 6365 6e73 652e 2059 6f75 2063  ` license. You c
+00001300: 616e 206c 6561 726e 206d 6f72 6520 6672  an learn more fr
+00001310: 6f6d 2074 6865 205b 2a2a 4c49 4345 4e53  om the [**LICENS
+00001320: 452a 2a5d 282f 4c49 4345 4e53 4529 2066  E**](/LICENSE) f
+00001330: 696c 652e 0d0a 0d0a 6060 600d 0a4d 6164  ile.....```..Mad
+00001340: 6520 7769 7468 20e2 9da4 2061 6e64 20f0  e with ... and .
+00001350: 9f8d b520 6279 2073 746e 6775 6c61 7269  ... by stngulari
+00001360: 7479 2066 6f72 2065 7665 7279 6f6e 650d  ty for everyone.
+00001370: 0a60 6060 0d0a                           .```..
```

### Comparing `tankioapi-1.0.0/src/tankioapi.egg-info/SOURCES.txt` & `tankioapi-1.0.1/src/tankioapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 requirements/dev.txt
+requirements/docs.txt
 requirements/speedup.txt
 src/tankioapi.egg-info/PKG-INFO
 src/tankioapi.egg-info/SOURCES.txt
 src/tankioapi.egg-info/dependency_links.txt
 src/tankioapi.egg-info/requires.txt
 src/tankioapi.egg-info/top_level.txt
 src/toapi/__init__.py
```

### Comparing `tankioapi-1.0.0/src/toapi/__init__.py` & `tankioapi-1.0.1/src/toapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from .errors import *
 from .types import *
 
 __name__ = "tankio_api"
 __author__ = "stngularity"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023-present stngularity"
-__version__ = "1.0.0"
+__version__ = "1.0.1"
```

### Comparing `tankioapi-1.0.0/src/toapi/client.py` & `tankioapi-1.0.1/src/toapi/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     """:class:`StableServerStatus`: Gets the status of stable game server.
     
     Maybe deprecated. I don't know this. Judging by the content of the
     response from the API, the chance of this is approximately `99%`"""
     response: Mapping[str, Any] = await request("GET", "/status.js", base="https://tankionline.com/s")
     return StableServerStatus.from_json(response)
 
+
 async def get_test_status() -> List[TestServerStatus]:
     """List[:class:`TestServerStatus`]: Gets the status of test game servers"""
     response: List[Mapping[str, Any]] = await request("GET", "/public_test", base="https://test.tankionline.com")
 
     output: List[TestServerStatus] = []
     for server in response:
         base: str = f"https://balancer.{server['Domain']}"
```

### Comparing `tankioapi-1.0.0/src/toapi/data/__init__.py` & `tankioapi-1.0.1/src/toapi/data/__init__.py`

 * *Files identical despite different names*

### Comparing `tankioapi-1.0.0/src/toapi/data/ranks.py` & `tankioapi-1.0.1/src/toapi/data/ranks.py`

 * *Files identical despite different names*

### Comparing `tankioapi-1.0.0/src/toapi/data/test_server.py` & `tankioapi-1.0.1/src/toapi/data/test_server.py`

 * *Files identical despite different names*

### Comparing `tankioapi-1.0.0/src/toapi/errors.py` & `tankioapi-1.0.1/src/toapi/errors.py`

 * *Files identical despite different names*

### Comparing `tankioapi-1.0.0/src/toapi/types/__init__.py` & `tankioapi-1.0.1/src/toapi/types/__init__.py`

 * *Files identical despite different names*

### Comparing `tankioapi-1.0.0/src/toapi/types/game_object.py` & `tankioapi-1.0.1/src/toapi/types/game_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # pylint: disable=C0103
 
 from dataclasses import dataclass
 from datetime import timedelta as td
 from typing import Any, List, Mapping, Optional, Type
 
-from ..http import request_bytes
+from ..http import request
 
 __all__ = ("GameObject", "SuppliesObject")
 
 
 @dataclass
 class BaseGameObject:
     """The base dataclass for the objects from Tanki Online
@@ -38,21 +38,21 @@
     name: str
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(id={self.id}, name=\"{self.name}\")"
 
     def __str__(self) -> str:
         return self.name
-    
+
     def __hash__(self) -> int:
         return hash(self.id)
 
     async def read_image(self) -> bytes:
         """:class:`bytes`: Reads the image data of this object and returns it"""
-        return await request_bytes("GET", self.image)
+        return await request("GET", self.image, base="", bytes=True)
 
 
 @dataclass
 class GameObject(BaseGameObject):
     """The dataclass for the objects from Tanki Online
     
     Attributes
```

### Comparing `tankioapi-1.0.0/src/toapi/types/mode.py` & `tankioapi-1.0.1/src/toapi/types/mode.py`

 * *Files identical despite different names*

### Comparing `tankioapi-1.0.0/src/toapi/types/rank.py` & `tankioapi-1.0.1/src/toapi/types/rank.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,15 @@
 class Rank:
     """The dataclass of user rank
     
     Attributes
     ----------
     number: :class:`int`
         The player's rank as number. Has the value from `1` to `31+N`,
-        where `N` is :attr:`legend_number`
-        
-    legend_number: :class:`int`
-        Only if player has `Legend` rank! The number of `Legend` rank"""
+        where `N` is :attr:`legend_number`"""
 
     number: int
 
     @property
     def legend_number(self) -> int:
         """:class:`int`: If the player has the `Legend` rank, then returns
         the number of this rank, otherwise returns `-1`"""
```

### Comparing `tankioapi-1.0.0/src/toapi/types/rating.py` & `tankioapi-1.0.1/src/toapi/types/rating.py`

 * *Files identical despite different names*

### Comparing `tankioapi-1.0.0/src/toapi/types/status.py` & `tankioapi-1.0.1/src/toapi/types/status.py`

 * *Files identical despite different names*

### Comparing `tankioapi-1.0.0/src/toapi/types/top.py` & `tankioapi-1.0.1/src/toapi/types/top.py`

 * *Files identical despite different names*

### Comparing `tankioapi-1.0.0/src/toapi/types/user.py` & `tankioapi-1.0.1/src/toapi/types/user.py`

 * *Files identical despite different names*

