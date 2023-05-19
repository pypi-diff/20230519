# Comparing `tmp/simpler_sf-1.0.0.tar.gz` & `tmp/simpler_sf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/simpler-sf/simpler-sf/dist/.tmp-f5t6fjui/simpler_sf-1.0.0.tar", last modified: Wed Apr 26 08:41:22 2023, max compression
+gzip compressed data, was "/home/runner/work/simpler-sf/simpler-sf/dist/.tmp-pijfae5_/simpler_sf-1.0.1.tar", last modified: Fri May 19 15:38:10 2023, max compression
```

## Comparing `simpler_sf-1.0.0.tar` & `simpler_sf-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:41:22.000000 simpler_sf-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 08:40:59.000000 simpler_sf-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-26 08:41:22.000000 simpler_sf-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-26 08:40:59.000000 simpler_sf-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-26 08:40:59.000000 simpler_sf-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:41:22.000000 simpler_sf-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-26 08:40:59.000000 simpler_sf-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:41:22.000000 simpler_sf-1.0.0/simpler_sf/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 08:40:59.000000 simpler_sf-1.0.0/simpler_sf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-04-26 08:40:59.000000 simpler_sf-1.0.0/simpler_sf/_simpler_sf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:41:22.000000 simpler_sf-1.0.0/simpler_sf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-26 08:41:22.000000 simpler_sf-1.0.0/simpler_sf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-26 08:41:22.000000 simpler_sf-1.0.0/simpler_sf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:41:22.000000 simpler_sf-1.0.0/simpler_sf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 08:41:22.000000 simpler_sf-1.0.0/simpler_sf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:38:10.000000 simpler_sf-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-19 15:38:01.000000 simpler_sf-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-19 15:38:10.000000 simpler_sf-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-19 15:38:01.000000 simpler_sf-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-19 15:38:01.000000 simpler_sf-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 15:38:10.000000 simpler_sf-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-19 15:38:01.000000 simpler_sf-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:38:10.000000 simpler_sf-1.0.1/simpler_sf/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-19 15:38:01.000000 simpler_sf-1.0.1/simpler_sf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-05-19 15:38:01.000000 simpler_sf-1.0.1/simpler_sf/_simpler_sf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:38:10.000000 simpler_sf-1.0.1/simpler_sf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-19 15:38:10.000000 simpler_sf-1.0.1/simpler_sf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-19 15:38:10.000000 simpler_sf-1.0.1/simpler_sf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:38:10.000000 simpler_sf-1.0.1/simpler_sf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 15:38:10.000000 simpler_sf-1.0.1/simpler_sf.egg-info/top_level.txt
```

### Comparing `simpler_sf-1.0.0/LICENSE` & `simpler_sf-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simpler_sf-1.0.0/PKG-INFO` & `simpler_sf-1.0.1/simpler_sf.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simpler_sf
-Version: 1.0.0
+Name: simpler-sf
+Version: 1.0.1
 Summary: Extending Simple Salesforce to support Pandas exports and more.
 Home-page: https://github.com/benvigano/simpler-sf
 Author: benvigano
 Author-email: beniamino.vigano@protonmail.com
 License: MIT
 Keywords: Salesforce,Simple Salesforce,Pandas,Dataframe,Unpack Salesforce
 Description-Content-Type: text/markdown
@@ -13,48 +13,38 @@
 # simpler-sf
 Extending the low-level Salesforce API client [Simple Salesforce](https://github.com/simple-salesforce/simple-salesforce) to support exports in Pandas, and other features.
 
 ## Usage
 ### Install
 `pip install simpler-sf`
 
-### Importing
+### Import
 ```python
-import simpler-sf
-simpler-sf.simple_salesforce()
+import simpler_sf
+simpler_sf.simple_salesforce()
 import simple_salesforce
 # That's it!
 ```
-### `smart_query()`
+### Query
 Simpler-sf adds the `smart_query()` method to the `simple_salesforce.Salesforce` class.
 
 The advantages over the existing methods are:
+- Un-nesting of results for relationship queries (aka the infamous `'attributes'` field) (not just for one level)
 - Query results in `pd.Dataframe` format
-- Un-nesting of results for relationship queries (aka the infamous `'attributes'` dictionary) 
 - No limit on the number of output rows as in `simple_salesforce.Salesforce.query()` **and** at the same time...
 - No need to use a different class for each Salesforce object as in `sf.bulk.Account.query(query)`
-- The option to filter dynamically, on large amounts of values without a limit on the number of characters (see example below)
+- The option to filter dynamically, on large amounts of values without a limit on the number of characters
 
-##### Example
+#### Example
 ```python 
 sf = simple_salesforce.Salesforce(username=username, password=password, security_token=token)
-df = sf.smart_query('SELECT Contact.Name, Account.Name Id FROM Call')
+df = sf.smart_query('SELECT Contact.Id, Contact.FirstName, Account.Name, Campaign FROM CampaignMember')
+print(df)
 ```
-
-##### Example with filtering
-```python 
-sf = simple_salesforce.Salesforce(username=username, password=password, security_token=token)
-
-ids = ['0032400000QZbmtAAD', '0032400000eGqdZAAS', '00324036u9QZbnGAAT', '50130000000014C']
-query = \
-'''
-SELECT
-Id,
-FirstName,
-LastName,
-Pronouns,
-Phone,
-Email
-FROM Contact
-'''
-df = sf.smart_query(query, filter_field='Id', filter_values=ids)
+Output:
+```
+            Contact.Id   Contact.FirstName   Account.Name           Campaign
+0   0032400000QZbmtAAD               Emily         Amazon   CampaignA_2023Q2
+1   0032400000eGqdZAAS             Jasmine         Amazon   CampaignA_2023Q2
+2   00324036u9QZbnGAAT                Míng      Microsoft   CampaignB_2022Q4
+3   0032400000QZbygAAX           Magdalena         Google   CampaignC_2023Q1
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `simpler_sf-1.0.0/README.md` & `simpler_sf-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,38 @@
 # simpler-sf
 Extending the low-level Salesforce API client [Simple Salesforce](https://github.com/simple-salesforce/simple-salesforce) to support exports in Pandas, and other features.
 
 ## Usage
 ### Install
 `pip install simpler-sf`
 
-### Importing
+### Import
 ```python
-import simpler-sf
-simpler-sf.simple_salesforce()
+import simpler_sf
+simpler_sf.simple_salesforce()
 import simple_salesforce
 # That's it!
 ```
-### `smart_query()`
+### Query
 Simpler-sf adds the `smart_query()` method to the `simple_salesforce.Salesforce` class.
 
 The advantages over the existing methods are:
+- Un-nesting of results for relationship queries (aka the infamous `'attributes'` field) (not just for one level)
 - Query results in `pd.Dataframe` format
-- Un-nesting of results for relationship queries (aka the infamous `'attributes'` dictionary) 
 - No limit on the number of output rows as in `simple_salesforce.Salesforce.query()` **and** at the same time...
 - No need to use a different class for each Salesforce object as in `sf.bulk.Account.query(query)`
-- The option to filter dynamically, on large amounts of values without a limit on the number of characters (see example below)
+- The option to filter dynamically, on large amounts of values without a limit on the number of characters
 
-##### Example
+#### Example
 ```python 
 sf = simple_salesforce.Salesforce(username=username, password=password, security_token=token)
-df = sf.smart_query('SELECT Contact.Name, Account.Name Id FROM Call')
+df = sf.smart_query('SELECT Contact.Id, Contact.FirstName, Account.Name, Campaign FROM CampaignMember')
+print(df)
 ```
-
-##### Example with filtering
-```python 
-sf = simple_salesforce.Salesforce(username=username, password=password, security_token=token)
-
-ids = ['0032400000QZbmtAAD', '0032400000eGqdZAAS', '00324036u9QZbnGAAT', '50130000000014C']
-query = \
-'''
-SELECT
-Id,
-FirstName,
-LastName,
-Pronouns,
-Phone,
-Email
-FROM Contact
-'''
-df = sf.smart_query(query, filter_field='Id', filter_values=ids)
+Output:
+```
+            Contact.Id   Contact.FirstName   Account.Name           Campaign
+0   0032400000QZbmtAAD               Emily         Amazon   CampaignA_2023Q2
+1   0032400000eGqdZAAS             Jasmine         Amazon   CampaignA_2023Q2
+2   00324036u9QZbnGAAT                Míng      Microsoft   CampaignB_2022Q4
+3   0032400000QZbygAAX           Magdalena         Google   CampaignC_2023Q1
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `simpler_sf-1.0.0/setup.py` & `simpler_sf-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `simpler_sf-1.0.0/simpler_sf/_simpler_sf.py` & `simpler_sf-1.0.1/simpler_sf/_simpler_sf.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,14 +73,24 @@
 
     if " from " not in query.lower():
         raise Exception(f"'from' not found in query '{query.lower()}'")
 
     return re.split(" from ", query, flags=re.IGNORECASE)[1].split(" ")[0]
 
 
+def _determine_fields(query):
+    '''Parse a query to determine the fields'''
+    
+    before_from = re.split(" from ", query, flags=re.IGNORECASE)[0]
+    after_select = re.split("select ", before_from, flags=re.IGNORECASE)[1]
+    fields = after_select.replace(" ", "").split(",")
+    
+    return fields
+
+
 def _generate_sub_queries(query, filter_field, filter_values, not_in):
     '''
     Split the input query in multiple sub-queries that respect Salesforce 10,000 character limit.
     If the input query already respects the character limit, the function returns a list containing just the input query.
     '''
     
     query_character_limit = 100000  # As per SalesForce documentation
@@ -145,14 +155,23 @@
         sub_queries = [query]
                  
     dfs = []
     for sub_query in tqdm(sub_queries):
         results = _unnest_query_output(object.query(sub_query))    
         partial_df = pd.DataFrame(results)
         dfs.append(partial_df)
+        
+    output_df = pd.concat(dfs)
+        
+    # If the query didn't output any records, add the columns for output consistency
+    if len(dfs) == 0:
+        # Determine the columns from the query
+        output_df = pd.DataFrame(columns=_determine_fields(query))
+    else:
+        pass
                     
-    return pd.concat(dfs)
+    return output_df
 
 
 def simple_salesforce():
     import simple_salesforce
     simple_salesforce.Salesforce.smart_query = _smart_query
```

### Comparing `simpler_sf-1.0.0/simpler_sf.egg-info/PKG-INFO` & `simpler_sf-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simpler-sf
-Version: 1.0.0
+Name: simpler_sf
+Version: 1.0.1
 Summary: Extending Simple Salesforce to support Pandas exports and more.
 Home-page: https://github.com/benvigano/simpler-sf
 Author: benvigano
 Author-email: beniamino.vigano@protonmail.com
 License: MIT
 Keywords: Salesforce,Simple Salesforce,Pandas,Dataframe,Unpack Salesforce
 Description-Content-Type: text/markdown
@@ -13,48 +13,38 @@
 # simpler-sf
 Extending the low-level Salesforce API client [Simple Salesforce](https://github.com/simple-salesforce/simple-salesforce) to support exports in Pandas, and other features.
 
 ## Usage
 ### Install
 `pip install simpler-sf`
 
-### Importing
+### Import
 ```python
-import simpler-sf
-simpler-sf.simple_salesforce()
+import simpler_sf
+simpler_sf.simple_salesforce()
 import simple_salesforce
 # That's it!
 ```
-### `smart_query()`
+### Query
 Simpler-sf adds the `smart_query()` method to the `simple_salesforce.Salesforce` class.
 
 The advantages over the existing methods are:
+- Un-nesting of results for relationship queries (aka the infamous `'attributes'` field) (not just for one level)
 - Query results in `pd.Dataframe` format
-- Un-nesting of results for relationship queries (aka the infamous `'attributes'` dictionary) 
 - No limit on the number of output rows as in `simple_salesforce.Salesforce.query()` **and** at the same time...
 - No need to use a different class for each Salesforce object as in `sf.bulk.Account.query(query)`
-- The option to filter dynamically, on large amounts of values without a limit on the number of characters (see example below)
+- The option to filter dynamically, on large amounts of values without a limit on the number of characters
 
-##### Example
+#### Example
 ```python 
 sf = simple_salesforce.Salesforce(username=username, password=password, security_token=token)
-df = sf.smart_query('SELECT Contact.Name, Account.Name Id FROM Call')
+df = sf.smart_query('SELECT Contact.Id, Contact.FirstName, Account.Name, Campaign FROM CampaignMember')
+print(df)
 ```
-
-##### Example with filtering
-```python 
-sf = simple_salesforce.Salesforce(username=username, password=password, security_token=token)
-
-ids = ['0032400000QZbmtAAD', '0032400000eGqdZAAS', '00324036u9QZbnGAAT', '50130000000014C']
-query = \
-'''
-SELECT
-Id,
-FirstName,
-LastName,
-Pronouns,
-Phone,
-Email
-FROM Contact
-'''
-df = sf.smart_query(query, filter_field='Id', filter_values=ids)
+Output:
+```
+            Contact.Id   Contact.FirstName   Account.Name           Campaign
+0   0032400000QZbmtAAD               Emily         Amazon   CampaignA_2023Q2
+1   0032400000eGqdZAAS             Jasmine         Amazon   CampaignA_2023Q2
+2   00324036u9QZbnGAAT                Míng      Microsoft   CampaignB_2022Q4
+3   0032400000QZbygAAX           Magdalena         Google   CampaignC_2023Q1
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

