# Comparing `tmp/zypl_macro-1.0.1.tar.gz` & `tmp/zypl_macro-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zypl_macro-1.0.1.tar", last modified: Sun May 14 10:17:40 2023, max compression
+gzip compressed data, was "zypl_macro-1.0.2.tar", last modified: Fri May 19 07:58:35 2023, max compression
```

## Comparing `zypl_macro-1.0.1.tar` & `zypl_macro-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 10:17:40.801996 zypl_macro-1.0.1/
--rw-rw-rw-   0        0        0     1099 2023-05-14 06:12:43.000000 zypl_macro-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     4211 2023-05-14 10:17:40.793967 zypl_macro-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3848 2023-05-14 10:17:28.000000 zypl_macro-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-14 10:17:40.801996 zypl_macro-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-05-14 10:11:10.000000 zypl_macro-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 10:17:40.786986 zypl_macro-1.0.1/zypl_macro/
--rw-rw-rw-   0        0        0        2 2023-05-14 06:12:43.000000 zypl_macro-1.0.1/zypl_macro/__init__.py
--rw-rw-rw-   0        0        0     4302 2023-05-14 08:45:09.000000 zypl_macro-1.0.1/zypl_macro/library.py
-drwxrwxrwx   0        0        0        0 2023-05-14 10:17:40.791972 zypl_macro-1.0.1/zypl_macro.egg-info/
--rw-rw-rw-   0        0        0     4211 2023-05-14 10:17:40.000000 zypl_macro-1.0.1/zypl_macro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-05-14 10:17:40.000000 zypl_macro-1.0.1/zypl_macro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 10:17:40.000000 zypl_macro-1.0.1/zypl_macro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-14 10:17:40.000000 zypl_macro-1.0.1/zypl_macro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-14 10:17:40.000000 zypl_macro-1.0.1/zypl_macro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 07:58:35.894135 zypl_macro-1.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-05-16 15:19:29.000000 zypl_macro-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4211 2023-05-19 07:58:35.893120 zypl_macro-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3848 2023-05-14 10:17:28.000000 zypl_macro-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 07:58:35.894135 zypl_macro-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-05-19 07:58:25.000000 zypl_macro-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:58:35.887135 zypl_macro-1.0.2/zypl_macro/
+-rw-rw-rw-   0        0        0        2 2023-05-14 06:12:43.000000 zypl_macro-1.0.2/zypl_macro/__init__.py
+-rw-rw-rw-   0        0        0     4658 2023-05-19 07:53:43.000000 zypl_macro-1.0.2/zypl_macro/library.py
+drwxrwxrwx   0        0        0        0 2023-05-19 07:58:35.891125 zypl_macro-1.0.2/zypl_macro.egg-info/
+-rw-rw-rw-   0        0        0     4211 2023-05-19 07:58:35.000000 zypl_macro-1.0.2/zypl_macro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-05-19 07:58:35.000000 zypl_macro-1.0.2/zypl_macro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 07:58:35.000000 zypl_macro-1.0.2/zypl_macro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-05-19 07:58:35.000000 zypl_macro-1.0.2/zypl_macro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-19 07:58:35.000000 zypl_macro-1.0.2/zypl_macro.egg-info/top_level.txt
```

### Comparing `zypl_macro-1.0.1/LICENSE` & `zypl_macro-1.0.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Another-Purple-Rabbit
+Copyright (c) 2023 zypl.ai
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `zypl_macro-1.0.1/PKG-INFO` & `zypl_macro-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zypl_macro
-Version: 1.0.1
+Version: 1.0.2
 Summary: zypl.ai alternative data API interface lib
 Author: Me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `zypl_macro-1.0.1/README.md` & `zypl_macro-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zypl_macro-1.0.1/setup.py` & `zypl_macro-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zypl_macro",
-    version="1.0.1",
+    version="1.0.2",
     author="Me",
     description="zypl.ai alternative data API interface lib",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `zypl_macro-1.0.1/zypl_macro/library.py` & `zypl_macro-1.0.2/zypl_macro/library.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 import datetime
 import os
 
 class NoAuthorization(Exception):
     def __init__(self, message="You're not authorized! Please call auth() method with a valid authorization key"):
         self.message = message
         super().__init__(self.message)
+        pass
 
 class DataGetter():
-    _URL = 'https://alt-data-api.azurewebsites.net/api/macro/get'
+    # _URL = 'https://alt-data-api.azurewebsites.net/api/macro/get'
+    _URL = 'http://localhost:8000/api/macro/get'
     _API_KEY = ''
     
     def _set_url(self, url):
         self._URL = url
     
     def _prettify_indicators(self, ind_list):
         return [" ".join([name.capitalize() if name not in ['gdp', 'cpi'] else name.upper() for name in indicator.split("_")]) for indicator in ind_list]
@@ -34,15 +36,16 @@
         self._API_KEY = token
         response = self._api_call(frequency='Yearly', country='Tajikistan')
         if response.status_code == 403:
             print('Invalid authorization key')
             self._API_KEY = ''
 
 
-    def get_data(self, **kwargs):
+    def get_data(self, indicators=None, **kwargs) -> pd.DataFrame | str:
+      
         if 'start' in kwargs.keys():
             try: datetime.date.fromisoformat(kwargs['start']) 
             except ValueError: 
                 print("Dates should be provided in YYYY-MM-DD format!")
                 return
         if 'end' in kwargs.keys():
             try: datetime.date.fromisoformat(kwargs['end']) 
@@ -53,57 +56,57 @@
         if not 'country' in kwargs.keys():
             print('Provide the country to get data for')
             return
 
         try:
             data = self._api_call( country = kwargs['country'], frequency = kwargs.get('frequency') or '' )
         except NoAuthorization as e:
-            print(e.message)
-            return
+            return e.message
         
         data = data.json()
-        if len(data) == 0: 
-            print('Invalid country name.')
-            return
+        if len(data) == 0: return 'Invalid country name.'
         
         df = pd.DataFrame(data)
         df['date'] = pd.to_datetime(df['date'])
         if 'start' in kwargs.keys() or 'end' in kwargs.keys():
             if 'start' in kwargs.keys() and not 'end' in kwargs.keys():
                 mask = (df['date'] >= kwargs['start'])
             elif not 'start' in kwargs.keys() and 'end' in kwargs.keys():
                 mask = (df['date'] <= kwargs['end'])
             else: 
                 mask = (df['date'] >= kwargs['start']) & (df['date'] <= kwargs['end'])
             df = df.loc[mask]
             if len(df) == 0: 
-                print('Start or end date are out of bounds.')
-                return
+                return 'Start or end date are out of bounds.'
         df.columns = self._prettify_indicators(df.columns)
-        df.to_csv("%s/%s_macrodata.csv" % (os.getcwd(), kwargs['country']), header=df.columns, index=False)
-        return
+        if isinstance(indicators, list):
+            cols = list(filter(lambda name: name not in indicators and name not in ['Country', 'Date'], df.columns))
+            df.drop(columns=cols, inplace=True)
+            df.dropna(inplace=True, how='all')
+
+        # df.to_csv("%s/%s_macrodata.csv" % (os.getcwd(), kwargs['country']), header=df.columns, index=False,  sep=";")
+        return df
     
-    def get_countries(self):
+    def get_countries(self) -> pd.DataFrame | str:
         try: data = self._api_call(frequency="Yearly").json()
         except NoAuthorization as e: 
-            print(e.message) 
-            return
+            return e.message
         
         entirety = pd.DataFrame(data)
         countries = pd.DataFrame({'Country name': entirety['country'].unique()})
-        countries.to_csv('%s/supported_countries.csv' % os.getcwd(), index=False)
-        return
+        # countries.to_csv('%s/supported_countries.csv' % os.getcwd(), index=False,  sep=";")
+        
+        return countries
 
-    def get_indicators(self, **kwargs):
+    def get_indicators(self, **kwargs) -> pd.DataFrame | str:
         try: data = self._api_call(country=kwargs.get('country') or '').json()
         except NoAuthorization as e: 
-            print(e.message)
-            return
+            return e.message
         
         if len(data) == 0: 
-            print('Invalid country name.')
-            return
+            return 'Invalid country name.'
 
         entirety = pd.DataFrame(data)
         indicators = pd.DataFrame({'Indicator name': self._prettify_indicators([name for name in entirety.columns if name not in ['date', 'country']])})
-        indicators.to_csv('%s/indicators.csv' % os.getcwd(), index=False)
-        return
+        # indicators.to_csv('%s/indicators.csv' % os.getcwd(), index=False, sep=";")
+        
+        return indicators
```

### Comparing `zypl_macro-1.0.1/zypl_macro.egg-info/PKG-INFO` & `zypl_macro-1.0.2/zypl_macro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zypl-macro
-Version: 1.0.1
+Version: 1.0.2
 Summary: zypl.ai alternative data API interface lib
 Author: Me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

