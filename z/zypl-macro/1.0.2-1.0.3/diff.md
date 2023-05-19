# Comparing `tmp/zypl_macro-1.0.2.tar.gz` & `tmp/zypl_macro-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zypl_macro-1.0.2.tar", last modified: Fri May 19 07:58:35 2023, max compression
+gzip compressed data, was "zypl_macro-1.0.3.tar", last modified: Fri May 19 08:42:13 2023, max compression
```

## Comparing `zypl_macro-1.0.2.tar` & `zypl_macro-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 07:58:35.894135 zypl_macro-1.0.2/
--rw-rw-rw-   0        0        0     1085 2023-05-16 15:19:29.000000 zypl_macro-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     4211 2023-05-19 07:58:35.893120 zypl_macro-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3848 2023-05-14 10:17:28.000000 zypl_macro-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 07:58:35.894135 zypl_macro-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-05-19 07:58:25.000000 zypl_macro-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 07:58:35.887135 zypl_macro-1.0.2/zypl_macro/
--rw-rw-rw-   0        0        0        2 2023-05-14 06:12:43.000000 zypl_macro-1.0.2/zypl_macro/__init__.py
--rw-rw-rw-   0        0        0     4658 2023-05-19 07:53:43.000000 zypl_macro-1.0.2/zypl_macro/library.py
-drwxrwxrwx   0        0        0        0 2023-05-19 07:58:35.891125 zypl_macro-1.0.2/zypl_macro.egg-info/
--rw-rw-rw-   0        0        0     4211 2023-05-19 07:58:35.000000 zypl_macro-1.0.2/zypl_macro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-05-19 07:58:35.000000 zypl_macro-1.0.2/zypl_macro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 07:58:35.000000 zypl_macro-1.0.2/zypl_macro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-19 07:58:35.000000 zypl_macro-1.0.2/zypl_macro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-19 07:58:35.000000 zypl_macro-1.0.2/zypl_macro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 08:42:13.607340 zypl_macro-1.0.3/
+-rw-rw-rw-   0        0        0     1085 2023-05-16 15:19:29.000000 zypl_macro-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4211 2023-05-19 08:42:13.598552 zypl_macro-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3848 2023-05-14 10:17:28.000000 zypl_macro-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 08:42:13.607340 zypl_macro-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-05-19 08:41:55.000000 zypl_macro-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:42:13.591571 zypl_macro-1.0.3/zypl_macro/
+-rw-rw-rw-   0        0        0        2 2023-05-14 06:12:43.000000 zypl_macro-1.0.3/zypl_macro/__init__.py
+-rw-rw-rw-   0        0        0     4711 2023-05-19 08:41:44.000000 zypl_macro-1.0.3/zypl_macro/library.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:42:13.597555 zypl_macro-1.0.3/zypl_macro.egg-info/
+-rw-rw-rw-   0        0        0     4211 2023-05-19 08:42:13.000000 zypl_macro-1.0.3/zypl_macro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-05-19 08:42:13.000000 zypl_macro-1.0.3/zypl_macro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 08:42:13.000000 zypl_macro-1.0.3/zypl_macro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-05-19 08:42:13.000000 zypl_macro-1.0.3/zypl_macro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-19 08:42:13.000000 zypl_macro-1.0.3/zypl_macro.egg-info/top_level.txt
```

### Comparing `zypl_macro-1.0.2/LICENSE` & `zypl_macro-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zypl_macro-1.0.2/PKG-INFO` & `zypl_macro-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zypl_macro
-Version: 1.0.2
+Version: 1.0.3
 Summary: zypl.ai alternative data API interface lib
 Author: Me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `zypl_macro-1.0.2/README.md` & `zypl_macro-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zypl_macro-1.0.2/setup.py` & `zypl_macro-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zypl_macro",
-    version="1.0.2",
+    version="1.0.3",
     author="Me",
     description="zypl.ai alternative data API interface lib",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `zypl_macro-1.0.2/zypl_macro/library.py` & `zypl_macro-1.0.3/zypl_macro/library.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 class NoAuthorization(Exception):
     def __init__(self, message="You're not authorized! Please call auth() method with a valid authorization key"):
         self.message = message
         super().__init__(self.message)
         pass
 
 class DataGetter():
-    # _URL = 'https://alt-data-api.azurewebsites.net/api/macro/get'
-    _URL = 'http://localhost:8000/api/macro/get'
+    _URL = 'https://alt-data-api.azurewebsites.net/api/macro/get'
+    # _URL = 'http://localhost:8000/api/macro/get'
     _API_KEY = ''
     
     def _set_url(self, url):
         self._URL = url
     
     def _prettify_indicators(self, ind_list):
         return [" ".join([name.capitalize() if name not in ['gdp', 'cpi'] else name.upper() for name in indicator.split("_")]) for indicator in ind_list]
@@ -77,15 +77,15 @@
             df = df.loc[mask]
             if len(df) == 0: 
                 return 'Start or end date are out of bounds.'
         df.columns = self._prettify_indicators(df.columns)
         if isinstance(indicators, list):
             cols = list(filter(lambda name: name not in indicators and name not in ['Country', 'Date'], df.columns))
             df.drop(columns=cols, inplace=True)
-            df.dropna(inplace=True, how='all')
+            df.dropna(subset=df.drop(columns=['Country', 'Date']).columns, inplace=True, how='all')
 
         # df.to_csv("%s/%s_macrodata.csv" % (os.getcwd(), kwargs['country']), header=df.columns, index=False,  sep=";")
         return df
     
     def get_countries(self) -> pd.DataFrame | str:
         try: data = self._api_call(frequency="Yearly").json()
         except NoAuthorization as e:
```

### Comparing `zypl_macro-1.0.2/zypl_macro.egg-info/PKG-INFO` & `zypl_macro-1.0.3/zypl_macro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zypl-macro
-Version: 1.0.2
+Version: 1.0.3
 Summary: zypl.ai alternative data API interface lib
 Author: Me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

