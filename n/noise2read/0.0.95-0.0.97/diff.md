# Comparing `tmp/noise2read-0.0.95.tar.gz` & `tmp/noise2read-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noise2read-0.0.95.tar", last modified: Fri May 19 01:04:23 2023, max compression
+gzip compressed data, was "noise2read-0.0.97.tar", last modified: Fri May 19 15:39:01 2023, max compression
```

## Comparing `noise2read-0.0.95.tar` & `noise2read-0.0.97.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 01:04:23.452378 noise2read-0.0.95/
--rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.95/LICENSE
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-19 01:04:23.453845 noise2read-0.0.95/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.95/README.rst
--rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.95/pyproject.toml
--rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-19 01:04:23.461772 noise2read-0.0.95/setup.cfg
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 01:04:22.740513 noise2read-0.0.95/src/
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 01:04:23.227350 noise2read-0.0.95/src/noise2read/
--rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-19 00:53:35.000000 noise2read-0.0.95/src/noise2read/__init__.py
--rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.0.95/src/noise2read/classifier.py
--rw-r--r--   0 pping    (55472) Research  (5010)    17347 2023-05-19 00:55:32.000000 noise2read-0.0.95/src/noise2read/config.py
--rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.95/src/noise2read/coverage.py
--rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.95/src/noise2read/data_analysis.py
--rw-r--r--   0 pping    (55472) Research  (5010)    56513 2023-05-19 00:52:07.000000 noise2read-0.0.95/src/noise2read/data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)    11534 2023-05-17 00:24:07.000000 noise2read-0.0.95/src/noise2read/data_preprocessing.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.0.95/src/noise2read/encoding.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30703 2023-05-18 23:59:43.000000 noise2read-0.0.95/src/noise2read/error_orrection.py
--rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.95/src/noise2read/isolates_correction.py
--rw-r--r--   0 pping    (55472) Research  (5010)    26351 2023-05-16 13:42:25.000000 noise2read-0.0.95/src/noise2read/noise2read.py
--rw-r--r--   0 pping    (55472) Research  (5010)    39686 2023-05-19 00:51:27.000000 noise2read-0.0.95/src/noise2read/reads2vectors.py
--rw-r--r--   0 pping    (55472) Research  (5010)    18547 2023-05-17 00:19:59.000000 noise2read-0.0.95/src/noise2read/simulation.py
--rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.95/src/noise2read/umitest.py
--rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.95/src/noise2read/utils.py
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 01:04:23.347170 noise2read-0.0.95/src/noise2read.egg-info/
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-19 01:04:22.000000 noise2read-0.0.95/src/noise2read.egg-info/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-19 01:04:22.000000 noise2read-0.0.95/src/noise2read.egg-info/SOURCES.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-19 01:04:22.000000 noise2read-0.0.95/src/noise2read.egg-info/dependency_links.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-19 01:04:22.000000 noise2read-0.0.95/src/noise2read.egg-info/entry_points.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.95/src/noise2read.egg-info/not-zip-safe
--rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-19 01:04:22.000000 noise2read-0.0.95/src/noise2read.egg-info/requires.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-19 01:04:22.000000 noise2read-0.0.95/src/noise2read.egg-info/top_level.txt
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 01:04:23.414633 noise2read-0.0.95/tests/
--rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.95/tests/test_data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.95/tests/test_reads2vector.py
--rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.95/tests/test_utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 15:39:01.240856 noise2read-0.0.97/
+-rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.97/LICENSE
+-rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-19 15:39:01.242006 noise2read-0.0.97/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.97/README.rst
+-rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.97/pyproject.toml
+-rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-19 15:39:01.244770 noise2read-0.0.97/setup.cfg
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 15:39:01.089205 noise2read-0.0.97/src/
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 15:39:01.191408 noise2read-0.0.97/src/noise2read/
+-rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-19 15:37:15.000000 noise2read-0.0.97/src/noise2read/__init__.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.0.97/src/noise2read/classifier.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    17347 2023-05-19 00:55:32.000000 noise2read-0.0.97/src/noise2read/config.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.97/src/noise2read/coverage.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.97/src/noise2read/data_analysis.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    56513 2023-05-19 00:52:07.000000 noise2read-0.0.97/src/noise2read/data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    11534 2023-05-17 00:24:07.000000 noise2read-0.0.97/src/noise2read/data_preprocessing.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.0.97/src/noise2read/encoding.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30703 2023-05-18 23:59:43.000000 noise2read-0.0.97/src/noise2read/error_orrection.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.97/src/noise2read/isolates_correction.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    26351 2023-05-16 13:42:25.000000 noise2read-0.0.97/src/noise2read/noise2read.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    39121 2023-05-19 15:26:15.000000 noise2read-0.0.97/src/noise2read/reads2vectors.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    18547 2023-05-17 00:19:59.000000 noise2read-0.0.97/src/noise2read/simulation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.97/src/noise2read/umitest.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.97/src/noise2read/utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 15:39:01.222558 noise2read-0.0.97/src/noise2read.egg-info/
+-rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-19 15:39:01.000000 noise2read-0.0.97/src/noise2read.egg-info/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-19 15:39:01.000000 noise2read-0.0.97/src/noise2read.egg-info/SOURCES.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-19 15:39:01.000000 noise2read-0.0.97/src/noise2read.egg-info/dependency_links.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-19 15:39:01.000000 noise2read-0.0.97/src/noise2read.egg-info/entry_points.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.97/src/noise2read.egg-info/not-zip-safe
+-rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-19 15:39:01.000000 noise2read-0.0.97/src/noise2read.egg-info/requires.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-19 15:39:01.000000 noise2read-0.0.97/src/noise2read.egg-info/top_level.txt
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 15:39:01.236762 noise2read-0.0.97/tests/
+-rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.97/tests/test_data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.97/tests/test_reads2vector.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.97/tests/test_utils.py
```

### Comparing `noise2read-0.0.95/LICENSE` & `noise2read-0.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/PKG-INFO` & `noise2read-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.95
+Version: 0.0.97
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.95/README.rst` & `noise2read-0.0.97/README.rst`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/setup.cfg` & `noise2read-0.0.97/setup.cfg`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/src/noise2read/classifier.py` & `noise2read-0.0.97/src/noise2read/classifier.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/src/noise2read/config.py` & `noise2read-0.0.97/src/noise2read/config.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/src/noise2read/coverage.py` & `noise2read-0.0.97/src/noise2read/coverage.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/src/noise2read/data_analysis.py` & `noise2read-0.0.97/src/noise2read/data_analysis.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/src/noise2read/data_generation.py` & `noise2read-0.0.97/src/noise2read/data_generation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/src/noise2read/data_preprocessing.py` & `noise2read-0.0.97/src/noise2read/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/src/noise2read/encoding.py` & `noise2read-0.0.97/src/noise2read/encoding.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/src/noise2read/error_orrection.py` & `noise2read-0.0.97/src/noise2read/error_orrection.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/src/noise2read/isolates_correction.py` & `noise2read-0.0.97/src/noise2read/isolates_correction.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/src/noise2read/noise2read.py` & `noise2read-0.0.97/src/noise2read/noise2read.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/src/noise2read/reads2vectors.py` & `noise2read-0.0.97/src/noise2read/reads2vectors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-19 10:51:27
+# @Last Modified time: 2023-05-20 01:26:15
 
 from typing import Counter
 import numpy as np
 # import os
 from sklearn.preprocessing import StandardScaler
 from noise2read.encoding import EncodeScheme
 from mpire import WorkerPool
@@ -17,74 +17,39 @@
 
 class Reads2Vectors():
     def __init__(self, logger, config, edit_dis):
         self.logger = logger
         self.edit_dis = edit_dis
         self.config = config
     
-    def read2features(self, shared_objects, i):
-        ES, original_feature = shared_objects
-        
-        cur_feture = original_feature[i]
-
+    def read2features(self, shared_objs, idx):
+        ES, ori_features = shared_objs
+        cur_feature = ori_features[idx]
         features = []
-        # pd_fe = ES.descriptors("PairDistance", reads_lst[i])
-        # features.extend(pd_fe)    
-        ###########################################################################
-        # features.append(read_count_lst[i]) 
-        # features.append(err_pos_lst[i]) 
-        # freq_pos.append([ori_seq_freq, err_pos])              
-        ###########################################################################
-        ft_fea1 = ES.descriptors("FourierTransform", cur_feture[0])
-        cg_fea1 = ES.descriptors("ChaosGame", cur_feture[0])
-        entropy_fea1 = ES.descriptors("Entropy", cur_feture[0])
-        fs_fea1 = ES.descriptors("FickettScore", cur_feture[0])
+        ft_fea1 = ES.descriptors("FourierTransform", cur_feature[0])
+        cg_fea1 = ES.descriptors("ChaosGame", cur_feature[0])
+        entropy_fea1 = ES.descriptors("Entropy", cur_feature[0])
+        fs_fea1 = ES.descriptors("FickettScore", cur_feature[0])
 
         features.extend(ft_fea1)
         features.extend(cg_fea1)
         features.extend(entropy_fea1)
         features.extend(fs_fea1)
-        # print(len(features))
-        # ft_fea2 = ES.descriptors("FourierTransform", reads_lst2[i])
-        # cg_fea2 = ES.descriptors("ChaosGame", reads_lst2[i])
-        # # entropy_fea2 = ES.descriptors("Entropy", reads_lst2[i])
-        # fs_fea2 = ES.descriptors("FickettScore", reads_lst2[i])
-
-        # features.extend(ft_fea2)
-        # features.extend(cg_fea2)
-        # # features.extend(entropy_fea2)
-        # features.extend(fs_fea2)
-        # self.logger.debug(len(features))
-        atomic_fea1 = ES.descriptors("atomic_number", cur_feture[0])
-        atomic_fea2 = ES.descriptors("atomic_number", cur_feture[1])
-        # atomic_fea1 = ES.descriptors("binary", reads_lst1[i])
-        # atomic_fea2 = ES.descriptors("binary", reads_lst2[i])
-        # print(int(other_features[i][0]))
+
+        atomic_fea1 = ES.descriptors("atomic_number", cur_feature[0])
+        atomic_fea2 = ES.descriptors("atomic_number", cur_feature[1])
         features.extend(atomic_fea1)
         features.extend(atomic_fea2)
-        # onehot_fea = ES.descriptors("OneHot", reads_lst1[i])
-        # features.extend(onehot_fea)
-        features.extend(cur_feture[2:])
+
+        features.extend(cur_feature[2:])
         # self.logger.debug(f'FourierTransform: {len(ft_fea)}, ChaosGame: {len(cg_fea)}, Entropy: {len(entropy_fea)}, FickettScore: {len(fs_fea)}')
         return features 
 
     def all_in_one_embedding(self, total_reads, genuine_df, negative_df, ambiguous_df, high_flag):
         self.logger.info("Embedding genuine and ambiguous data.")
-        genuine_reads_lst1 = []
-        negtive_reads_lst1 = []
-        ambiguous_reads_lst1 = []
-
-        genuine_reads_lst2 = []
-        negtive_reads_lst2 = []
-        ambiguous_reads_lst2 = []
-
-        genuine_reads_features = []
-        negtive_reads_features = []
-        ambiguous_reads_features = [] 
-
         if self.edit_dis == 1:
             base_lst = ['A', 'C', 'G', 'T', 'N']
             if self.config.read_type == "DNA":
                 error_tyes = ["A-G", "G-A", "A-T", "T-A", "A-C", "C-A", "G-T", "T-G", "G-C", "C-G", "T-C", "C-T", "T-X", "X-T", "C-X", "X-C", "A-X", "X-A", "G-X", "X-G", "X-N", "N-X"]
                 
                 kmers = ['NX', 'XN', 'XA', 'XC', 'XG', 'XT', 'AX', 'CX', 'GX', 'TX'] + [''.join(i) for i in itertools.product(base_lst, repeat = 2)] + [''.join(i) for i in itertools.product(base_lst, repeat = 3)] + ['AXA', 'CXA', 'TXA', 'GXA', 'AXC', 'CXC', 'TXC', 'GXC', 'AXG', 'CXG', 'TXG', 'GXG', 'AXT', 'CXT', 'TXT', 'GXT', 'NXA', 'NXC', 'NXG', 'NXT', 'NXN','AXN','CXN','GXN','TXN']
                 # kmers3 = ['ANA', 'CNA', 'TNA', 'GNA', 'ANC', 'CNC', 'TNC', 'GNC', 'ANG', 'CNG', 'TNG', 'GNG', 'ANT', 'CNT', 'TNT', 'GNT'] + [''.join(i) for i in itertools.product(base_lst, repeat = 3)]
@@ -138,36 +103,45 @@
                 kmers_priors[item] = base_prior
                 base_prior += 0.01        
             self.logger.debug(err_kmers2count)
             self.logger.debug(err_tyes2count)
             juge_indels = err_tyes2count.keys() & set(['N-X', 'X-N', 'X-A', 'X-C', 'X-G', 'X-T', 'A-X', 'C-X', 'G-X', 'T-X'])
             indel_num = len(juge_indels)
 
+        genuine_feature_lst = []
         for idx, row in genuine_df.iterrows():
-            genuine_reads_lst1.append(row['StartRead'])
-            genuine_reads_lst2.append(row['EndRead'])
+            # genuine_feature_lst.append(row['StartRead'])
+            # genuine_feature_lst.append(row['EndRead'])
             if self.edit_dis == 1:
                 cur_err_tye = row['ErrorTye']
                 cur_kmer1 = row['StartErrKmer']
                 cur_kmer2 = row['EndErrKmer']
                 # self.logger.debug(row['StartRead'])
                 # self.logger.debug(row['EndRead'])
                 # self.logger.debug(f'{cur_kmer1}, {cur_kmer2}')
                 cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
                 cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
                 cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
                 # 
                 if high_flag:
-                    genuine_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, error_tyes[row['ErrorTye']] , row["StartDegree"], row['ErrorPosition']
+                    # genuine_feature_lst.extend([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, error_tyes[row['ErrorTye']] , row["StartDegree"], row['ErrorPosition']
+                    genuine_feature_lst.append((row['StartRead'], row['EndRead'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
                 else:
-                    genuine_reads_features.append([row['StartReadCount'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, error_tyes[row['ErrorTye']] , row["StartDegree"], row['ErrorPosition']
+                    # genuine_feature_lst.extend([row['StartReadCount'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, error_tyes[row['ErrorTye']] , row["StartDegree"], row['ErrorPosition']
+                    genuine_feature_lst.append((row['StartRead'], row['EndRead'], row['StartReadCount'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
             else:
-                genuine_reads_features.append([row['StartReadCount']])
+                # genuine_feature_lst.append(row['StartReadCount'])
+                genuine_feature_lst.append((row['StartRead'], row['EndRead'], row['StartReadCount']))
             # genuine_reads_count.append(row['StartReadCount'])
-        
+
+        genuine_fea = self.read2vec(genuine_feature_lst)
+        del genuine_feature_lst
+
+        #################################################################################
+        print("encoding negative samples...")
         negative_count = 0
         neg_read2seqs = {}
         if self.edit_dis == 1:
             for idx, row in negative_df.iterrows():
                 read = row['StartRead']
                 if indel_num == 0:
                     pos_reads = seq2substitution(read)
@@ -184,65 +158,74 @@
             if genuine_reads_num >= negative_num * 2:
                 each_negative_num = int(genuine_reads_num / negative_num)
             else:
                 each_negative_num = 1
         if negative_count >= self.config.negative_sample_num:
             self.logger.warning("Negative samples larger than {}, noise2read will use random sampling to generate negative samples.".format(self.config.negative_sample_num))
 
+        negative_feature_lst = []
         for idx, row in negative_df.iterrows():
             read = row['StartRead']
             if self.edit_dis == 1:
                 if negative_count < self.config.negative_sample_num:
                     pos_reads = neg_read2seqs[read]
                     for read2 in pos_reads:
-                        negtive_reads_lst1.append(read) 
-                        negtive_reads_lst2.append(read2)  
+                        # negative_feature_lst.append(read) 
+                        # negative_feature_lst.append(read2)  
                         cur_err_tye_kmers = error_type_classification(read, read2)
                         cur_err_tye = cur_err_tye_kmers[0]
                         cur_kmer1 = cur_err_tye_kmers[1]
                         cur_kmer2 = cur_err_tye_kmers[2]
                         cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
                         cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
                         cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
                         if high_flag:
-                            negtive_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, row["StartDegree"]
+                            # negative_feature_lst.extend([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, row["StartDegree"]
+                            negative_feature_lst.append((read, read2, cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
                         else:
-                            negtive_reads_features.append([row['StartReadCount'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) 
+                            # negative_feature_lst.extend([row['StartReadCount'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) 
+                            negative_feature_lst.append((read, read2, row['StartReadCount'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
                 else:
                     pos_reads = neg_read2seqs[read]
                     candidates = list(pos_reads - total_reads)
                     if len(candidates) > 0:
                         for i in range(each_negative_num):
                             if len(candidates) > 0:
-                                negtive_reads_lst1.append(read) 
+                                # negative_feature_lst.append(read) 
                                 
                                 select_read = random.choice(candidates) 
                                 candidates.remove(select_read)
-                                negtive_reads_lst2.append(select_read)  
+                                # negative_feature_lst.append(select_read)  
 
                                 cur_err_tye_kmers = error_type_classification(read, select_read)
                                 cur_err_tye = cur_err_tye_kmers[0]
                                 cur_kmer1 = cur_err_tye_kmers[1]
                                 cur_kmer2 = cur_err_tye_kmers[2]
                                 cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
                                 cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
                                 cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
                                 # 
                                 if high_flag:
-                                    negtive_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, row["StartDegree"]
+                                    # negative_feature_lst.extend([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, row["StartDegree"]
+                                    negative_feature_lst.append((read, select_read, cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
                                 else:
-                                    negtive_reads_features.append([row['StartReadCount'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) 
+                                    # negative_feature_lst.extend([row['StartReadCount'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) 
+                                    negative_feature_lst.append((read, select_read, row['StartReadCount'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
             elif self.edit_dis == 2:
                 # pos_reads = enumerate_ed2_seqs(read) 
                 random_seqs = random_ed2_seq(read, total_reads, each_negative_num)
                 for i in range(len(random_seqs)):
-                    negtive_reads_lst1.append(read) 
-                    negtive_reads_lst2.append(random_seqs[i])  
-                    negtive_reads_features.append([row['StartReadCount']]) #, row["StartDegree"]
-
+                    # negative_feature_lst.append(read) 
+                    # negative_feature_lst.append(random_seqs[i])  
+                    # negative_feature_lst.append(row['StartReadCount']) #, row["StartDegree"]
+                    negative_feature_lst.append((read, random_seqs[i], row['StartReadCount']))
+
+        negative_fea = self.read2vec(negative_feature_lst)
+        del negative_feature_lst
+        ###############################################################
         '''
         for idx, row in negative_df.iterrows():
             read = row['StartRead']
             if self.edit_dis == 1:
                 if self.config.over_sampling:
                     if indel_num == 0:
                         pos_reads = seq2substitution(read)
@@ -297,42 +280,34 @@
                 random_seqs = random_ed2_seq(read, total_reads, each_negative_num)
                 for i in range(len(random_seqs)):
                     negtive_reads_lst1.append(read) 
                     negtive_reads_lst2.append(random_seqs[i])  
                     negtive_reads_features.append([row['StartReadCount']]) #, row["StartDegree"]
                     # negtive_reads_count.append(row['StartReadCount']) 
         '''
+        ambiguous_feature_lst = []
         for idx, row in ambiguous_df.iterrows():
-            ambiguous_reads_lst1.append(row['StartRead'])
-            ambiguous_reads_lst2.append(row['EndRead'])
             if self.edit_dis == 1:
                 cur_err_tye = row['ErrorTye']
                 cur_kmer1 = row['StartErrKmer']
                 cur_kmer2 = row['EndErrKmer']
                 cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
                 cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
                 cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
                 # 
                 if high_flag:
-                    ambiguous_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])#, row["StartDegree"]
+                    ambiguous_feature_lst.append((row['StartRead'], row['EndRead'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
                 else:
-                    ambiguous_reads_features.append([row['StartReadCount'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])#, row["StartDegree"]
+                    ambiguous_feature_lst.append((row['StartRead'], row['EndRead'], row['StartReadCount'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
             else:
-                ambiguous_reads_features.append([row['StartReadCount']])
-
-        # self.logger.debug(f'{len(negtive_reads_lst1), len(negtive_reads_lst2), len(negtive_reads_features)}')
-        genuine_fea = self.read2vec(genuine_reads_lst1, genuine_reads_lst2, genuine_reads_features)
-        del genuine_reads_lst1, genuine_reads_lst2, genuine_reads_features
-
-        negative_fea = self.read2vec(negtive_reads_lst1, negtive_reads_lst2, negtive_reads_features)
-        del negtive_reads_lst1, negtive_reads_lst2, negtive_reads_features
-        
-        ambiguous_fea = self.read2vec(ambiguous_reads_lst1, ambiguous_reads_lst2, ambiguous_reads_features)
-        del ambiguous_reads_lst1, ambiguous_reads_lst2, ambiguous_reads_features
+                ambiguous_feature_lst.append((row['StartRead'], row['EndRead'], row['StartReadCount']))
 
+        ambiguous_fea = self.read2vec(ambiguous_feature_lst)
+        del ambiguous_feature_lst
+        ##################################################################
         read_features = genuine_fea + negative_fea
         feature_len = len(read_features[0])
         train_data = np.array(read_features, dtype=object)
         gen_len = len(genuine_fea)
         neg_len = len(negative_fea)
         del read_features, genuine_fea, negative_fea
 
@@ -434,15 +409,14 @@
             del lab_scale_f0, lab_scale_f1, lab_scale_f3, ulab_scale_f0, ulab_scale_f1, ulab_scale_f3
                 
         # lab_scale_f = np.hstack((lab_scale_f0, lab_scale_f1, lab_scale_f2, lab_scale_f3))
         # ulab_scale_f = np.hstack((ulab_scale_f0, ulab_scale_f1, ulab_scale_f2, ulab_scale_f3))
         
         return lab_scale_f, ulab_scale_f 
 
-    # def read2features(self, shared_objects, i):
     '''
     def read2features(self, ES, ori_feature):
         # ES, reads_lst1, reads_lst2, other_features = shared_objects
         features = []
         
         ###########################################################################
         ft_fea1 = ES.descriptors("FourierTransform", ori_feature[0])
@@ -457,84 +431,69 @@
         atomic_fea2 = ES.descriptors("atomic_number", ori_feature[1])
         features.extend(atomic_fea1)
         features.extend(atomic_fea2)
         
         features.extend(ori_feature[2:])
         return features 
     '''
-    def read2vec(self, reads_lst1, reads_lst2, other_features):  
+    def read2vec(self, original_features_lst):  
         ES = EncodeScheme(self.config.read_max_len, self.config.entropy_kmer, self.config.entropy_q, self.config.kmer_freq, self.config.read_type)
 
-        # Combine the features of each sample into one list
-        combined_features = []
-        for seq1, seq2, lst in zip(reads_lst1, reads_lst2, other_features):
-            tmp_lst = []
-            tmp_lst.append(seq1)
-            tmp_lst.append(seq2)
-            tmp_lst.extend(lst)
-            combined_features.append(tmp_lst)
-            del tmp_lst
-
-        chunk_size = len(combined_features) // self.config.chunks_num
-        if chunk_size > 0:
-            chunks = [combined_features[i:i+chunk_size] for i in range(0, len(combined_features), chunk_size)]
+        if len(original_features_lst) > (self.config.chunks_num * 10):
+            chunk_size = len(original_features_lst) // self.config.chunks_num
+            remainder = len(original_features_lst) % self.config.chunks_num
+            # chunks = [original_features_lst[i:i+chunk_size] for i in range(0, len(original_features_lst), chunk_size)]
+            chunks = []
+            for i in range(self.config.chunks_num):
+                # print(i)
+                cur_idx = chunk_size * i
+                chunks.append(original_features_lst[cur_idx:cur_idx+chunk_size])
+            # Handle the remaining elements
+            if remainder > 0:
+                chunks[-1].extend(original_features_lst[-remainder:])   
+                # print(chunks[-1])         
+            chunk_names = []
+            for i in range(len(chunks)):
+                chunk = chunks[i]
+                print(i)
+                print(len(chunk), type(chunk))
+                # print(chunk)
+                shared_objects = ES, chunk
+                vectors = []
+                with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
+                    for item in pool.imap(self.read2features, range(len(chunk))):
+                        vectors.append(item)
+                # Generate the pickle file name
+                file_name = self.config.result_dir + f"chunk_{i}.pickle"
+                # Write the vectors to the pickle file
+                with open(file_name, "wb") as file:
+                    pickle.dump(vectors, file)
+                chunk_names.append(file_name)
+                del vectors
+            del chunks
+            
+            combined_data = []
+            for file_name in chunk_names:
+                with open(file_name, "rb") as file:
+                    vectors = pickle.load(file)
+                    combined_data.extend(vectors)
+                    del vectors
+                os.remove(file_name)
+            return combined_data
         else:
-            chunks = combined_features
-
-        # Use multiprocessing to write each chunk to a separate pickle file
-        chunk_names = []
-        for i, chunk in enumerate(chunks):
-
-            shared_objects = ES, chunk
             vectors = []
+            shared_objects = ES, original_features_lst
             with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
-                for fea_lst in pool.imap(self.read2features, range(len(chunk))):
-                    vectors.append(fea_lst)
-
-            # Generate the pickle file name
-            file_name = self.config.result_dir + f"chunk_{i}.pickle"
-            # Write the vectors to the pickle file
-            with open(file_name, "wb") as file:
-                pickle.dump(vectors, file)
-            chunk_names.append(file_name)
-            del vectors
-            
-        combined_data = []
-        for file_name in chunk_names:
-            with open(file_name, "rb") as file:
-                vectors = pickle.load(file)
-                combined_data.extend(vectors)
-                del vectors
-            os.remove(file_name)
+                for item in pool.imap(self.read2features, range(len(original_features_lst))):
+                    vectors.append(item)
+            return vectors
 
-        del combined_features, chunks      
-        return combined_data
     
     def high_all_in_one_embedding(self, genuine_df, negative_df, new_negative_df, ambiguous_df):
         self.logger.info("Embedding genuine and high ambiguous data.")
-        genuine_reads_lst1 = []
-        negtive_reads_lst1 = []
-        ambiguous_reads_lst1 = []
-
-        genuine_reads_lst2 = []
-        negtive_reads_lst2 = []
-        ambiguous_reads_lst2 = []
-
-        genuine_reads_features = []
-        negtive_reads_features = []
-        ambiguous_reads_features = [] 
-        # if self.config.read_type == "DNA":
-        #     error_tyes = ["A-G", "G-A", "A-T", "T-A", "A-C", "C-A", "G-T", "T-G", "G-C", "C-G", "T-C", "C-T", "T-N", "N-T", "C-N", "N-C", "A-N", "N-A", "G-N", "N-G"]
-        #     base_lst = ['A', 'C', 'G', 'T', 'N']
-        #     kmers = [''.join(i) for i in itertools.product(base_lst, repeat = 2)] + [''.join(i) for i in itertools.product(base_lst, repeat = 3)]
-        #     # kmers3 = ['ANA', 'CNA', 'TNA', 'GNA', 'ANC', 'CNC', 'TNC', 'GNC', 'ANG', 'CNG', 'TNG', 'GNG', 'ANT', 'CNT', 'TNT', 'GNT'] + [''.join(i) for i in itertools.product(base_lst, repeat = 3)]
-        #     # kmers = kmers2 + kmers3
-        # elif self.config.read_type == "RNA":
-        #     base_lst = ['A', 'C', 'G', 'U', 'N']
-        #     kmers = [''.join(i) for i in itertools.product(base_lst, repeat = 2)] + [''.join(i) for i in itertools.product(base_lst, repeat = 3)]    
         base_lst = ['A', 'C', 'G', 'T', 'N']
         if self.config.read_type == "DNA":
             error_tyes = ["A-G", "G-A", "A-T", "T-A", "A-C", "C-A", "G-T", "T-G", "G-C", "C-G", "T-C", "C-T", "T-X", "X-T", "C-X", "X-C", "A-X", "X-A", "G-X", "X-G", "X-N", "N-X", 'A-N', 'T-N','G-N','C-N','N-A','N-T', 'N-C', 'N-G']
             kmers = ['NX', 'XN', 'XA', 'XC', 'XG', 'XT', 'AX', 'CX', 'GX', 'TX'] + [''.join(i) for i in itertools.product(base_lst, repeat = 2)] + [''.join(i) for i in itertools.product(base_lst, repeat = 3)] + ['AXA', 'CXA', 'TXA', 'GXA', 'AXC', 'CXC', 'TXC', 'GXC', 'AXG', 'CXG', 'TXG', 'GXG', 'AXT', 'CXT', 'TXT', 'GXT', 'NXA', 'NXC', 'NXG', 'NXT', 'NXN','AXN','CXN','GXN','TXN']
             # kmers3 = ['ANA', 'CNA', 'TNA', 'GNA', 'ANC', 'CNC', 'TNC', 'GNC', 'ANG', 'CNG', 'TNG', 'GNG', 'ANT', 'CNT', 'TNT', 'GNT'] + [''.join(i) for i in itertools.product(base_lst, repeat = 3)]
             # kmers = kmers2 + kmers3
         elif self.config.read_type == "RNA":
@@ -583,73 +542,78 @@
         kmers_priors = {}
         base_prior = 0.1
         for item in kmer_keys:
             kmers_priors[item] = base_prior
             base_prior += 0.01        
         self.logger.debug(err_kmers2count)
         self.logger.debug(err_tyes2count)
-
+        ##################################################################################
+        genuine_feature_lst = []
         for idx, row in genuine_df.iterrows():
-            genuine_reads_lst1.append(row['StartRead'])
-            genuine_reads_lst2.append(row['EndRead'])
-
             cur_err_tye = row['ErrorTye']
             cur_kmer1 = row['StartErrKmer']
             cur_kmer2 = row['EndErrKmer']
             # self.logger.debug(row['StartRead'])
             # self.logger.debug(row['EndRead'])
             # self.logger.debug(f'{cur_kmer1}, {cur_kmer2}')
             cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
             cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
             cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
-            genuine_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, error_tyes[row['ErrorTye']] , row["StartDegree"], row['ErrorPosition']
-        
+            # genuine_feature_lst.extend([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, error_tyes[row['ErrorTye']] , row["StartDegree"], row['ErrorPosition']
+            genuine_feature_lst.append((row['StartRead'], row['EndRead'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
+        genuine_fea = self.read2vec(genuine_feature_lst)
+        del genuine_feature_lst
+        #################################################################################
+        negative_feature_lst = []
         for idx, row in new_negative_df.iterrows():
-            negtive_reads_lst1.append(row['StartRead'])
-            negtive_reads_lst2.append(row['EndRead'])
+            # negative_feature_lst.append()
+            # negative_feature_lst.append()
             cur_err_tye = row['ErrorTye']
             cur_kmer1 = row['StartErrKmer']
             cur_kmer2 = row['EndErrKmer']
             cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
             cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
             cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
-            negtive_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, row["StartDegree"]
-
+            # negative_feature_lst.extend([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, row["StartDegree"]
+            negative_feature_lst.append((row['StartRead'], row['EndRead'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
         # isolates negative
         for idx, row in negative_df.iterrows():
             read = row['StartRead']
             pos_reads = enumerate_ed1_seqs(read)
             for read2 in pos_reads:
-                negtive_reads_lst1.append(read) 
-                negtive_reads_lst2.append(read2)  
+                # negative_feature_lst.append(read) 
+                # negative_feature_lst.append(read2)  
                 cur_err_tye_kmers = error_type_classification(read, read2)
                 cur_err_tye = cur_err_tye_kmers[0]
                 cur_kmer1 = cur_err_tye_kmers[1]
                 cur_kmer2 = cur_err_tye_kmers[2]
                 cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
                 cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
                 cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
-                negtive_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])  
-
+                # negative_feature_lst.extend([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])  
+                negative_feature_lst.append((read, read2, cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
+        
+        negative_fea = self.read2vec(negative_feature_lst)
+        del negative_feature_lst
+        ###############################################################
+        ambiguous_feature_lst = []
         for idx, row in ambiguous_df.iterrows():
-            ambiguous_reads_lst1.append(row['StartRead'])
-            ambiguous_reads_lst2.append(row['EndRead'])
+            # ambiguous_feature_lst.append(row['StartRead'])
+            # ambiguous_feature_lst.append(row['EndRead'])
             cur_err_tye = row['ErrorTye']
             cur_kmer1 = row['StartErrKmer']
             cur_kmer2 = row['EndErrKmer']
             cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
             cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
             cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
-            ambiguous_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])#, row["StartDegree"]
-
-        genuine_fea = self.read2vec(genuine_reads_lst1, genuine_reads_lst2, genuine_reads_features)
-        negative_fea = self.read2vec(negtive_reads_lst1, negtive_reads_lst2, negtive_reads_features)
-        ambiguous_fea = self.read2vec(ambiguous_reads_lst1, ambiguous_reads_lst2, ambiguous_reads_features)
-        del genuine_reads_lst1, genuine_reads_lst2, genuine_reads_features, negtive_reads_lst1, negtive_reads_lst2, negtive_reads_features, ambiguous_reads_lst1, ambiguous_reads_lst2, ambiguous_reads_features
-
+            # ambiguous_feature_lst.extend([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])#, row["StartDegree"]
+            ambiguous_feature_lst.append((row['StartRead'], row['EndRead'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2))
+        ambiguous_fea = self.read2vec(ambiguous_feature_lst)
+        del ambiguous_feature_lst
+        ##################################################################
         read_features = genuine_fea + negative_fea
         labels = np.array([1] * len(genuine_fea) + [0] * len(negative_fea))
         train_data = np.array(read_features)
         shape1 = (len(labels), len(read_features[0]))
         train_data.reshape(shape1)   
 
         ambiguous_data = np.array(ambiguous_fea)
```

### Comparing `noise2read-0.0.95/src/noise2read/simulation.py` & `noise2read-0.0.97/src/noise2read/simulation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/src/noise2read/umitest.py` & `noise2read-0.0.97/src/noise2read/umitest.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/src/noise2read/utils.py` & `noise2read-0.0.97/src/noise2read/utils.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/src/noise2read.egg-info/PKG-INFO` & `noise2read-0.0.97/src/noise2read.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.95
+Version: 0.0.97
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.95/src/noise2read.egg-info/SOURCES.txt` & `noise2read-0.0.97/src/noise2read.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/tests/test_data_generation.py` & `noise2read-0.0.97/tests/test_data_generation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/tests/test_reads2vector.py` & `noise2read-0.0.97/tests/test_reads2vector.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.95/tests/test_utils.py` & `noise2read-0.0.97/tests/test_utils.py`

 * *Files identical despite different names*

