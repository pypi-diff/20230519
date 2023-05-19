# Comparing `tmp/easy_gtfs-0.1.0.2.tar.gz` & `tmp/easy_gtfs-0.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_gtfs-0.1.0.2.tar", max compression
+gzip compressed data, was "easy_gtfs-0.1.0.3.tar", max compression
```

## Comparing `easy_gtfs-0.1.0.2.tar` & `easy_gtfs-0.1.0.3.tar`

### file list

```diff
@@ -1,13 +1,27 @@
--rw-r--r--   0        0        0       23 2023-05-15 16:28:56.423189 easy_gtfs-0.1.0.2/easy_gtfs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 16:24:21.223177 easy_gtfs-0.1.0.2/easy_gtfs/managers/__init__.py
--rw-r--r--   0        0        0     7000 2023-05-15 16:21:53.793005 easy_gtfs-0.1.0.2/easy_gtfs/managers/agencymanager.py
--rw-r--r--   0        0        0      730 2023-05-15 16:16:25.863078 easy_gtfs-0.1.0.2/easy_gtfs/managers/errormanager.py
--rw-r--r--   0        0        0        0 2023-05-15 16:24:14.442747 easy_gtfs-0.1.0.2/easy_gtfs/models/__init__.py
--rw-r--r--   0        0        0      369 2023-05-15 16:20:49.948447 easy_gtfs-0.1.0.2/easy_gtfs/models/errors.py
--rw-r--r--   0        0        0        0 2023-05-15 14:09:30.614598 easy_gtfs-0.1.0.2/easy_gtfs/objects/__init__.py
--rw-r--r--   0        0        0     2614 2023-05-15 16:12:40.836501 easy_gtfs-0.1.0.2/easy_gtfs/objects/agency.py
--rw-r--r--   0        0        0     1269 2023-05-15 16:12:05.818115 easy_gtfs-0.1.0.2/easy_gtfs/utility.py
--rw-r--r--   0        0        0     1389 2023-05-15 15:26:25.897851 easy_gtfs-0.1.0.2/easy_gtfs/variables.py
--rw-r--r--   0        0        0      343 2023-05-15 16:28:33.751198 easy_gtfs-0.1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 14:06:25.799294 easy_gtfs-0.1.0.2/README.md
--rw-r--r--   0        0        0      411 1970-01-01 00:00:00.000000 easy_gtfs-0.1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-05-15 16:28:56.423189 easy_gtfs-0.1.0.3/easy_gtfs/__init__.py
+-rw-r--r--   0        0        0      113 2023-05-19 15:27:42.521125 easy_gtfs-0.1.0.3/easy_gtfs/agency.txt
+-rw-r--r--   0        0        0        0 2023-05-15 16:24:21.223177 easy_gtfs-0.1.0.3/easy_gtfs/managers/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-17 19:43:33.659534 easy_gtfs-0.1.0.3/easy_gtfs/managers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5502 2023-05-19 20:03:36.971506 easy_gtfs-0.1.0.3/easy_gtfs/managers/__pycache__/agencymanager.cpython-39.pyc
+-rw-r--r--   0        0        0     1477 2023-05-19 20:03:36.961011 easy_gtfs-0.1.0.3/easy_gtfs/managers/__pycache__/errormanager.cpython-39.pyc
+-rw-r--r--   0        0        0     2875 2023-05-19 20:03:36.951409 easy_gtfs-0.1.0.3/easy_gtfs/managers/__pycache__/gtfsmanager.cpython-39.pyc
+-rw-r--r--   0        0        0     7039 2023-05-19 20:30:44.809385 easy_gtfs-0.1.0.3/easy_gtfs/managers/agencymanager.py
+-rw-r--r--   0        0        0      828 2023-05-19 19:59:56.002870 easy_gtfs-0.1.0.3/easy_gtfs/managers/errormanager.py
+-rw-r--r--   0        0        0     5819 2023-05-19 20:57:22.548209 easy_gtfs-0.1.0.3/easy_gtfs/managers/gtfsmanager.py
+-rw-r--r--   0        0        0     6683 2023-05-19 20:38:50.085033 easy_gtfs-0.1.0.3/easy_gtfs/managers/stopmanager.py
+-rw-r--r--   0        0        0        0 2023-05-15 16:24:14.442747 easy_gtfs-0.1.0.3/easy_gtfs/models/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-19 15:28:11.632756 easy_gtfs-0.1.0.3/easy_gtfs/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1267 2023-05-19 20:03:36.979111 easy_gtfs-0.1.0.3/easy_gtfs/models/__pycache__/errors.cpython-39.pyc
+-rw-r--r--   0        0        0      995 2023-05-19 20:52:02.586564 easy_gtfs-0.1.0.3/easy_gtfs/models/errors.py
+-rw-r--r--   0        0        0     6955 2023-05-19 20:08:49.060106 easy_gtfs-0.1.0.3/easy_gtfs/models/models.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:09:30.614598 easy_gtfs-0.1.0.3/easy_gtfs/objects/__init__.py
+-rw-r--r--   0        0        0      191 2023-05-15 16:32:34.727557 easy_gtfs-0.1.0.3/easy_gtfs/objects/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2398 2023-05-15 16:32:34.737067 easy_gtfs-0.1.0.3/easy_gtfs/objects/__pycache__/agency.cpython-39.pyc
+-rw-r--r--   0        0        0     2762 2023-05-15 16:31:14.415464 easy_gtfs-0.1.0.3/easy_gtfs/objects/agency.py
+-rw-r--r--   0        0        0     6437 2023-05-19 20:26:24.793506 easy_gtfs-0.1.0.3/easy_gtfs/objects/stop.py
+-rw-r--r--   0        0        0     3217 2023-05-17 19:26:25.836427 easy_gtfs-0.1.0.3/easy_gtfs/sample-feed.zip
+-rw-r--r--   0        0        0     1277 2023-05-17 19:43:57.791496 easy_gtfs-0.1.0.3/easy_gtfs/utility.py
+-rw-r--r--   0        0        0     1423 2023-05-19 17:52:23.436347 easy_gtfs-0.1.0.3/easy_gtfs/variables.py
+-rw-r--r--   0        0        0      343 2023-05-15 16:29:16.528178 easy_gtfs-0.1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 14:06:25.799294 easy_gtfs-0.1.0.3/README.md
+-rw-r--r--   0        0        0      411 1970-01-01 00:00:00.000000 easy_gtfs-0.1.0.3/PKG-INFO
```

### Comparing `easy_gtfs-0.1.0.2/easy_gtfs/managers/agencymanager.py` & `easy_gtfs-0.1.0.3/easy_gtfs/managers/agencymanager.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,34 +18,34 @@
 
 
 
 
 class Agencies():
     """A class to manage multiple 'Agency' models and write them to a file, load them from a file or parse them from a json object."""
 
-    def __init__(self, error_manager = get_error_manager(), agencies: List[Agency] = None, file: str = None):
+    def __init__(self, agencies: List[Agency] = None, file: str = None):
         """
             A class to manage multiple 'Agency' models and write them to a file, load them from a file or parse them from a json object.
 
             :param agencies [List[Agency]] -- A list of 'Agency' models, can be passed later with the respective function on function call
             :param file [str] -- The file to write to or load from, can be passed later with the respective function on function call
         """
-        self.error_manager = error_manager
+        self.error_manager = get_error_manager()
         self.agencies: List[Agency] = agencies
         self.file: str = file
     
 
     def to_file(self, agencies: Optional[List[Agency]] = None, file: Optional[str] = None) -> bool:
         """
             Writes a list of 'Agency' models to a file in csv format.
 
             :param agencies [Optional[List[Agency]]] -- A list containing 'Agency' models, if not given it will take 'self.agencies' if set
             :param file [Optional[str]] -- The file to write to, if not given it will take 'self.file' if set
 
-            :return None
+            :return bool -- True on success, else False or raises Error if not silent error enabled
         """
 
         if not agencies:
             if self.agencies == None:
                 raise TypeError("Got no agencies to write to file!")
             agencies = self.agencies
 
@@ -63,16 +63,16 @@
             obj_as_dict = obj.dict(exclude_unset=False)
             agencies_ids.append(obj_as_dict["agency_id"]) # add the id of the agency to our ids list for verification later on
             rows.append(obj_as_dict) # add the agency as json to our rows that will be written to the csv file
 
         if len(agencies_ids) > 1:
             duplicates = [k for k, v in Counter(agencies_ids).items() if v>1] # returns a list with all duplicate ids; if the id '123' was for example at least 2 times in the ids list the output would be: ['123']
             if len(duplicates) > 0:
-                if self.error_manager.is_silent_error():
-                    self.error_manager.new_error(AgencyError(
+                if self.error_manager.is_silent_errors():
+                    self.error_manager.add_error(AgencyError(
                         caller = "AgencyManager",
                         error_type=ErrorTypes.AgencyErrorDuplicateID,
                         message="Multiple agencies cannot have the same id!",
                         values = duplicates
                     ))
                     return False
                 else:
@@ -95,16 +95,16 @@
         """
         agencies = []
 
         for agency in agencies_list:
             if self.is_valid_agency(agency):
                 agencies.append(Agency.parse_obj(agency))
             else:
-                if self.error_manager.is_silent_error():
-                    self.error_manager.new_error(AgencyError(
+                if self.error_manager.is_silent_errors():
+                    self.error_manager.add_error(AgencyError(
                         caller = "AgencyManager",
                         error_type = ErrorTypes.AgencyErrorInvalidAgency,
                         message="Invalid agency from dict!",
                         values = [agency]
                     ))
                     return False
                 else:
@@ -127,23 +127,23 @@
             if self.file == None:
                 raise TypeError("Got no file to load from!")
             file = self.file
         
 
         with open(file, "r") as _file:
             csvreader = list(csv.DictReader(_file)) # gives a list of dictionaries where each dict is a json representation of an agency
-        
+
         agencies = self.parse(csvreader)
 
         agencies_ids = []
 
         for agency in agencies:
             if agency.agency_id in agencies_ids:
-                if self.error_manager.is_silent_error():
-                    self.error_manager.new_error(AgencyError(
+                if self.error_manager.is_silent_errors():
+                    self.error_manager.add_error(AgencyError(
                         caller = "AgencyManager",
                         error_type = ErrorTypes.AgencyErrorDuplicateID,
                         message="Cannot have multiple agencies with the same id!",
                         values = [agency.agency_id]
                     ))
                     return False
                 else:
```

### Comparing `easy_gtfs-0.1.0.2/easy_gtfs/managers/errormanager.py` & `easy_gtfs-0.1.0.3/easy_gtfs/managers/errormanager.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,24 +8,29 @@
     def set_silent_errors(self, silent_errors: bool) -> bool:
         if isinstance(silent_errors, bool):
             self.silent_errors = silent_errors
             return True
         
         return False
     
-
+    
     def get_silent_errors(self) -> bool:
         return self.silent_errors
     
+    
+    def is_silent_errors(self) -> bool:
+        return self.silent_errors
+    
 
     def errors(self) -> list:
         return self._errors
 
 
     def clear(self) -> bool:
         self._errors = []
         return True
 
     
     def add_error(self, error) -> bool:
         self._errors.append(error)
-        return True
+        return True
+
```

### Comparing `easy_gtfs-0.1.0.2/easy_gtfs/objects/agency.py` & `easy_gtfs-0.1.0.3/easy_gtfs/objects/agency.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class Agency(BaseModel):
     """
         https://developers.google.com/transit/gtfs/reference#agencytxt
 
         :param id [Optional[str]] -- The unique id for this agency (only needed if multiple agencies are present in the dataset)
         :param name [str] -- The full name of the agency
-        :param url [str] -- The url of the agency
+        :param url [str] -- The url of the agency (f.ex.: 'https://example.com' )
         :param timezone [str] -- The timezone of the agency (if multiple agencies in this dataset, all must have the same timezone)
         :param lang [Optional[str]] -- The primary language this agency uses
         :param phone [Optional[str]] -- A phone number for the agency
         :param fare_url [Optional[]] -- The website on which travellers can buy tickets to travel with this agency
         :param email [Optional[str]] -- An email address to reach the agency (should be the support email address of the agency or another email which is actively used by the agency)
     """
     agency_id: Optional[str] = ""
@@ -34,17 +34,17 @@
             try:
                 result = urlparse(url)
                 if all([result.scheme, result.netloc]):
                     return url
 
             except ValueError:
                 # ValueError can happen if an invalid ip (v4, v6) or a byte object has been passed
-                return ValueError("must be a valid url")
+                return ValueError("must be a valid url (f.ex.: https://example.com)")
         
-        raise ValueError("must be a valid url")
+        raise ValueError("must be a valid url (f.ex.: https://example.com)")
     
 
     @validator("agency_fare_url")
     def is_agency_fare_url_valid(cls, url):
         if isinstance(url, str):
             if len(url) < 1: # url is empty and we can accept that (mainly for when parsing from file)
                 return url
@@ -53,12 +53,12 @@
             try:
                 result = urlparse(url)
                 if all([result.scheme, result.netloc]):
                     return url
 
             except ValueError:
                 # ValueError can happen if an invalid ip (v4, v6) or a byte object has been passed
-                return ValueError("must be a valid url")
+                return ValueError("must be a valid url (f.ex.: https://example.com)")
         
-        raise ValueError("must be a valid url")
+        raise ValueError("must be a valid url (f.ex.: https://example.com)")
```

### Comparing `easy_gtfs-0.1.0.2/easy_gtfs/utility.py` & `easy_gtfs-0.1.0.3/easy_gtfs/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Some utility functions used all around the files
 """
 
-import variables
-from managers.errormanager import ErrorManager
+from . import variables
+from .managers.errormanager import ErrorManager
 
 
 
 def get_error_manager() -> ErrorManager:
     """
         Returns the current error manager, if none is set it will create one.
```

### Comparing `easy_gtfs-0.1.0.2/easy_gtfs/variables.py` & `easy_gtfs-0.1.0.3/easy_gtfs/variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,8 +58,11 @@
     },
     "translations.txt": {
         "required": "optional"
     },
     "attributions.txt": {
         "required": "optional"
     }
-}
+}
+
+
+OUTPUT_FOLDER: str = "/data"
```

