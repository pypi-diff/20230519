# Comparing `tmp/clams-python-0.6.0.tar.gz` & `tmp/clams-python-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-0.6.0.tar", last modified: Wed May  3 02:46:30 2023, max compression
+gzip compressed data, was "clams-python-0.6.1.tar", last modified: Fri May 19 12:56:04 2023, max compression
```

## Comparing `clams-python-0.6.0.tar` & `clams-python-0.6.1.tar`

### file list

```diff
@@ -1,32 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-03 02:45:59.000000 clams-python-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 02:45:59.000000 clams-python-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-03 02:46:30.703936 clams-python-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-03 02:45:59.000000 clams-python-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 02:45:59.000000 clams-python-0.6.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-03 02:45:59.000000 clams-python-0.6.0/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/app/
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-05-03 02:45:59.000000 clams-python-0.6.0/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (123)    16339 2023-05-03 02:45:59.000000 clams-python-0.6.0/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-03 02:45:59.000000 clams-python-0.6.0/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-05-03 02:45:59.000000 clams-python-0.6.0/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-03 02:45:59.000000 clams-python-0.6.0/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/source/
--rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-05-03 02:45:59.000000 clams-python-0.6.0/clams/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 02:46:30.000000 clams-python-0.6.0/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:46:30.703936 clams-python-0.6.0/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-03 02:46:30.000000 clams-python-0.6.0/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-03 02:46:30.000000 clams-python-0.6.0/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 02:46:30.000000 clams-python-0.6.0/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 02:46:30.000000 clams-python-0.6.0/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 02:46:30.000000 clams-python-0.6.0/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 02:46:30.000000 clams-python-0.6.0/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-03 02:45:59.000000 clams-python-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 02:46:30.703936 clams-python-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-03 02:45:59.000000 clams-python-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.832249 clams-python-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-19 12:55:41.000000 clams-python-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 12:55:41.000000 clams-python-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-19 12:56:04.832249 clams-python-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-19 12:55:41.000000 clams-python-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 12:55:41.000000 clams-python-0.6.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    16524 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.824250 clams-python-0.6.1/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/CLAMS-generic-readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/app/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/develop/templates/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/develop/templates/github/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-05-19 12:55:41.000000 clams-python-0.6.1/clams/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.828250 clams-python-0.6.1/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 12:56:04.000000 clams-python-0.6.1/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:56:04.832249 clams-python-0.6.1/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-19 12:56:04.000000 clams-python-0.6.1/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-19 12:56:04.000000 clams-python-0.6.1/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:56:04.000000 clams-python-0.6.1/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 12:56:04.000000 clams-python-0.6.1/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-19 12:56:04.000000 clams-python-0.6.1/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 12:56:04.000000 clams-python-0.6.1/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 12:55:41.000000 clams-python-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 12:56:04.832249 clams-python-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-19 12:55:41.000000 clams-python-0.6.1/setup.py
```

### Comparing `clams-python-0.6.0/LICENSE` & `clams-python-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.0/PKG-INFO` & `clams-python-0.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 0.6.0
+Version: 0.6.1
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
-Description: # CLAMS sdk for python 
-        
-        **NOTE** that this project is in pre-alpha stage and being actively developed. Nothing is guaranteed to reliably work for the moment and developers need to be very careful when using APIs implemented here. Please use [the issue track](https://github.com/clamsproject/clams-python/issues) to report bugs and malfunctions, or send us pull requests for even more contribution. 
-        
-        ## CLAMS project
-        [CLAMS project](https://clams.ai) aims at free and open-source software platform for computational analysis and metadata generation applications for multimedia material. To achieve interoperability between various computational applications developed be different vendors, which is absolutely necessary for piping applications together supported by user-friendly workflow engines, we are also developing JSON(-LD)-based MultiMedia Interchange Format ([MMIF](https://mmif.clams.ai))
+Description: ## CLAMS project
+        [CLAMS project](https://clams.ai) aims at free and open-source software platform for computational analysis and metadata generation applications for multimedia material. We believe free and open AI-based multimedia processing platform can bring many benefits of technical advancement to libraries, archives, and museums. To achieve interoperability between various computational applications developed be different vendors, which is absolutely necessary for using applications together supported by user-friendly workflow engines, we are also developing JSON-based MultiMedia Interchange Format ([MMIF](https://mmif.clams.ai))
         
         ## clams-python
-        `clams-python` is a Python implementation of the CLAMS SDK. `clams-python` supports; 
+        `clams-python` is a Python implementation of the CLAMS SDK. `clams-python` provides CLAMS app developers with the following assistance ; 
         
         1. handling MMIF files for input and output specification for CLAMS apps
-        1. a base class to start developing a CLAMS app
-        1. a flask-based wrapper to run a Python CLAMS app as a HTTP web app
+        1. a base Python class to start developing a CLAMS app
+        1. a flask-based wrapper to run a Python CLAMS app as an HTTP web app
+        1. cookie-cutter shell command that sets up everything and starts a new CLAMS app project
+        
+        ### Start now from [Getting Started](introduction.html)!
         
         ## For more ...
-        For user manuals and Python API documentation, take a look at [the SDK website](https://clams.ai/clams-python).
+        For user manuals and Python API documentation, take a look at [Python modules](https://clams.ai/clams-python/modules.html).
         
         For MMIF-specific Python API documentation, take a look at the [mmif-python website](https://clams.ai/mmif-python).
         
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-0.6.0/clams/__init__.py` & `clams-python-0.6.1/clams/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from clams import source
 from clams import develop
 from clams.app import *
 from clams.app import __all__ as app_all
 from clams.appmetadata import AppMetadata
 from clams.restify import Restifier
-from clams.source import PipelineSource
+from clams.source import WorkflowSource
 from clams.develop import CookieCutter
 from clams.ver import __version__
 
-__all__ = [AppMetadata, Restifier, PipelineSource] + app_all
+__all__ = [AppMetadata, Restifier, WorkflowSource] + app_all
 version_template = "{} (based on MMIF spec: {})"
 
 
 def prep_argparser():
     import argparse
     parser = argparse.ArgumentParser()
     parser.add_argument(
```

### Comparing `clams-python-0.6.0/clams/app/__init__.py` & `clams-python-0.6.1/clams/app/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         {
             'name': 'pretty', 'type': 'boolean', 'choices': None, 'default': False, 'multivalued': False,
             'description': 'The JSON body of the HTTP response will be re-formatted with 2-space indentation',
         },
     ]
 
     def __init__(self):
-        self.metadata: AppMetadata = self._load_metadata()
+        self.metadata: AppMetadata = self._load_appmetadata()
         super().__init__()
         # data type specification for common parameters
         python_type = {"boolean": bool, "number": float, "integer": int, "string": str}
 
         self.metadata_param_spec = {}
         self.annotate_param_spec = {}
         for param in ClamsApp.universal_parameters:
@@ -48,39 +48,41 @@
         A public method to get metadata for this app as a string.
 
         :return: Serialized JSON string of the metadata
         """
         pretty = kwargs.pop('pretty') if 'pretty' in kwargs else False
         return self.metadata.jsonify(pretty)
     
-    def _load_metadata(self):
-        cwd = pathlib.Path(sys.modules[self.__module__].__file__).parent
+    def _load_appmetadata(self) -> AppMetadata:
+        """
+        A private method to load the app metadata. This is called in __init__, 
+        (only once) and it uses three sources to load the metadata (in the order 
+        of priority):
+        
+        #. using a ``metadata.py`` file (recommended)
+        #. using self._appmetadata() method (legacy, no longer recommended)
+        
+        In any case, :class:`~clams.appmetadata.AppMetadata` class must be useful.
         
-        # metadata compilation priority
-        # 1. metadata.py
-        # 2. metadata.json
-        # 3. _appmetadata() method (for legacy)
+        For metadata specification, 
+        see `https://sdk.clams.ai/appmetadata.jsonschema <../appmetadata.jsonschema>`_. 
+        """
+        cwd = pathlib.Path(sys.modules[self.__module__].__file__).parent
         
         if (cwd / 'metadata.py').exists():
             import metadata as metadatapy  # pytype: disable=import-error
             metadata = metadatapy.appmetadata()
-        elif (cwd / 'metadata.json').exists():
-            import json
-            with open(cwd / 'metadata.json') as f:
-                metadata = json.load(f)
         else:
             metadata = self._appmetadata()
         return metadata
 
     @abstractmethod
     def _appmetadata(self) -> AppMetadata:
         """
-        An abstract method to generate (or load if stored elsewhere) the app metadata
-        at runtime. All CLAMS app must implement this. For metadata specification, 
-        see `https://sdk.clams.ai/appmetadata.jsonschema <../appmetadata.jsonschema>`_. 
+        An abstract method to generate the app metadata. 
 
         :return: A Python object of the metadata, must be JSON-serializable
         """
         raise NotImplementedError()
 
     @staticmethod
     def _check_mmif_compatibility(target_specver, input_specver):
@@ -92,15 +94,14 @@
         wrapper around :meth:`~clams.app.ClamsApp._annotate` method where some common operations
         (that are invoked by keyword arguments) are implemented.
 
         :param mmif: An input MMIF object to annotate
         :param runtime_params: An arbitrary set of k-v pairs to configure the app at runtime
         :return: Serialized JSON string of the output of the app
         """
-        # TODO (krim @ 12/17/20): add documentation on what are "common" operations
         pretty = runtime_params.get('pretty', False)
         if not isinstance(mmif, Mmif):
             mmif = Mmif(mmif)
         issued_warnings = []
         for key in runtime_params:
             if key not in self.annotate_param_spec:
                 issued_warnings.append(UserWarning(f'An undefined parameter {key} (value: {runtime_params[key]}) is passed'))
@@ -116,21 +117,23 @@
 
     @abstractmethod
     def _annotate(self, mmif: Mmif, **runtime_params) -> Mmif:
         """
         An abstract method to generate (or load if stored elsewhere) the app 
         metadata at runtime. All CLAMS app must implement this.
         
+        This is where the bulk of your logic will go.
         A typical implementation of this method would be 
         
         #. Create a new view (or views) by calling :meth:`~mmif.serialize.mmif.Mmif.new_view` on the input mmif object.
         #. Call :meth:`~clams.app.ClamsApp.sign_view` with the input runtime parameters for the record.
         #. Call :meth:`~clams.app.ClamsApp.get_configuration` to get an "upgraded" runtime parameters with default values.
         #. Call :meth:`~mmif.serialize.view.View.new_contain` on the new view object with any annotation properties specified by the configuration.
         #. Process the data and create :class:`~mmif.serialize.annotation.Annotation` objects and add them to the new view. 
+        #. While doing so, get help from :class:`~mmif.vocabulary.document_types.DocumentTypes`, :class:`~mmif.vocabulary.annotation_types.AnnotationTypes` classes to generate ``@type`` strings.
         #. Return the mmif object
 
         :param mmif: An input MMIF object to annotate
         :param runtime_params: An arbitrary set of k-v pairs to configure the app at runtime
         :return: A :class:`~mmif.serialize.mmif.Mmif` object of the annotated output, ready for serialization
         """
         raise NotImplementedError()
```

### Comparing `clams-python-0.6.0/clams/appmetadata/__init__.py` & `clams-python-0.6.1/clams/appmetadata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import subprocess
 import sys
+import shutil
 from pathlib import Path
 from typing import Union, Dict, List, Optional, Literal
 
 import mmif
 import pydantic
 from mmif import vocabulary
 
@@ -12,15 +13,15 @@
 app_version_envvar_key = 'CLAMS_APP_VERSION'
 # type aliases to use in app metadata and runtime parameter processing 
 primitives = Union[int, float, bool, str]
 # these names are taken from the JSON schema data types
 param_value_types = Literal['integer', 'number', 'string', 'boolean']
 
 param_value_types_values = param_value_types.__args__  # pytype: disable=attribute-error
-app_directory_baseurl = "http://apps.clams.ai"
+app_directory_baseurl = "https://apps.clams.ai"
 
 
 def get_clams_pyver():
     # real hack to avoid import clams as a package in gh-action workflow
     try:
         import clams
         return clams.__version__
@@ -30,16 +31,23 @@
             with open(version_fname) as version_f:
                 return version_f.read().strip()
         else:
             raise Exception('cannot find clams-python version')
 
 
 def generate_app_version(cwd=None):
-    proc = subprocess.run(f'git --git-dir {Path(sys.modules["__main__"].__file__).parent.resolve() if cwd is None else cwd}/.git describe --tags --always'.split(), capture_output=True)
-    if proc.returncode == 0:
+    gitcmd = shutil.which('git') 
+    gitdir = (Path(sys.modules["__main__"].__file__).parent.resolve() if cwd is None else Path(cwd)) / '.git'
+    if gitcmd is not None and gitdir.exists():
+        proc = subprocess.run(
+            f'{gitcmd} --git-dir "{gitdir}" describe --tags --always',
+            capture_output=True,
+            shell=True,
+            check=True,
+        )
         return proc.stdout.decode('utf8').strip()
     elif app_version_envvar_key in os.environ:
         return os.environ[app_version_envvar_key]
     else:
         return unresolved_app_version_num
```

### Comparing `clams-python-0.6.0/clams/develop/__init__.py` & `clams-python-0.6.1/clams/develop/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,27 +63,31 @@
         default='app',
         choices=['app'],
         help="Pick a recipe to use. Currently `app` is the only option, hence there's no need to use the flag at all."
     )
     parser.add_argument(
         '--no-github-actions',
         action='store_true', 
-        help='The cookiecutter by default assumes that the app codebase will be hosted on `github.com/clamsproejct`,'
-             'and add pre-shipped github actions for the `clamsproject` organization setup to the skeleton codebase.'
+        help='The cookiecutter by default assumes that the app codebase will be hosted on `github.com/clamsproejct`, '
+             'and add pre-shipped github actions for the `clamsproject` organization setup to the skeleton codebase. '
              'Use this options to disable this behavior.'
     )
     parser.add_argument(
         '-n', '--name',
         action='store',
         required=True,
-        help='The name of the directory where the baked app skeleton is placed. This name is also used to generate'
+        help='The name of the directory where the baked app skeleton is placed. This name is also used to generate '
              '1) Python class name of the app, 2) values for `name` and `identifier` fields in app-metadata, '
-             'based on heuristic tokenizing and casing rules. RECOMMENDATION: only use lower case ASCII alpha-numerics,'
+             'based on heuristic tokenizing and casing rules. RECOMMENDATION: only use lower case alpha-numerics, '
              'do not use whitespace, use dash (`-`) character instead for word boundaries, always check for the '
-             'generated names and make changes if they are incorrect.'
+             'generated names and make changes if they are incorrect. NOTE: if the name starts with `app-` or ends '
+             'with `-app`, those affixes will be removed from Python class name and app identifier, but will be '
+             'retained in the directory name. (e.g. `app-foo-bar-app` will be converted to `FooBar` for class name, '
+             '`foo-bar-app` for app identifier, and `app-foo-bar-app` for directory name.)'
+        
     )
     parser.add_argument(
         '-p', '--parent-dir',
         default='.',
         metavar='PATH',
         action='store',
         nargs='?',
```

### Comparing `clams-python-0.6.0/clams/restify/__init__.py` & `clams-python-0.6.1/clams/restify/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.0/clams/source/__init__.py` & `clams-python-0.6.1/clams/source/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,39 +4,37 @@
 import sys
 from os import path
 from typing import Union, Generator, List, Optional, Iterable
 
 from mmif import Mmif, Document, DocumentTypes, __specver__
 from mmif.serialize.mmif import MmifMetadata
 
-__all__ = ['PipelineSource']
+__all__ = ['WorkflowSource']
 
 DOC_JSON = Union[str, dict]
 DOC = Union[DOC_JSON, Document]
 METADATA_JSON = Union[str, dict]
 METADATA = Union[METADATA_JSON, MmifMetadata]
 
 
-class PipelineSource:
+class WorkflowSource:
     """
-    The PipelineSource class.
+    A WorkflowSource object is used at the beginning of a
+    CLAMS workflow to populate a new MMIF file with media.
 
-    A PipelineSource object is used at the beginning of a
-    CLAMS pipeline to populate a new MMIF file with media.
-
-    The same PipelineSource object can be used repeatedly
+    The same WorkflowSource object can be used repeatedly
     to generate multiple MMIF objects.
 
     :param common_documents_json:
         JSON doc_lists for any documents that should be common
-        to all MMIF objects produced by this pipeline.
+        to all MMIF objects produced by this workflow.
 
     :param common_metadata_json:
         JSON doc_lists for metadata that should be common to
-        all MMIF objects produced by this pipeline.
+        all MMIF objects produced by this workflow.
     """
     mmif: Mmif
 
     def __init__(
             self,
             common_documents_json: Optional[List[DOC_JSON]] = None,
             common_metadata_json: Optional[METADATA_JSON] = None
@@ -76,42 +74,42 @@
         :param key: the desired key of the metadata property
         :param value: the desired value of the metadata property
         """
         self.mmif.metadata[key] = value
 
     def prime(self) -> None:
         """
-        Primes the PipelineSource with a fresh MMIF object.
+        Primes the WorkflowSource with a fresh MMIF object.
 
-        Call this method if you want to reset the PipelineSource
+        Call this method if you want to reset the WorkflowSource
         without producing a MMIF object with produce().
         """
         self.mmif = Mmif(self.mmif_start)
 
     def produce(self) -> Mmif:
         """
-        Returns the source MMIF and resets the PipelineSource.
+        Returns the source MMIF and resets the WorkflowSource.
 
         Call this method once you have added all the documents
-        for your pipeline.
+        for your Workflow.
 
         :return: the current MMIF object that has been prepared
         """
         source = self.mmif
         self.prime()
         return source
 
     def __call__(
             self,
             documents: Optional[List[DOC]] = None,
             metadata: Optional[METADATA] = None
     ) -> Mmif:
         """
         Callable API that produces a new MMIF object from
-        this pipeline source given a list of documents and
+        this workflow source given a list of documents and
         a metadata object.
 
         Call with no parameters to produce the default MMIF
         object from ``self.mmif_start``.
 
         :param documents: a list of additional documents to add
         :param metadata: additional metadata fields to add
@@ -143,15 +141,15 @@
         """
         Provided with an iterable of document lists and an
         optional iterable of metadata objects, generates
         MMIF objects produced from that data.
 
         ``doc_lists`` and ``metadata_objs`` should be matched pairwise,
         so that if they are zipped together, each pair defines
-        a single MMIF object from this pipeline source.
+        a single MMIF object from this workflow source.
 
         :param doc_lists: an iterable of document lists to generate MMIF from
         :param metadata_objs: an iterable of metadata objects paired with the document lists
         :return: a generator of produced MMIF files from the data
         """
         if metadata_objs is None:
             metadata_objs = itertools.repeat(None)
@@ -159,15 +157,15 @@
             yield self(documents, metadata)
 
     def __iter__(self):
         """
         Endlessly produces MMIF directly from ``self.mmif_start``.
 
         If called after adding documents or changing metadata,
-        these changes are discarded, as the pipeline source
+        these changes are discarded, as the workflow source
         gets re-primed.
         """
         self.prime()
         while True:
             yield self.produce()
 
 
@@ -182,15 +180,15 @@
     template = Template('''{
           "@type": "${at_type}",
           "properties": {
             "id": "${aid}",
             "mime": "${mime}",
             "location": "${location}" }
         }''')
-    pl = PipelineSource()
+    pl = WorkflowSource()
     if prefix and not path.isabs(prefix):
         raise ValueError(f"prefix must be an absolute path; given \"{prefix}\".")
 
     for doc_id, arg in enumerate(documents, start=1):
         arg = arg.strip()
         if len(arg) < 1:
             continue
@@ -215,15 +213,15 @@
         )
         pl.add_document(doc)
     return pl.produce().serialize(pretty=True)
 
 
 def prep_argparser(**kwargs):
     """
-    provides CLI to create a "source" MMIF json. A source MMIF is a MMIF with a list of source documents but empty views. It can be used as a starting point for a CLAMS pipeline. 
+    provides CLI to create a "source" MMIF json. A source MMIF is a MMIF with a list of source documents but empty views. It can be used as a starting point for a CLAMS workflow. 
     """
     parser = argparse.ArgumentParser(**kwargs)
     parser.add_argument(
         'documents',
         default=None,
         action='store',
         nargs='+',
@@ -235,15 +233,15 @@
     parser.add_argument(
         '-p', '--prefix',
         default=None,
         metavar='PATH',
         nargs='?',
         help='An absolute path to use as prefix for document file paths. When prefix is set, document file paths MUST '
              'be relative. This can be useful when creating source MMIF files from a system that\'s different from '
-             'the system that actually runs the pipeline (e.g. in a docker container).'
+             'the system that actually runs the workflow (e.g. in a container).'
     )
     parser.add_argument(
         '-o', '--output',
         default=None,
         action='store',
         nargs='?',
         help='A name of a file to capture a generated MMIF json. When not given, MMIF is printed to stdout.'
```

### Comparing `clams-python-0.6.0/clams_python.egg-info/PKG-INFO` & `clams-python-0.6.1/clams_python.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 0.6.0
+Version: 0.6.1
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
-Description: # CLAMS sdk for python 
-        
-        **NOTE** that this project is in pre-alpha stage and being actively developed. Nothing is guaranteed to reliably work for the moment and developers need to be very careful when using APIs implemented here. Please use [the issue track](https://github.com/clamsproject/clams-python/issues) to report bugs and malfunctions, or send us pull requests for even more contribution. 
-        
-        ## CLAMS project
-        [CLAMS project](https://clams.ai) aims at free and open-source software platform for computational analysis and metadata generation applications for multimedia material. To achieve interoperability between various computational applications developed be different vendors, which is absolutely necessary for piping applications together supported by user-friendly workflow engines, we are also developing JSON(-LD)-based MultiMedia Interchange Format ([MMIF](https://mmif.clams.ai))
+Description: ## CLAMS project
+        [CLAMS project](https://clams.ai) aims at free and open-source software platform for computational analysis and metadata generation applications for multimedia material. We believe free and open AI-based multimedia processing platform can bring many benefits of technical advancement to libraries, archives, and museums. To achieve interoperability between various computational applications developed be different vendors, which is absolutely necessary for using applications together supported by user-friendly workflow engines, we are also developing JSON-based MultiMedia Interchange Format ([MMIF](https://mmif.clams.ai))
         
         ## clams-python
-        `clams-python` is a Python implementation of the CLAMS SDK. `clams-python` supports; 
+        `clams-python` is a Python implementation of the CLAMS SDK. `clams-python` provides CLAMS app developers with the following assistance ; 
         
         1. handling MMIF files for input and output specification for CLAMS apps
-        1. a base class to start developing a CLAMS app
-        1. a flask-based wrapper to run a Python CLAMS app as a HTTP web app
+        1. a base Python class to start developing a CLAMS app
+        1. a flask-based wrapper to run a Python CLAMS app as an HTTP web app
+        1. cookie-cutter shell command that sets up everything and starts a new CLAMS app project
+        
+        ### Start now from [Getting Started](introduction.html)!
         
         ## For more ...
-        For user manuals and Python API documentation, take a look at [the SDK website](https://clams.ai/clams-python).
+        For user manuals and Python API documentation, take a look at [Python modules](https://clams.ai/clams-python/modules.html).
         
         For MMIF-specific Python API documentation, take a look at the [mmif-python website](https://clams.ai/mmif-python).
         
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-0.6.0/setup.py` & `clams-python-0.6.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -73,14 +73,19 @@
             'project': ('setup.py', name),
             'version': ('setup.py', version),
             #  'release': ('setup.py', release),
             'build_dir': ('setup.py', 'documentation/_build'),
             'builder': ('setup.py', 'html'),
         }
     },
+    # this is for *building*, building (build, bdist_*) doesn't get along with MANIFEST.in
+    # so using this param explicitly is much safer implementation
+    package_data={
+        'clams': ['develop/templates/**/*', 'develop/templates/**/.*']
+    },
     install_requires=requires,
     python_requires='>=3.8',
     packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
             'clams = clams.__init__:cli',
         ],
```

