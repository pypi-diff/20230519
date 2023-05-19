# Comparing `tmp/mfhpo_simulator-0.0.1-py3-none-any.whl.zip` & `tmp/mfhpo_simulator-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 15286 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      401 b- defN 23-May-13 07:23 benchmark_simulator/__init__.py
+Zip file size: 15271 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      401 b- defN 23-May-19 18:02 benchmark_simulator/__init__.py
 -rw-rw-r--  2.0 unx     2758 b- defN 23-May-18 10:18 benchmark_simulator/_constants.py
 -rw-rw-r--  2.0 unx     6157 b- defN 23-May-18 10:19 benchmark_simulator/_secure_proc.py
 -rw-rw-r--  2.0 unx     1846 b- defN 23-May-17 23:06 benchmark_simulator/_utils.py
 -rw-rw-r--  2.0 unx    23531 b- defN 23-May-18 18:30 benchmark_simulator/simulator.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-May-19 17:57 mfhpo_simulator-0.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      320 b- defN 23-May-19 17:57 mfhpo_simulator-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-19 17:57 mfhpo_simulator-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 23-May-19 17:57 mfhpo_simulator-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      871 b- defN 23-May-19 17:57 mfhpo_simulator-0.0.1.dist-info/RECORD
-10 files, 46756 bytes uncompressed, 13786 bytes compressed:  70.5%
+-rw-rw-r--  2.0 unx    10760 b- defN 23-May-19 18:02 mfhpo_simulator-0.0.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      290 b- defN 23-May-19 18:02 mfhpo_simulator-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-19 18:02 mfhpo_simulator-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       20 b- defN 23-May-19 18:02 mfhpo_simulator-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      871 b- defN 23-May-19 18:02 mfhpo_simulator-0.0.2.dist-info/RECORD
+10 files, 46726 bytes uncompressed, 13771 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: benchmark_simulator/_utils.py
 Comment: 
 
 Filename: benchmark_simulator/simulator.py
 Comment: 
 
-Filename: mfhpo_simulator-0.0.1.dist-info/LICENSE
+Filename: mfhpo_simulator-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_simulator-0.0.1.dist-info/METADATA
+Filename: mfhpo_simulator-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_simulator-0.0.1.dist-info/WHEEL
+Filename: mfhpo_simulator-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_simulator-0.0.1.dist-info/top_level.txt
+Filename: mfhpo_simulator-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_simulator-0.0.1.dist-info/RECORD
+Filename: mfhpo_simulator-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_simulator/__init__.py

```diff
@@ -1,11 +1,11 @@
 from benchmark_simulator.simulator import CentralWorkerManager, ObjectiveFuncWorker
 
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-simulator"
```

## Comparing `mfhpo_simulator-0.0.1.dist-info/LICENSE` & `mfhpo_simulator-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mfhpo_simulator-0.0.1.dist-info/RECORD` & `mfhpo_simulator-0.0.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-benchmark_simulator/__init__.py,sha256=OHq-vbBFbaCiy2oWTWHAzr56H1iKcwWAg8aYUNeQ7N0,401
+benchmark_simulator/__init__.py,sha256=9kwxCxzaf0SychjNr0K_12cyAHx8ybmagA5TJfKVfOI,401
 benchmark_simulator/_constants.py,sha256=-rIXqW2a_YwMd7wxQRsSB0N3WD9GRb88Gx5ZZOsPsHo,2758
 benchmark_simulator/_secure_proc.py,sha256=yyHFcH5KitO35oyF7M2iQRcu2PPuHnmbeg36e82sdBo,6157
 benchmark_simulator/_utils.py,sha256=SBu3r9mAYgwgB2CLo4YVxGcSthUZOO8quyX7cGbikks,1846
 benchmark_simulator/simulator.py,sha256=r8UG_DJhkLVusCdZtVCVsPuVxYshqJadd_BXa9apotk,23531
-mfhpo_simulator-0.0.1.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
-mfhpo_simulator-0.0.1.dist-info/METADATA,sha256=Km3zCrlwrbV5aar36bEOcpB449AuAgNX1ARQHGrpqiU,320
-mfhpo_simulator-0.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mfhpo_simulator-0.0.1.dist-info/top_level.txt,sha256=pT5LiPwT78978UOly1oZst_RacTpjrU_SDaUE8xvA_c,20
-mfhpo_simulator-0.0.1.dist-info/RECORD,,
+mfhpo_simulator-0.0.2.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
+mfhpo_simulator-0.0.2.dist-info/METADATA,sha256=ZXaYT6tm3G9ZwqrGgJR02l1GqHixdByMl-aEL2YGdEw,290
+mfhpo_simulator-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mfhpo_simulator-0.0.2.dist-info/top_level.txt,sha256=pT5LiPwT78978UOly1oZst_RacTpjrU_SDaUE8xvA_c,20
+mfhpo_simulator-0.0.2.dist-info/RECORD,,
```

