# Comparing `tmp/redataprocessing-0.0.8.tar.gz` & `tmp/redataprocessing-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redataprocessing-0.0.8.tar", last modified: Mon Feb  6 21:47:03 2023, max compression
+gzip compressed data, was "redataprocessing-0.0.9.tar", last modified: Tue Feb  7 19:37:22 2023, max compression
```

## Comparing `redataprocessing-0.0.8.tar` & `redataprocessing-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 vojtechkania   (501) staff       (20)        0 2023-02-06 21:47:03.951357 redataprocessing-0.0.8/
--rw-r--r--   0 vojtechkania   (501) staff       (20)     6148 2023-02-06 17:52:59.000000 redataprocessing-0.0.8/.DS_Store
--rw-r--r--   0 vojtechkania   (501) staff       (20)     1073 2023-02-03 19:25:24.000000 redataprocessing-0.0.8/LICENSE
--rw-r--r--   0 vojtechkania   (501) staff       (20)      715 2023-02-06 21:47:03.951574 redataprocessing-0.0.8/PKG-INFO
--rw-r--r--   0 vojtechkania   (501) staff       (20)       72 2023-02-03 19:24:26.000000 redataprocessing-0.0.8/README.md
--rw-r--r--   0 vojtechkania   (501) staff       (20)      748 2023-02-06 21:46:44.000000 redataprocessing-0.0.8/pyproject.toml
-drwxr-xr-x   0 vojtechkania   (501) staff       (20)        0 2023-02-06 21:47:03.944595 redataprocessing-0.0.8/redataprocessing/
--rw-r--r--   0 vojtechkania   (501) staff       (20)        0 2023-02-02 20:18:34.000000 redataprocessing-0.0.8/redataprocessing/__init__.py
-drwxr-xr-x   0 vojtechkania   (501) staff       (20)        0 2023-02-06 21:47:03.950855 redataprocessing-0.0.8/redataprocessing/__pycache__/
--rw-r--r--   0 vojtechkania   (501) staff       (20)      193 2023-02-03 20:33:48.000000 redataprocessing-0.0.8/redataprocessing/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 vojtechkania   (501) staff       (20)     5937 2023-02-06 18:29:26.000000 redataprocessing-0.0.8/redataprocessing/__pycache__/sreality_api_dictionaries.cpython-311.pyc
--rw-r--r--   0 vojtechkania   (501) staff       (20)    11775 2023-02-06 19:50:54.000000 redataprocessing-0.0.8/redataprocessing/__pycache__/sreality_description_download_decoding.cpython-311.pyc
--rw-r--r--   0 vojtechkania   (501) staff       (20)    15253 2023-02-06 21:43:54.000000 redataprocessing-0.0.8/redataprocessing/sreality.py
--rw-r--r--   0 vojtechkania   (501) staff       (20)     6459 2023-02-06 21:46:27.000000 redataprocessing-0.0.8/redataprocessing/sreality_api_dictionaries.py
--rw-r--r--   0 vojtechkania   (501) staff       (20)     3169 2023-02-06 21:44:12.000000 redataprocessing-0.0.8/redataprocessing/sreality_description_asyncio.py
--rw-r--r--   0 vojtechkania   (501) staff       (20)    10040 2023-02-06 21:44:37.000000 redataprocessing-0.0.8/redataprocessing/sreality_description_download_decoding.py
-drwxr-xr-x   0 vojtechkania   (501) staff       (20)        0 2023-02-06 21:47:03.948815 redataprocessing-0.0.8/redataprocessing.egg-info/
--rw-r--r--   0 vojtechkania   (501) staff       (20)      715 2023-02-06 21:47:03.000000 redataprocessing-0.0.8/redataprocessing.egg-info/PKG-INFO
--rw-r--r--   0 vojtechkania   (501) staff       (20)      659 2023-02-06 21:47:03.000000 redataprocessing-0.0.8/redataprocessing.egg-info/SOURCES.txt
--rw-r--r--   0 vojtechkania   (501) staff       (20)        1 2023-02-06 21:47:03.000000 redataprocessing-0.0.8/redataprocessing.egg-info/dependency_links.txt
--rw-r--r--   0 vojtechkania   (501) staff       (20)       17 2023-02-06 21:47:03.000000 redataprocessing-0.0.8/redataprocessing.egg-info/top_level.txt
--rw-r--r--   0 vojtechkania   (501) staff       (20)      117 2023-02-05 17:21:56.000000 redataprocessing-0.0.8/requirements.txt
--rw-r--r--   0 vojtechkania   (501) staff       (20)      281 2023-02-06 21:47:03.954187 redataprocessing-0.0.8/setup.cfg
--rw-r--r--   0 vojtechkania   (501) staff       (20)      123 2023-02-06 21:46:52.000000 redataprocessing-0.0.8/setup.py
+drwxr-xr-x   0 vojtechkania   (501) staff       (20)        0 2023-02-07 19:37:22.298292 redataprocessing-0.0.9/
+-rw-r--r--   0 vojtechkania   (501) staff       (20)     6148 2023-02-06 17:52:59.000000 redataprocessing-0.0.9/.DS_Store
+-rw-r--r--   0 vojtechkania   (501) staff       (20)     1073 2023-02-03 19:25:24.000000 redataprocessing-0.0.9/LICENSE
+-rw-r--r--   0 vojtechkania   (501) staff       (20)     2464 2023-02-07 19:37:22.298389 redataprocessing-0.0.9/PKG-INFO
+-rw-r--r--   0 vojtechkania   (501) staff       (20)     1822 2023-02-07 19:17:30.000000 redataprocessing-0.0.9/README.md
+-rw-r--r--   0 vojtechkania   (501) staff       (20)      183 2023-02-07 18:13:08.000000 redataprocessing-0.0.9/examples.py
+-rw-r--r--   0 vojtechkania   (501) staff       (20)      748 2023-02-07 18:12:32.000000 redataprocessing-0.0.9/pyproject.toml
+drwxr-xr-x   0 vojtechkania   (501) staff       (20)        0 2023-02-07 19:37:22.290644 redataprocessing-0.0.9/redataprocessing/
+-rw-r--r--   0 vojtechkania   (501) staff       (20)        0 2023-02-02 20:18:34.000000 redataprocessing-0.0.9/redataprocessing/__init__.py
+-rw-r--r--   0 vojtechkania   (501) staff       (20)    15921 2023-02-07 18:48:30.000000 redataprocessing-0.0.9/redataprocessing/sreality.py
+-rw-r--r--   0 vojtechkania   (501) staff       (20)     5528 2023-02-07 18:46:51.000000 redataprocessing-0.0.9/redataprocessing/sreality_api_dictionaries.py
+-rw-r--r--   0 vojtechkania   (501) staff       (20)     2221 2023-02-07 18:49:24.000000 redataprocessing-0.0.9/redataprocessing/sreality_description_asyncio.py
+-rw-r--r--   0 vojtechkania   (501) staff       (20)    10455 2023-02-07 17:55:27.000000 redataprocessing-0.0.9/redataprocessing/sreality_description_download_decoding.py
+drwxr-xr-x   0 vojtechkania   (501) staff       (20)        0 2023-02-07 19:37:22.298160 redataprocessing-0.0.9/redataprocessing.egg-info/
+-rw-r--r--   0 vojtechkania   (501) staff       (20)     2464 2023-02-07 19:37:21.000000 redataprocessing-0.0.9/redataprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 vojtechkania   (501) staff       (20)      501 2023-02-07 19:37:22.000000 redataprocessing-0.0.9/redataprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 vojtechkania   (501) staff       (20)        1 2023-02-07 19:37:21.000000 redataprocessing-0.0.9/redataprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 vojtechkania   (501) staff       (20)      101 2023-02-07 19:37:21.000000 redataprocessing-0.0.9/redataprocessing.egg-info/requires.txt
+-rw-r--r--   0 vojtechkania   (501) staff       (20)       17 2023-02-07 19:37:21.000000 redataprocessing-0.0.9/redataprocessing.egg-info/top_level.txt
+-rw-r--r--   0 vojtechkania   (501) staff       (20)      126 2023-02-07 18:11:27.000000 redataprocessing-0.0.9/requirements.txt
+-rw-r--r--   0 vojtechkania   (501) staff       (20)      416 2023-02-07 19:37:22.300619 redataprocessing-0.0.9/setup.cfg
+-rw-r--r--   0 vojtechkania   (501) staff       (20)      123 2023-02-06 21:46:52.000000 redataprocessing-0.0.9/setup.py
```

### Comparing `redataprocessing-0.0.8/.DS_Store` & `redataprocessing-0.0.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `redataprocessing-0.0.8/LICENSE` & `redataprocessing-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `redataprocessing-0.0.8/pyproject.toml` & `redataprocessing-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "redataprocessing"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Vojtěch Kania", email="vojtech.kania@gmail.com" },
   { name="Lukáš Novotný", email="30702889@fsv.cuni.cz" }
 ]
 description = "A package for download of real estate offers from Sreality.cz"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `redataprocessing-0.0.8/redataprocessing/sreality.py` & `redataprocessing-0.0.9/redataprocessing/sreality.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,21 @@
-"""Example NumPy style docstrings.
+"""Downloading and storing sreality offers to SQLite database.
 
-This module demonstrates documentation as specified by the `NumPy
-Documentation HOWTO`_. Docstrings may extend over multiple lines. Sections
-are created with a section header followed by an underline of equal length.
+This module contains functions that send requests to Sreality API,
+get json data, decode the data and store it into SQLite database. 
+List with offers and their detiled descriptions are requested separately.
+All functions are wrapped up in function get_re_offers.
 
 Example
 -------
-Examples can be given using either the ``Example`` or ``Examples``
-sections. Sections support any reStructuredText formatting, including
-literal blocks::
-
-    $ python example_numpy.py
-
-
-Section breaks are created with two blank lines. Section breaks are also
-implicitly created anytime a new section starts. Section bodies *may* be
-indented:
-
-Notes
------
-    This is an example of an indented section. It's like any other section,
-    but the body is indented to help it stand out from surrounding text.
-
-If a section is indented, then a section break is created by
-resuming unindented text.
-
-Attributes
-----------
-module_level_variable1 : int
-    Module level variables may be documented in either the ``Attributes``
-    section of the module docstring, or in an inline docstring immediately
-    following the variable.
-
-    Either form is acceptable, but the two should not be mixed. Choose
-    one convention to document module level variables and be consistent
-    with it.
+Example of simplest use of this module could be found in the following file:
 
-"""
+    examples.py
 
+"""
 
 # importing all packages
 import pandas as pd
 import numpy as np
 
 import requests
 import sqlite3
@@ -64,29 +38,28 @@
 # requesting information from sreality api
 
 def download_lists(category_main: int, category_type: int, locality_region_id: Optional[Union[int, list]], category_sub: Optional[Union[int, list]]=None) -> list:
     """
 
     Parameters
     ----------
-    category_main :
-        
-    category_type :
-        
-    category_sub :
+    category_main : int :
+        code of main real estate category
+    category_type : int :
+        code of real estate type
+    category_sub : int :
+        code of real estate subcategory
+    locality_region_id : int :
+        indicator of region of the Czech Republic
         
-    locality_region_id :
-        
-
     Returns
     -------
-
+    This function returns a collector which is a list containing all requests as json.
     """
 
-
     if isinstance(category_sub, int):
         category_sub_string=str(category_sub)
     elif isinstance(category_sub, list):
         category_sub_string = '%7C'.join(str(v) for v in category_sub)
     else:
         raise TypeError("category_sub: must be an integer or a list")
     
@@ -153,47 +126,50 @@
 
 def get_gps_lat_lon(estate_raw: Dict) -> Tuple[str, str]:
     """
 
     Parameters
     ----------
     estate_raw: Dict :
+        Requested data in json
         
     Returns
     -------
+    Latitude and longitude of respective sreality offer.
 
     """
     gps_ = estate_raw['gps']
     return gps_['lat'], gps_['lon']
 
 def get_flat_type_from_name(name: str) -> str:
     """
 
     Parameters
     ----------
     name: str :
-        
+        Always represented by string "Prodej bytu [type of flat] [Area] m^2"
 
     Returns
     -------
+    Returns a string with apartment type.
 
     """
     return name.split()[2]
 
 def get_area_from_name(name: str) -> int:
     """
 
     Parameters
     ----------
     name: str :
-        
+        always represented by string "Prodej bytu [type of flat] [Area] m^2"
 
     Returns
     -------
-
+    Integer with area of the real estate in the respective offer.
     """
     if category_main == 1:
         name_ = name.split()
         return int(''.join(re.findall('(\d*)', ''.join(name_[3:]))))
     else:
         name_ = re.sub("m2", "", name)
         name_ = name_.split()
@@ -201,18 +177,19 @@
 
 def get_company_details(estate_raw: Dict) -> Tuple[str, str]:
     """
 
     Parameters
     ----------
     estate_raw: Dict :
-        
+        requested data in json
 
     Returns
     -------
+    Company ID and company name stored in respective json.
 
     """
     try:
             company_id = estate_raw["_embedded"]["company"]["id"]
             company_name = estate_raw["_embedded"]["company"]["name"]
     except (KeyError):
             company_id = np.nan
@@ -223,20 +200,20 @@
 # wrapping up all decoding
 
 def decode_collector(collector: list, category_main: int) -> pd.DataFrame:
     """
 
     Parameters
     ----------
-    collector :
-        
+    collector : list :
+        list containing all requests as json
 
     Returns
     -------
-
+    It returns pandas dataframe with decoded data.
     """
     estates_individual = {}
 
     for page, r in tqdm(collector.items(),desc="decoding pages with offers: "):
         for estate in r['_embedded']['estates']: 
 
             estate_relevant = pd.Series(dtype="object")
@@ -279,25 +256,26 @@
     category_type: int, 
     locality_region_id: int, 
     category_sub: list=None) -> pd.DataFrame:
     """
 
     Parameters
     ----------
-    category_main :
-        
-    category_type :
-        
-    category_sub :
-        
-    locality_region_id :
+    category_main : int :
+        code of main real estate main category
+    category_type : int : 
+        code of real estate type
+    category_sub : int :
+        code of real estate subcategory
+    locality_region_id : int :
+        indicator of region of the Czech Republic
         
     Returns
     -------
-
+    dataframe with decoded data
     """
 
     category_main_input=category_main
     category_type_input=category_type
     category_sub_input=category_sub
     locality_region_id_input=locality_region_id
 
@@ -320,21 +298,23 @@
 # Saving data (SQLite)
 
 def save_re_offers(df: pd.DataFrame, path_to_sqlite: str, category_main: int, category_type: int) -> None:
     """
 
     Parameters
     ----------
-    df :
+    df :  pandas.DataFrame
+        dataframe with decoded real estate data
         
-    path_to_sqlite :
+    path_to_sqlite : str : 
+        path to sqlite database where table with offers is already stored
         
-
-    Returns
+    Returns 
     -------
+    Data will be saved to SQLite.
 
     """
     con = sqlite3.connect(path_to_sqlite) # We must choose the name for our DB !
 
     # Creates a table or appends if exists
     db_table_name=create_db_table_name(category_main=category_main, category_type=category_type)
     db_table_name_offers="OFFERS_"+db_table_name
@@ -354,33 +334,33 @@
     df.to_sql(name = db_table_name_offers, con= con, index = False, if_exists = 'append')
     # Loading again: df = pd.read_sql('SELECT * FROM OFFERS_TABLE', con = con)
 
     # Closing the connection
     con.close()
 
 def get_re_offers(path_to_sqlite: str, category_main: str, category_type: str, 
-locality_region: Optional[Union[int, list]], category_sub: Optional[Union[int, list]]=None) -> None:
+locality_region: Optional[Union[str, list]], category_sub: Optional[Union[str, list]]=None) -> None:
     """
 
     Parameters
     ----------
-    path_to_sqlite :
+    path_to_sqlite : str :
         Path to sqlite database. If the database does not exist it will be created base on name and path provided.
-    category_main :
-        
-    category_type :
-        
-    category_sub :
-        
-    locality_region_id :
-        
+    category_main : str :
+        Name of main real estate category (e.g., "apartments")
+    category_type : str : 
+        Name of real estate type (e.g., "sale").
+    category_sub : list, int : 
+        Name of real estate categories (e.g. "2+kk")
+    locality_region_id : list, int :
+        Name of region of the Czech Republic in Czech language (e.g., "Hlavní město Praha").
 
     Returns
     -------
-
+    Data is saved to SQLite database in folder specified by path_to_sqlite.
     """
     
     # inputs to further functions
     if isinstance(category_main, str):
         if category_main not in category_main_dict.keys():
             raise ValueError("category_main: must be one of %r." % list(category_main_dict.keys()))
         else:
@@ -464,20 +444,20 @@
     print("initiating download of description of offers")
 
     get_re_offers_description(path_to_sqlite=path_to_sqlite_input, 
     category_main=category_main_input, category_type=category_type_input)
 
 # INPUTS
 #sleep(2)
-path_to_sqlite='estate_data.sqlite'
+#path_to_sqlite='estate_data.sqlite'
 
-category_main = "apartments" # 1=byty, 2=domy, 3=pozemky, 4=komerční, 5=ostatní
-category_type = "sale" # 1=prodej, 2=nájem, 3=dražba
-category_sub = [] # 34=garáže, 52=garážové stání
-locality_region = ["Královéhradecký kraj"] #10=Praha, 11=Středočeský kraj, 5: Liberecký kraj, 1: Českobudějovický kraj
+#category_main = "apartments" # 1=byty, 2=domy, 3=pozemky, 4=komerční, 5=ostatní
+#category_type = "sale" # 1=prodej, 2=nájem, 3=dražba
+#category_sub = [] # 34=garáže, 52=garážové stání
+#locality_region = ["Královéhradecký kraj"] #10=Praha, 11=Středočeský kraj, 5: Liberecký kraj, 1: Českobudějovický kraj
 
 #category_main = 1 # 1=byty, 2=domy, 3=pozemky, 4=komerční, 5=ostatní
 #category_type = 1 # 1=prodej, 2=nájem, 3=dražba
 #category_sub = [] # 34=garáže, 52=garážové stání
 #locality_region_id = [13] #10=Praha, 11=Středočeský kraj, 5: Liberecký kraj, 1: Českobudějovický kraj
 
 #get_re_offers(path_to_sqlite="estate_data.sqlite", category_main="apartments", category_type="sale", category_sub=[], locality_region=["Královéhradecký kraj"])
```

### Comparing `redataprocessing-0.0.8/redataprocessing/sreality_description_download_decoding.py` & `redataprocessing-0.0.9/redataprocessing/sreality_description_download_decoding.py`

 * *Files 10% similar despite different names*

```diff
@@ -93,52 +93,50 @@
     return indices
 
 def urls_from_indices(indices:list) -> list:
     """
 
     Parameters
     ----------
-    indices :
+    indices : list of hash_ids
         
-
     Returns
     -------
-
+    urls - list of urls to APIs
     """
     urls=["https://www.sreality.cz/api/cs/v2/estates/"+str(i) for i in indices]
     return urls
 
 # %%
 # preparation of functions for decoding
 
 def note_missing_values(r_dict_names_all:Dict):
     """
 
     Parameters
     ----------
-    r_dict_names_all :
+    r_dict_names_all : dictionary with Czech and English column names to be scrapped
         
     Returns
     -------
-
+    nothing (prints the missing values whcich could be added to dictionary and be scrapped)
     """
     print("Add these values to description_items_dict in sreality_api_dictionaries.py:")
     print(r_dict_names_all[~r_dict_names_all.isin(description_items_dict.keys())])
 
 def individual_description_into_pd_df(description_individual) -> pd.DataFrame:
     """
 
     Parameters
     ----------
-    description_individual :
-        
+    description_individual :    
 
     Returns
     -------
-
+    dataframe
     """
     df_desc = pd.concat(description_individual).unstack()
     df_desc["equipped"]=df_desc["equipped"].map({True: "ano", False: "ne", "Částečně":"částečně"}) 
     df_desc.reset_index(inplace=True)
     df_desc = df_desc.rename(columns = {'index':'hash_id'})
     return df_desc
 
@@ -146,18 +144,17 @@
 def description_decoding(responses_list: list) -> pd.DataFrame:
     """
 
     Parameters
     ----------
     responses_list : list : list of responses of real estate descriptions downloaded from sreality
     
-
     Returns
     -------
-
+    decoded dataframe
     """
         
     description_individual = {}
     r_dict_names_all=pd.Series(dtype="object")
     r_dict_types_all=pd.DataFrame(columns=["name", "type"])
     
     total=len(responses_list)
@@ -207,44 +204,43 @@
 
 # We transform columns with list so we could save to DB
 def transformer(value) -> str:
     """
 
     Parameters
     ----------
-    value :
-        
+    value : value to be transformed        
 
     Returns
     -------
-
+    string sperating the values with double spaces
     """
     if type(value) == list:
         string = ""
         for i in value:
             string += i['value'] + "  "
         return string[:-2]
 
 def save_to_db(df: pd.DataFrame, path_to_sqlite: str, category_main: int, category_type: int):
     """
 
     Parameters
     ----------
-    df : pandas data frame : 
+    df : pandas data frame : dataframe to be saved
         
     path_to_sqlite : str : 
         path to sqlite database where the dataframe will be stored
         
-    category_main : int :
+    category_main : int : code of main real estate category
 
-    category_type : int : 
+    category_type : int : code of real estate type
 
     Returns
     -------
-
+    nothing (SQLite will be saved)
     """
     
     for column in columns_w_list:
         df[column] = df[column].apply(lambda row: transformer(row))
 
     # Creates a table or appends if exists
     con = sqlite3.connect(path_to_sqlite)
@@ -303,8 +299,8 @@
     df = description_decoding(output_list)
 
     db_table_name=create_db_table_name(category_main=category_main_input, category_type=category_type_input)
     db_table_name_description="DESCRIPTION_"+db_table_name
     print("saving description of offers to database (table {})".format(db_table_name_description))
 
     save_to_db(df, path_to_sqlite=path_to_sqlite_input, category_main=category_main_input, category_type=category_type_input)
-    print("saved description of offers to database (table {})".format(db_table_name_description))
+    print("saved description of offers to database (table {})".format(db_table_name_description))
```

