# Comparing `tmp/parquet_datastore_utils-0.1.0-py3-none-any.whl.zip` & `tmp/parquet_datastore_utils-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3906 bytes, number of entries: 6
+Zip file size: 3999 bytes, number of entries: 6
 -rw-r--r--  2.0 fat       37 b- defN 80-Jan-01 00:00 parquet_datastore_utils/__init__.py
 -rw-r--r--  2.0 fat      570 b- defN 80-Jan-01 00:00 parquet_datastore_utils/cleaner.py
--rw-r--r--  2.0 fat     5526 b- defN 80-Jan-01 00:00 parquet_datastore_utils/read_write.py
--rw-r--r--  2.0 fat      419 b- defN 80-Jan-01 00:00 parquet_datastore_utils-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 parquet_datastore_utils-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 fat      527 b- defN 16-Jan-01 00:00 parquet_datastore_utils-0.1.0.dist-info/RECORD
-6 files, 7167 bytes uncompressed, 2938 bytes compressed:  59.0%
+-rw-r--r--  2.0 fat     5837 b- defN 80-Jan-01 00:00 parquet_datastore_utils/read_write.py
+-rw-r--r--  2.0 fat      419 b- defN 80-Jan-01 00:00 parquet_datastore_utils-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 parquet_datastore_utils-0.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 fat      527 b- defN 16-Jan-01 00:00 parquet_datastore_utils-0.1.1.dist-info/RECORD
+6 files, 7478 bytes uncompressed, 3031 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: parquet_datastore_utils/cleaner.py
 Comment: 
 
 Filename: parquet_datastore_utils/read_write.py
 Comment: 
 
-Filename: parquet_datastore_utils-0.1.0.dist-info/METADATA
+Filename: parquet_datastore_utils-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: parquet_datastore_utils-0.1.0.dist-info/WHEEL
+Filename: parquet_datastore_utils-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: parquet_datastore_utils-0.1.0.dist-info/RECORD
+Filename: parquet_datastore_utils-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## parquet_datastore_utils/read_write.py

```diff
@@ -1,28 +1,40 @@
 import pyarrow as pa
 import pyarrow.parquet as pq
 import pyarrow.dataset as ds
 import pandas as pd
 import os
 import fsspec
 from fsspec.parquet import open_parquet_file
+import numpy as np
 import datetime
 import pyarrow.compute as pc
 
 from parquet_datastore_utils.cleaner import delete_all_except_newest
 
 
 def get_merged_schema(dataset, schema=None):
     if schema is None:
         schema = dataset.schema
     for p in dataset.get_fragments():
         schema = pa.unify_schemas([schema, p.scanner().dataset_schema])
     return schema
 
 
+def _create_schema(types_dict):
+    schema = []
+    for key, val in types_dict.items():
+        if val in (datetime.datetime, np.datetime64, pd.core.dtypes.dtypes.DatetimeTZDtype):
+            schema.append((key, pa.TimestampType))
+        else:
+            schema.append((key, pa.from_numpy_dtype(val)))
+
+    return pa.schema(schema)
+
+
 def read(uri: str, columns: list = None, types_dict: dict = None, merge_schemas: bool = None, **kwargs):
     """
     Reads a parquet dataset and returns a pandas dataframe. Optionally performing a schema merge to allow for schema
     evolution. Note that schema merges can be expensive, specifying an explicit schema with the `schema` kwarg or
     `types_dict` is likely to improve performance in the case that the column(s) you want have been added after initial
     dataset creation.
 
@@ -47,15 +59,15 @@
 
     Returns
     -------
     pandas.Dataframe
     """
 
     if types_dict is not None:
-        kwargs['schema'] = pa.schema([(key, pa.from_numpy_dtype(value)) for key, value in types_dict.items()])
+        kwargs['schema'] = _create_schema(types_dict)
 
     if merge_schemas is True:
         dataset = ds.dataset(uri)
         kwargs['schema'] = get_merged_schema(dataset, kwargs.get('schema'))
 
     try:
         return pd.read_parquet(uri, columns=columns, **kwargs)
```

## Comparing `parquet_datastore_utils-0.1.0.dist-info/RECORD` & `parquet_datastore_utils-0.1.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 parquet_datastore_utils/__init__.py,sha256=XxoVYuFy3yGwKLNGU2tMsNEzP4gvKgE_cQmzcjmzthY,37
 parquet_datastore_utils/cleaner.py,sha256=nBjY8IYPN9hGTUbgwVsi0iCb3EC42dE6HRojcfHfZdg,570
-parquet_datastore_utils/read_write.py,sha256=K5byBQS4-HrpZOK7lDoPFOO1x3-fdcsa-l3rW7DJUnc,5526
-parquet_datastore_utils-0.1.0.dist-info/METADATA,sha256=ZtztzhT28-qMh4DogkSAnDTKRj0GLSgqhFL98h-i9JM,419
-parquet_datastore_utils-0.1.0.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-parquet_datastore_utils-0.1.0.dist-info/RECORD,,
+parquet_datastore_utils/read_write.py,sha256=n9hT5Gn1GbzIoCeXDnJWZpVef1amh58Jn9QloYM8AFc,5837
+parquet_datastore_utils-0.1.1.dist-info/METADATA,sha256=XE_EUqHZdObGLQcjk1EkcEM5-AbSy4nDtng-edyswi0,419
+parquet_datastore_utils-0.1.1.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+parquet_datastore_utils-0.1.1.dist-info/RECORD,,
```

