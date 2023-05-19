# Comparing `tmp/modbus-wrapper-1.0.2a0.tar.gz` & `tmp/modbus-wrapper-1.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modbus-wrapper-1.0.2a0.tar", last modified: Tue Apr  4 08:16:30 2023, max compression
+gzip compressed data, was "modbus-wrapper-1.0.2b0.tar", last modified: Wed Apr  5 07:24:50 2023, max compression
```

## Comparing `modbus-wrapper-1.0.2a0.tar` & `modbus-wrapper-1.0.2b0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-04 08:16:30.164612 modbus-wrapper-1.0.2a0/
--rw-r--r--   0 bubba     (1000) bubba     (1000)      277 2023-04-04 08:16:30.164612 modbus-wrapper-1.0.2a0/PKG-INFO
--rw-r--r--   0 bubba     (1000) bubba     (1000)     1977 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2a0/README.md
-drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-04 08:16:30.148613 modbus-wrapper-1.0.2a0/modbus_wrapper/
--rw-r--r--   0 bubba     (1000) bubba     (1000)       71 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2a0/modbus_wrapper/__init__.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)     6133 2023-04-03 16:11:59.000000 modbus-wrapper-1.0.2a0/modbus_wrapper/client.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)     6573 2023-04-03 16:11:59.000000 modbus-wrapper-1.0.2a0/modbus_wrapper/function_argument.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)      233 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2a0/modbus_wrapper/modbus_function_code.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)     1700 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2a0/modbus_wrapper/object_factory.py
-drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-04 08:16:30.160612 modbus-wrapper-1.0.2a0/modbus_wrapper/objects/
--rw-r--r--   0 bubba     (1000) bubba     (1000)       77 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2a0/modbus_wrapper/objects/__init__.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)      366 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2a0/modbus_wrapper/objects/config.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)     3273 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2a0/modbus_wrapper/objects/fatek_object.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)     3086 2023-04-03 16:11:59.000000 modbus-wrapper-1.0.2a0/modbus_wrapper/objects/modbus_object.py
--rw-r--r--   0 bubba     (1000) bubba     (1000)     2569 2023-04-04 08:12:14.000000 modbus-wrapper-1.0.2a0/modbus_wrapper/objects/modbus_value.py
-drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-04 08:16:30.152613 modbus-wrapper-1.0.2a0/modbus_wrapper.egg-info/
--rw-r--r--   0 bubba     (1000) bubba     (1000)      277 2023-04-04 08:16:30.000000 modbus-wrapper-1.0.2a0/modbus_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 bubba     (1000) bubba     (1000)      589 2023-04-04 08:16:30.000000 modbus-wrapper-1.0.2a0/modbus_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 bubba     (1000) bubba     (1000)        1 2023-04-04 08:16:30.000000 modbus-wrapper-1.0.2a0/modbus_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 bubba     (1000) bubba     (1000)       12 2023-04-04 08:16:30.000000 modbus-wrapper-1.0.2a0/modbus_wrapper.egg-info/requires.txt
--rw-r--r--   0 bubba     (1000) bubba     (1000)       15 2023-04-04 08:16:30.000000 modbus-wrapper-1.0.2a0/modbus_wrapper.egg-info/top_level.txt
--rw-r--r--   0 bubba     (1000) bubba     (1000)       38 2023-04-04 08:16:30.164612 modbus-wrapper-1.0.2a0/setup.cfg
--rw-r--r--   0 bubba     (1000) bubba     (1000)      393 2023-04-04 08:13:56.000000 modbus-wrapper-1.0.2a0/setup.py
-drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-04 08:16:30.160612 modbus-wrapper-1.0.2a0/tests/
--rw-r--r--   0 bubba     (1000) bubba     (1000)     1992 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2a0/tests/test_modbus_client_wrapper.py
+drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-05 07:24:50.174574 modbus-wrapper-1.0.2b0/
+-rw-r--r--   0 bubba     (1000) bubba     (1000)      277 2023-04-05 07:24:50.174574 modbus-wrapper-1.0.2b0/PKG-INFO
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     1977 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/README.md
+drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-05 07:24:50.158574 modbus-wrapper-1.0.2b0/modbus_wrapper/
+-rw-r--r--   0 bubba     (1000) bubba     (1000)       71 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/__init__.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     6132 2023-04-05 07:20:35.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/client.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     6564 2023-04-05 07:20:11.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/function_argument.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)      233 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/modbus_function_code.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     1700 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/object_factory.py
+drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-05 07:24:50.170574 modbus-wrapper-1.0.2b0/modbus_wrapper/objects/
+-rw-r--r--   0 bubba     (1000) bubba     (1000)       77 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/objects/__init__.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)      366 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/objects/config.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     3273 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/objects/fatek_object.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     3085 2023-04-05 07:18:55.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/objects/modbus_object.py
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     2569 2023-04-04 08:12:14.000000 modbus-wrapper-1.0.2b0/modbus_wrapper/objects/modbus_value.py
+drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-05 07:24:50.166574 modbus-wrapper-1.0.2b0/modbus_wrapper.egg-info/
+-rw-r--r--   0 bubba     (1000) bubba     (1000)      277 2023-04-05 07:24:50.000000 modbus-wrapper-1.0.2b0/modbus_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 bubba     (1000) bubba     (1000)      589 2023-04-05 07:24:50.000000 modbus-wrapper-1.0.2b0/modbus_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 bubba     (1000) bubba     (1000)        1 2023-04-05 07:24:50.000000 modbus-wrapper-1.0.2b0/modbus_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 bubba     (1000) bubba     (1000)       12 2023-04-05 07:24:50.000000 modbus-wrapper-1.0.2b0/modbus_wrapper.egg-info/requires.txt
+-rw-r--r--   0 bubba     (1000) bubba     (1000)       15 2023-04-05 07:24:50.000000 modbus-wrapper-1.0.2b0/modbus_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 bubba     (1000) bubba     (1000)       38 2023-04-05 07:24:50.174574 modbus-wrapper-1.0.2b0/setup.cfg
+-rw-r--r--   0 bubba     (1000) bubba     (1000)      393 2023-04-05 07:23:46.000000 modbus-wrapper-1.0.2b0/setup.py
+drwxr-xr-x   0 bubba     (1000) bubba     (1000)        0 2023-04-05 07:24:50.174574 modbus-wrapper-1.0.2b0/tests/
+-rw-r--r--   0 bubba     (1000) bubba     (1000)     1992 2023-03-30 08:41:48.000000 modbus-wrapper-1.0.2b0/tests/test_modbus_client_wrapper.py
```

### Comparing `modbus-wrapper-1.0.2a0/README.md` & `modbus-wrapper-1.0.2b0/README.md`

 * *Files identical despite different names*

### Comparing `modbus-wrapper-1.0.2a0/modbus_wrapper/client.py` & `modbus-wrapper-1.0.2b0/modbus_wrapper/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             if range_entry:
                 modbus_objects = modbus_objects + get_modbus_object_from_range(n)
             else:
                 modbus_objects.append(get_modbus_object(n))
 
         self.read_modbus_objects(modbus_objects, *args, **kwargs)
 
-        result = {obj.__repr__():obj.value.__repr__() for obj in modbus_objects}
+        result = {obj.__repr__():obj.current.__repr__() for obj in modbus_objects}
 
         return result
     
     def read_modbus_objects(
             self, 
             modbus_objects: List[ModbusObject],  
             max_read_size: int = None, 
@@ -72,15 +72,15 @@
         self.close()
 
     def write(self, modbus_numbers_with_values: dict) -> dict:
         modbus_objects = [get_modbus_object(n,v) for n,v in modbus_numbers_with_values.items()]
 
         self.write_modbus_objects(modbus_objects)
 
-        result = {obj.__repr__():obj.value.__repr__() for obj in modbus_objects}
+        result = {obj.__repr__():obj.current.__repr__() for obj in modbus_objects}
 
         return result
 
     def write_modbus_objects(self, modbus_objects: List[ModbusObject]):
         arguments = WriteFunctionArgument.get_arguments(
                                         modbus_objects,
                                         )
@@ -98,15 +98,15 @@
         values_to_write = write_argument.values_to_write
         function_string = write_function.__doc__.splitlines()[0]
         LOG.debug (f'executing function: "{function_string}" for argument: "{write_argument}"')
 
         write_ok = write_function(starting_address, values_to_write)
         objects = write_argument.object_list.objects
         if write_ok:
-            [obj.value.update(obj.value_to_write.value) for obj in objects]
+            [obj.current.update(obj.write.value) for obj in objects]
         else:
             LOG.error(f'failed to write "{function_string}" for argument: "{write_argument}"')
 
         return write_ok
         
     def _get_function(self, code:[hex, int]):
         """Get modbus function by code"""
@@ -157,14 +157,14 @@
 
         increment = 0
         for value in collected_values[starting_address]:
             collected_values[starting_address+increment] = value
             increment+=1
 
         for object in argument.object_list.objects:
-            object.value.update(
+            object.current.update(
                 collected_values[object.address]
                 )
```

### Comparing `modbus-wrapper-1.0.2a0/modbus_wrapper/function_argument.py` & `modbus-wrapper-1.0.2b0/modbus_wrapper/function_argument.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                 )
 
             for write in calculated_write_sizes:
                 number_of_values_to_write = write['size']
                 starting_address = write['starting_address'] 
                 ending_address = starting_address + number_of_values_to_write
                 get_write_value_for_address = lambda address: next(
-                        obj.value_to_write.value
+                        obj.write.value
                         for obj in single_type.objects 
                         if obj.address == address
                         )
                 get_objets_for_address = lambda address: next(obj for obj in single_type.objects if obj.address == address)
                 addresses_range = range(starting_address, ending_address)
 
                 values_to_write = list(
```

### Comparing `modbus-wrapper-1.0.2a0/modbus_wrapper/object_factory.py` & `modbus-wrapper-1.0.2b0/modbus_wrapper/object_factory.py`

 * *Files identical despite different names*

### Comparing `modbus-wrapper-1.0.2a0/modbus_wrapper/objects/fatek_object.py` & `modbus-wrapper-1.0.2b0/modbus_wrapper/objects/fatek_object.py`

 * *Files identical despite different names*

### Comparing `modbus-wrapper-1.0.2a0/modbus_wrapper/objects/modbus_object.py` & `modbus-wrapper-1.0.2b0/modbus_wrapper/objects/modbus_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
     def __init__(
             self, modbus_number: int,
             value_to_write: int | bool = None,
             target_range: TargetRangeInt | TargetRangeBool = None
         ):
         self.number = modbus_number
-        self.value_to_write = self.VALUE_CLS(value_to_write)
-        self.value = self.VALUE_CLS()
+        self.current = self.VALUE_CLS()   
+        self.write = self.VALUE_CLS(value_to_write)   
         self.target_range = target_range
 
     def __repr__(self):
         return str(self.number)
 
     @property
     def address(self):
```

### Comparing `modbus-wrapper-1.0.2a0/modbus_wrapper/objects/modbus_value.py` & `modbus-wrapper-1.0.2b0/modbus_wrapper/objects/modbus_value.py`

 * *Files identical despite different names*

### Comparing `modbus-wrapper-1.0.2a0/modbus_wrapper.egg-info/SOURCES.txt` & `modbus-wrapper-1.0.2b0/modbus_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modbus-wrapper-1.0.2a0/tests/test_modbus_client_wrapper.py` & `modbus-wrapper-1.0.2b0/tests/test_modbus_client_wrapper.py`

 * *Files identical despite different names*

