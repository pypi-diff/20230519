# Comparing `tmp/smalltools_st-0.1.1.tar.gz` & `tmp/smalltools_st-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smalltools_st-0.1.1.tar", last modified: Tue Mar 28 20:56:38 2023, max compression
+gzip compressed data, was "smalltools_st-0.2.0.tar", max compression
```

## Comparing `smalltools_st-0.1.1.tar` & `smalltools_st-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,8 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 20:56:38.976511 smalltools_st-0.1.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2023-03-28 20:56:23.000000 smalltools_st-0.1.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7598 2023-03-28 20:56:38.976511 smalltools_st-0.1.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6791 2023-03-28 20:56:23.000000 smalltools_st-0.1.1/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      881 2023-03-28 20:56:23.000000 smalltools_st-0.1.1/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-03-28 20:56:38.976511 smalltools_st-0.1.1/setup.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 20:56:38.972511 smalltools_st-0.1.1/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 20:56:38.976511 smalltools_st-0.1.1/src/smalltools_st/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-28 20:56:23.000000 smalltools_st-0.1.1/src/smalltools_st/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 20:56:38.976511 smalltools_st-0.1.1/src/smalltools_st/behavior/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-28 20:56:23.000000 smalltools_st-0.1.1/src/smalltools_st/behavior/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2801 2023-03-28 20:56:23.000000 smalltools_st-0.1.1/src/smalltools_st/behavior/suitable_class_finder.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 20:56:38.976511 smalltools_st-0.1.1/src/smalltools_st.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7598 2023-03-28 20:56:38.000000 smalltools_st-0.1.1/src/smalltools_st.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      353 2023-03-28 20:56:38.000000 smalltools_st-0.1.1/src/smalltools_st.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-28 20:56:38.000000 smalltools_st-0.1.1/src/smalltools_st.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2023-03-28 20:56:38.000000 smalltools_st-0.1.1/src/smalltools_st.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-28 20:56:38.976511 smalltools_st-0.1.1/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1945 2023-03-28 20:56:23.000000 smalltools_st-0.1.1/tests/test_suitable_class_finder.py
+-rw-r--r--   0        0        0     1080 2023-05-18 23:23:26.494875 smalltools_st-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1636 2023-05-18 23:23:26.494875 smalltools_st-0.2.0/README.md
+-rw-r--r--   0        0        0     1215 2023-05-18 23:23:26.494875 smalltools_st-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-18 23:23:26.494875 smalltools_st-0.2.0/smalltools_st/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 23:23:26.494875 smalltools_st-0.2.0/smalltools_st/behavior/__init__.py
+-rw-r--r--   0        0        0     3795 2023-05-18 23:23:26.494875 smalltools_st-0.2.0/smalltools_st/behavior/cascading.py
+-rw-r--r--   0        0        0     2916 2023-05-18 23:23:26.494875 smalltools_st-0.2.0/smalltools_st/behavior/suitable_class_finder.py
+-rw-r--r--   0        0        0     2828 1970-01-01 00:00:00.000000 smalltools_st-0.2.0/PKG-INFO
```

### Comparing `smalltools_st-0.1.1/LICENSE` & `smalltools_st-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smalltools_st-0.1.1/src/smalltools_st/behavior/suitable_class_finder.py` & `smalltools_st-0.2.0/smalltools_st/behavior/suitable_class_finder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from typing import List, Union
+
+
 is_concrete = lambda subclass: len(subclass.__subclasses__()) == 0
 
 
-def concrete_subclasses(a_class, accumulator):
+def concrete_subclasses(a_class: type, accumulator: List[type]) -> List[type]:
     """For this package, concrete class is any with no subclasses.
     
     Parameters:
     - :a_class: : Any class object
     - :accumulator: (optional): A list with all concrete subclasses partially found for :a_class:
 
     Returns:
@@ -23,25 +26,25 @@
     """Given the hierarchy of an abstract class, it detects the appropriate 
     concrete subclass (deterministically) that satisfies certain attributes 
     obtained as a parameter.
     Useful for implementing the Strategy design pattern.
     """
 
 
-    def __init__(self, abstract_class):
+    def __init__(self, abstract_class: type) -> None:
         """Initialization of the subclass finder.
 
         Parameter:
         - :abstract_class: : Any class object
         """
         self.abstract_class = abstract_class
         super().__init__()
 
 
-    def suitable_for(self, *suitable_object, default_subclass=None, suitable_method='can_handle'):
+    def suitable_for(self, *suitable_object, default_subclass: Union[None, type] = None, suitable_method: str = 'can_handle') -> type:
         """Finds the concrete subclass that satisfies the conditions modeled 
         with the :suitable_object: and the :suitable_method:
 
         Parameters:
         - :*suitable_object: : Positional arguments of any kind
         - :default_subclass: (optional): Its the object to be returned when no subclass is found. Keep
         it as :None: to ensure a match or an exception.
```

