# Comparing `tmp/vmk_spectrum-0.0.7-cp311-cp311-win_amd64.whl.zip` & `tmp/vmk_spectrum-0.0.8-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 80812 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat   161280 b- defN 23-May-03 19:02 _pyspectrum.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      159 b- defN 23-May-03 18:59 pyspectrum/__init__.py
--rw-rw-rw-  2.0 fat     4358 b- defN 23-May-03 18:59 pyspectrum/data.py
--rw-rw-rw-  2.0 fat     1257 b- defN 23-May-03 18:59 pyspectrum/device_factory.py
--rw-rw-rw-  2.0 fat      435 b- defN 23-May-03 18:59 pyspectrum/errors.py
--rw-rw-rw-  2.0 fat     4747 b- defN 23-May-03 18:59 pyspectrum/ethernet_device.py
--rw-rw-rw-  2.0 fat     9575 b- defN 23-May-03 18:59 pyspectrum/spectrometer.py
--rw-rw-rw-  2.0 fat      317 b- defN 23-May-03 19:02 vmk_spectrum-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-May-03 19:02 vmk_spectrum-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       25 b- defN 23-May-03 19:02 vmk_spectrum-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      891 b- defN 23-May-03 19:02 vmk_spectrum-0.0.7.dist-info/RECORD
-11 files, 183146 bytes uncompressed, 79310 bytes compressed:  56.7%
+Zip file size: 77386 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat   147968 b- defN 23-May-19 08:53 _pyspectrum.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      159 b- defN 23-May-19 08:50 pyspectrum/__init__.py
+-rw-rw-rw-  2.0 fat     5344 b- defN 23-May-19 08:50 pyspectrum/data.py
+-rw-rw-rw-  2.0 fat     1257 b- defN 23-May-19 08:50 pyspectrum/device_factory.py
+-rw-rw-rw-  2.0 fat      435 b- defN 23-May-19 08:50 pyspectrum/errors.py
+-rw-rw-rw-  2.0 fat     4747 b- defN 23-May-19 08:50 pyspectrum/ethernet_device.py
+-rw-rw-rw-  2.0 fat     9575 b- defN 23-May-19 08:50 pyspectrum/spectrometer.py
+-rw-rw-rw-  2.0 fat      339 b- defN 23-May-19 08:53 vmk_spectrum-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-May-19 08:53 vmk_spectrum-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       25 b- defN 23-May-19 08:53 vmk_spectrum-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      891 b- defN 23-May-19 08:53 vmk_spectrum-0.0.8.dist-info/RECORD
+11 files, 170842 bytes uncompressed, 75884 bytes compressed:  55.6%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: pyspectrum/ethernet_device.py
 Comment: 
 
 Filename: pyspectrum/spectrometer.py
 Comment: 
 
-Filename: vmk_spectrum-0.0.7.dist-info/METADATA
+Filename: vmk_spectrum-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: vmk_spectrum-0.0.7.dist-info/WHEEL
+Filename: vmk_spectrum-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: vmk_spectrum-0.0.7.dist-info/top_level.txt
+Filename: vmk_spectrum-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: vmk_spectrum-0.0.7.dist-info/RECORD
+Filename: vmk_spectrum-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyspectrum/data.py

```diff
@@ -3,14 +3,25 @@
 
 import numpy as np
 from numpy.typing import NDArray
 
 from .errors import LoadError
 
 
+def _check_slice_key(key):
+    if type(key) == slice:
+        return
+    if type(key) == tuple:
+        for k in key:
+            if type(k) != slice:
+                raise Exception('Only slices are supported')
+        return
+    raise Exception('Only slices are supported')
+
+
 @dataclass()
 class Data:
     """Сырые данные, полученные со спектрометра"""
     intensity: NDArray[float]
     """Двумерный массив данных измерения. Первый индекс - номер кадра, второй - номер сэмпла в кадре"""
     clipped: NDArray[bool]
     """Массив boolean значений. Если `clipped[i,j]==True`, `intensity[i,j]` содержит зашкаленное значение"""
@@ -100,14 +111,22 @@
             self.exposure
         )
 
     def __repr__(self) -> str:
         cls = self.__class__
         return f'{cls.__name__}({self.n_times = }, {self.n_numbers = })'
 
+    def __getitem__(self, key) -> 'Data':
+        _check_slice_key(key)
+        return Data(
+            intensity=self.intensity.__getitem__(key),
+            clipped=self.clipped.__getitem__(key),
+            exposure=self.exposure
+        )
+
 
 @dataclass()
 class Spectrum(Data):
     """Обработанные данные, полученные со спектрометра.
     Содержит в себе информацию о длинах волн измерения.
     В данный момент обработка заключается в вычитании темнового сигнала.
     """
@@ -121,7 +140,21 @@
         return super().__add__(other).to_spectrum(self.wavelength)
 
     def __sub__(self, other):
         return super().__sub__(other).to_spectrum(self.wavelength)
 
     def __mul__(self, other):
         return super().__mul__(other).to_spectrum(self.wavelength)
+
+    def __getitem__(self, key) -> 'Spectrum':
+        _check_slice_key(key)
+        if type(key) == tuple and len(key) >= 2:
+            new_wl = self.wavelength[key[1]]
+        else:
+            new_wl = self.wavelength
+        return Spectrum(
+            wavelength=new_wl,
+            exposure=self.exposure,
+            intensity=self.intensity.__getitem__(key),
+            clipped=self.clipped.__getitem__(key)
+        )
+
```

## Comparing `vmk_spectrum-0.0.7.dist-info/RECORD` & `vmk_spectrum-0.0.8.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-_pyspectrum.cp311-win_amd64.pyd,sha256=pE8cXWZ04Z8l0Ju2ADoD8CNskDfb6tstwqXVMflf2KU,161280
+_pyspectrum.cp311-win_amd64.pyd,sha256=rCXj7xti25fmOfoqKbwjuny3nNHki7G3wTuF1rlihC8,147968
 pyspectrum/__init__.py,sha256=mSRAZpwuFOv65WJCeoTzRG7NdnXDmjvGgreEt1ejw6s,159
-pyspectrum/data.py,sha256=NFihALx9BB7rpZZ1HBclNCxcdLXTdnbNlTRSxpoNi2Q,4358
+pyspectrum/data.py,sha256=HPJHbyaGsWwSQMF6qNlRe48MhYwEHasz3yh_8AfG9H8,5344
 pyspectrum/device_factory.py,sha256=xGVCDVtQC8RkAkcxjg7JiLdkiR4lz9VxQikhyUhSo2c,1257
 pyspectrum/errors.py,sha256=MkI7kErUUpMkkMlwE5MU0kMlp27CcOigYszKmzNXDyY,435
 pyspectrum/ethernet_device.py,sha256=nYPBnjRJmO8TdKuMsMepB0DDiLlvE5zbXr1FWJnk-NA,4747
 pyspectrum/spectrometer.py,sha256=qvori44YiIp7FXwz-NVhGhtM6iQpD-i5t0-GvDUF9oA,9575
-vmk_spectrum-0.0.7.dist-info/METADATA,sha256=x4Ud8OUeYEanzIClys_Cr4RO3EgcoZKO8OE7sP9JT_M,317
-vmk_spectrum-0.0.7.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
-vmk_spectrum-0.0.7.dist-info/top_level.txt,sha256=NT9XfeydHYXZsKuKvLYXhwUnK_kXYb2MHLtB1hRQLY0,25
-vmk_spectrum-0.0.7.dist-info/RECORD,,
+vmk_spectrum-0.0.8.dist-info/METADATA,sha256=hZCtzVHxlBsZvPuD2Ygi3u1crrG3WoRRLnHmADxZ0Bk,339
+vmk_spectrum-0.0.8.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
+vmk_spectrum-0.0.8.dist-info/top_level.txt,sha256=NT9XfeydHYXZsKuKvLYXhwUnK_kXYb2MHLtB1hRQLY0,25
+vmk_spectrum-0.0.8.dist-info/RECORD,,
```

