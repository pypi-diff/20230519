# Comparing `tmp/intake_dataframe_catalog-0.2.0.tar.gz` & `tmp/intake_dataframe_catalog-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake_dataframe_catalog-0.2.0.tar", last modified: Wed May 17 05:20:44 2023, max compression
+gzip compressed data, was "intake_dataframe_catalog-0.2.1.tar", last modified: Fri May 19 05:59:52 2023, max compression
```

## Comparing `intake_dataframe_catalog-0.2.0.tar` & `intake_dataframe_catalog-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:20:44.765790 intake_dataframe_catalog-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 05:20:28.000000 intake_dataframe_catalog-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-17 05:20:44.765790 intake_dataframe_catalog-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-17 05:20:28.000000 intake_dataframe_catalog-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-17 05:20:28.000000 intake_dataframe_catalog-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 05:20:44.765790 intake_dataframe_catalog-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-17 05:20:28.000000 intake_dataframe_catalog-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:20:44.761790 intake_dataframe_catalog-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:20:44.765790 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-17 05:20:28.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-17 05:20:28.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-17 05:20:44.765790 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    20958 2023-05-17 05:20:28.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:20:44.765790 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-17 05:20:44.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-17 05:20:44.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 05:20:44.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 05:20:44.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 05:20:44.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 05:20:44.000000 intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:20:44.765790 intake_dataframe_catalog-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21350 2023-05-17 05:20:29.000000 intake_dataframe_catalog-0.2.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-17 05:20:29.000000 intake_dataframe_catalog-0.2.0/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-17 05:20:29.000000 intake_dataframe_catalog-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:59:52.462027 intake_dataframe_catalog-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 05:59:37.000000 intake_dataframe_catalog-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-19 05:59:52.462027 intake_dataframe_catalog-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-19 05:59:37.000000 intake_dataframe_catalog-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-19 05:59:37.000000 intake_dataframe_catalog-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 05:59:52.462027 intake_dataframe_catalog-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-19 05:59:37.000000 intake_dataframe_catalog-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:59:52.462027 intake_dataframe_catalog-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:59:52.462027 intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-19 05:59:37.000000 intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-19 05:59:37.000000 intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-19 05:59:52.462027 intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23720 2023-05-19 05:59:37.000000 intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:59:52.462027 intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-19 05:59:52.000000 intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-19 05:59:52.000000 intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 05:59:52.000000 intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-19 05:59:52.000000 intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 05:59:52.000000 intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 05:59:52.000000 intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:59:52.462027 intake_dataframe_catalog-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23406 2023-05-19 05:59:37.000000 intake_dataframe_catalog-0.2.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-19 05:59:37.000000 intake_dataframe_catalog-0.2.1/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-19 05:59:37.000000 intake_dataframe_catalog-0.2.1/versioneer.py
```

### Comparing `intake_dataframe_catalog-0.2.0/LICENSE` & `intake_dataframe_catalog-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.2.0/PKG-INFO` & `intake_dataframe_catalog-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake_dataframe_catalog
-Version: 0.2.0
+Version: 0.2.1
 Summary: An intake driver for a searchable table of intake sources and associated metadata
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `intake_dataframe_catalog-0.2.0/README.rst` & `intake_dataframe_catalog-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.2.0/pyproject.toml` & `intake_dataframe_catalog-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog/_search.py` & `intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog/_search.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog/core.py` & `intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from intake.catalog import Catalog
 from intake.catalog.local import LocalCatalogEntry
 
 from . import __version__
 from ._search import search
 
 pd.set_option("display.max_colwidth", 200)
-pd.set_option("display.max_rows", 8)
+pd.set_option("display.max_rows", None)
 
 
 class DfFileCatalogError(Exception):
     pass
 
 
 class DfFileCatalog(Catalog):
@@ -96,14 +96,15 @@
                         "in `columns_with_iterables`."
                     )
         self._read_kwargs = read_kwargs
 
         self._entries = {}
         self._df = pd.DataFrame(columns=[self.name_column, self.yaml_column])
         self._df_summary = None
+        self._previous_search_query = None
 
         self._allow_write = False
         self._try_overwrite = False
         if self.mode in ["w", "x"]:
             self._try_overwrite = True
         if self.mode in ["w", "x", "a", "r+"]:
             self._allow_write = True
@@ -178,15 +179,15 @@
         )
 
     def _repr_html_(self) -> str:
         """
         Return an html summary for the dataframe catalog object. Mainly for IPython notebook.
         """
 
-        text = self.df_summary._repr_html_()
+        text = f"<div style='max-height: 300px'>{self.df_summary._repr_html_()}</div>"
 
         return (
             f"<p><strong>{self.name or 'Intake dataframe'} catalog with {len(self)} source(s) across "
             f"{len(self.df)} rows</strong>:</p> {text}"
         )
 
     def _ipython_display_(self):
@@ -390,14 +391,15 @@
             columns_with_iterables=self.columns_with_iterables,
             storage_options=self.storage_options,
             read_kwargs=self._read_kwargs,
             **self._intake_kwargs,
         )
         cat.path = self.path
         cat._df = results
+        cat._previous_search_query = query
 
         return cat
 
     def save(
         self,
         path: str = None,
         **kwargs: dict[str, typing.Any],
@@ -431,20 +433,26 @@
         else:
             raise UnsupportedOperation(
                 f"Cannot save catalog initialised with mode='{self.mode}'"
             )
 
     serialize = save
 
-    def to_source_dict(self, **kwargs: dict[str, typing.Any]) -> dict[str, typing.Any]:
+    def to_source_dict(
+        self, pass_query=False, **kwargs: dict[str, typing.Any]
+    ) -> dict[str, typing.Any]:
         """
         Load dataframe catalog entries into a dictionary of intake sources.
 
         Parameters
         ----------
+        pass_query: boolean, optional
+            If True, blindly pass the most recent query provided to `self.search` on to the `.search` method of the
+            source(s). An exception is thrown if the source does not have a `.search` method, or if a method exists
+            that does not support dictionary queries of the type provided to `self.search`.
         kwargs: dict
             Arguments/user parameters to use for opening the sources. For example, many intake drivers support
             a `storage_options` argument with parameters to be passed to the backend file-system. Note, this function
             passes the same kwargs to all sources in the dataframe catalog. To pass different kwargs to different
             sources, load each source using it's key (name), e.g. `cat["<source_name>"](**kwargs)`.
 
         Returns
@@ -456,35 +464,76 @@
         if not self.keys():
             warnings.warn(
                 "There are no sources to open. Returning an empty dictionary.",
                 UserWarning,
                 stacklevel=2,
             )
 
-        return {key: source(**kwargs) for key, source in self.items()}
+        sources = {key: source(**kwargs) for key, source in self.items()}
 
-    def to_source(self, **kwargs: dict[str, typing.Any]) -> intake.DataSource:
+        if pass_query:
+            if self._previous_search_query:
+                for key, source in sources.items():
+                    try:
+                        source.search(**self._previous_search_query)
+                    except AttributeError:
+                        raise DfFileCatalogError(
+                            f"The source corresponding to key '{key}' ({source.classname}) does not have a "
+                            "`.search` method and so cannot be loaded with `pass_query = True`."
+                        )
+                    except TypeError:
+                        raise DfFileCatalogError(
+                            f"The source corresponding to key '{key}' ({source.classname}) has a `.search` "
+                            "method with a different API than `self.search` and so cannot be loaded with "
+                            "`pass_query = True`."
+                        )
+                    except Exception:
+                        raise DfFileCatalogError(
+                            f"Unable to load the source corresponding to key '{key}' with `pass_query = True`. This "
+                            "is usually because the query includes keys that are not valid for the source. For example, "
+                            "if the source is an intake-esm datastore, its columns may have different names than those "
+                            "in this dataframe catalog. Please set `pass_query = False`."
+                        )
+
+                sources = {
+                    key: source.search(**self._previous_search_query)
+                    for key, source in sources.items()
+                }
+            else:
+                raise DfFileCatalogError(
+                    "No previous queries exist to pass on to source(s)"
+                )
+
+        return sources
+
+    def to_source(
+        self, pass_query=False, **kwargs: dict[str, typing.Any]
+    ) -> intake.DataSource:
         """
         Load intake source. This is only possible if there is only one remaining source in the dataframe
         catalog.
 
         Parameters
         ----------
+        pass_query: boolean, optional
+            If True, blindly pass the most recent query provided to `self.search` on to the `.search` method of the
+            source. An exception is thrown if the source does not have a `.search` method, or if a method exists
+            that does not support dictionary queries of the type provided to `self.search`.
         kwargs: dict
             Arguments/user parameters to use for opening the intake source. For example, many intake drivers support
             a `storage_options` argument with parameters to be passed to the backend file-system.`.
 
         Returns
         -------
         source: :py:class:`intake.DataSource`
             A dictionary of sources.
         """
 
         if len(self) == 1:
-            res = self.to_source_dict(**kwargs)
+            res = self.to_source_dict(pass_query, **kwargs)
             _, source = res.popitem()
             return source
         else:
             raise ValueError(
                 f"Expected exactly one source, received {len(self)}. Please refine your search or use "
                 "`.to_source_dict()`."
             )
```

### Comparing `intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/PKG-INFO` & `intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-dataframe-catalog
-Version: 0.2.0
+Version: 0.2.1
 Summary: An intake driver for a searchable table of intake sources and associated metadata
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `intake_dataframe_catalog-0.2.0/src/intake_dataframe_catalog.egg-info/SOURCES.txt` & `intake_dataframe_catalog-0.2.1/src/intake_dataframe_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.2.0/tests/test_core.py` & `intake_dataframe_catalog-0.2.1/tests/test_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -661,14 +661,66 @@
     assert cat.df_summary.to_dict(orient="split", index=False) == expected_dict
 
     cat.remove("gistemp")
     expected_dict = {"columns": [], "data": []}
     assert cat.df_summary.to_dict(orient="split", index=False) == expected_dict
 
 
+def test_pass_query(catalog_path):
+    """
+    Test the pass_query flag on the to_source* methods
+    """
+    cat = intake.open_df_catalog(
+        path=str(catalog_path / "dfcat.csv"),
+        columns_with_iterables=["variable"],
+        mode="a",
+    )
+
+    # Check error message when there is no .search method on source
+    with pytest.raises(DfFileCatalogError) as excinfo:
+        cat.search(variable="tas").to_source(pass_query=True)
+    assert "does not have a `.search` method" in str(excinfo.value)
+
+    # Check error message when search API is different on source
+    # A dummy catalog with a .search method
+    dummy_cat = intake.catalog.base.Catalog(
+        entries={"dummy": None},
+        name="dummy",
+    )
+    cat.add(dummy_cat, {"realm": "dummy", "variable": ["dummy"]})
+    with pytest.raises(DfFileCatalogError) as excinfo:
+        cat.search(variable="dummy").to_source(pass_query=True)
+    assert "has a `.search` method with a different API" in str(excinfo.value)
+
+    # Check error message when columns in query are not valid for source
+    with pytest.raises(DfFileCatalogError) as excinfo:
+        cat.search(variable="prsn").to_source(pass_query=True)
+    assert (
+        "This is usually because the query includes keys that are not valid for the source"
+        in str(excinfo.value)
+    )
+
+    # Check that it works when it should
+    source = cat.search(variable="hfls").to_source(pass_query=True)
+    assert len(source) == 1
+
+    # Check with multiple entries. Should work on cmip5 and throw error on cmip6
+    with pytest.raises(DfFileCatalogError) as excinfo:
+        cat.search(variable="tasmax").to_source_dict(pass_query=True)
+    assert (
+        "Unable to load the source corresponding to key 'cmip6' with `pass_query = True`"
+        in str(excinfo.value)
+    )
+
+    # Check error message when no previous query has been made
+    with pytest.raises(DfFileCatalogError) as excinfo:
+        cat.to_source_dict(pass_query=True)
+    assert "No previous queries exist to pass on to source(s)" in str(excinfo.value)
+
+
 def test_subclassing_catalog(catalog_path):
     """
     Test subclassing DfFileCatalog
     """
 
     class ChildCatalog(DfFileCatalog):
         pass
```

### Comparing `intake_dataframe_catalog-0.2.0/tests/test_search.py` & `intake_dataframe_catalog-0.2.1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.2.0/versioneer.py` & `intake_dataframe_catalog-0.2.1/versioneer.py`

 * *Files identical despite different names*

