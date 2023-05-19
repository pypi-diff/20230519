# Comparing `tmp/mmif-python-0.5.1.tar.gz` & `tmp/mmif-python-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmif-python-0.5.1.tar", last modified: Tue May  2 02:25:15 2023, max compression
+gzip compressed data, was "mmif-python-0.5.2.tar", last modified: Fri May 19 09:07:42 2023, max compression
```

## Comparing `mmif-python-0.5.1.tar` & `mmif-python-0.5.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.922579 mmif-python-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-02 02:24:47.000000 mmif-python-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 02:24:47.000000 mmif-python-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-02 02:25:15.922579 mmif-python-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-02 02:24:47.000000 mmif-python-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 02:24:47.000000 mmif-python-0.5.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.918579 mmif-python-0.5.1/mmif/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-02 02:24:47.000000 mmif-python-0.5.1/mmif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.922579 mmif-python-0.5.1/mmif/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/res/clams.vocabulary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/res/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/res/mmif.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.922579 mmif-python-0.5.1/mmif/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-02 02:24:47.000000 mmif-python-0.5.1/mmif/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-05-02 02:24:47.000000 mmif-python-0.5.1/mmif/serialize/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-05-02 02:24:47.000000 mmif-python-0.5.1/mmif/serialize/mmif.py
--rw-r--r--   0 runner    (1001) docker     (123)    18396 2023-05-02 02:24:47.000000 mmif-python-0.5.1/mmif/serialize/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-05-02 02:24:47.000000 mmif-python-0.5.1/mmif/serialize/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.922579 mmif-python-0.5.1/mmif/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/ver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/ver/do-not-edit.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.922579 mmif-python-0.5.1/mmif/vocabulary/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/vocabulary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/vocabulary/annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/vocabulary/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/vocabulary/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/vocabulary/document_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.922579 mmif-python-0.5.1/mmif_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 02:24:47.000000 mmif-python-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 02:25:15.922579 mmif-python-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-05-02 02:24:47.000000 mmif-python-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:42.171131 mmif-python-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-19 09:07:13.000000 mmif-python-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-19 09:07:13.000000 mmif-python-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-19 09:07:42.171131 mmif-python-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-19 09:07:13.000000 mmif-python-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 09:07:13.000000 mmif-python-0.5.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:42.167131 mmif-python-0.5.2/mmif/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-19 09:07:13.000000 mmif-python-0.5.2/mmif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:42.167131 mmif-python-0.5.2/mmif/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:41.000000 mmif-python-0.5.2/mmif/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-05-19 09:07:41.000000 mmif-python-0.5.2/mmif/res/clams.vocabulary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-19 09:07:41.000000 mmif-python-0.5.2/mmif/res/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-19 09:07:41.000000 mmif-python-0.5.2/mmif/res/mmif.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:42.167131 mmif-python-0.5.2/mmif/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-19 09:07:13.000000 mmif-python-0.5.2/mmif/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-05-19 09:07:13.000000 mmif-python-0.5.2/mmif/serialize/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-05-19 09:07:13.000000 mmif-python-0.5.2/mmif/serialize/mmif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18712 2023-05-19 09:07:13.000000 mmif-python-0.5.2/mmif/serialize/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-05-19 09:07:13.000000 mmif-python-0.5.2/mmif/serialize/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:42.167131 mmif-python-0.5.2/mmif/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 09:07:41.000000 mmif-python-0.5.2/mmif/ver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-19 09:07:41.000000 mmif-python-0.5.2/mmif/ver/do-not-edit.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:42.167131 mmif-python-0.5.2/mmif/vocabulary/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif/vocabulary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif/vocabulary/annotation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif/vocabulary/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif/vocabulary/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif/vocabulary/document_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:42.167131 mmif-python-0.5.2/mmif_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 09:07:13.000000 mmif-python-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 09:07:42.171131 mmif-python-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-05-19 09:07:13.000000 mmif-python-0.5.2/setup.py
```

### Comparing `mmif-python-0.5.1/LICENSE` & `mmif-python-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.1/PKG-INFO` & `mmif-python-0.5.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
-Description: # MMIF for python 
-        
-        **NOTE** that this project is in pre-alpha and being actively developed. Nothing is guaranteed to reliably work for the moment and developer need to be very careful when using APIs implemented here. Please use [the issue track](https://github.com/clamsproject/mmif/issues) to report bugs and malfunctions.
-        
-        ## MultiMedia Interchange Format
+Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai). 
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers 
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mmif-python-0.5.1/mmif/res/clams.vocabulary.yaml` & `mmif-python-0.5.2/mmif/res/clams.vocabulary.yaml`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.1/mmif/res/mmif.json` & `mmif-python-0.5.2/mmif/res/mmif.json`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.1/mmif/serialize/annotation.py` & `mmif-python-0.5.2/mmif/serialize/annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,18 @@
     subdocuments grouped together logically.
 
     If ``document_obj`` is not provided, an empty Document will be generated.
 
     :param document_obj: the JSON data that defines the document
     """
     def __init__(self, doc_obj: Optional[Union[bytes, str, dict]] = None) -> None:
+        # to store the parent view ID
         self._parent_view_id = ''
+        self.reserved_names.add('_parent_view_id')
+        
         self._type: Union[ThingTypesBase, DocumentTypesBase] = ThingTypesBase('')
         self.properties: DocumentProperties = DocumentProperties()
         self.disallow_additional_properties()
         self._attribute_classes = {'properties': DocumentProperties}
         super().__init__(doc_obj)
 
     @property
```

### Comparing `mmif-python-0.5.1/mmif/serialize/mmif.py` & `mmif-python-0.5.2/mmif/serialize/mmif.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.1/mmif/serialize/model.py` & `mmif-python-0.5.2/mmif/serialize/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """
     Abstract superclass for MMIF related key-value pair objects.
 
     Any MMIF object can be initialized as an empty placeholder or
     an actual representation with a JSON formatted string or equivalent
     `dict` object argument.
 
-    This superclass has three specially designed instance variables, and these
+    This superclass has four specially designed instance variables, and these
     variable names cannot be used as attribute names for MMIF objects.
 
     1. _unnamed_attributes:
        Only can be either None or an empty dictionary. If it's set to None,
        it means the class won't take any ``Additional Attributes`` in the JSON
        schema sense. If it's a dict, users can throw any k-v pairs to the
        class, EXCEPT for the reserved two key names.
@@ -50,52 +50,55 @@
        deserialize the value. Note that a key name in this dict does NOT
        have to be a *named* attribute, but is recommended to be one.
     3. _required_attributes:
        This is a simple list of names of attributes that are required in the object.
        When serialize, an object will skip its *empty* (e.g. zero-length, or None)
        attributes unless they are in this list. Otherwise, the serialized JSON
        string would have empty representations (e.g. ``""``, ``[]``).
+    4. _exclude_from_diff:
+       This is a simple list of names of attributes that should be excluded from
+       the diff calculation in ``__eq__``. 
 
     # TODO (krim @ 8/17/20): this dict is however, a duplicate with the type hints in the class definition.
     Maybe there is a better way to utilize type hints (e.g. getting them as a programmatically), but for now
     developers should be careful to add types to hints as well as to this dict.
 
-    Also note that those two special attributes MUST be set in the __init__()
+    Also note that those special attributes MUST be set in the __init__()
     before calling super method, otherwise deserialization will not work.
 
     And also, a subclass that has one or more *named* attributes, it must
     set those attributes in the __init__() before calling super method. When
     serializing a MmifObject, all *empty* attributes will be ignored, so for
     optional named attributes, you must leave the values empty (len == 0), but
     NOT None. Any None-valued named attributes will cause issues with current
     implementation.
 
     :param mmif_obj: JSON string or `dict` to initialize an object.
      If not given, an empty object will be initialized, sometimes with
      an ID value automatically generated, based on its parent object.
     """
     
-    reserved_names: Set = {
+    reserved_names: Set[str] = {
         'reserved_names',
         '_unnamed_attributes',
         '_attribute_classes',
         '_required_attributes',
-        # used in Document class to store parent view id
-        '_parent_view_id', 
-        # used in View class to autogenerate annotation ids
-        '_id_counts'
+        '_exclude_from_diff'
     }
     _unnamed_attributes: Optional[dict]
+    _exclude_from_diff: Set[str]
     _attribute_classes: Dict[str, Type] = {}  # Mapping: str -> Type
 
     def __init__(self, mmif_obj: Optional[Union[bytes, str, dict]] = None) -> None:
         if isinstance(mmif_obj, bytes):
             mmif_obj = mmif_obj.decode('utf8')
         if not hasattr(self, '_required_attributes'):
             self._required_attributes = []
+        if not hasattr(self, '_exclude_from_diff'):
+            self._exclude_from_diff = set()
         if not hasattr(self, '_unnamed_attributes'):
             self._unnamed_attributes = {}
         if mmif_obj is not None:
             self.deserialize(mmif_obj)
 
     def disallow_additional_properties(self) -> None:
         """
@@ -249,15 +252,18 @@
                 self[k] = v
 
     def __str__(self) -> str:
         return self.serialize(False)
 
     def __eq__(self, other) -> bool:
         return isinstance(other, type(self)) and \
-               len(DeepDiff(self, other, report_repetition=True, exclude_types=[datetime])) == 0
+               len(DeepDiff(self, other, report_repetition=True, exclude_types=[datetime],
+                            # https://github.com/clamsproject/mmif-python/issues/214
+                            exclude_paths=self._exclude_from_diff)
+                   ) == 0
 
     def __len__(self) -> int:
         """
         Returns number of attributes that are not *empty*. 
         """
         return sum([named in self and not self.is_empty(self[named]) for named in self._named_attributes()]) \
                + (len(self._unnamed_attributes) if self._unnamed_attributes else 0)
```

### Comparing `mmif-python-0.5.1/mmif/serialize/view.py` & `mmif-python-0.5.2/mmif/serialize/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,19 @@
 
     If ``view_obj`` is not provided, an empty View will be generated.
 
     :param view_obj: the JSON data that defines the view
     """
 
     def __init__(self, view_obj: Optional[Union[bytes, str, dict]] = None) -> None:
+        # used to autogenerate annotation ids
         self._id_counts = {}
+        self.reserved_names.add("_id_counts")
+        self._exclude_from_diff = {"_id_counts"}
+        
         self.id: str = ''
         self.metadata: ViewMetadata = ViewMetadata()
         self.annotations: AnnotationsList = AnnotationsList()
         self.disallow_additional_properties()
         self._attribute_classes = {
             'metadata': ViewMetadata,
             'annotations': AnnotationsList
```

### Comparing `mmif-python-0.5.1/mmif/vocabulary/annotation_types.py` & `mmif-python-0.5.2/mmif/vocabulary/annotation_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.1/mmif/vocabulary/base_types.py` & `mmif-python-0.5.2/mmif/vocabulary/base_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.1/mmif/vocabulary/document_types.py` & `mmif-python-0.5.2/mmif/vocabulary/document_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.1/mmif_python.egg-info/PKG-INFO` & `mmif-python-0.5.2/mmif_python.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
-Description: # MMIF for python 
-        
-        **NOTE** that this project is in pre-alpha and being actively developed. Nothing is guaranteed to reliably work for the moment and developer need to be very careful when using APIs implemented here. Please use [the issue track](https://github.com/clamsproject/mmif/issues) to report bugs and malfunctions.
-        
-        ## MultiMedia Interchange Format
+Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai). 
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers 
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mmif-python-0.5.1/mmif_python.egg-info/SOURCES.txt` & `mmif-python-0.5.2/mmif_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.1/setup.py` & `mmif-python-0.5.2/setup.py`

 * *Files identical despite different names*

