# Comparing `tmp/reactpy_jupyter-0.9.0-py3-none-any.whl.zip` & `tmp/reactpy_jupyter-0.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 9933 bytes, number of entries: 12
--rw-r--r--  2.0 unx      647 b- defN 23-May-19 01:43 reactpy_jupyter/__init__.py
--rw-r--r--  2.0 unx     3982 b- defN 23-May-19 01:43 reactpy_jupyter/import_resources.py
--rw-r--r--  2.0 unx     1277 b- defN 23-May-19 01:43 reactpy_jupyter/jupyter_server_extension.py
--rw-r--r--  2.0 unx     5276 b- defN 23-May-19 01:43 reactpy_jupyter/layout_widget.py
--rw-r--r--  2.0 unx      841 b- defN 23-May-19 01:43 reactpy_jupyter/monkey_patch.py
--rw-r--r--  2.0 unx      851 b- defN 23-May-19 01:43 reactpy_jupyter/widget_component.py
--rw-r--r--  2.0 unx      115 b- defN 23-May-19 01:43 reactpy_jupyter-0.9.0.data/data/etc/jupyter/jupyter_server_config.d/reactpy-jupyter.json
--rw-r--r--  2.0 unx     1070 b- defN 23-May-19 01:43 reactpy_jupyter-0.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3869 b- defN 23-May-19 01:43 reactpy_jupyter-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-19 01:43 reactpy_jupyter-0.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-19 01:43 reactpy_jupyter-0.9.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1112 b- defN 23-May-19 01:43 reactpy_jupyter-0.9.0.dist-info/RECORD
-12 files, 19148 bytes uncompressed, 8019 bytes compressed:  58.1%
+Zip file size: 26377 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      647 b- defN 23-May-19 01:54 reactpy_jupyter/__init__.py
+-rw-r--r--  2.0 unx     3982 b- defN 23-May-19 01:54 reactpy_jupyter/import_resources.py
+-rw-r--r--  2.0 unx     1277 b- defN 23-May-19 01:54 reactpy_jupyter/jupyter_server_extension.py
+-rw-r--r--  2.0 unx     5276 b- defN 23-May-19 01:54 reactpy_jupyter/layout_widget.py
+-rw-r--r--  2.0 unx      841 b- defN 23-May-19 01:54 reactpy_jupyter/monkey_patch.py
+-rw-r--r--  2.0 unx      851 b- defN 23-May-19 01:54 reactpy_jupyter/widget_component.py
+-rw-r--r--  2.0 unx    55659 b- defN 23-May-19 01:55 reactpy_jupyter/static/index.js
+-rw-r--r--  2.0 unx      115 b- defN 23-May-19 01:54 reactpy_jupyter-0.9.1.data/data/etc/jupyter/jupyter_server_config.d/reactpy-jupyter.json
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-19 01:55 reactpy_jupyter-0.9.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3869 b- defN 23-May-19 01:55 reactpy_jupyter-0.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-19 01:55 reactpy_jupyter-0.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-19 01:55 reactpy_jupyter-0.9.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1201 b- defN 23-May-19 01:55 reactpy_jupyter-0.9.1.dist-info/RECORD
+13 files, 74896 bytes uncompressed, 24325 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -12,26 +12,29 @@
 
 Filename: reactpy_jupyter/monkey_patch.py
 Comment: 
 
 Filename: reactpy_jupyter/widget_component.py
 Comment: 
 
-Filename: reactpy_jupyter-0.9.0.data/data/etc/jupyter/jupyter_server_config.d/reactpy-jupyter.json
+Filename: reactpy_jupyter/static/index.js
 Comment: 
 
-Filename: reactpy_jupyter-0.9.0.dist-info/LICENSE
+Filename: reactpy_jupyter-0.9.1.data/data/etc/jupyter/jupyter_server_config.d/reactpy-jupyter.json
 Comment: 
 
-Filename: reactpy_jupyter-0.9.0.dist-info/METADATA
+Filename: reactpy_jupyter-0.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: reactpy_jupyter-0.9.0.dist-info/WHEEL
+Filename: reactpy_jupyter-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: reactpy_jupyter-0.9.0.dist-info/top_level.txt
+Filename: reactpy_jupyter-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: reactpy_jupyter-0.9.0.dist-info/RECORD
+Filename: reactpy_jupyter-0.9.1.dist-info/top_level.txt
+Comment: 
+
+Filename: reactpy_jupyter-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reactpy_jupyter/__init__.py

```diff
@@ -6,15 +6,15 @@
 
 from . import jupyter_server_extension
 from .import_resources import setup_import_resources
 from .layout_widget import run, set_import_source_base_url, to_widget
 from .monkey_patch import execute_patch
 from .widget_component import from_widget
 
-__version__ = "0.9.0"  # DO NOT MODIFY
+__version__ = "0.9.1"  # DO NOT MODIFY
 
 __all__ = (
     "from_widget",
     "load_ipython_extension",
     "unload_ipython_extension",
     "to_widget",
     "run",
```

## Comparing `reactpy_jupyter-0.9.0.dist-info/LICENSE` & `reactpy_jupyter-0.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `reactpy_jupyter-0.9.0.dist-info/METADATA` & `reactpy_jupyter-0.9.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy-jupyter
-Version: 0.9.0
+Version: 0.9.1
 Summary: It's React, but in Python
 Home-page: https://github.com/reactive-python/reactpy
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
```

## Comparing `reactpy_jupyter-0.9.0.dist-info/RECORD` & `reactpy_jupyter-0.9.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-reactpy_jupyter/__init__.py,sha256=0x4nb4uBfNimUkAaNPjP2cJVSPABfZTVXXJQGfDylEw,647
+reactpy_jupyter/__init__.py,sha256=TrLRzzYWrliPVr5yTsyz76xtheif26rvxAtTQaencgw,647
 reactpy_jupyter/import_resources.py,sha256=AbyOdSUdH4MfAu-liqn8YF_AIOcGMD7RC6gsk1cDv1I,3982
 reactpy_jupyter/jupyter_server_extension.py,sha256=7DrCkoOo0kCsuwA5FiX9gJiEhvFF2lr3MQW6SzzYlUA,1277
 reactpy_jupyter/layout_widget.py,sha256=ER9vO8uxLCo5jtJP6ao3ECYQsjKT52DGMEPPcFJRf2A,5276
 reactpy_jupyter/monkey_patch.py,sha256=mkQtRM7roZr7GvdDWQFJgyXN_w_DKWlPHPiQrfaQQ0g,841
 reactpy_jupyter/widget_component.py,sha256=ijvBG8nUhYdZ8sE_R6OgWBUhvIKnPR2LYZM1jIHI1Tw,851
-reactpy_jupyter-0.9.0.data/data/etc/jupyter/jupyter_server_config.d/reactpy-jupyter.json,sha256=obmXphQVEmBAmMyIqkwOuUpaEKVv1a0hBeORY3INWKM,115
-reactpy_jupyter-0.9.0.dist-info/LICENSE,sha256=nfoDPqpXukz9ocjDeRG8RLMsasZWiB7AEK3RaH8CjMQ,1070
-reactpy_jupyter-0.9.0.dist-info/METADATA,sha256=cuC_pcSFpwwSwmhd5tdE7chFzkWff-inOrCNtiZsFEI,3869
-reactpy_jupyter-0.9.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-reactpy_jupyter-0.9.0.dist-info/top_level.txt,sha256=nBOiqS4hMNmHHQf2b_51tWq5KHZFw7FPg_hvZQjDejY,16
-reactpy_jupyter-0.9.0.dist-info/RECORD,,
+reactpy_jupyter/static/index.js,sha256=TdtvsN7GU6Xg6K1WPKqvjLFBYRTnueJUVyWXw7t_HCY,55659
+reactpy_jupyter-0.9.1.data/data/etc/jupyter/jupyter_server_config.d/reactpy-jupyter.json,sha256=obmXphQVEmBAmMyIqkwOuUpaEKVv1a0hBeORY3INWKM,115
+reactpy_jupyter-0.9.1.dist-info/LICENSE,sha256=nfoDPqpXukz9ocjDeRG8RLMsasZWiB7AEK3RaH8CjMQ,1070
+reactpy_jupyter-0.9.1.dist-info/METADATA,sha256=755aECaVPvKc95fgev_T8NAtsNqtivnBRZeCBEviXh8,3869
+reactpy_jupyter-0.9.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+reactpy_jupyter-0.9.1.dist-info/top_level.txt,sha256=nBOiqS4hMNmHHQf2b_51tWq5KHZFw7FPg_hvZQjDejY,16
+reactpy_jupyter-0.9.1.dist-info/RECORD,,
```

