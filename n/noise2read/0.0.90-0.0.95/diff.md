# Comparing `tmp/noise2read-0.0.90.tar.gz` & `tmp/noise2read-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noise2read-0.0.90.tar", last modified: Thu May 18 05:27:35 2023, max compression
+gzip compressed data, was "noise2read-0.0.95.tar", last modified: Fri May 19 01:04:23 2023, max compression
```

## Comparing `noise2read-0.0.90.tar` & `noise2read-0.0.95.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-18 05:27:35.019289 noise2read-0.0.90/
--rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.90/LICENSE
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-18 05:27:35.020595 noise2read-0.0.90/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.90/README.rst
--rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.90/pyproject.toml
--rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-18 05:27:35.023817 noise2read-0.0.90/setup.cfg
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-18 05:27:34.870083 noise2read-0.0.90/src/
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-18 05:27:34.958417 noise2read-0.0.90/src/noise2read/
--rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-18 05:21:34.000000 noise2read-0.0.90/src/noise2read/__init__.py
--rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.0.90/src/noise2read/classifier.py
--rw-r--r--   0 pping    (55472) Research  (5010)    17347 2023-05-18 03:36:23.000000 noise2read-0.0.90/src/noise2read/config.py
--rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.90/src/noise2read/coverage.py
--rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.90/src/noise2read/data_analysis.py
--rw-r--r--   0 pping    (55472) Research  (5010)    57229 2023-05-18 05:19:49.000000 noise2read-0.0.90/src/noise2read/data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)    11534 2023-05-17 00:24:07.000000 noise2read-0.0.90/src/noise2read/data_preprocessing.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.0.90/src/noise2read/encoding.py
--rw-r--r--   0 pping    (55472) Research  (5010)    31011 2023-05-18 03:59:25.000000 noise2read-0.0.90/src/noise2read/error_orrection.py
--rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.90/src/noise2read/isolates_correction.py
--rw-r--r--   0 pping    (55472) Research  (5010)    26351 2023-05-16 13:42:25.000000 noise2read-0.0.90/src/noise2read/noise2read.py
--rw-r--r--   0 pping    (55472) Research  (5010)    45616 2023-05-18 05:21:13.000000 noise2read-0.0.90/src/noise2read/reads2vectors.py
--rw-r--r--   0 pping    (55472) Research  (5010)    18547 2023-05-17 00:19:59.000000 noise2read-0.0.90/src/noise2read/simulation.py
--rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.90/src/noise2read/umitest.py
--rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.90/src/noise2read/utils.py
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-18 05:27:34.990267 noise2read-0.0.90/src/noise2read.egg-info/
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-18 05:27:34.000000 noise2read-0.0.90/src/noise2read.egg-info/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-18 05:27:34.000000 noise2read-0.0.90/src/noise2read.egg-info/SOURCES.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-18 05:27:34.000000 noise2read-0.0.90/src/noise2read.egg-info/dependency_links.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-18 05:27:34.000000 noise2read-0.0.90/src/noise2read.egg-info/entry_points.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.90/src/noise2read.egg-info/not-zip-safe
--rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-18 05:27:34.000000 noise2read-0.0.90/src/noise2read.egg-info/requires.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-18 05:27:34.000000 noise2read-0.0.90/src/noise2read.egg-info/top_level.txt
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-18 05:27:35.014917 noise2read-0.0.90/tests/
--rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.90/tests/test_data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.90/tests/test_reads2vector.py
--rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.90/tests/test_utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 01:04:23.452378 noise2read-0.0.95/
+-rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.95/LICENSE
+-rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-19 01:04:23.453845 noise2read-0.0.95/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.95/README.rst
+-rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.95/pyproject.toml
+-rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-19 01:04:23.461772 noise2read-0.0.95/setup.cfg
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 01:04:22.740513 noise2read-0.0.95/src/
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 01:04:23.227350 noise2read-0.0.95/src/noise2read/
+-rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-19 00:53:35.000000 noise2read-0.0.95/src/noise2read/__init__.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.0.95/src/noise2read/classifier.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    17347 2023-05-19 00:55:32.000000 noise2read-0.0.95/src/noise2read/config.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.95/src/noise2read/coverage.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.95/src/noise2read/data_analysis.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    56513 2023-05-19 00:52:07.000000 noise2read-0.0.95/src/noise2read/data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    11534 2023-05-17 00:24:07.000000 noise2read-0.0.95/src/noise2read/data_preprocessing.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.0.95/src/noise2read/encoding.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30703 2023-05-18 23:59:43.000000 noise2read-0.0.95/src/noise2read/error_orrection.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.95/src/noise2read/isolates_correction.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    26351 2023-05-16 13:42:25.000000 noise2read-0.0.95/src/noise2read/noise2read.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    39686 2023-05-19 00:51:27.000000 noise2read-0.0.95/src/noise2read/reads2vectors.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    18547 2023-05-17 00:19:59.000000 noise2read-0.0.95/src/noise2read/simulation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.95/src/noise2read/umitest.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.95/src/noise2read/utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 01:04:23.347170 noise2read-0.0.95/src/noise2read.egg-info/
+-rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-19 01:04:22.000000 noise2read-0.0.95/src/noise2read.egg-info/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-19 01:04:22.000000 noise2read-0.0.95/src/noise2read.egg-info/SOURCES.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-19 01:04:22.000000 noise2read-0.0.95/src/noise2read.egg-info/dependency_links.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-19 01:04:22.000000 noise2read-0.0.95/src/noise2read.egg-info/entry_points.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.95/src/noise2read.egg-info/not-zip-safe
+-rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-19 01:04:22.000000 noise2read-0.0.95/src/noise2read.egg-info/requires.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-19 01:04:22.000000 noise2read-0.0.95/src/noise2read.egg-info/top_level.txt
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-19 01:04:23.414633 noise2read-0.0.95/tests/
+-rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.95/tests/test_data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.95/tests/test_reads2vector.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.95/tests/test_utils.py
```

### Comparing `noise2read-0.0.90/LICENSE` & `noise2read-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/PKG-INFO` & `noise2read-0.0.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.90
+Version: 0.0.95
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.90/README.rst` & `noise2read-0.0.95/README.rst`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/setup.cfg` & `noise2read-0.0.95/setup.cfg`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/src/noise2read/classifier.py` & `noise2read-0.0.95/src/noise2read/classifier.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/src/noise2read/config.py` & `noise2read-0.0.95/src/noise2read/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-19 10:56:38
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-18 13:36:23
+# @Last Modified time: 2023-05-19 10:55:32
 
 import configparser
 import os
 
 class Config(object):
     def __init__(self, config_file, logger):
         conf = configparser.ConfigParser()
@@ -60,15 +60,15 @@
                 self.min_read_len = conf.getint("General", "min_read_len")
             else:
                 self.min_read_len = 30 
             # when the number of negative samples larger than preseting threshold, noise2read will downsample negative samples for training
             if conf.has_option("General", "negative_sample_num"):
                 self.negative_sample_num = conf.getint("General", "negative_sample_num")
             else:
-                self.negative_sample_num = 500000 # when 
+                self.negative_sample_num = 300000 # when 
             # if conf.has_option("General", "over_sampling"):
             #     self.over_sampling = conf.getboolean("General", "over_sampling")
             # else:
             #     self.over_sampling = True
             # GraphSetup
             if conf.has_option("GraphSetup", "high_freq_thre"):
                 self.high_freq_thre = conf.getint("GraphSetup", "high_freq_thre")
@@ -305,15 +305,15 @@
             self.num_workers = -1 
             self.chunks_num = 100
             self.min_iters = 1000
             self.verbose = True 
             self.iso_change_detail = False     
             self.top_n = 100      
             # self.over_sampling = True 
-            self.negative_sample_num = 500000
+            self.negative_sample_num = 300000
             self.min_read_len = 30
 
             # GraphSetup
             self.high_freq_thre = 4
             self.max_error_freq = 4
             self.save_graph = False
             self.graph_visualization = False
```

### Comparing `noise2read-0.0.90/src/noise2read/coverage.py` & `noise2read-0.0.95/src/noise2read/coverage.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/src/noise2read/data_analysis.py` & `noise2read-0.0.95/src/noise2read/data_analysis.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/src/noise2read/data_generation.py` & `noise2read-0.0.95/src/noise2read/data_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-16 15:52:44
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-18 15:19:49
+# @Last Modified time: 2023-05-19 10:52:07
 
 import editdistance
 import networkx as nx
 import os
 import csv
 from tqdm import tqdm
 from noise2read.utils import *
 from mpire import WorkerPool
 import matplotlib.pyplot as plt
 from networkx.drawing.nx_agraph import graphviz_layout
 from collections import Counter
 import sys
 import pandas as pd
-from multiprocessing import Pool
 
 class DataGneration():
     """
     A class to generate genuine and ambiguous errors from 1nt/2nt-edit-distance-based graphs construted from short reads dataset
     """
     def __init__(self, logger, config):
         """
@@ -206,26 +205,19 @@
         """
         extract genuine errors from umi graph
 
         Returns:
             DataFrame: one pandas dataframe saving genuine errors
         """
         graph, seqs_lens_lst, seqs2id_dict, unique_seqs = self.generate_graph(self.config.input_file, edit_dis=1)
-        subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph) if len(c) >= 2]
+        subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph) ]#if len(c) >= 2
 
         chunk_size = len(subgraphs) // self.config.chunks_num
-        remainder = len(subgraphs) % self.config.chunks_num
-
         if chunk_size > 0:
-            groups = []
-            for i in range(self.config.chunks_num):
-                groups.append(subgraphs[i:i+chunk_size])
-            # Handle the remaining elements
-            if remainder > 0:
-                groups.append(subgraphs[-remainder:])
+            groups = [subgraphs[i:i+chunk_size] for i in range(0, len(subgraphs), chunk_size)]
         else:
             groups = subgraphs
 
         # Write each group of subgraphs to separate files
         gexf_files = []
         for i, group in enumerate(groups):
             # Create a new graph for the group of subgraphs
@@ -237,44 +229,41 @@
                     group_G.nodes[node].update(graph.nodes[node])
             # Generate the file name for the group
             file_name = self.config.result_dir + f"group_{i}.gexf"
 
             # Write the group of subgraphs to the file
             nx.write_gexf(group_G, file_name)
             gexf_files.append(file_name)
-        
+
         del groups, subgraphs, graph
 
         genuine_lst = []
         for gexf_file in gexf_files:
             graph = nx.read_gexf(gexf_file)
             sub_graphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph)]
             
-            # Process the subgraphs in parallel
-            pool = Pool(processes=self.config.num_workers)
-            genuine_lsts = pool.starmap(self.extract_umi_genuine_errs_subgraph, [(sub_graph) for sub_graph in sub_graphs])
-            # Close the multiprocessing pool
-            pool.close()
-            pool.join()
-
-            for item1 in genuine_lsts:
+            subgraph_num = len(sub_graphs)
+            with WorkerPool(self.config.num_workers, shared_objects=sub_graphs, start_method='fork') as pool:
+                cur_genuine_lsts = pool.imap(self.extract_umi_genuine_errs_subgraph, range(subgraph_num))
+            for item in cur_genuine_lsts:
                 genuine_lst.extend(item)
 
             os.remove(gexf_file)
             del graph, sub_graphs
 
         genuine_df = pd.DataFrame(genuine_lst, columns=["StartRead","StartReadCount", "StartDegree", "ErrorTye","ErrorPosition", "StartErrKmer", "EndErrKmer", "EndRead", "EndReadCount", "EndDegree"])
 
         if self.config.verbose:
             genuine_csv = os.path.join(self.config.result_dir, "umi_gnuine.csv")
             genuine_df.to_csv(genuine_csv, index=False) 
         return genuine_df
 
-    def extract_umi_genuine_errs_subgraph(self, sub_graph): 
+    def extract_umi_genuine_errs_subgraph(self, sub_graphs, i): 
         gen_lst = []
+        sub_graph = sub_graphs[i]
         nodes_lst = list(sub_graph.nodes)
         for node in nodes_lst:
             node_count = sub_graph.nodes[node]['count']
             node_degree = sub_graph.degree[node]
             line = []
             if node_degree >= 1 and node_count <= self.config.max_error_freq and not sub_graph.nodes[node]['flag']: #and node_degree <= 4
                 node_neis = [n for n in sub_graph.neighbors(node)]
@@ -319,81 +308,67 @@
             ambiguous_csv = self.config.result_dir + "ambiguous1.csv"
         elif edit_dis == 2: #or edit_dis == 3:
             genu_columns = ["StartRead","StartReadCount", "StartDegree", "EndRead", "EndReadCount", "EndDegree"]
             ambiguous_df= pd.DataFrame(columns=["idx", "StartRead", "StartReadCount", "StartDegree", "EndRead", "EndReadCount", "EndDegree"])
             genuine_csv = self.config.result_dir + "genuine2.csv"
             ambiguous_csv = self.config.result_dir + "ambiguous2.csv"  
 
-        subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph) if len(c) >= 2]
+        subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph) if len(c) >= 2 ]#
+        # subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph)]
 
         self.logger.info("Extracting genuine and ambiguous errors...")
 
         chunk_size = len(subgraphs) // self.config.chunks_num
-        remainder = len(subgraphs) % self.config.chunks_num
-
         if chunk_size > 0:
-            groups = []
-            for i in range(self.config.chunks_num):
-                groups.append(subgraphs[i:i+chunk_size])
-            # Handle the remaining elements
-            if remainder > 0:
-                groups.append(subgraphs[-remainder:])
+            groups = [subgraphs[i:i+chunk_size] for i in range(0, len(subgraphs), chunk_size)]
         else:
             groups = subgraphs
 
         # Write each group of subgraphs to separate files
         gexf_files = []
         for i, group in enumerate(groups):
-            # print(i)
             # Create a new graph for the group of subgraphs
             group_G = nx.Graph()
             for subgraph_nodes in group:
                 group_G.add_edges_from(graph.subgraph(subgraph_nodes).edges())
                 # Add node attributes to the new graph
                 for node in subgraph_nodes:
                     group_G.nodes[node].update(graph.nodes[node])
             # Generate the file name for the group
             file_name = self.config.result_dir + f"group_{i}.gexf"
 
             # Write the group of subgraphs to the file
             nx.write_gexf(group_G, file_name)
             gexf_files.append(file_name)
-        
-        del groups, subgraphs, graph
-
-        genuine_lst = []
-        ambiguous_lst = []
 
         if self.config.high_ambiguous:
             high_ambiguous_df = pd.DataFrame(columns=["idx", "StartRead", "StartReadCount", "StartDegree", "ErrorTye","ErrorPosition", "StartErrKmer", "EndErrKmer", "EndRead", "EndReadCount", "EndDegree"])    
             high_ambi_lst = []        
 
         high_idx = 0
+        genuine_lst = []
+        ambiguous_lst = []
         for gexf_file in gexf_files:
-            graph = nx.read_gexf(gexf_file)
-            sub_graphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph)]
-            
-            # Process the subgraphs in parallel
-            pool = Pool(processes=self.config.num_workers)
-            results = pool.starmap(self.extract_genuine_ambi_errs_subgraph, [(sub_graph, edit_dis) for sub_graph in sub_graphs])
-            # Close the multiprocessing pool
-            pool.close()
-            pool.join()
+            cur_graph = nx.read_gexf(gexf_file)
+            sub_graphs = [cur_graph.subgraph(c).copy() for c in nx.connected_components(cur_graph)]
             
-            genuine_lsts, ambiguous_lsts = zip(*results)
-            for item1, item2 in zip(genuine_lsts, ambiguous_lsts):
-                genuine_lst.extend(item1)
-                ambiguous_lst.extend(item2)
+            subgraph_num = len(sub_graphs)
+            shared_obs = sub_graphs, edit_dis
+            with WorkerPool(self.config.num_workers, shared_objects=shared_obs, start_method='fork') as pool:
+                for genu_ambi_lst in pool.imap(self.extract_genuine_ambi_errs_subgraph, range(subgraph_num)): # progress_bar=self.config.verbose
+                    if genu_ambi_lst[0]:
+                        genuine_lst.extend(genu_ambi_lst[0])
+                        ambiguous_lst.extend(genu_ambi_lst[1])
 
             if self.config.high_ambiguous:
                 cur_lst, cur_idx = self.extract_high_ambiguous_errs(sub_graphs, high_idx)
                 high_ambi_lst.extend(cur_lst)
                 high_idx = cur_idx + 1
             os.remove(gexf_file)
-            del graph, sub_graphs
+            del cur_graph, sub_graphs
         
         # genuine_lst = []
         # ambiguous_lst = []
         # subgraph_num = len(subgraphs)
         # shared_obs = subgraphs, edit_dis
         # with WorkerPool(self.config.num_workers, shared_objects=shared_obs, start_method='fork') as pool:
         #     for genu_ambi_lst in pool.imap(self.extract_genuine_ambi_errs_subgraph, range(subgraph_num), progress_bar=self.config.verbose):
@@ -459,14 +434,15 @@
         for a_item in item_lst:
             for sub_item in a_item:
                 sub_item.insert(0, idx)
                 tmp_df.loc[len(tmp_df)] = sub_item
             idx += 1
         return tmp_df
 
+    '''
     def extract_genuine_ambi_errs_subgraph(self, sub_graph, edit_dis):
         gen_lst = []
         ambi_lst = []
         nodes_lst = list(sub_graph.nodes)
         for node in nodes_lst:
             node_count = sub_graph.nodes[node]['count']
             node_degree = sub_graph.degree[node]
@@ -534,15 +510,16 @@
                         if tmp_lst:
                             ambi_lst.append(tmp_lst)  
                         # idx += 1 
                 sub_graph.nodes[node]['flag'] = True        
             else:
                 continue
         return gen_lst, ambi_lst
-
+    '''
+    
     def data_files(self, edit_dis):
         """
         function to return the results produced by DataGneration class
 
         Args:
             edit_dis (int): set edit distance 1 or 2 to search edges for constructing graph
 
@@ -817,23 +794,16 @@
             if len(edges_lst) > 0:
                 nodes_lst = list(sub_graph.nodes)
                 for node in nodes_lst:
                     # reset node visit status
                     sub_graph.nodes[node]['flag'] = False
 
         chunk_size = len(subgraphs) // self.config.chunks_num
-        remainder = len(subgraphs) % self.config.chunks_num
-
         if chunk_size > 0:
-            groups = []
-            for i in range(self.config.chunks_num):
-                groups.append(subgraphs[i:i+chunk_size])
-            # Handle the remaining elements
-            if remainder > 0:
-                groups.append(subgraphs[-remainder:])
+            groups = [subgraphs[i:i+chunk_size] for i in range(0, len(subgraphs), chunk_size)]
         else:
             groups = subgraphs
 
         # Write each group of subgraphs to separate files
         gexf_files = []
         for i, group in enumerate(groups):
             # Create a new graph for the group of subgraphs
@@ -849,16 +819,16 @@
             # Write the group of subgraphs to the file
             nx.write_gexf(group_G, file_name)
             gexf_files.append(file_name)
 
         amplicon_lst = []
         idx = 0
         for gexf_file in gexf_files:
-            graph = nx.read_gexf(gexf_file)
-            sub_graphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph)]
+            cur_graph = nx.read_gexf(gexf_file)
+            sub_graphs = [graph.subgraph(c).copy() for c in nx.connected_components(cur_graph)]
             
             cur_lst, cur_idx = self.extract_amplicon_errs(sub_graphs, idx)
             amplicon_lst.extend(cur_lst)
             idx = cur_idx + 1
             os.remove(gexf_file)
             del graph, sub_graphs
 
@@ -967,15 +937,15 @@
         #     high_ambiguous_csv = self.config.result_dir + "high_ambiguous_1nt.csv"
         #     high_ambiguous_df.to_csv(high_ambiguous_csv, index=False)  
         # self.logger.info("Done!")
         # return high_ambiguous_df
         return high_ambi_lst, idx
 
 
-'''
+    '''
     def extract_genuine_ambi_errs(self, subgraphs, edit_dis):
         """
         extract genuine and ambiguous errors from read graph
 
         Args:
             subgraphs (class): Subgraphs of graph constructed using NetworkX.
             edit_dis (int): set edit distance 1 or 2 to search edges for constructing graph
@@ -1055,17 +1025,16 @@
                         sub_graph.nodes[node]['flag'] = True        
                     else:
                         continue
         if self.config.verbose:
             genuine_df.to_csv(genuine_csv, index=False)  
             ambiguous_df.to_csv(ambiguous_csv, index=False)    
         return genuine_df, ambiguous_df
-'''
+    '''
 
-'''
     def extract_genuine_ambi_errs_subgraph(self, shared_obs, ii):
         gen_lst = []
         ambi_lst = []
         sub_graphs, edit_dis = shared_obs 
         sub_graph = sub_graphs[ii]
         edges_lst = [e for e in sub_graph.edges()]
         if len(edges_lst) > 0:
@@ -1137,17 +1106,17 @@
                             if tmp_lst:
                                 ambi_lst.append(tmp_lst)  
                             # idx += 1 
                     sub_graph.nodes[node]['flag'] = True        
                 else:
                     continue
         return [gen_lst, ambi_lst]
-'''
 
-'''
+
+    '''
     def extract_high_ambiguous_errs(self, subgraphs):
         """
         extract high ambiguous errors from read graph
 
         Args:
             subgraphs (class): Subgraphs of graph constructed using NetworkX.
 
@@ -1177,8 +1146,8 @@
                         idx += 1
             del edges_lst
         if self.config.verbose:
             high_ambiguous_csv = self.config.result_dir + "high_ambiguous_1nt.csv"
             high_ambiguous_df.to_csv(high_ambiguous_csv, index=False)  
         self.logger.info("Done!")
         return high_ambiguous_df
-'''
+    '''
```

### Comparing `noise2read-0.0.90/src/noise2read/data_preprocessing.py` & `noise2read-0.0.95/src/noise2read/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/src/noise2read/encoding.py` & `noise2read-0.0.95/src/noise2read/encoding.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/src/noise2read/error_orrection.py` & `noise2read-0.0.95/src/noise2read/error_orrection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-18 13:59:25
+# @Last Modified time: 2023-05-19 09:59:43
 
 import os
 from Bio import SeqIO
 import pandas as pd
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
 from noise2read.isolates_correction import IsolatesErrorCorrection
@@ -139,37 +139,34 @@
         TM = MLClassifier(self.logger, self.config, study_name, train_data, train_labels, ambiguous_data)
         predictions = TM.tunning(self.config.n_trials)
         ambiguous_df.insert(ambiguous_df.shape[1], 'predictand', predictions)
 
         # merge genuine and ambiguous errors
         grouped_ambiguous_df = ambiguous_df.groupby("idx")
         new_negative_df = pd.DataFrame()
-        new_genuine_df = pd.DataFrame()
         for name, group_df in grouped_ambiguous_df:
             self.logger.debug(group_df['predictand'])
             # if "N-X" or "X-N" in group_df['ErrorTye'].tolist():
             if len(group_df) > 0:
                 pred_index = group_df['predictand'].idxmax()
                 new_df = group_df.loc[:, ~group_df.columns.isin(['idx', 'predictand'])]
                 entry = copy.deepcopy(new_df.loc[[pred_index]])
                 bad_df = group_df.index.isin([pred_index])
                 cur_negative = group_df[~bad_df]
-                # genuine_df = pd.concat([genuine_df, entry], ignore_index=True)
-                new_genuine_df = pd.concat([new_genuine_df, entry], ignore_index=True)
+                genuine_df = pd.concat([genuine_df, entry], ignore_index=True)
                 new_negative_df = pd.concat([new_negative_df, cur_negative], ignore_index=True)
                 
         if edit_dis == 1 and self.config.verbose:
             ambiguous_df.to_csv(self.config.result_dir + 'ambiguous_1nt_prediction.csv', index=False)
         elif edit_dis == 2 and self.config.verbose:
             ambiguous_df.to_csv(self.config.result_dir + 'ambiguous_2nt_prediction.csv', index=False)
         del TM, ambiguous_data, ambiguous_df, grouped_ambiguous_df
         #######################################################################################################
         if isinstance(high_ambiguous_df, pd.DataFrame):
-            # high_train_data, high_train_labels, high_ambiguous_data = RV.high_all_in_one_embedding(genuine_df, negative_df, new_negative_df, high_ambiguous_df)
-            high_train_data, high_train_labels, high_ambiguous_data = RV.high_all_in_one_embedding(train_data, train_labels, new_genuine_df, new_negative_df, high_ambiguous_df)
+            high_train_data, high_train_labels, high_ambiguous_data = RV.high_all_in_one_embedding(genuine_df, negative_df, new_negative_df, high_ambiguous_df)
             study_name = 'high_ambiguous_1nt'
             TM = MLClassifier(self.logger, self.config, study_name, high_train_data, high_train_labels, high_ambiguous_data)
             high_predictions = TM.tunning(self.config.n_trials)
             high_ambiguous_df.insert(high_ambiguous_df.shape[1], 'predictand', high_predictions)
             del RV, TM, high_train_data, high_train_labels, high_ambiguous_data, negative_df
             return genuine_df, new_negative_df, high_ambiguous_df           
         else:
```

### Comparing `noise2read-0.0.90/src/noise2read/isolates_correction.py` & `noise2read-0.0.95/src/noise2read/isolates_correction.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/src/noise2read/noise2read.py` & `noise2read-0.0.95/src/noise2read/noise2read.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/src/noise2read/reads2vectors.py` & `noise2read-0.0.95/src/noise2read/reads2vectors.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-18 15:21:13
+# @Last Modified time: 2023-05-19 10:51:27
 
 from typing import Counter
 import numpy as np
 # import os
 from sklearn.preprocessing import StandardScaler
 from noise2read.encoding import EncodeScheme
 from mpire import WorkerPool
-from tqdm import tqdm
+# from tqdm import tqdm
 from noise2read.utils import *
 import itertools
 import pickle
-import multiprocessing as mp
-
 
 class Reads2Vectors():
     def __init__(self, logger, config, edit_dis):
         self.logger = logger
         self.edit_dis = edit_dis
         self.config = config
-    '''
+    
     def read2features(self, shared_objects, i):
-        ES, reads_lst1, reads_lst2, other_features = shared_objects
+        ES, original_feature = shared_objects
+        
+        cur_feture = original_feature[i]
+
         features = []
         # pd_fe = ES.descriptors("PairDistance", reads_lst[i])
         # features.extend(pd_fe)    
         ###########################################################################
         # features.append(read_count_lst[i]) 
         # features.append(err_pos_lst[i]) 
         # freq_pos.append([ori_seq_freq, err_pos])              
         ###########################################################################
-        ft_fea1 = ES.descriptors("FourierTransform", reads_lst1[i])
-        cg_fea1 = ES.descriptors("ChaosGame", reads_lst1[i])
-        entropy_fea1 = ES.descriptors("Entropy", reads_lst1[i])
-        fs_fea1 = ES.descriptors("FickettScore", reads_lst1[i])
+        ft_fea1 = ES.descriptors("FourierTransform", cur_feture[0])
+        cg_fea1 = ES.descriptors("ChaosGame", cur_feture[0])
+        entropy_fea1 = ES.descriptors("Entropy", cur_feture[0])
+        fs_fea1 = ES.descriptors("FickettScore", cur_feture[0])
 
         features.extend(ft_fea1)
         features.extend(cg_fea1)
         features.extend(entropy_fea1)
         features.extend(fs_fea1)
         # print(len(features))
         # ft_fea2 = ES.descriptors("FourierTransform", reads_lst2[i])
@@ -49,165 +50,26 @@
         # fs_fea2 = ES.descriptors("FickettScore", reads_lst2[i])
 
         # features.extend(ft_fea2)
         # features.extend(cg_fea2)
         # # features.extend(entropy_fea2)
         # features.extend(fs_fea2)
         # self.logger.debug(len(features))
-        atomic_fea1 = ES.descriptors("atomic_number", reads_lst1[i])
-        atomic_fea2 = ES.descriptors("atomic_number", reads_lst2[i])
+        atomic_fea1 = ES.descriptors("atomic_number", cur_feture[0])
+        atomic_fea2 = ES.descriptors("atomic_number", cur_feture[1])
         # atomic_fea1 = ES.descriptors("binary", reads_lst1[i])
         # atomic_fea2 = ES.descriptors("binary", reads_lst2[i])
         # print(int(other_features[i][0]))
         features.extend(atomic_fea1)
         features.extend(atomic_fea2)
         # onehot_fea = ES.descriptors("OneHot", reads_lst1[i])
         # features.extend(onehot_fea)
-        features.extend(other_features[i])
+        features.extend(cur_feture[2:])
         # self.logger.debug(f'FourierTransform: {len(ft_fea)}, ChaosGame: {len(cg_fea)}, Entropy: {len(entropy_fea)}, FickettScore: {len(fs_fea)}')
         return features 
-    '''
-    def high_all_in_one_embedding(self, train_data, train_labels, new_genuine_df, new_negative_df, ambiguous_df):
-        self.logger.info("Embedding genuine and high ambiguous data.")
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
-        base_lst = ['A', 'C', 'G', 'T', 'N']
-        if self.config.read_type == "DNA":
-            error_tyes = ["A-G", "G-A", "A-T", "T-A", "A-C", "C-A", "G-T", "T-G", "G-C", "C-G", "T-C", "C-T", "T-X", "X-T", "C-X", "X-C", "A-X", "X-A", "G-X", "X-G", "X-N", "N-X", 'A-N', 'T-N','G-N','C-N','N-A','N-T', 'N-C', 'N-G']
-            kmers = ['NX', 'XN', 'XA', 'XC', 'XG', 'XT', 'AX', 'CX', 'GX', 'TX'] + [''.join(i) for i in itertools.product(base_lst, repeat = 2)] + [''.join(i) for i in itertools.product(base_lst, repeat = 3)] + ['AXA', 'CXA', 'TXA', 'GXA', 'AXC', 'CXC', 'TXC', 'GXC', 'AXG', 'CXG', 'TXG', 'GXG', 'AXT', 'CXT', 'TXT', 'GXT', 'NXA', 'NXC', 'NXG', 'NXT', 'NXN','AXN','CXN','GXN','TXN']
-            # kmers3 = ['ANA', 'CNA', 'TNA', 'GNA', 'ANC', 'CNC', 'TNC', 'GNC', 'ANG', 'CNG', 'TNG', 'GNG', 'ANT', 'CNT', 'TNT', 'GNT'] + [''.join(i) for i in itertools.product(base_lst, repeat = 3)]
-            # kmers = kmers2 + kmers3
-        elif self.config.read_type == "RNA":
-            # error_tyes = ["A-G", "G-A", "A-U", "U-A", "A-C", "C-A", "G-U", "U-G", "G-C", "C-G", "U-C", "C-U", "U-N", "N-U", "C-N", "N-C", "A-N", "N-A", "G-N", "N-G"]
-            error_tyes = ["A-G", "G-A", "A-T", "T-A", "A-C", "C-A", "G-T", "T-G", "G-C", "C-G", "T-C", "C-T", "T-X", "X-T", "C-X", "X-C", "A-X", "X-A", "G-X", "X-G", "X-N", "N-X", 'A-N', 'T-N','G-N','C-N','N-A','N-T', 'N-C', 'N-G']
-            kmers = ['NX', 'XN', 'XA', 'XC', 'XG', 'XT', 'AX', 'CX', 'GX', 'TX'] + [''.join(i) for i in itertools.product(base_lst, repeat = 2)] + [''.join(i) for i in itertools.product(base_lst, repeat = 3)] + ['AXA', 'CXA', 'TXA', 'GXA', 'AXC', 'CXC', 'TXC', 'GXC', 'AXG', 'CXG', 'TXG', 'GXG', 'AXT', 'CXT', 'TXT', 'GXT', 'NXA', 'NXC', 'NXG', 'NXU', 'NXN','AXN','CXN','GXN','UXN']
-
-        error_tye_priors = {}
-        err_tye_base_prior = 0.1
-        for it in error_tyes:
-            error_tye_priors[it] = err_tye_base_prior
-            err_tye_base_prior += 0.01
-
-        self.logger.debug(len(kmers))
-        total_err_tyes = []
-        total_err_kmers = []
-        for idx, row in new_genuine_df.iterrows():
-            total_err_tyes.append(row['ErrorTye'])
-            total_err_kmers.append(row['StartErrKmer'])
-            total_err_kmers.append(row['EndErrKmer'])
-
-        for idx, row in ambiguous_df.iterrows():
-            total_err_tyes.append(row['ErrorTye'])
-            total_err_kmers.append(row['StartErrKmer'])
-            total_err_kmers.append(row['EndErrKmer'])
-
-        for idx, row in new_negative_df.iterrows():
-            read = row['StartRead']
-            total_err_tyes.append(row['ErrorTye'])
-            total_err_kmers.append(row['StartErrKmer'])
-            total_err_kmers.append(row['EndErrKmer'])
-            
-        total_err_kmers_count = len(total_err_kmers)
-        total_err_tyes_count = len(total_err_tyes)
-        
-        err_kmers2count = Counter(total_err_kmers)
-        err_tyes2count = Counter(total_err_tyes)
-        self.logger.debug(len(err_kmers2count.keys()))
-        kmer_keys = err_kmers2count.keys()
-
-        not_exist_kmer = set(kmers) - set(kmer_keys)
-        if not_exist_kmer:
-            for mer in not_exist_kmer:
-                err_kmers2count[mer] = 0
-
-        kmers_priors = {}
-        base_prior = 0.1
-        for item in kmer_keys:
-            kmers_priors[item] = base_prior
-            base_prior += 0.01        
-        self.logger.debug(err_kmers2count)
-        self.logger.debug(err_tyes2count)
-
-        for idx, row in new_genuine_df.iterrows():
-            genuine_reads_lst1.append(row['StartRead'])
-            genuine_reads_lst2.append(row['EndRead'])
-
-            cur_err_tye = row['ErrorTye']
-            cur_kmer1 = row['StartErrKmer']
-            cur_kmer2 = row['EndErrKmer']
-            # self.logger.debug(row['StartRead'])
-            # self.logger.debug(row['EndRead'])
-            # self.logger.debug(f'{cur_kmer1}, {cur_kmer2}')
-            cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
-            cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
-            cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
-            genuine_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, error_tyes[row['ErrorTye']] , row["StartDegree"], row['ErrorPosition']
-        
-        for idx, row in new_negative_df.iterrows():
-            negtive_reads_lst1.append(row['StartRead'])
-            negtive_reads_lst2.append(row['EndRead'])
-            cur_err_tye = row['ErrorTye']
-            cur_kmer1 = row['StartErrKmer']
-            cur_kmer2 = row['EndErrKmer']
-            cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
-            cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
-            cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
-            negtive_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2]) #, row["StartDegree"]
-
-
-        for idx, row in ambiguous_df.iterrows():
-            ambiguous_reads_lst1.append(row['StartRead'])
-            ambiguous_reads_lst2.append(row['EndRead'])
-            cur_err_tye = row['ErrorTye']
-            cur_kmer1 = row['StartErrKmer']
-            cur_kmer2 = row['EndErrKmer']
-            cur_err_tye_val = (err_tyes2count[cur_err_tye] + error_tye_priors[cur_err_tye]) / (total_err_tyes_count + 1)
-            cur_err_kmer_val1 = (err_kmers2count[cur_kmer1] + kmers_priors[cur_kmer1]) / (total_err_kmers_count + 1)
-            cur_err_kmer_val2 = (err_kmers2count[cur_kmer2] + kmers_priors[cur_kmer2]) / (total_err_kmers_count + 1)
-            ambiguous_reads_features.append([cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])#, row["StartDegree"]
-
-        genuine_fea = self.read2vec(genuine_reads_lst1, genuine_reads_lst2, genuine_reads_features)
-        negative_fea = self.read2vec(negtive_reads_lst1, negtive_reads_lst2, negtive_reads_features)
-        ambiguous_fea = self.read2vec(ambiguous_reads_lst1, ambiguous_reads_lst2, ambiguous_reads_features)
-        del genuine_reads_lst1, genuine_reads_lst2, genuine_reads_features, negtive_reads_lst1, negtive_reads_lst2, negtive_reads_features, ambiguous_reads_lst1, ambiguous_reads_lst2, ambiguous_reads_features
-
-        read_features = genuine_fea + negative_fea
-        new_labels = np.array([1] * len(genuine_fea) + [0] * len(negative_fea))
-        new_train_data = np.array(read_features)
-        shape1 = (len(labels), len(read_features[0]))
-        new_train_data.reshape(shape1)   
-
-        # merge the genuine and negative training data of ambiguous prediction to traininig data for high ambiguous prediction
-        merged_train_data = np.concatenate((train_data, new_train_data), axis=0)
-        merged_train_labels = np.concatenate((train_labels, new_labels), axis=0)
-
-        ambiguous_data = np.array(ambiguous_fea)
-        shape2 = (len(ambiguous_fea), len(ambiguous_fea[0]))
-        ambiguous_data.reshape(shape2) 
-
-        # scaling data
-        self.logger.debug(merged_train_data.shape)
-        self.logger.debug(ambiguous_data.shape)
-
-        train, ambiguous = self.scaler(merged_train_data, ambiguous_data, high_flag=True)
-        
-        self.logger.debug(train[0])
-        
-        del merged_train_data, ambiguous_data, genuine_fea, negative_fea, ambiguous_fea, read_features
-        return train, merged_train_labels, ambiguous
 
     def all_in_one_embedding(self, total_reads, genuine_df, negative_df, ambiguous_df, high_flag):
         self.logger.info("Embedding genuine and ambiguous data.")
         genuine_reads_lst1 = []
         negtive_reads_lst1 = []
         ambiguous_reads_lst1 = []
 
@@ -455,36 +317,46 @@
                 else:
                     ambiguous_reads_features.append([row['StartReadCount'], cur_err_tye_val, cur_err_kmer_val1, cur_err_kmer_val2])#, row["StartDegree"]
             else:
                 ambiguous_reads_features.append([row['StartReadCount']])
 
         # self.logger.debug(f'{len(negtive_reads_lst1), len(negtive_reads_lst2), len(negtive_reads_features)}')
         genuine_fea = self.read2vec(genuine_reads_lst1, genuine_reads_lst2, genuine_reads_features)
+        del genuine_reads_lst1, genuine_reads_lst2, genuine_reads_features
+
         negative_fea = self.read2vec(negtive_reads_lst1, negtive_reads_lst2, negtive_reads_features)
+        del negtive_reads_lst1, negtive_reads_lst2, negtive_reads_features
+        
         ambiguous_fea = self.read2vec(ambiguous_reads_lst1, ambiguous_reads_lst2, ambiguous_reads_features)
-        del genuine_reads_lst1, genuine_reads_lst2, genuine_reads_features, negtive_reads_lst1, negtive_reads_lst2, negtive_reads_features, ambiguous_reads_lst1, ambiguous_reads_lst2, ambiguous_reads_features
+        del ambiguous_reads_lst1, ambiguous_reads_lst2, ambiguous_reads_features
 
         read_features = genuine_fea + negative_fea
-        labels = np.array([1] * len(genuine_fea) + [0] * len(negative_fea))
+        feature_len = len(read_features[0])
         train_data = np.array(read_features, dtype=object)
-        shape1 = (len(labels), len(read_features[0]))
+        gen_len = len(genuine_fea)
+        neg_len = len(negative_fea)
+        del read_features, genuine_fea, negative_fea
+
+        labels = np.array([1] * gen_len + [0] * neg_len)
+        shape1 = ((gen_len + neg_len), feature_len)
         train_data.reshape(shape1)   
-        print(train_data.size)
+
         ambiguous_data = np.array(ambiguous_fea, dtype=object)
         shape2 = (len(ambiguous_fea), len(ambiguous_fea[0]))
+        del ambiguous_fea
         ambiguous_data.reshape(shape2) 
         # scaling data
         self.logger.debug(train_data.shape)
         self.logger.debug(ambiguous_data.shape)
         if self.edit_dis == 1:
             train, ambiguous = self.scaler(train_data, ambiguous_data, high_flag)
         else:
             train, ambiguous = self.scaler2(train_data, ambiguous_data)
         self.logger.debug(train[0])
-        del train_data, ambiguous_data, genuine_fea, negative_fea, ambiguous_fea, read_features
+        del train_data, ambiguous_data
         return train, labels, ambiguous
 
     def scaler2(self, lab_fea, ambiguous_ulab_fea):
         # pos0 = 179
         pos0 = 65
         lab_fea0 = lab_fea[:,0:pos0]
 
@@ -562,16 +434,16 @@
             del lab_scale_f0, lab_scale_f1, lab_scale_f3, ulab_scale_f0, ulab_scale_f1, ulab_scale_f3
                 
         # lab_scale_f = np.hstack((lab_scale_f0, lab_scale_f1, lab_scale_f2, lab_scale_f3))
         # ulab_scale_f = np.hstack((ulab_scale_f0, ulab_scale_f1, ulab_scale_f2, ulab_scale_f3))
         
         return lab_scale_f, ulab_scale_f 
 
-
     # def read2features(self, shared_objects, i):
+    '''
     def read2features(self, ES, ori_feature):
         # ES, reads_lst1, reads_lst2, other_features = shared_objects
         features = []
         
         ###########################################################################
         ft_fea1 = ES.descriptors("FourierTransform", ori_feature[0])
         cg_fea1 = ES.descriptors("ChaosGame", ori_feature[0])
@@ -584,86 +456,63 @@
         atomic_fea1 = ES.descriptors("atomic_number",ori_feature[0])
         atomic_fea2 = ES.descriptors("atomic_number", ori_feature[1])
         features.extend(atomic_fea1)
         features.extend(atomic_fea2)
         
         features.extend(ori_feature[2:])
         return features 
-
+    '''
     def read2vec(self, reads_lst1, reads_lst2, other_features):  
         ES = EncodeScheme(self.config.read_max_len, self.config.entropy_kmer, self.config.entropy_q, self.config.kmer_freq, self.config.read_type)
 
         # Combine the features of each sample into one list
         combined_features = []
         for seq1, seq2, lst in zip(reads_lst1, reads_lst2, other_features):
             tmp_lst = []
             tmp_lst.append(seq1)
             tmp_lst.append(seq2)
             tmp_lst.extend(lst)
             combined_features.append(tmp_lst)
             del tmp_lst
 
         chunk_size = len(combined_features) // self.config.chunks_num
-        remainder = len(combined_features) % self.config.chunks_num
-
         if chunk_size > 0:
-            chunks = []
-            for i in range(self.config.chunks_num):
-                chunks.append(combined_features[i:i+chunk_size])
-            # Handle the remaining elements
-            if remainder > 0:
-                chunks.append(combined_features[-remainder:])
+            chunks = [combined_features[i:i+chunk_size] for i in range(0, len(combined_features), chunk_size)]
         else:
             chunks = combined_features
 
         # Use multiprocessing to write each chunk to a separate pickle file
         chunk_names = []
         for i, chunk in enumerate(chunks):
-            pool = mp.Pool(processes=self.config.num_workers)
-            vectors = pool.starmap(self.read2features, [(ES, sequence) for sequence in chunk])
-            pool.close()
-            pool.join()
+
+            shared_objects = ES, chunk
+            vectors = []
+            with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
+                for fea_lst in pool.imap(self.read2features, range(len(chunk))):
+                    vectors.append(fea_lst)
+
             # Generate the pickle file name
             file_name = self.config.result_dir + f"chunk_{i}.pickle"
             # Write the vectors to the pickle file
             with open(file_name, "wb") as file:
                 pickle.dump(vectors, file)
-
             chunk_names.append(file_name)
-
+            del vectors
+            
         combined_data = []
         for file_name in chunk_names:
             with open(file_name, "rb") as file:
                 vectors = pickle.load(file)
                 combined_data.extend(vectors)
+                del vectors
             os.remove(file_name)
 
         del combined_features, chunks      
         return combined_data
     
-'''
-    def read2vec(self, reads_lst1, reads_lst2, other_features):
-        read_features = []    
-        ES = EncodeScheme(self.config.read_max_len, self.config.entropy_kmer, self.config.entropy_q, self.config.kmer_freq, self.config.read_type)
-
-        shared_objects = ES, reads_lst1, reads_lst2, other_features
-        # with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
-        #     with tqdm(total=len(reads_lst1), desc=self.logger.info("Encoding reads")) as pbar:   
-        #         for fea_lst in pool.imap(self.read2features, range(len(reads_lst1))):
-        #             read_features.append(fea_lst)
-        #             pbar.update()  
-        with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
-            for fea_lst in pool.imap(self.read2features, range(len(reads_lst1)), progress_bar=self.config.verbose):
-                read_features.append(fea_lst)
-        
-        self.logger.debug(f'{len(read_features)}, {len(read_features[0])}')
-        return read_features
-'''
-
-'''
     def high_all_in_one_embedding(self, genuine_df, negative_df, new_negative_df, ambiguous_df):
         self.logger.info("Embedding genuine and high ambiguous data.")
         genuine_reads_lst1 = []
         negtive_reads_lst1 = []
         ambiguous_reads_lst1 = []
 
         genuine_reads_lst2 = []
@@ -809,8 +658,73 @@
         # scaling data
         self.logger.debug(train_data.shape)
         self.logger.debug(ambiguous_data.shape)
         train, ambiguous = self.scaler(train_data, ambiguous_data, high_flag=True)
         self.logger.debug(train[0])
         del train_data, ambiguous_data, genuine_fea, negative_fea, ambiguous_fea, read_features
         return train, labels, ambiguous
-'''
+
+    '''
+    def read2vec(self, reads_lst1, reads_lst2, other_features):
+        read_features = []    
+        ES = EncodeScheme(self.config.read_max_len, self.config.entropy_kmer, self.config.entropy_q, self.config.kmer_freq, self.config.read_type)
+
+        shared_objects = ES, reads_lst1, reads_lst2, other_features
+        # with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
+        #     with tqdm(total=len(reads_lst1), desc=self.logger.info("Encoding reads")) as pbar:   
+        #         for fea_lst in pool.imap(self.read2features, range(len(reads_lst1))):
+        #             read_features.append(fea_lst)
+        #             pbar.update()  
+        with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
+            for fea_lst in pool.imap(self.read2features, range(len(reads_lst1)), progress_bar=self.config.verbose):
+                read_features.append(fea_lst)
+        
+        self.logger.debug(f'{len(read_features)}, {len(read_features[0])}')
+        return read_features
+    '''
+
+    '''
+    def read2features(self, shared_objects, i):
+        ES, reads_lst1, reads_lst2, other_features = shared_objects
+        features = []
+        # pd_fe = ES.descriptors("PairDistance", reads_lst[i])
+        # features.extend(pd_fe)    
+        ###########################################################################
+        # features.append(read_count_lst[i]) 
+        # features.append(err_pos_lst[i]) 
+        # freq_pos.append([ori_seq_freq, err_pos])              
+        ###########################################################################
+        ft_fea1 = ES.descriptors("FourierTransform", reads_lst1[i])
+        cg_fea1 = ES.descriptors("ChaosGame", reads_lst1[i])
+        entropy_fea1 = ES.descriptors("Entropy", reads_lst1[i])
+        fs_fea1 = ES.descriptors("FickettScore", reads_lst1[i])
+
+        features.extend(ft_fea1)
+        features.extend(cg_fea1)
+        features.extend(entropy_fea1)
+        features.extend(fs_fea1)
+        # print(len(features))
+        # ft_fea2 = ES.descriptors("FourierTransform", reads_lst2[i])
+        # cg_fea2 = ES.descriptors("ChaosGame", reads_lst2[i])
+        # # entropy_fea2 = ES.descriptors("Entropy", reads_lst2[i])
+        # fs_fea2 = ES.descriptors("FickettScore", reads_lst2[i])
+
+        # features.extend(ft_fea2)
+        # features.extend(cg_fea2)
+        # # features.extend(entropy_fea2)
+        # features.extend(fs_fea2)
+        # self.logger.debug(len(features))
+        atomic_fea1 = ES.descriptors("atomic_number", reads_lst1[i])
+        atomic_fea2 = ES.descriptors("atomic_number", reads_lst2[i])
+        # atomic_fea1 = ES.descriptors("binary", reads_lst1[i])
+        # atomic_fea2 = ES.descriptors("binary", reads_lst2[i])
+        # print(int(other_features[i][0]))
+        features.extend(atomic_fea1)
+        features.extend(atomic_fea2)
+        # onehot_fea = ES.descriptors("OneHot", reads_lst1[i])
+        # features.extend(onehot_fea)
+        features.extend(other_features[i])
+        # self.logger.debug(f'FourierTransform: {len(ft_fea)}, ChaosGame: {len(cg_fea)}, Entropy: {len(entropy_fea)}, FickettScore: {len(fs_fea)}')
+        return features 
+    '''
+
+
```

### Comparing `noise2read-0.0.90/src/noise2read/simulation.py` & `noise2read-0.0.95/src/noise2read/simulation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/src/noise2read/umitest.py` & `noise2read-0.0.95/src/noise2read/umitest.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/src/noise2read/utils.py` & `noise2read-0.0.95/src/noise2read/utils.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/src/noise2read.egg-info/PKG-INFO` & `noise2read-0.0.95/src/noise2read.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.90
+Version: 0.0.95
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.90/src/noise2read.egg-info/SOURCES.txt` & `noise2read-0.0.95/src/noise2read.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/tests/test_data_generation.py` & `noise2read-0.0.95/tests/test_data_generation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/tests/test_reads2vector.py` & `noise2read-0.0.95/tests/test_reads2vector.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.90/tests/test_utils.py` & `noise2read-0.0.95/tests/test_utils.py`

 * *Files identical despite different names*

