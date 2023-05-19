# Comparing `tmp/cads_sdk-0.0.22-py3-none-any.whl.zip` & `tmp/cads_sdk-0.0.23-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 56001 bytes, number of entries: 18
--rw-rw-r--  2.0 unx     1265 b- defN 23-May-19 02:38 cads_sdk/__init__.py
+Zip file size: 56028 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx     1265 b- defN 23-May-19 04:21 cads_sdk/__init__.py
 -rw-rw-r--  2.0 unx     1264 b- defN 23-Apr-01 02:59 cads_sdk/nosql/__init__.py
 -rw-rw-r--  2.0 unx    11231 b- defN 23-Apr-17 08:04 cads_sdk/nosql/codec.py
 -rw-rw-r--  2.0 unx    86938 b- defN 23-May-18 09:04 cads_sdk/nosql/converter.py
--rw-rw-r--  2.0 unx    19183 b- defN 23-May-19 02:40 cads_sdk/nosql/display.py
+-rw-rw-r--  2.0 unx    19283 b- defN 23-May-19 04:21 cads_sdk/nosql/display.py
 -rw-rw-r--  2.0 unx     1187 b- defN 23-Apr-10 10:46 cads_sdk/nosql/etl.py
 -rw-rw-r--  2.0 unx     1291 b- defN 23-May-19 02:11 cads_sdk/nosql/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 14:03 cads_sdk/petastorm/__init__.py
 -rw-rw-r--  2.0 unx    19967 b- defN 23-Apr-10 04:34 cads_sdk/petastorm/dataset_metadata.py
 -rw-rw-r--  2.0 unx    10508 b- defN 23-Apr-10 07:19 cads_sdk/petastorm/fs_utils.py
 -rw-rw-r--  2.0 unx     5427 b- defN 23-Apr-10 04:42 cads_sdk/petastorm/utils.py
 -rw-rw-r--  2.0 unx    22554 b- defN 23-Apr-18 15:18 cads_sdk/pytorch/__init__.py
 -rw-rw-r--  2.0 unx    10653 b- defN 23-Apr-17 08:05 cads_sdk/pytorch/codec.py
 -rw-rw-r--  2.0 unx    78369 b- defN 23-Apr-20 08:23 cads_sdk/pytorch/converter.py
--rw-rw-r--  2.0 unx     7126 b- defN 23-May-19 02:40 cads_sdk-0.0.22.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-19 02:40 cads_sdk-0.0.22.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-19 02:40 cads_sdk-0.0.22.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1480 b- defN 23-May-19 02:40 cads_sdk-0.0.22.dist-info/RECORD
-18 files, 278544 bytes uncompressed, 53595 bytes compressed:  80.8%
+-rw-rw-r--  2.0 unx     7126 b- defN 23-May-19 04:22 cads_sdk-0.0.23.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-19 04:22 cads_sdk-0.0.23.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-19 04:22 cads_sdk-0.0.23.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1480 b- defN 23-May-19 04:22 cads_sdk-0.0.23.dist-info/RECORD
+18 files, 278644 bytes uncompressed, 53622 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: cads_sdk/pytorch/codec.py
 Comment: 
 
 Filename: cads_sdk/pytorch/converter.py
 Comment: 
 
-Filename: cads_sdk-0.0.22.dist-info/METADATA
+Filename: cads_sdk-0.0.23.dist-info/METADATA
 Comment: 
 
-Filename: cads_sdk-0.0.22.dist-info/WHEEL
+Filename: cads_sdk-0.0.23.dist-info/WHEEL
 Comment: 
 
-Filename: cads_sdk-0.0.22.dist-info/top_level.txt
+Filename: cads_sdk-0.0.23.dist-info/top_level.txt
 Comment: 
 
-Filename: cads_sdk-0.0.22.dist-info/RECORD
+Filename: cads_sdk-0.0.23.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cads_sdk/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.22'
+__version__ = '0.0.23'
 
 __doc__ = """
 cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
 =====================================================================
 **cads-sdk**
 Function to convert 
 -------------
```

## cads_sdk/nosql/display.py

```diff
@@ -505,35 +505,36 @@
             
         elif '.wav' in row.path:
             from scipy.io import wavfile
             samplerate, data = wavfile.read(BytesIO(row.audio))
             from IPython.display import Audio, display
             self.output.append_display_data(Audio(data.T, rate=samplerate))
             
-        elif 'mp3' in row.path:
+        elif '.mp3' in row.path:
             samplerate, data = read_mp3(BytesIO(row.audio))
             from IPython.display import Audio, display
             self.output.append_display_data(Audio(data.T, rate=samplerate))
             
     def displayAudio(self, ex):
         get_value = ex.description
         
         df = self.generate_sql("*")
         
         if 'rel_path' in df.schema.names:
             print("DEUBG filter", f"rel_path like '%{os.path.basename(get_value)}'")
-            df = df.filter(f"rel_path like '%{os.path.basename(get_value)}'").limit(1)
+            df.createOrReplaceTempView("tmp_df")
+            df = ss.sql(f"""SELECT * FROM tmp_df where rel_path like '%{os.path.basename(get_value)}'""")
         else:
             df = df.filter(f"path = '{get_value}'").limit(1)
         
         if df.count() == 0:
+            df = self.generate_sql("*")
             df = df.filter(f"path = '{get_value}'").limit(1)
             
         _ = [self.write_to_folder(row) for row in df.collect()]
-        
         # df.foreach(self.write_to_folder)
         
         
     def _repr_html_(self):
         width = height = ''
         if self.width:
             width = ' width="%d"' % self.width
```

## Comparing `cads_sdk-0.0.22.dist-info/METADATA` & `cads_sdk-0.0.23.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-sdk
-Version: 0.0.22
+Version: 0.0.23
 Summary: Function to help Data Scientist work more effectively with DWH
 Home-page: http://git.bigdata.local/data-engineers/sdk/utilities
 Author: duyvnc
 Author-email: duyvnc@fpt.com.vn
 License: duyvnc
 Platform: UNKNOWN
 Requires-Python: >=3.5
@@ -16,15 +16,15 @@
 Requires-Dist: pydub
 Requires-Dist: ipywidgets
 Requires-Dist: petastorm
 
 -----------------
 
 # cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
-[![PyPI Latest Release](https://img.shields.io/badge/pypi-0.0.22-blue)](https://pypi.org/project/cads-sdk/)
+[![PyPI Latest Release](https://img.shields.io/badge/pypi-0.0.23-blue)](https://pypi.org/project/cads-sdk/)
 [![Package Status](https://img.shields.io/badge/status-stable-green)](https://pypi.org/project/cads-sdk/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cads-sdk?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cads-sdk)
 [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-CADS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://blog.cads.live/)
 
 
 
 ## What is it?
```

## Comparing `cads_sdk-0.0.22.dist-info/RECORD` & `cads_sdk-0.0.23.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-cads_sdk/__init__.py,sha256=XnX6xXtQ5mZ-yuWPOqNtOUrHBLw_MPOpfdS9RrEaA28,1265
+cads_sdk/__init__.py,sha256=zwcmYI4WuxBuYAxJZ-A11xdLaQVP-lzvOTXYMMUCSJs,1265
 cads_sdk/nosql/__init__.py,sha256=Yu2Zt5cpSXSLqIRAvIxaXOtoyj3yBisGTbnFlH4UD2A,1264
 cads_sdk/nosql/codec.py,sha256=Z0RdndLtSHAnqHOpDGE-Wb_jD9eIWvKiuX4Yj1KudX4,11231
 cads_sdk/nosql/converter.py,sha256=TUVOQIEqE60zpoxZbyc9fcgaFOVkYy37ZmwtBVG8LoI,86938
-cads_sdk/nosql/display.py,sha256=fXszt0PMRJXWGLNv1E9e5fkKmmadz5tN2TnuqjrxJ5w,19183
+cads_sdk/nosql/display.py,sha256=xoPolRkz6LUhCAKOVZWrgKdFzoj91Gfte3hO7iJ1ADY,19283
 cads_sdk/nosql/etl.py,sha256=PWhXNWZyIFFEEvTIoUNuKK5cDqTy8A4FPn07BGMr0Vk,1187
 cads_sdk/nosql/utils.py,sha256=nQVGBLBx7mhIgLulY1_bUefBEOqHhZbht4jI9E9azuY,1291
 cads_sdk/petastorm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cads_sdk/petastorm/dataset_metadata.py,sha256=3sXVulFmpZEJC7mM0cwEXBVmB-0TD-U746ltLcsqIno,19967
 cads_sdk/petastorm/fs_utils.py,sha256=qFAzfi_VM4Rr2mBW8JsgxPUojLFFQGZI93MpI4sL_Xo,10508
 cads_sdk/petastorm/utils.py,sha256=CyeRPL_ih9wC1BdElvf1VknF1lBdNvJxgldSiU1OkFs,5427
 cads_sdk/pytorch/__init__.py,sha256=qyLEDZ_2BXLQBqievSj4wg2h4EQf9AdbIi_1SKFyIsM,22554
 cads_sdk/pytorch/codec.py,sha256=5XZulM21El-lsL3jZMexnJAHc2cIeRZj721PMuPhsJU,10653
 cads_sdk/pytorch/converter.py,sha256=lT2c3ix8Q35TEOUdFzlQVIzf7GfRklomwrdfRaXcY7k,78369
-cads_sdk-0.0.22.dist-info/METADATA,sha256=xapCAlv-joanNl8Tez857C3GH7m8JCzlZ4wlj8vVPmo,7126
-cads_sdk-0.0.22.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-cads_sdk-0.0.22.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
-cads_sdk-0.0.22.dist-info/RECORD,,
+cads_sdk-0.0.23.dist-info/METADATA,sha256=sGgeOoM69xQF9TQNJpFnSbtPJdPxGIp_XnLWEWsqiKE,7126
+cads_sdk-0.0.23.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+cads_sdk-0.0.23.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
+cads_sdk-0.0.23.dist-info/RECORD,,
```

