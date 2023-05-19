# Comparing `tmp/qgate_graph-1.3rc1-py3-none-any.whl.zip` & `tmp/qgate_graph-1.3rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10835 bytes, number of entries: 12
+Zip file size: 10842 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_graph/__init__.py
 -rw-rw-rw-  2.0 fat      913 b- defN 23-Apr-27 20:17 qgate_graph/constant.py
 -rw-rw-rw-  2.0 fat     1057 b- defN 23-Apr-30 11:34 qgate_graph/file_format.py
 -rw-rw-rw-  2.0 fat     8694 b- defN 23-Apr-29 15:40 qgate_graph/graph.py
 -rw-rw-rw-  2.0 fat     2378 b- defN 23-May-01 17:36 qgate_graph/graph_base.py
--rw-rw-rw-  2.0 fat     7360 b- defN 23-May-01 17:36 qgate_graph/graph_executor.py
+-rw-rw-rw-  2.0 fat     7378 b- defN 23-May-04 20:53 qgate_graph/graph_executor.py
 -rw-rw-rw-  2.0 fat     7150 b- defN 23-May-01 17:36 qgate_graph/graph_performance.py
--rw-rw-rw-  2.0 fat      216 b- defN 23-May-01 17:51 qgate_graph/version.py
--rw-rw-rw-  2.0 fat     1206 b- defN 23-May-01 17:51 qgate_graph-1.3rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-01 17:51 qgate_graph-1.3rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-01 17:51 qgate_graph-1.3rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      970 b- defN 23-May-01 17:51 qgate_graph-1.3rc1.dist-info/RECORD
-12 files, 30088 bytes uncompressed, 9205 bytes compressed:  69.4%
+-rw-rw-rw-  2.0 fat      216 b- defN 23-May-04 20:54 qgate_graph/version.py
+-rw-rw-rw-  2.0 fat     1204 b- defN 23-May-04 20:55 qgate_graph-1.3rc2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-04 20:55 qgate_graph-1.3rc2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-04 20:55 qgate_graph-1.3rc2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      970 b- defN 23-May-04 20:55 qgate_graph-1.3rc2.dist-info/RECORD
+12 files, 30104 bytes uncompressed, 9212 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: qgate_graph/graph_performance.py
 Comment: 
 
 Filename: qgate_graph/version.py
 Comment: 
 
-Filename: qgate_graph-1.3rc1.dist-info/METADATA
+Filename: qgate_graph-1.3rc2.dist-info/METADATA
 Comment: 
 
-Filename: qgate_graph-1.3rc1.dist-info/WHEEL
+Filename: qgate_graph-1.3rc2.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_graph-1.3rc1.dist-info/top_level.txt
+Filename: qgate_graph-1.3rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_graph-1.3rc1.dist-info/RECORD
+Filename: qgate_graph-1.3rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_graph/graph_executor.py

```diff
@@ -117,16 +117,16 @@
                     if executor:
                         plan=f"{input_dict[const.FileFormat.PRF_CORE_PLAN_EXECUTOR][0]},{input_dict[const.FileFormat.PRF_CORE_PLAN_EXECUTOR][1]}"
                         executors[plan]=executor
 
                         if input_dict.get(const.FileFormat.PRF_CORE_TIME_END):
                             end_date=input_dict[const.FileFormat.PRF_CORE_TIME_END]
 
-                        file_name=f"{file_name}-plan-{plan}"
-                        self._show_graph(start_date, executors, end_date, title, file_name, output_dir)
+                        #file_name=f"{file_name}-plan-{plan}"
+                        self._show_graph(start_date, executors, end_date, title, f"{file_name}-plan-{plan}", output_dir)
                         executors.clear()
                         executor.clear()
                 elif input_dict[const.FileFormat.PRF_TYPE] == const.FileFormat.PRF_DETAIL_TYPE:
                     # detail
                     executor.append([
                         input_dict[const.FileFormat.PRF_DETAIL_TIME_INIT],
                         input_dict[const.FileFormat.PRF_DETAIL_TIME_START],
```

## qgate_graph/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '1.3rc1'
+__version__ = '1.3rc2'
```

## Comparing `qgate_graph-1.3rc1.dist-info/METADATA` & `qgate_graph-1.3rc2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-graph
-Version: 1.3rc1
+Version: 1.3rc2
 Summary: Generate graphs based on outputs from Quality Gate
 Home-page: https://github.com/george0st/qgate-graph/
 Download-URL: https://pypi.org/project/qgate_graph/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: Quality,QualityGate,Graph
@@ -30,13 +30,12 @@
     # generate performance/throughput graphs
     graph=GraphPerformance()
     graph.generate_from_dir()
     
     # generate excutors in time graphs
     graph=grp.GraphExecutor()
     graph.generate_from_dir()
-
 ```
 
 # Outputs
 ![graph](./assets/NoSQL_bdp_nonprod-2023-04-22_17-08-34-bulk-10000x50.png)
```

## Comparing `qgate_graph-1.3rc1.dist-info/RECORD` & `qgate_graph-1.3rc2.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 qgate_graph/__init__.py,sha256=1_WzwjEn3Ro-VrDe9uO1r2TbTq6YPSaErStlN5aF3_4,40
 qgate_graph/constant.py,sha256=-M9nKz0nSLhAefMDv8ojwVEB7mhqPDDVb3fDiZmfSEA,913
 qgate_graph/file_format.py,sha256=SGkMW-ecYHH6uL6qoTdLq6cIlUR49Cyn3ZmHRh_tOS8,1057
 qgate_graph/graph.py,sha256=qBPR1ur2pfBkkweY-EX7TcF5ycv7Y4j6Vr5FkS_tAFg,8694
 qgate_graph/graph_base.py,sha256=TfeXdujn7hNkFa1KJRhMpggzJT9PmTtv3Tf-2Y7po7o,2378
-qgate_graph/graph_executor.py,sha256=pSzgyCzsGvRq12XLME0CieqvYTRQqOj83Tfm887tLuY,7360
+qgate_graph/graph_executor.py,sha256=IsrcQ9JLlQ2k28HDlPtL_oOwJj15TAVkucPeNaVUd2c,7378
 qgate_graph/graph_performance.py,sha256=VXyl_cQbyiocsGlFKKhz09-LvWr7yYTqXNWyi2J6xTI,7150
-qgate_graph/version.py,sha256=kDwTqkkA3Orz4Usx49OacQvMeg7cYq2MFYV02keCSVA,216
-qgate_graph-1.3rc1.dist-info/METADATA,sha256=PE0sS29sEOZ2Yo3Tu2xvEPgufg48KZCtisjmjA6BVoU,1206
-qgate_graph-1.3rc1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qgate_graph-1.3rc1.dist-info/top_level.txt,sha256=r_EQSAP5T-YDt1-k2dnDdf7x3Zc3IECXzqMMH0AaDjo,12
-qgate_graph-1.3rc1.dist-info/RECORD,,
+qgate_graph/version.py,sha256=CmNuUzrmzYASk-7BTWX2Et4zaIaO-K-_DNEymdrJXiA,216
+qgate_graph-1.3rc2.dist-info/METADATA,sha256=kjLfN1ejucJqkKXPFQqVuavtQom9Jue7eQjgeHP8_WY,1204
+qgate_graph-1.3rc2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qgate_graph-1.3rc2.dist-info/top_level.txt,sha256=r_EQSAP5T-YDt1-k2dnDdf7x3Zc3IECXzqMMH0AaDjo,12
+qgate_graph-1.3rc2.dist-info/RECORD,,
```

