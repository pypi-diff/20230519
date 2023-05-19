# Comparing `tmp/gardener-component-model-0.0.92.tar.gz` & `tmp/gardener-component-model-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-component-model-0.0.92.tar", last modified: Thu May  4 08:46:35 2023, max compression
+gzip compressed data, was "gardener-component-model-0.0.93.tar", last modified: Fri May 19 05:47:01 2023, max compression
```

## Comparing `gardener-component-model-0.0.92.tar` & `gardener-component-model-0.0.93.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 08:46:35.713161 gardener-component-model-0.0.92/
--rw-r--r--   0 root         (0) root         (0)      126 2023-05-04 08:46:35.713161 gardener-component-model-0.0.92/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 08:46:35.713161 gardener-component-model-0.0.92/gardener_component_model.egg-info/
--rw-r--r--   0 root         (0) root         (0)      126 2023-05-04 08:46:35.000000 gardener-component-model-0.0.92/gardener_component_model.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      338 2023-05-04 08:46:35.000000 gardener-component-model-0.0.92/gardener_component_model.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 08:46:35.000000 gardener-component-model-0.0.92/gardener_component_model.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-05-04 08:46:35.000000 gardener-component-model-0.0.92/gardener_component_model.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-04 08:46:35.000000 gardener-component-model-0.0.92/gardener_component_model.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 08:46:35.713161 gardener-component-model-0.0.92/gci/
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-04 08:45:08.000000 gardener-component-model-0.0.92/gci/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10026 2023-05-04 08:45:09.000000 gardener-component-model-0.0.92/gci/component-descriptor.json-schema.yaml
--rw-r--r--   0 root         (0) root         (0)    17845 2023-05-04 08:45:08.000000 gardener-component-model-0.0.92/gci/componentmodel.py
--rw-r--r--   0 root         (0) root         (0)     3021 2023-05-04 08:45:08.000000 gardener-component-model-0.0.92/gci/oci.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 08:46:35.713161 gardener-component-model-0.0.92/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      942 2023-05-04 08:45:08.000000 gardener-component-model-0.0.92/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 05:47:01.346053 gardener-component-model-0.0.93/
+-rw-r--r--   0 root         (0) root         (0)      126 2023-05-19 05:47:01.346053 gardener-component-model-0.0.93/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 05:47:01.346053 gardener-component-model-0.0.93/gardener_component_model.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      126 2023-05-19 05:47:01.000000 gardener-component-model-0.0.93/gardener_component_model.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      338 2023-05-19 05:47:01.000000 gardener-component-model-0.0.93/gardener_component_model.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 05:47:01.000000 gardener-component-model-0.0.93/gardener_component_model.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-19 05:47:01.000000 gardener-component-model-0.0.93/gardener_component_model.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-19 05:47:01.000000 gardener-component-model-0.0.93/gardener_component_model.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 05:47:01.346053 gardener-component-model-0.0.93/gci/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-19 05:44:42.000000 gardener-component-model-0.0.93/gci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2023-05-19 05:44:43.000000 gardener-component-model-0.0.93/gci/component-descriptor.json-schema.yaml
+-rw-r--r--   0 root         (0) root         (0)    17784 2023-05-19 05:44:42.000000 gardener-component-model-0.0.93/gci/componentmodel.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2023-05-19 05:44:42.000000 gardener-component-model-0.0.93/gci/oci.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 05:47:01.346053 gardener-component-model-0.0.93/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      942 2023-05-19 05:44:42.000000 gardener-component-model-0.0.93/setup.py
```

### Comparing `gardener-component-model-0.0.92/gci/component-descriptor.json-schema.yaml` & `gardener-component-model-0.0.93/gci/component-descriptor.json-schema.yaml`

 * *Files identical despite different names*

### Comparing `gardener-component-model-0.0.92/gci/componentmodel.py` & `gardener-component-model-0.0.93/gci/componentmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -486,16 +486,14 @@
 
     sources: typing.List[ComponentSource]
     componentReferences: typing.List[ComponentReference]
     resources: typing.List[Resource]
 
     labels: typing.List[Label] = dataclasses.field(default_factory=list)
 
-    creationTime: typing.Optional[datetime.datetime] = None
-
     def current_repository_ctx(self):
         if not self.repositoryContexts:
             return None
         return self.repositoryContexts[-1]
 
     def identity(self):
         return ComponentIdentity(name=self.name, version=self.version)
```

### Comparing `gardener-component-model-0.0.92/gci/oci.py` & `gardener-component-model-0.0.93/gci/oci.py`

 * *Files identical despite different names*

### Comparing `gardener-component-model-0.0.92/setup.py` & `gardener-component-model-0.0.93/setup.py`

 * *Files identical despite different names*

