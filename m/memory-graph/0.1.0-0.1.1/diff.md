# Comparing `tmp/memory_graph-0.1.0.tar.gz` & `tmp/memory_graph-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_graph-0.1.0.tar", last modified: Fri May 19 18:26:27 2023, max compression
+gzip compressed data, was "memory_graph-0.1.1.tar", last modified: Fri May 19 19:57:22 2023, max compression
```

## Comparing `memory_graph-0.1.0.tar` & `memory_graph-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-19 18:26:27.904592 memory_graph-0.1.0/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.0/LICENSE.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.0/MANIFEST.in
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      543 2023-05-19 18:26:27.904592 memory_graph-0.1.0/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1454 2023-05-19 18:20:27.000000 memory_graph-0.1.0/README.md
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-19 18:26:27.904592 memory_graph-0.1.0/memory_graph/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.0/memory_graph/Node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2167 2023-05-19 18:17:38.000000 memory_graph-0.1.0/memory_graph/__init__.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3528 2023-05-19 18:17:38.000000 memory_graph-0.1.0/memory_graph/grapviz_nodes.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4890 2023-05-19 18:17:38.000000 memory_graph-0.1.0/memory_graph/rewrite.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1411 2023-05-19 18:17:38.000000 memory_graph-0.1.0/memory_graph/rewrite_to_node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.0/memory_graph/rewrite_to_string.py
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-19 18:26:27.904592 memory_graph-0.1.0/memory_graph.egg-info/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      543 2023-05-19 18:26:27.000000 memory_graph-0.1.0/memory_graph.egg-info/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      387 2023-05-19 18:26:27.000000 memory_graph-0.1.0/memory_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-19 18:26:27.000000 memory_graph-0.1.0/memory_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-19 18:26:27.000000 memory_graph-0.1.0/memory_graph.egg-info/requires.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-19 18:26:27.000000 memory_graph-0.1.0/memory_graph.egg-info/top_level.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-19 18:26:27.904592 memory_graph-0.1.0/setup.cfg
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      664 2023-05-19 18:17:38.000000 memory_graph-0.1.0/setup.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-19 19:57:22.229490 memory_graph-0.1.1/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.1/LICENSE.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.1/MANIFEST.in
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2151 2023-05-19 19:57:22.229490 memory_graph-0.1.1/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1576 2023-05-19 19:53:02.000000 memory_graph-0.1.1/README.md
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-19 19:57:22.229490 memory_graph-0.1.1/memory_graph/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.1/memory_graph/Node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2167 2023-05-19 19:57:05.000000 memory_graph-0.1.1/memory_graph/__init__.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3528 2023-05-19 18:17:38.000000 memory_graph-0.1.1/memory_graph/grapviz_nodes.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4890 2023-05-19 18:17:38.000000 memory_graph-0.1.1/memory_graph/rewrite.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1457 2023-05-19 19:02:30.000000 memory_graph-0.1.1/memory_graph/rewrite_to_node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.1/memory_graph/rewrite_to_string.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-19 19:57:22.229490 memory_graph-0.1.1/memory_graph.egg-info/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2151 2023-05-19 19:57:22.000000 memory_graph-0.1.1/memory_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      387 2023-05-19 19:57:22.000000 memory_graph-0.1.1/memory_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-19 19:57:22.000000 memory_graph-0.1.1/memory_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-19 19:57:22.000000 memory_graph-0.1.1/memory_graph.egg-info/requires.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-19 19:57:22.000000 memory_graph-0.1.1/memory_graph.egg-info/top_level.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-19 19:57:22.229490 memory_graph-0.1.1/setup.cfg
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      966 2023-05-19 19:57:01.000000 memory_graph-0.1.1/setup.py
```

### Comparing `memory_graph-0.1.0/LICENSE.txt` & `memory_graph-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.0/README.md` & `memory_graph-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 data = [ (1, 2), [3, 4], {5:'five', 6:'six'} ]
 memory_graph.show( data )
 ```
 
 This shows the graph with the starting point of your 'data' drawn using thick
 lines, the program blocks until the <ENTER> key is pressed.
 
-![image](images/example1.png)
+![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example1.png)
 
 If `show()` doesn't work well on your system (the PDF viewer integration
 is platform specific) use `render()` to output the graph in the format
 of your choosing. Use `block=False` to turn off blocking.
 
 ```
 memory_graph.render( data, "my_graph.png", block=False)
@@ -47,22 +47,22 @@
 
 data=[my_list, my_list, obj1, obj2]
 
 my_list.append(data) # recursive reference
 
 memory_graph.show( data )
 ```
-![image](images/example2.png)
+![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example2.png)
 
 ### Install ###
 
 Install using pip:
 
 ```
-pip install memory_graph
+pip install memory-graph
 ```
 
 ### Author ###
 Bas Terwijn
 
 ### Inspiration ###
 Inspired by [PythonTutor](https://pythontutor.com/visualize.html).
```

### Comparing `memory_graph-0.1.0/memory_graph/Node.py` & `memory_graph-0.1.1/memory_graph/Node.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.0/memory_graph/__init__.py` & `memory_graph-0.1.1/memory_graph/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from memory_graph import rewrite
 from memory_graph import Node
 from memory_graph import rewrite_to_node
 from memory_graph import grapviz_nodes
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __author__ = 'Bas Terwijn'
 
 def show(data,block=True):
     graph=create(data)
     graph.view()
     if block:
         input(f"showing '{graph.filename}', press <ENTER> to continue...")
```

### Comparing `memory_graph-0.1.0/memory_graph/grapviz_nodes.py` & `memory_graph-0.1.1/memory_graph/grapviz_nodes.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.0/memory_graph/rewrite.py` & `memory_graph-0.1.1/memory_graph/rewrite.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.0/memory_graph/rewrite_to_node.py` & `memory_graph-0.1.1/memory_graph/rewrite_to_node.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from types import NoneType
 from types import MappingProxyType
 
 from memory_graph import rewrite
 from memory_graph import Node
 
 reduce_references=True
+reduce_reference_types={NoneType, bool, int, float, str, complex, range, bytes}
 
 def is_duplication_type(value):
-    return type(value) in {NoneType, bool, int, float, str, complex, range, bytes}
+    return type(value) in reduce_reference_types
 
 def my_construct_singular(data):
     node=Node.Node(data)
     node.add_element(Node.Element(value=data))
     return node
 
 def my_construct_iterable(data):
```

### Comparing `memory_graph-0.1.0/memory_graph/rewrite_to_string.py` & `memory_graph-0.1.1/memory_graph/rewrite_to_string.py`

 * *Files identical despite different names*

