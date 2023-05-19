# Comparing `tmp/hydrotools.nwis_client-3.2.1.tar.gz` & `tmp/hydrotools.nwis_client-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrotools.nwis_client-3.2.1.tar", last modified: Thu Mar 24 13:53:13 2022, max compression
+gzip compressed data, was "hydrotools.nwis_client-3.3.1.tar", last modified: Fri May 19 16:25:03 2023, max compression
```

## Comparing `hydrotools.nwis_client-3.2.1.tar` & `hydrotools.nwis_client-3.3.1.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 araney     (502) staff       (20)        0 2022-03-24 13:53:13.878807 hydrotools.nwis_client-3.2.1/
--rw-r--r--   0 araney     (502) staff       (20)      527 2021-08-25 14:54:34.000000 hydrotools.nwis_client-3.2.1/LICENSE
--rw-r--r--   0 araney     (502) staff       (20)       16 2021-08-25 14:54:34.000000 hydrotools.nwis_client-3.2.1/MANIFEST.in
--rw-r--r--   0 araney     (502) staff       (20)     7051 2022-03-24 13:53:13.878953 hydrotools.nwis_client-3.2.1/PKG-INFO
--rw-r--r--   0 araney     (502) staff       (20)     5932 2022-03-24 13:51:59.000000 hydrotools.nwis_client-3.2.1/README.md
--rw-r--r--   0 araney     (502) staff       (20)      101 2021-08-25 14:54:34.000000 hydrotools.nwis_client-3.2.1/pyproject.toml
--rw-r--r--   0 araney     (502) staff       (20)     1452 2022-03-24 13:53:13.879657 hydrotools.nwis_client-3.2.1/setup.cfg
-drwxr-xr-x   0 araney     (502) staff       (20)        0 2022-03-24 13:53:13.873230 hydrotools.nwis_client-3.2.1/src/
-drwxr-xr-x   0 araney     (502) staff       (20)        0 2022-03-24 13:53:13.873318 hydrotools.nwis_client-3.2.1/src/hydrotools/
-drwxr-xr-x   0 araney     (502) staff       (20)        0 2022-03-24 13:53:13.878483 hydrotools.nwis_client-3.2.1/src/hydrotools/nwis_client/
--rw-r--r--   0 araney     (502) staff       (20)      196 2021-10-29 18:47:44.000000 hydrotools.nwis_client-3.2.1/src/hydrotools/nwis_client/__init__.py
--rw-r--r--   0 araney     (502) staff       (20)     3247 2022-03-24 13:51:44.000000 hydrotools.nwis_client-3.2.1/src/hydrotools/nwis_client/_utilities.py
--rw-r--r--   0 araney     (502) staff       (20)       22 2022-03-24 13:51:59.000000 hydrotools.nwis_client-3.2.1/src/hydrotools/nwis_client/_version.py
--rw-r--r--   0 araney     (502) staff       (20)     3322 2022-03-24 13:51:59.000000 hydrotools.nwis_client-3.2.1/src/hydrotools/nwis_client/cli.py
--rw-r--r--   0 araney     (502) staff       (20)    30249 2022-03-24 13:51:59.000000 hydrotools.nwis_client-3.2.1/src/hydrotools/nwis_client/iv.py
-drwxr-xr-x   0 araney     (502) staff       (20)        0 2022-03-24 13:53:13.876574 hydrotools.nwis_client-3.2.1/src/hydrotools.nwis_client.egg-info/
--rw-r--r--   0 araney     (502) staff       (20)     7051 2022-03-24 13:53:13.000000 hydrotools.nwis_client-3.2.1/src/hydrotools.nwis_client.egg-info/PKG-INFO
--rw-r--r--   0 araney     (502) staff       (20)      542 2022-03-24 13:53:13.000000 hydrotools.nwis_client-3.2.1/src/hydrotools.nwis_client.egg-info/SOURCES.txt
--rw-r--r--   0 araney     (502) staff       (20)        1 2022-03-24 13:53:13.000000 hydrotools.nwis_client-3.2.1/src/hydrotools.nwis_client.egg-info/dependency_links.txt
--rw-r--r--   0 araney     (502) staff       (20)       63 2022-03-24 13:53:13.000000 hydrotools.nwis_client-3.2.1/src/hydrotools.nwis_client.egg-info/entry_points.txt
--rw-r--r--   0 araney     (502) staff       (20)       90 2022-03-24 13:53:13.000000 hydrotools.nwis_client-3.2.1/src/hydrotools.nwis_client.egg-info/requires.txt
--rw-r--r--   0 araney     (502) staff       (20)       11 2022-03-24 13:53:13.000000 hydrotools.nwis_client-3.2.1/src/hydrotools.nwis_client.egg-info/top_level.txt
+drwxrwxr-x   0 jregina   (1000) jregina   (1000)        0 2023-05-19 16:25:03.200613 hydrotools.nwis_client-3.3.1/
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)      527 2023-05-10 18:02:15.000000 hydrotools.nwis_client-3.3.1/LICENSE
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)       16 2023-05-10 18:02:15.000000 hydrotools.nwis_client-3.3.1/MANIFEST.in
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)     7031 2023-05-19 16:25:03.200613 hydrotools.nwis_client-3.3.1/PKG-INFO
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)     5932 2023-05-10 18:02:15.000000 hydrotools.nwis_client-3.3.1/README.md
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)      101 2023-05-10 18:02:15.000000 hydrotools.nwis_client-3.3.1/pyproject.toml
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)     1452 2023-05-19 16:25:03.200613 hydrotools.nwis_client-3.3.1/setup.cfg
+drwxrwxr-x   0 jregina   (1000) jregina   (1000)        0 2023-05-19 16:25:03.200613 hydrotools.nwis_client-3.3.1/src/
+drwxrwxr-x   0 jregina   (1000) jregina   (1000)        0 2023-05-19 16:25:03.200613 hydrotools.nwis_client-3.3.1/src/hydrotools/
+drwxrwxr-x   0 jregina   (1000) jregina   (1000)        0 2023-05-19 16:25:03.200613 hydrotools.nwis_client-3.3.1/src/hydrotools/nwis_client/
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)      196 2023-05-10 18:02:15.000000 hydrotools.nwis_client-3.3.1/src/hydrotools/nwis_client/__init__.py
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)     3247 2023-05-10 18:02:15.000000 hydrotools.nwis_client-3.3.1/src/hydrotools/nwis_client/_utilities.py
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)       22 2023-05-19 16:18:38.000000 hydrotools.nwis_client-3.3.1/src/hydrotools/nwis_client/_version.py
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)     3322 2023-05-10 18:02:15.000000 hydrotools.nwis_client-3.3.1/src/hydrotools/nwis_client/cli.py
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)    32292 2023-05-19 16:18:38.000000 hydrotools.nwis_client-3.3.1/src/hydrotools/nwis_client/iv.py
+drwxrwxr-x   0 jregina   (1000) jregina   (1000)        0 2023-05-19 16:25:03.200613 hydrotools.nwis_client-3.3.1/src/hydrotools.nwis_client.egg-info/
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)     7031 2023-05-19 16:25:03.000000 hydrotools.nwis_client-3.3.1/src/hydrotools.nwis_client.egg-info/PKG-INFO
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)      611 2023-05-19 16:25:03.000000 hydrotools.nwis_client-3.3.1/src/hydrotools.nwis_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)        1 2023-05-19 16:25:03.000000 hydrotools.nwis_client-3.3.1/src/hydrotools.nwis_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)       63 2023-05-19 16:25:03.000000 hydrotools.nwis_client-3.3.1/src/hydrotools.nwis_client.egg-info/entry_points.txt
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)       90 2023-05-19 16:25:03.000000 hydrotools.nwis_client-3.3.1/src/hydrotools.nwis_client.egg-info/requires.txt
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)       11 2023-05-19 16:25:03.000000 hydrotools.nwis_client-3.3.1/src/hydrotools.nwis_client.egg-info/top_level.txt
+drwxrwxr-x   0 jregina   (1000) jregina   (1000)        0 2023-05-19 16:25:03.200613 hydrotools.nwis_client-3.3.1/tests/
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)     1283 2023-05-10 18:02:15.000000 hydrotools.nwis_client-3.3.1/tests/test__utilities.py
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)     1587 2023-05-10 18:02:15.000000 hydrotools.nwis_client-3.3.1/tests/test_client_cli.py
+-rw-rw-r--   0 jregina   (1000) jregina   (1000)    18617 2023-05-19 16:18:38.000000 hydrotools.nwis_client-3.3.1/tests/test_nwis.py
```

### Comparing `hydrotools.nwis_client-3.2.1/LICENSE` & `hydrotools.nwis_client-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrotools.nwis_client-3.2.1/PKG-INFO` & `hydrotools.nwis_client-3.3.1/src/hydrotools.nwis_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
-Name: hydrotools.nwis_client
-Version: 3.2.1
+Name: hydrotools.nwis-client
+Version: 3.3.1
 Summary: A convenient interface to the USGS NWIS Instantaneous Values (IV) REST Service API.
 Home-page: https://github.com/NOAA-OWP/hydrotools
 Author: Austin Raney
 Author-email: aaraney@protonmail.com
 License: USDOC
 Project-URL: Documentation, https://noaa-owp.github.io/hydrotools/hydrotools.nwis_client.html
 Project-URL: Source, https://github.com/NOAA-OWP/hydrotools/tree/main/python/nwis_client
 Project-URL: Tracker, https://github.com/NOAA-OWP/hydrotools/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free To Use But Restricted
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -168,9 +167,7 @@
 2021-05-31 23:35:00,gage height,02146470,ft,3.14,['A'],0
 2021-05-31 23:40:00,gage height,02146470,ft,3.14,['A'],0
 2021-05-31 23:45:00,gage height,02146470,ft,3.14,['A'],0
 2021-05-31 23:50:00,gage height,02146470,ft,3.14,['A'],0
 2021-05-31 23:55:00,gage height,02146470,ft,3.14,['A'],0
 2021-06-01 00:00:00,gage height,02146470,ft,3.14,['A'],0
 ```
-
-
```

### Comparing `hydrotools.nwis_client-3.2.1/README.md` & `hydrotools.nwis_client-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hydrotools.nwis_client-3.2.1/setup.cfg` & `hydrotools.nwis_client-3.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hydrotools.nwis_client-3.2.1/src/hydrotools/nwis_client/_utilities.py` & `hydrotools.nwis_client-3.3.1/src/hydrotools/nwis_client/_utilities.py`

 * *Files identical despite different names*

### Comparing `hydrotools.nwis_client-3.2.1/src/hydrotools/nwis_client/cli.py` & `hydrotools.nwis_client-3.3.1/src/hydrotools/nwis_client/cli.py`

 * *Files identical despite different names*

### Comparing `hydrotools.nwis_client-3.2.1/src/hydrotools/nwis_client/iv.py` & `hydrotools.nwis_client-3.3.1/src/hydrotools/nwis_client/iv.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,15 @@
             datetime.datetime,
             np.datetime64,
             pd.Timestamp,
             None,
         ] = None,
         period: Union[str, None] = None,
         siteStatus: str = "all",
+        include_expanded_metadata: bool = False,
         **params,
     ):
         """Return Pandas DataFrame of NWIS IV data.
 
         Parameters
         ----------
         sites: str, List[str], pandas.Series[str], or numpy.Array[str], optional
@@ -185,14 +186,17 @@
         endDT: str, datetime.datetime, np.datetime64, pd.Timestamp, or None, optional, default None
             Observation record end time. If timezone information not provided, defaults to UTC.
         period: str, None
             Observation record for period until current time. Uses ISO 8601 period time.
         siteStatus: str, optional, default 'all'
             Site status in string format.
             Options: 'all', 'active', 'inactive'
+        include_expanded_metadata: bool, default False
+            Setting to True will add latitude, longitude, srs, hucCd, stateCd, countyCd, and siteName
+            columns to the returned dataframe.
         params:
             Additional parameters passed directly to service.
 
         Returns
         -------
         pandas.DataFrame :
             DataFrame in semi-WRES compatible format
@@ -240,14 +244,15 @@
             bBox=bBox,
             countyCd=countyCd,
             parameterCd=parameterCd,
             startDT=startDT,
             endDT=endDT,
             period=period,
             siteStatus=siteStatus,
+            include_expanded_metadata=include_expanded_metadata,
             **params,
         )
 
         def list_to_df_helper(item: dict):
             values = item.pop("values")
             df = pd.DataFrame(values)
 
@@ -276,20 +281,19 @@
         if dfs.empty:
             empty_df_warning_helper()
             empty_df = _create_empty_canonical_df()
             empty_df = empty_df.rename(columns={"value_time": self.value_time_label})
             return empty_df
 
         # Convert values to numbers
-        dfs.loc[:, "value"] = pd.to_numeric(dfs["value"], downcast="float")
+        dfs["value"] = pd.to_numeric(dfs["value"], downcast="float")
 
         # Convert all times to UTC
         dfs[self.value_time_label] = pd.to_datetime(
-            dfs["dateTime"], utc=True, infer_datetime_format=True
-        ).dt.tz_localize(None)
+            dfs["dateTime"], utc=True).dt.tz_localize(None)
 
         # Simplify variable name
         dfs["variable_name"] = dfs["variableName"].apply(self.simplify_variable_name)
 
         # Sort DataFrame
         dfs = dfs.sort_values(
             ["usgs_site_code", "measurement_unit", self.value_time_label], ignore_index=True
@@ -300,36 +304,55 @@
 
         # Convert categories
         cols = [
             "variable_name",
             "usgs_site_code",
             "measurement_unit",
             "qualifiers",
-            "series",
+            "series"
         ]
+        if include_expanded_metadata:
+            expanded_columns = [
+                "siteTypeCd",
+                "hucCd",
+                "countyCd",
+                "stateCd",
+                "siteName",
+                "srs"
+                ]
+            cols += expanded_columns
         dfs[cols] = dfs[cols].astype(str)
         dfs[cols] = dfs[cols].astype(dtype="category")
 
         # Downcast floats
         df_float = dfs.select_dtypes(include=["float"])
         converted_float = df_float.apply(pd.to_numeric, downcast="float")
         dfs[converted_float.columns] = converted_float
 
         # DataFrame in semi-WRES compatible format
-        return dfs[
-            [
-                self.value_time_label,
-                "variable_name",
-                "usgs_site_code",
-                "measurement_unit",
-                "value",
-                "qualifiers",
-                "series",
-            ]
+        output_columns = [
+            self.value_time_label,
+            "variable_name",
+            "usgs_site_code",
+            "measurement_unit",
+            "value",
+            "qualifiers",
+            "series",
         ]
+        if include_expanded_metadata:
+            expanded_column_mapping = {
+                "siteTypeCd": "site_type_code",
+                "hucCd": "huc_code",
+                "countyCd": "county_code",
+                "stateCd": "state_code",
+                "siteName": "site_name"
+                }
+            dfs = dfs.rename(columns=expanded_column_mapping)
+            output_columns += list(expanded_column_mapping.values()) + ["latitude", "longitude"]
+        return dfs[output_columns]
 
     def get_raw(
         self,
         sites: Union[
             str,
             List[str],
             np.ndarray,
@@ -364,14 +387,15 @@
             np.datetime64,
             pd.Timestamp,
             None,
         ] = None,
         period: Union[str, None] = None,
         siteStatus: str = "all",
         max_sites_per_request: int = 20,
+        include_expanded_metadata: bool = False,
         **params,
     ) -> List[aiohttp.ClientResponse]:
         """
         Return raw requests data from the NWIS IV Rest API in a list.
         See `IVDataService.get` for argument documentation.
         """
         # handle start, end, and period parameters
@@ -442,15 +466,16 @@
         for query_params_dict in query_params:
             query_params_dict.update(params)
 
         # return query_params
         results = self._restclient.mget(parameters=query_params, headers=self._headers)
 
         # flatten list of lists
-        return [item for r in results for item in self._handle_response(r)]
+        return [item for r in results for item in self._handle_response(r,
+            include_expanded_metadata=include_expanded_metadata)]
 
     def _handle_start_end_period_url_params(
         self, startDT=None, endDT=None, period=None
     ) -> dict:
         """Handle passed date or period ranges, returning valid parameters and
         parameter combinations. Valid parameters are returned as a dictionary with
         parameter name keys (i.e. startDT) and associated validated/transformed
@@ -552,15 +577,18 @@
                 "`endDT`"
             )
             raise KeyError(error_message)
 
         return params
 
     @staticmethod
-    def _handle_response(raw_response: aiohttp.ClientResponse) -> List[dict]:
+    def _handle_response(
+        raw_response: aiohttp.ClientResponse,
+        include_expanded_metadata: bool = False
+        ) -> List[dict]:
         """From a raw response, return a list of extracted sites in dictionary form.
         Relevant dictionary keys are:
 
             "usgs_site_code"
             "variableName"
             "measurement_unit"
             "values"
@@ -589,23 +617,40 @@
                 "variableName": IVDataService.simplify_variable_name(
                     json_time_series["variable"]["variableName"]
                 ),
                 # Add units
                 "measurement_unit": json_time_series["variable"]["unit"]["unitCode"],
             }
 
+        def extract_expanded_metadata(json_time_series):
+            # Add site type code, huc, county, and state codes
+            d = {s["name"]: s["value"] for s in json_time_series["sourceInfo"]["siteProperty"]}
+
+            # Add site name
+            d["siteName"] = json_time_series["sourceInfo"]["siteName"]
+
+            # Add geo coordinates
+            d["srs"] = json_time_series["sourceInfo"]["geoLocation"]["geogLocation"]["srs"]
+            d["latitude"] = json_time_series["sourceInfo"]["geoLocation"]["geogLocation"]["latitude"]
+            d["longitude"] = json_time_series["sourceInfo"]["geoLocation"]["geogLocation"]["longitude"]
+            return d
+
         flattened_data = []
 
         for response_value_timeSeries in deserialized_response["value"]["timeSeries"]:
 
             for indicies, site_data in enumerate(response_value_timeSeries["values"]):
 
                 # Create general site metadata dictionary
                 site_metadata = extract_metadata(response_value_timeSeries)
 
+                # Add expanded metadata
+                if include_expanded_metadata:
+                    site_metadata.update(extract_expanded_metadata(response_value_timeSeries))
+
                 # Add site time series values and its index number
                 site_metadata.update({"values": site_data["value"], "series": indicies})
                 flattened_data.append(site_metadata)
 
         return flattened_data
 
     @staticmethod
```

### Comparing `hydrotools.nwis_client-3.2.1/src/hydrotools.nwis_client.egg-info/PKG-INFO` & `hydrotools.nwis_client-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
-Name: hydrotools.nwis-client
-Version: 3.2.1
+Name: hydrotools.nwis_client
+Version: 3.3.1
 Summary: A convenient interface to the USGS NWIS Instantaneous Values (IV) REST Service API.
 Home-page: https://github.com/NOAA-OWP/hydrotools
 Author: Austin Raney
 Author-email: aaraney@protonmail.com
 License: USDOC
 Project-URL: Documentation, https://noaa-owp.github.io/hydrotools/hydrotools.nwis_client.html
 Project-URL: Source, https://github.com/NOAA-OWP/hydrotools/tree/main/python/nwis_client
 Project-URL: Tracker, https://github.com/NOAA-OWP/hydrotools/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free To Use But Restricted
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -168,9 +167,7 @@
 2021-05-31 23:35:00,gage height,02146470,ft,3.14,['A'],0
 2021-05-31 23:40:00,gage height,02146470,ft,3.14,['A'],0
 2021-05-31 23:45:00,gage height,02146470,ft,3.14,['A'],0
 2021-05-31 23:50:00,gage height,02146470,ft,3.14,['A'],0
 2021-05-31 23:55:00,gage height,02146470,ft,3.14,['A'],0
 2021-06-01 00:00:00,gage height,02146470,ft,3.14,['A'],0
 ```
-
-
```

### Comparing `hydrotools.nwis_client-3.2.1/src/hydrotools.nwis_client.egg-info/SOURCES.txt` & `hydrotools.nwis_client-3.3.1/src/hydrotools.nwis_client.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,11 @@
 src/hydrotools.nwis_client.egg-info/entry_points.txt
 src/hydrotools.nwis_client.egg-info/requires.txt
 src/hydrotools.nwis_client.egg-info/top_level.txt
 src/hydrotools/nwis_client/__init__.py
 src/hydrotools/nwis_client/_utilities.py
 src/hydrotools/nwis_client/_version.py
 src/hydrotools/nwis_client/cli.py
-src/hydrotools/nwis_client/iv.py
+src/hydrotools/nwis_client/iv.py
+tests/test__utilities.py
+tests/test_client_cli.py
+tests/test_nwis.py
```

