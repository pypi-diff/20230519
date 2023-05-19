# Comparing `tmp/gordo_core-0.3.0rc0-py3-none-any.whl.zip` & `tmp/gordo_core-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,31 @@
-Zip file size: 60901 bytes, number of entries: 26
+Zip file size: 63714 bytes, number of entries: 29
 -rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx       74 b- defN 80-Jan-01 00:00 gordo_core/__init__.py
--rw-r--r--  2.0 unx       84 b- defN 80-Jan-01 00:00 gordo_core/_version.py
--rw-r--r--  2.0 unx     2233 b- defN 80-Jan-01 00:00 gordo_core/back_compatibles.py
--rw-r--r--  2.0 unx     7723 b- defN 80-Jan-01 00:00 gordo_core/base.py
+-rw-r--r--  2.0 unx       81 b- defN 80-Jan-01 00:00 gordo_core/_version.py
+-rw-r--r--  2.0 unx     2438 b- defN 80-Jan-01 00:00 gordo_core/back_compatibles.py
+-rw-r--r--  2.0 unx     7750 b- defN 80-Jan-01 00:00 gordo_core/base.py
 -rw-r--r--  2.0 unx      102 b- defN 80-Jan-01 00:00 gordo_core/data_providers/__init__.py
--rw-r--r--  2.0 unx     5269 b- defN 80-Jan-01 00:00 gordo_core/data_providers/base.py
--rw-r--r--  2.0 unx     1942 b- defN 80-Jan-01 00:00 gordo_core/data_providers/partition.py
--rw-r--r--  2.0 unx     8455 b- defN 80-Jan-01 00:00 gordo_core/data_providers/providers.py
--rw-r--r--  2.0 unx      482 b- defN 80-Jan-01 00:00 gordo_core/data_providers/utils.py
--rw-r--r--  2.0 unx     3617 b- defN 80-Jan-01 00:00 gordo_core/exceptions.py
+-rw-r--r--  2.0 unx     4947 b- defN 80-Jan-01 00:00 gordo_core/data_providers/base.py
+-rw-r--r--  2.0 unx       42 b- defN 80-Jan-01 00:00 gordo_core/data_providers/contrib/__init__.py
+-rw-r--r--  2.0 unx     1981 b- defN 80-Jan-01 00:00 gordo_core/data_providers/contrib/csv_provider.py
+-rw-r--r--  2.0 unx     2296 b- defN 80-Jan-01 00:00 gordo_core/data_providers/partition.py
+-rw-r--r--  2.0 unx     8377 b- defN 80-Jan-01 00:00 gordo_core/data_providers/providers.py
+-rw-r--r--  2.0 unx      616 b- defN 80-Jan-01 00:00 gordo_core/data_providers/utils.py
+-rw-r--r--  2.0 unx      372 b- defN 80-Jan-01 00:00 gordo_core/dist.py
+-rw-r--r--  2.0 unx     4050 b- defN 80-Jan-01 00:00 gordo_core/exceptions.py
 -rw-r--r--  2.0 unx       49 b- defN 80-Jan-01 00:00 gordo_core/file_systems/__init__.py
--rw-r--r--  2.0 unx     1925 b- defN 80-Jan-01 00:00 gordo_core/file_systems/base.py
+-rw-r--r--  2.0 unx     3568 b- defN 80-Jan-01 00:00 gordo_core/file_systems/base.py
 -rw-r--r--  2.0 unx       63 b- defN 80-Jan-01 00:00 gordo_core/filters/__init__.py
--rw-r--r--  2.0 unx     9196 b- defN 80-Jan-01 00:00 gordo_core/filters/periods.py
--rw-r--r--  2.0 unx     9178 b- defN 80-Jan-01 00:00 gordo_core/filters/rows.py
--rw-r--r--  2.0 unx     3800 b- defN 80-Jan-01 00:00 gordo_core/import_utils.py
--rw-r--r--  2.0 unx     2454 b- defN 80-Jan-01 00:00 gordo_core/metadata.py
--rw-r--r--  2.0 unx     9017 b- defN 80-Jan-01 00:00 gordo_core/sensor_tag.py
--rw-r--r--  2.0 unx    30462 b- defN 80-Jan-01 00:00 gordo_core/time_series.py
--rw-r--r--  2.0 unx    13507 b- defN 80-Jan-01 00:00 gordo_core/utils.py
--rw-r--r--  2.0 unx     3834 b- defN 80-Jan-01 00:00 gordo_core/validators.py
--rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 gordo_core-0.3.0rc0.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 gordo_core-0.3.0rc0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2147 b- defN 16-Jan-01 00:00 gordo_core-0.3.0rc0.dist-info/METADATA
-?rw-r--r--  2.0 unx     2160 b- defN 16-Jan-01 00:00 gordo_core-0.3.0rc0.dist-info/RECORD
-26 files, 186907 bytes uncompressed, 57423 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx     9280 b- defN 80-Jan-01 00:00 gordo_core/filters/periods.py
+-rw-r--r--  2.0 unx     9352 b- defN 80-Jan-01 00:00 gordo_core/filters/rows.py
+-rw-r--r--  2.0 unx     4016 b- defN 80-Jan-01 00:00 gordo_core/import_utils.py
+-rw-r--r--  2.0 unx     2514 b- defN 80-Jan-01 00:00 gordo_core/metadata.py
+-rw-r--r--  2.0 unx     9046 b- defN 80-Jan-01 00:00 gordo_core/sensor_tag.py
+-rw-r--r--  2.0 unx    30150 b- defN 80-Jan-01 00:00 gordo_core/time_series.py
+-rw-r--r--  2.0 unx    13406 b- defN 80-Jan-01 00:00 gordo_core/utils.py
+-rw-r--r--  2.0 unx     3910 b- defN 80-Jan-01 00:00 gordo_core/validators.py
+-rw-r--r--  2.0 unx    34523 b- defN 80-Jan-01 00:00 gordo_core-0.3.1.dist-info/LICENSE
+?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 gordo_core-0.3.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2446 b- defN 16-Jan-01 00:00 gordo_core-0.3.1.dist-info/METADATA
+?rw-r--r--  2.0 unx     2428 b- defN 16-Jan-01 00:00 gordo_core-0.3.1.dist-info/RECORD
+29 files, 192488 bytes uncompressed, 59808 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -15,23 +15,32 @@
 
 Filename: gordo_core/data_providers/__init__.py
 Comment: 
 
 Filename: gordo_core/data_providers/base.py
 Comment: 
 
+Filename: gordo_core/data_providers/contrib/__init__.py
+Comment: 
+
+Filename: gordo_core/data_providers/contrib/csv_provider.py
+Comment: 
+
 Filename: gordo_core/data_providers/partition.py
 Comment: 
 
 Filename: gordo_core/data_providers/providers.py
 Comment: 
 
 Filename: gordo_core/data_providers/utils.py
 Comment: 
 
+Filename: gordo_core/dist.py
+Comment: 
+
 Filename: gordo_core/exceptions.py
 Comment: 
 
 Filename: gordo_core/file_systems/__init__.py
 Comment: 
 
 Filename: gordo_core/file_systems/base.py
@@ -60,20 +69,20 @@
 
 Filename: gordo_core/utils.py
 Comment: 
 
 Filename: gordo_core/validators.py
 Comment: 
 
-Filename: gordo_core-0.3.0rc0.dist-info/LICENSE
+Filename: gordo_core-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: gordo_core-0.3.0rc0.dist-info/WHEEL
+Filename: gordo_core-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: gordo_core-0.3.0rc0.dist-info/METADATA
+Filename: gordo_core-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: gordo_core-0.3.0rc0.dist-info/RECORD
+Filename: gordo_core-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gordo_core/_version.py

```diff
@@ -1,3 +1,3 @@
 # coding: utf-8
 # file generated by scripts/prepare_version.sh
-version = "0.3.0rc0"
+version = "0.3.1"
```

## gordo_core/back_compatibles.py

```diff
@@ -62,7 +62,11 @@
         "gordo_core.data_providers.providers.InfluxDataProvider",
     ),
 ]
 
 DEFAULT_BACK_COMPATIBLES: Final[
     BackCompatibleLocations
 ] = prepare_back_compatible_locations(BACK_COMPATIBLE_LOCATIONS)
+"""
+This constant have to be used as default value for ``back_compatibles`` argument for :func:`gordo_core.import_utils.import_location`.
+Most of these paths are temporary and will be deprecated soon.
+"""
```

## gordo_core/base.py

```diff
@@ -18,26 +18,26 @@
 logger = logging.getLogger(__name__)
 
 
 def import_dataset(
     location: str, *, back_compatibles: Optional[BackCompatibleLocations] = None
 ):
     """
-    Import `GordoBaseDataset` class.
+    Import :class:`gordo_core.base.GordoBaseDataset` class.
 
     Parameters
     ----------
-    location: str
+    location
         Class import location.
-    back_compatibles: Optional[BackCompatibleLocations]
-        See `gordo_core.import_utils.prepare_back_compatible_locations()` function for reference.
+    back_compatibles
+        See :func:`gordo_core.import_utils.prepare_back_compatible_locations` function for reference.
 
     Returns
     -------
-        `GordoBaseDataset` class.
+        Class with :class:`gordo_core.base.GordoBaseDataset` interface implemented.
 
     """
     if not location:
         location = "TimeSeriesDataset"
     if back_compatibles is None:
         back_compatibles = DEFAULT_BACK_COMPATIBLES
     try:
@@ -60,30 +60,30 @@
     dataset_cls: Type["DatasetWithProvider"],
     config: dict[str, Any],
     *,
     back_compatibles: Optional[BackCompatibleLocations] = None,
     default_data_provider: Optional[str] = None,
 ):
     """
-    Instantiate `DatasetWithProvider`. Call `DatasetWithProvider.with_data_provider()` under the hood.
+    Instantiate :class:`.DatasetWithProvider`. Call :func:`DatasetWithProvider.with_data_provider` under the hood.
 
     Parameters
     ----------
-    dataset_cls: Type["DatasetWithProvider"]
-        `DatasetWithProvider` class.
-    config: dict[str, Any]
+    dataset_cls
+        :class:`.DatasetWithProvider` class.
+    config
         Dataset arguments.
-    back_compatibles: Optional[BackCompatibleLocations]
-        See `gordo_core.import_utils.prepare_back_compatible_locations()` function for reference.
-    default_data_provider: Optional[str]
-        Default data provider type. Will be taken if `data_provider.type` is empty.
+    back_compatibles
+        See :func:`gordo_core.import_utils.prepare_back_compatible_locations` function for reference.
+    default_data_provider
+        Default data provider type. Will be taken if ``data_provider.type`` is empty.
 
     Returns
     -------
-        `DatasetWithProvider` instance.
+        :class:`.DatasetWithProvider` instance.
 
     """
     args = copy.copy(config)
     data_provider = args.pop("data_provider", None)
     if isinstance(data_provider, dict):
         provider_type = data_provider.get("type")
         if not provider_type:
@@ -108,21 +108,21 @@
     default_data_provider: Optional[str] = None,
 ) -> "GordoBaseDataset":
     """
     Create GordoBaseDataset instance.
 
     Parameters
     ----------
-    dataset_cls: Type[GordoBaseDataset]
+    dataset_cls
         Dataset class.
-    args: dict[str, Any]
-        __init__ arguments.
-    back_compatibles: Optional[BackCompatibleLocations]
-        See `gordo_core.import_utils.prepare_back_compatible_locations()` function for reference.
-    default_data_provider: Optional[str]
+    args
+        ``__init__`` arguments.
+    back_compatibles
+        See :func:`gordo_core.import_utils.prepare_back_compatible_locations` function for reference.
+    default_data_provider
         Default data provider type. Will be taken if `data_provider.type` is empty.
 
     Returns
     -------
     """
     if issubclass(dataset_cls, DatasetWithProvider):
         return create_with_provider(
@@ -160,35 +160,34 @@
     def get_client_data(
         self, build_dataset_metadata: dict
     ) -> Tuple[
         Union[np.ndarray, pd.DataFrame, xr.DataArray],
         Union[np.ndarray, pd.DataFrame, xr.DataArray],
     ]:
         """
-        The version of `get_data` used by gordo-client
+        The version of :func:`~GordoBaseDataset.get_data` used by gordo-client
 
         Parameters
         ----------
-        build_dataset_metadata: dict
-            build_metadata.dataset part of the metadata
+        build_dataset_metadata
+            ``build_metadata.dataset`` part of the metadata
 
         Returns
         -------
 
         """
         return self.get_data()
 
     def to_dict(self) -> dict:
         """
         Serialize this object into a dict representation, which can be used to
         initialize a new object using :func:`~GordoBaseDataset.from_dict`
 
         Returns
         -------
-        dict
         """
         if not hasattr(self, "_params"):
             raise AttributeError(
                 "Failed to lookup init parameters, ensure the "
                 "object's __init__ is decorated with 'capture_args'"
             )
         # Update dict with the class
@@ -217,22 +216,26 @@
         return create_dataset(
             dataset_cls,
             args,
             back_compatibles=back_compatibles,
             default_data_provider=default_data_provider,
         )
 
-    def get_metadata(self):
+    def get_metadata(self) -> dict:
         """
         Get metadata about the current state of the dataset
         """
         return dict()
 
 
 class DatasetWithProvider(GordoBaseDataset, metaclass=ABCMeta):
+    """
+    This class have to be used if you want to use :class:`.GordoBaseDataset` with ``DataProvider``
+    """
+
     @classmethod
     @abstractmethod
     def with_data_provider(
         cls,
         data_provider: Optional[Union[dict[str, Any], GordoBaseDataProvider]],
         args: dict[str, Any],
         *,
```

## gordo_core/data_providers/base.py

```diff
@@ -25,61 +25,44 @@
         train_end_date: datetime,
         tag_list: list[Tag],
         dry_run: Optional[bool] = False,
         **kwargs,
     ) -> Iterable[Tuple[pd.Series, Tag]]:
         """
         Load the required data as an iterable of series where each
-        contains the values of the tag with time index
+        contains the values of the tag with time index.
 
         Parameters
         ----------
-        train_start_date: datetime
+        train_start_date
             Datetime object representing the start of fetching data
-        train_end_date: datetime
+        train_end_date
             Datetime object representing the end of fetching data
-        tag_list: list[Tag]
+        tag_list
             List of tags to fetch, where each will end up being its own dataframe
-        dry_run: Optional[bool]
+        dry_run
             Set to true to perform a "dry run" of the loading.
             Up to the implementations to determine what that means.
-        kwargs: dict
-            With these - additional data might be passed by data_provider.
-
-        Returns
-        -------
-        Iterable[Tuple[pd.Series, SensorTag]]
+        kwargs
+            With these - additional data might be passed by ``data_provider``.
         """
         ...
 
     @abc.abstractmethod
     def can_handle_tag(self, tag: Tag):
         """
         Returns true if the dataprovider thinks it can possibly read this tag.
         Typically checks if the asset part of the tag is known to the reader.
-
-        Parameters
-        ----------
-        tag: SensorTag - Dictionary with a "tag" key and optional "asset"
-
-        Returns
-        -------
-        bool
-
         """
         ...
 
     def to_dict(self):
         """
         Serialize this object into a dict representation, which can be used to
-        initialize a new object after popping 'type' from the dict.
-
-        Returns
-        -------
-        dict
+        initialize a new object after popping ``type`` from the dict.
         """
         if not hasattr(self, "_params"):
             raise AttributeError(
                 "Failed to lookup init parameters, ensure the "
                 "object's __init__ is decorated with 'capture_args'"
             )
         # Update dict with the class
@@ -130,32 +113,32 @@
 
     def get_closest_datapoint(
         self, tag: Tag, before_time: datetime, point_max_look_back: pd.Timedelta
     ) -> Optional[pd.Series]:
         """
         Latest data point of tag from some time in the past till before_time, None if nothing found.
         This function is optional for implementing in the child classes,
-        if it's not implemented NotImplementedError will be thrown.
+        if it's not implemented :exc:`NotImplementedError` will be thrown.
         """
         raise NotImplementedError()
 
     def get_metadata(self):
         """
-        Get metadata about the current state of the data provider
+        Get metadata about the current state of the data provider.
         """
         return dict()
 
     def tag_normalizer(
         self,
         sensors: list[Sensor],
         **kwargs: Optional[str],
     ) -> list[Tag]:
         """
         Prepare and validate sensors list.
-        This function might be useful for overwriting in the extended class
+        This function might be useful for overwriting in the extended class.
         """
         tag_list = [
             normalize_sensor_tag(sensor, self.tags_required_fields, **kwargs)
             for sensor in sensors
         ]
         unique_tag_names(tag_list)
         return tag_list
```

## gordo_core/data_providers/partition.py

```diff
@@ -1,7 +1,11 @@
+"""
+ .. todo::
+    Move module :mod:`gordo_core.data_providers.partition` to ``gordo_core.partition``
+"""
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from typing import Iterable, Optional, Union
 
 
 @dataclass(frozen=True)
@@ -41,14 +45,26 @@
                 return enum
         return None
 
 
 def split_by_partitions(
     partition_by: PartitionBy, start_period: datetime, end_period: datetime
 ) -> Iterable[Partition]:
+    """
+    Split time span by partitions
+
+    Parameters
+    ----------
+    partition_by
+        Partition chunks size, either year or month.
+    start_period
+        First date of time span.
+    end_period
+        Last date of time span.
+    """
     if start_period > end_period:
         message = "start_period bigger then end_period."
         message += "'%s' > '%s'" % (start_period.isoformat(), end_period.isoformat())
         raise ValueError(message)
     if partition_by is PartitionBy.YEAR:
         for year in range(start_period.year, end_period.year + 1):
             yield YearPartition(year)
```

## gordo_core/data_providers/providers.py

```diff
@@ -32,26 +32,26 @@
         client: Optional[DataFrameClient] = None,
         uri: Optional[str] = None,
         **kwargs,
     ):
         """
         Parameters
         ----------
-        measurement: str
+        measurement
             Name of the measurement to select from in Influx
-        value_name: str
+        value_name
             Name of value to select, default to 'Value'
-        api_key: str
+        api_key
             Api key to use in header
-        api_key_header: str
+        api_key_header
             Key of header to insert the api key for requests
-        uri: str
+        uri
             Create a client from a URI
-            format: <username>:<password>@<host>:<port>/<optional-path>/<db_name>
-        kwargs: dict
+            format: ``<username>:<password>@<host>:<port>/<optional-path>/<db_name>``
+        kwargs
             These are passed directly to the init args of influxdb.DataFrameClient
         """
         self.measurement = measurement
         self.value_name = value_name
         influx_client = client
         if kwargs.pop("threads", None):
             logger.warning(
@@ -91,15 +91,15 @@
         train_start_date: datetime,
         train_end_date: datetime,
         tag_list: list[Tag],
         dry_run: Optional[bool] = False,
         **kwargs,
     ) -> Iterable[Tuple[pd.Series, Tag]]:
         """
-        See GordoBaseDataProvider for documentation
+        See :class:`~GordoBaseDataProvider` for documentation
         """
         if dry_run:
             raise NotImplementedError(
                 "Dry run for InfluxDataProvider is not implemented"
             )
         # TODO better way to handle SensorTag here
         return (
@@ -129,17 +129,14 @@
                 Datetime to start querying for data
             train_end_date: datetime
                 Datetime to stop query for data
             tag: str
                 Name of the tag to match in influx
             measurement: str
                 name of the measurement to select from
-        Returns
-        -------
-            One column DataFrame
         """
 
         logger.info(f"Reading tag: {tag}")
         logger.info(f"Fetching data from {train_start_date} to {train_end_date}")
         query_string = f"""
             SELECT "{self.value_name}" as "{tag}"
             FROM "{measurement}"
@@ -172,32 +169,30 @@
             list_of_tags.append(item["value"])
         return list_of_tags
 
     @cached(cache=TTLCache(maxsize=10, ttl=600))
     def get_list_of_tags(self) -> list[str]:
         """
         Queries Influx for the list of tags, using a TTL cache of 600 seconds. The
-        cache can be cleared with :func:`cache_clear()` as is usual with cachetools.
+        cache can be cleared with ``provider.get_list_of_tags.cache_clear()`` as is usual with cachetools.
 
         Returns
         -------
-        typing.list[str]
             The list of tags in Influx
-
         """
         return self._list_of_tags_from_influx()
 
     def can_handle_tag(self, tag: Tag):
         tag_name = extract_tag_name(tag)
         return tag_name in self.get_list_of_tags()
 
 
 class RandomDataProvider(GordoBaseDataProvider):
     """
-    Get a GordoBaseDataset which returns unstructed values for X and y. Each instance
+    Get :class:`~GordoBaseDataset` which returns unstructed values for X and y. Each instance
     uses the same seed, so should be a function (same input -> same output)
     """
 
     def can_handle_tag(self, tag: Tag):
         return True  # We can be random about everything
 
     @capture_args
```

## gordo_core/data_providers/utils.py

```diff
@@ -1,17 +1,25 @@
 from typing import Iterable, Tuple
 from urllib.parse import quote
 
 from gordo_core.file_systems import FileSystem
 
 
 def partition_dir_name(field: str, value: str):
+    """
+    .. deprecated:: 0.3.0
+        Will be removed.
+    """
     return field + "=" + quote(value, safe=" ")
 
 
 def build_dir_path(
     storage: FileSystem, base_dir: str, field_values: Iterable[Tuple[str, str]]
 ) -> str:
+    """
+    .. deprecated:: 0.3.0
+        Will be removed.
+    """
     dir_path = base_dir
     for field, value in field_values:
         dir_path = storage.join(dir_path, partition_dir_name(field, value))
     return dir_path
```

## gordo_core/exceptions.py

```diff
@@ -1,7 +1,20 @@
+"""
+This module defines the following exception hierarchy:
+
+* :exc:`ValueError`
+    * :exc:`InsufficientDataError`
+        * :exc:`EmptyDataframeError`
+            * :exc:`EmptyGeneratedDataframeError`
+            * :exc:`EmptyFilteredDataframeError`
+                * :exc:`RowFilterEmptyDataError`
+                * :exc:`KnownPeriodsEmptyDataError`
+                * :exc:`NuisanceEmptyDataError`
+    * :exc:`ConfigException`
+"""
 from typing import Optional, Union
 
 
 class InsufficientDataError(ValueError):
     """Generic error raised if the data is not enough to process."""
```

## gordo_core/file_systems/base.py

```diff
@@ -3,25 +3,45 @@
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from typing import IO, Iterable, Optional, Tuple
 
 
 class FileType(Enum):
+    """
+    Type of file system item.
+    """
+
     DIRECTORY = 1
     FILE = 2
 
 
 @dataclass(frozen=True)
 class FileInfo:
+    """
+    File/directory information.
+    """
+
     file_type: FileType
     size: int
+    """
+    Size of the file.
+    """
     access_time: Optional[datetime] = None
+    """
+    Time of last access.
+    """
     modify_time: Optional[datetime] = None
+    """
+    Time of last modification.
+    """
     create_time: Optional[datetime] = None
+    """
+    Time of creation.
+    """
 
     def isfile(self) -> bool:
         return self.file_type == FileType.FILE
 
     def isdir(self) -> bool:
         return self.file_type == FileType.DIRECTORY
 
@@ -31,62 +51,113 @@
         p = p[:-1]
     if not p:
         return ""
     return posixpath.join(*p)
 
 
 class FileSystem(metaclass=ABCMeta):
+    """
+    An interface for file system implementations.
+    """
+
     @property
     @abstractmethod
     def name(self) -> str:
+        """
+        Unique name for this file system. Example: ``S3://mybucket/home``
+        """
         ...
 
     @abstractmethod
     def open(self, path: str, mode: str = "r") -> IO:
         """
-        Open a file
+        Open a file. :func:`open` analog for this file system.
 
         Parameters
         ----------
         path
             Path to the file
         mode
             Required support at least of `r`,`b` modes
-        Returns
-        -------
-        IOBase
         """
         ...
 
     @abstractmethod
     def exists(self, path: str) -> bool:
+        """
+        Tests whether a path exists.
+        """
         ...
 
     @abstractmethod
     def isfile(self, path: str) -> bool:
+        """
+        Tests whether a path is a regular file.
+        """
         ...
 
     @abstractmethod
     def isdir(self, path: str) -> bool:
+        """
+        Returns true if ``path`` refers to an existing directory.
+        """
         ...
 
     @abstractmethod
     def info(self, path: str) -> FileInfo:
+        """
+        Retrieves :class:`.FileInfo` of a path.
+        """
         ...
 
     @abstractmethod
     def ls(
         self, path: str, with_info: bool = True
     ) -> Iterable[Tuple[str, Optional[FileInfo]]]:
+        """
+        Returns a list containing the names of the files in the directory.
+
+        Parameters
+        ----------
+        path
+            Directory path.
+        with_info
+            Retrieves :class:`.FileInfo` for each item. Otherwise, will be ``None`` for all items.
+        """
         ...
 
     @abstractmethod
     def walk(
         self, base_path: str, with_info: bool = True
     ) -> Iterable[Tuple[str, Optional[FileInfo]]]:
+        """
+        Directory tree recursive iterator.
+
+        Parameters
+        ----------
+        base_path
+            Directory path.
+        with_info
+            :class:`~FileSystem.ls` ``with_info`` argument analog.
+
+        Returns
+        -------
+        The first item of ``tuple`` is a path directory tree item, the second is :class:`.FileInfo` if ``with_info=True``
+        """
         ...
 
     def join(self, *p) -> str:
+        """
+        Join two or more pathname components, specific for this file system.
+
+        Parameters
+        ----------
+        p
+            Path components list.
+        """
         return default_join(*p)
 
-    def split(self, p) -> Tuple[str, str]:
+    def split(self, p: str) -> Tuple[str, str]:
+        """
+        Split a pathname.
+        """
         return posixpath.split(p)
```

## gordo_core/filters/periods.py

```diff
@@ -1,10 +1,9 @@
 import logging
 from pprint import pformat
-from typing import Optional
 
 import pandas as pd
 from sklearn.ensemble import IsolationForest
 from sklearn.preprocessing import MinMaxScaler
 
 from .rows import pandas_filter_rows
 
@@ -12,67 +11,67 @@
 
 
 class WrongFilterMethodType(TypeError):
     pass
 
 
 class FilterPeriods:
-    """Model class with methods for data pre-processing.
-    Performs a series of algorithms that drops noisy data.
-
-    Either a rolling median or an isolation forest algorithm is executed.
-    Both provide drop periods in a dict-type element on the class object
-    `object.drop_periods["iforest"]` and `object.drop_periods["median"]`,
-    and data is filtered accordingly.
-
-    Parameters:
-    data: pandas.DataFrame
-        Data frame containing already filtered data (global max/min + dropped known periods).
-        Time consecutively is not required.
-    granularity: str
-        The bucket size for grouping all incoming time data (e.g. "10T").
-        Available strings come from https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#dateoffset-objects
-    **kwargs:
-        See below.
-
-    Keyword arguments:
-    filter_method: str
-        Which method should be used for data cleaning, either "median" (default), "iforest" or "all" which returns
-        results for both methods.
-    iforest_smooth: bool
-        If exponential weighted smoothing should be applied to data before isolation forest
-        algorithm is run.
-    """
+    """Model class with methods for data pre-processing."""
 
     def __init__(
         self,
         granularity: str = "10T",
         filter_method: str = "median",
-        window=144,
-        n_iqr=5,
-        iforest_smooth=False,
-        contamination=0.03,
-        quantile_lower=0.05,
-        quantile_upper=0.95,
+        window: int = 144,
+        n_iqr: int = 5,
+        iforest_smooth: bool = False,
+        contamination: float = 0.03,
+        quantile_lower: float = 0.05,
+        quantile_upper: float = 0.95,
     ):
+        """
+        Performs a series of algorithms that drops noisy data.
+
+        Either a rolling median or an isolation forest algorithm is executed.
+        Both provide drop periods in a dict-type element on the class object
+        ``object.drop_periods["iforest"]`` and ``object.drop_periods["median"]``,
+        and data is filtered accordingly.
+
+        Parameters
+        ----------
+        granularity
+            The bucket size for grouping all incoming time data (e.g. "10T").
+            Available strings come from `timeseries <https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#dateoffset-objects>`_.
+        filter_method
+            Which method should be used for data cleaning, either "median" (default), "iforest" or "all" which returns
+            results for both methods.
+        iforest_smooth
+            If exponential weighted smoothing should be applied to data before isolation forest
+            algorithm is run.
+        """
         self.granularity = granularity
         self.filter_method = filter_method
         if self.filter_method not in ["quantile", "median", "iforest", "all"]:
             raise WrongFilterMethodType
         self._window = window
         self._n_iqr = n_iqr
         self._iforest_smooth = iforest_smooth
         self._contamination = contamination
         self._quantile_lower = quantile_lower
         self._quantile_upper = quantile_upper
 
-    def filter_data(self, data):
-        """Method for filtering data.
+    def filter_data(self, data: pd.DataFrame):
+        """
+        Method for filtering data.
         Returns the filtered dataset, a dict containing the different periods that have been dropped arranged
         by filtering method and the actual predictions from the filter model.
+
+        data
+            Data frame containing already filtered data (global max/min + dropped known periods).
+            Time consecutively is not required.
         """
         predictions = {}
         if self.filter_method in ["median", "all"]:
             predictions["median"] = self._rolling_median(data)
 
         if self.filter_method in ["quantile", "all"]:
             predictions["quantile"] = self._quantile_filter(data)
```

## gordo_core/filters/rows.py

```diff
@@ -71,24 +71,42 @@
     escape_str: escape_char for escape_char, escape_str in _escaped_chars
 }
 
 _unescaping_re = re.compile(r"_([A-Z]+)_")
 
 
 def escape_python_identifier(name: str) -> str:
+    """
+    Escapes special symbols such as: ``.``, ``-`` etc., from the python variable identifier.
+
+    Parameters
+    ----------
+    name
+        Python variable name.
+    """
     if name.isidentifier():
         return name
     result_name = "".join(_escaping_chars_dict.get(char, char) for char in name)
     result_name = _escaped_prefix + result_name
     if not result_name.isidentifier():
         raise SyntaxError(f"Can not convert '{name}' to a valid Python identifier.")
     return result_name
 
 
 def unescape_python_identifier(name: str) -> str:
+    """
+    Does opposite to :func:`~escape_python_identifier`.
+    Takes an escaped string and converts it to the python variable identifier.
+
+    Parameters
+    ----------
+    name
+        Escaped python variable name.
+    """
+
     def unescape_repl(m):
         if m.group(1) in _unescaping_strings_dict:
             return _unescaping_strings_dict[m.group(1)]
         return m.group(0)
 
     if name.find(_escaped_prefix) == 0:
         name = name[len(_escaped_prefix) :]
@@ -103,27 +121,14 @@
     toknum, tokval = tok
     if toknum == BACKTICK_QUOTED_STRING:
         return tokenize.NAME, escape_python_identifier(tokval)
     return toknum, tokval
 
 
 def _parse_pandas_filter_vars(pandas_filter: str, with_special_vars: bool) -> list[str]:
-    """
-    Parsing one ``pandas.eval`` expression. Uses python build-in ``ast`` parser under the hood
-
-    Parameters
-    ----------
-    pandas_filter: str
-    with_special_vars: bool
-
-    Returns
-    -------
-    list[str]
-
-    """
     pre_parsed_filter = _preparse(
         pandas_filter,
         _compose(
             _replace_locals,
             _replace_booleans,
             _rewrite_assign,
             _clean_backtick_quoted_toks,
@@ -142,33 +147,30 @@
     return result_vars
 
 
 def parse_pandas_filter_vars(
     pandas_filter: Union[str, list[str]], with_special_vars: bool = False
 ) -> list[str]:
     """
-    Parsing ``pandas.eval`` expression and returns list of all used variables
+    Parsing :func:`pandas.eval` expression and returns list of all used variables.
+    Uses python build-in :mod:`ast` parser under the hood.
 
     Parameters
     ----------
-    pandas_filter: Union[str, list[str]]
+    pandas_filter
         Pandas eval expression
-    with_special_vars: bool
-        Include special variables such as `index`, math functions `sin`, 'log10` etc into the output
+    with_special_vars
+        Include special variables such as ``index``, math functions ``sin``, ``log10`` etc into the output
 
     Examples
     --------
     >>> vars_list = parse_pandas_filter_vars('Col1 > 0 & Col2 < 100')
     >>> sorted(vars_list)
     ['Col1', 'Col2']
 
-    Returns
-    -------
-    list[str]
-
     """
     if isinstance(pandas_filter, list):
         filters_list = pandas_filter
     else:
         filters_list = [pandas_filter]
     result_vars = set()
     for pandas_filter in filters_list:
@@ -180,17 +182,17 @@
     """
     Take a mask (boolean series) where True indicates keeping a value, and False
     represents removing the value. This will 'expand' those indexes marked as `False`
     to the symmetrical bounds of ``buffer_size``
 
     Parameters
     ----------
-    mask: pandas.core.Series
+    mask
         Boolean pandas series
-    buffer_size: int
+    buffer_size
         Size to buffer around ``False`` values
 
     Examples
     --------
     >>> import pandas as pd
     >>> series = pd.Series([True, True, False, True, True])
     >>> series = apply_buffer(series, buffer_size=1)
@@ -219,42 +221,41 @@
     ans = np.convolve(a=array, v=kernel, mode="same")
     mask.values[:] = ans < 1
     return mask
 
 
 def pandas_filter_rows(
     df: pd.DataFrame, filter_str: Union[str, list], buffer_size: int = 0
-):
+) -> pd.DataFrame:
     """Filter pandas data frame based on list or string of conditions.
 
-    Note:
-    pd.DataFrame.eval of a list returns a numpy.ndarray and is limited to 100 list items.
-    The sparse evaluation with numexpr pd.DataFrame.eval of a combined string logic, can only consist of
-    a maximum 32 (current dependency) or 242 logical parts (latest release) and returns a pd.Series
-    Therefore, list elements are evaluated in batches of n=15 (to be safe) and evaluate iterative.
+    .. note::
+        :func:`pd.DataFrame.eval` of a list returns a numpy.ndarray and is limited to 100 list items.
+        The sparse evaluation with numexpr :func:`pd.DataFrame.eval` of a combined string logic, can only consist of
+        a maximum 32 (current dependency) or 242 logical parts (latest release) and returns a pd.Series
+        Therefore, list elements are evaluated in batches of ``n=15`` (to be safe) and evaluate iterative.
 
     Parameters
     ----------
-    df: pandas.Dataframe
-      Dataframe to filter rows from. Does not modify the parameter
-    filter_str: str or list
-      String representing the filter. Can be a boolean combination of conditions,
-      where conditions are comparisons of column names and either other columns
-      or numeric values. The rows matching the filter are kept.
-      Column names with spaces must be quoted with backticks,
-      names without spaces could be quoted with backticks or be unquoted.
-      Example of legal filters are " `Tag A` > 5 " , " (`Tag B` > 1) | (`Tag C` > 4)"
-      '(`Tag D` < 5) ', " (TagB > 5) "
-      The parameter can also be a list, in which the items will be joined by logical " & ".
-    buffer_size: int
-      Area fore and aft of the application of ``fitler_str`` to also mark for removal.
+    df
+        Dataframe to filter rows from. Does not modify the parameter
+    filter_str
+        String representing the filter. Can be a boolean combination of conditions,
+        where conditions are comparisons of column names and either other columns
+        or numeric values. The rows matching the filter are kept.
+        Column names with spaces must be quoted with backticks,
+        names without spaces could be quoted with backticks or be unquoted.
+        Example of legal filters are ```Tag A` > 5`` , ``(`Tag B` > 1) | (`Tag C` > 4)``
+        ``(`Tag D` < 5)``, ``(TagB > 5)``
+        The parameter can also be a list, in which the items will be joined by logical " & ".
+    buffer_size
+        Area fore and aft of the application of ``fitler_str`` to also mark for removal.
 
     Returns
     -------
-    pandas.Dataframe
         The dataframe containing only rows matching the filter
 
     Examples
     --------
     >>> import numpy as np
     >>> import pandas as pd
     >>> df = pd.DataFrame(list(np.ndindex((3,3))), columns=list('AB'))
```

## gordo_core/import_utils.py

```diff
@@ -30,30 +30,32 @@
 
 
 def prepare_back_compatible_locations(
     locations: Iterable[tuple[str, str]]
 ) -> BackCompatibleLocations:
     """
     The result of this function can be used as `back_compatibles` argument
-    in `import_location()` functions.
+    in :func:`.import_location` functions.
 
     Example
     -------
     >>> prepare_back_compatible_locations([('old_module.MyClass', 'new_module.MyClass'),('OldClass', 'NewClass')])
     {('old_module', 'MyClass'): ('new_module', 'MyClass'), (None, 'OldClass'): (None, 'NewClass')}
 
+    Result items in this example are ``tuple[str, str]`` where the first item is a module location and the second is a class name.
+
     Parameters
     ----------
-    locations: Iterable[tuple[str, str]]
+    locations
         List of locations. The first item of each tuple is a location in the previous version,
         the second item is the location of the current version.
 
     Returns
     -------
-        Key-Value pair with locations of the previous version to the current version.
+        Key/Value pair with locations of the previous version to the current version.
 
     """
     back_compatibles: BackCompatibleLocations = {}
     for from_location, to_location in locations:
         key = _parse_str_location(from_location)
         if key in back_compatibles:
             raise ValueError("Duplicate locations: '%s'" % from_location)
@@ -68,29 +70,31 @@
 def import_location(
     location: str,
     *,
     import_path: Optional[str] = None,
     back_compatibles: Optional[BackCompatibleLocations] = None
 ) -> Any:
     """
-    Imports entity from provided `location`, or finds an entity with `location` name in `import_path` module.
+    Imports entity from provided ``location``, or finds an entity with `location` name in `import_path` module.
 
     Example
     -------
     >>> import_location("multiprocessing.Process")
     <class 'multiprocessing.context.Process'>
     >>> import_location("Process", import_path="multiprocessing")
     <class 'multiprocessing.context.Process'>
 
     Parameters
     ----------
-    location: str
-    import_path: Optional[str]
-    back_compatibles: Optional[BackCompatibleLocations]
-        See `prepare_back_compatible_locations()` function for reference.
+    location
+        Import location. Could be either a full import path or just a class name.
+    import_path
+        Should be provided if ``location`` contains only the class name.
+    back_compatibles
+        See :func:`prepare_back_compatible_locations` function for reference.
 
     Returns
     -------
         Imported entity.
     """
     parsed_location = _parse_str_location(location)
     if back_compatibles is not None:
```

## gordo_core/metadata.py

```diff
@@ -1,13 +1,12 @@
 from typing import Iterable, Optional, Set
 
 from gordo_core.sensor_tag import (
     SensorTag,
     Tag,
-    extract_tag_name,
     load_sensor_tag,
     tag_to_json,
     unique_tag_names,
 )
 
 
 def tags_to_json_representation(tags: Iterable[Tag]) -> dict:
@@ -42,26 +41,26 @@
 )
 
 
 def sensor_tags_from_build_metadata(
     build_dataset_metadata: dict, tag_names: Set[str]
 ) -> dict[str, SensorTag]:
     """
-    Fetch tags information from the metadata
+    Fetch sensor tags information from the metadata.
+    This info should be placed in ``build_dataset_metadata["dataset_meta"]["tag_loading_metadata"]["tags"]``
 
     Parameters
     ----------
-    build_dataset_metadata: dict
-        build_metadata.dataset part of the metadata
-    tag_names: Set[str]
+    build_dataset_metadata
+        ``build_metadata.dataset`` part of the metadata
+    tag_names
         Contains tag names for which we should fetch information
     Returns
     -------
-    dict[str, SensorTag]
-        Key here is tag name passed though `tag_names` argument
+        Key here is tag name passed though ``tag_names`` argument
 
     """
     tags_build_metadata = _tags_from_build_metadata(build_dataset_metadata)
     sensor_tags: dict[str, SensorTag] = {}
     if tags_build_metadata is None:
         raise ValueError(
             "Unable to find tags information in build_metadata. "
```

## gordo_core/sensor_tag.py

```diff
@@ -10,29 +10,29 @@
     """Error indicating that something went wrong normalizing a sensor tag"""
 
     pass
 
 
 class SensorTag:
     """
-    Representation of sensor tag. It contains the sensor tag name and additional fields.
+    Representation of the sensor tag. It contains the sensor tag name and additional fields/metadata.
 
     Example
     -------
     >>> SensorTag("Test tag", field1="value1", field2="value2")
     SensorTag("Test tag",field1="value1",field2="value2")
 
     """
 
     def __init__(self, name: str, **kwargs: Optional[str]):
         """
         Parameters
         ----------
-        name: str
-            Sensor tag name. Required field.
+        name
+            Sensor tag name. Required field and should be unique among all the tags.
         kwargs
             Additional fields.
         """
         self.name = name
         self._fields = kwargs
         self._validate()
 
@@ -94,28 +94,26 @@
         """
         fields: dict[str, Optional[str]] = {"name": self.name}
         fields.update(self._fields)
         return fields
 
     def mutate_fields(self, **kwargs: Optional[str]) -> "SensorTag":
         """
-        Update `SensorTag` fields from `kwargs`. Instantiate a new object if needed
+        Update :class:`~SensorTag` fields from ``kwargs``. Instantiate a new object if needed.
 
         Examples
         --------
         >>> sensor_tag = SensorTag("Test tag", field1="value1", field2="value2")
         >>> sensor_tag.mutate_fields(field1="value", field3="value3")
         SensorTag("Test tag",field1="value",field2="value2",field3="value3")
 
         Parameters
         ----------
         kwargs
-
-        Returns
-        -------
+            Fields to update.
 
         """
         new_fields = copy.copy(self._fields)
         new_fields.update(kwargs)
         if new_fields != self._fields:
             return SensorTag(self.name, **new_fields)
         else:
@@ -163,23 +161,19 @@
     Example
     -------
     >>> load_sensor_tag({"name": "tag", "field1": "value1"})
     SensorTag("tag",field1="value1")
 
     Parameters
     ----------
-    sensor: dict[str, Optional[str]]
-        It should at least contain `name` field.
-    required_fields: Optional[Iterable[str]]
+    sensor
+        It should at least contain ``name`` field.
+    required_fields
         Required additional fields.
 
-    Returns
-    -------
-        SensorTag
-
     """
     _validate_required_fields(sensor, required_fields)
     sensor = copy.copy(sensor)
     name = sensor.pop("name", None)
     if not name:
         raise SensorTagNormalizationError(
             "Sensor representation %s does not have name" % repr(sensor)
@@ -189,21 +183,21 @@
 
 def normalize_sensor_tag(
     sensor: Sensor,
     required_fields: Optional[Iterable[str]] = None,
     **kwargs: Optional[str],
 ) -> Tag:
     """
-    Take sensor tag information and tries to convert it to SensorTag.
+    Take sensor tag information and tries to convert it to :class:`.SensorTag`.
 
     Parameters
     ----------
-    sensor: Sensor
-        Sensor tag information. Could be either dict suitable for `load_sensor_tag()` function or str
-    required_fields: Optional[Iterable[str]]
+    sensor
+        Sensor tag information. Could be either dict suitable for :func:`.load_sensor_tag` function or str
+    required_fields
         Required additional fields.
     kwargs
         Additional fields.
 
     Returns
     -------
 
@@ -233,63 +227,65 @@
 
 def to_list_of_strings(sensor_tag_list: list[SensorTag]) -> list[str]:
     """
     List of sensor tags names.
 
     Parameters
     ----------
-    sensor_tag_list: list[SensorTag]
+    sensor_tag_list
+        Sensor tags list
 
     """
     return [sensor_tag.name for sensor_tag in sensor_tag_list]
 
 
 def extract_tag_name(tag: Tag) -> str:
     """
     Get tag name.
 
     Parameters
     ----------
-    tag: Tag
+    tag
+        Sensor tag to extract.
 
     """
     if type(tag) is str:
         return cast(str, tag)
     else:
         return cast(SensorTag, tag).name
 
 
 def tag_to_json(tag: Tag) -> Union[str, dict[str, Optional[str]]]:
     """
-    Convert `Tag` to JSON representation.
+    Convert ::`.Tag` to JSON representation.
 
     Parameters
     ----------
-    tag: Tag
-
-    Returns
-    -------
+    tag
+        Tag to convert.
 
     """
     if type(tag) is str:
         return cast(str, tag)
     else:
         sensor_tag = cast(SensorTag, tag)
         return sensor_tag.to_json()
 
 
 def validate_tag_equality(tag1: Tag, tag2: Tag):
     """
-    SensorTags with the same name should not have different fields.
-    str and SensorTag should not have the same name.
+    :class:`.SensorTags` with the same name should not have different fields.
+    str and :class:`.SensorTag` should not have the same name.
 
     Parameters
     ----------
-    tag1: Tag
-    tag2: Tag
+    tag1
+        First tag to compare.
+    tag2
+        Second tag to compare.
 
     """
     type_tag1, type_tag2 = type(tag1), type(tag2)
     if type_tag1 is SensorTag and type_tag2 is SensorTag:
         if cast(SensorTag, tag1) != cast(SensorTag, tag2):
             raise ValueError(
                 "Tags %s and %s with the same name but different fields"
@@ -314,15 +310,14 @@
     Parameters
     ----------
     tags
         Iterables of tags.
 
     Returns
     -------
-    dict[str, Tag]
         Keys here are the unique tag names.
         Tags will be in lower case if `case_insensitive` True.
 
     """
     orig_tags: dict[str, Tag] = {}
     for tag in itertools.chain(*tags):
         tag_name = extract_tag_name(tag)
```

## gordo_core/time_series.py

```diff
@@ -51,17 +51,17 @@
 
 class NotEnoughDataWarning(RuntimeWarning):
     pass
 
 
 def compat(init):
     """
-    __init__ decorator for compatibility where the Gordo config file's ``dataset`` keys have
+    ``__init__`` decorator for compatibility where the Gordo config file's ``dataset`` keys have
     drifted from what kwargs are actually expected in the given dataset. For example,
-    using `train_start_date` is common in the configs, but :class:`~TimeSeriesDataset`
+    using ``train_start_date`` is common in the configs, but :class:`~TimeSeriesDataset`
     takes this parameter as ``train_start_date``, as well as :class:`~RandomDataset`
 
     Renames old/other acceptable kwargs to the ones that the dataset type expects
     """
 
     @wraps(init)
     def wrapper(*args, **kwargs):
@@ -124,76 +124,77 @@
         n_samples_threshold: int = 0,
         interpolation_method: str = "linear_interpolation",
         interpolation_limit: str = DEFAULT_INTERPOLATION_LIMIT,
         filter_periods: Optional[Union[dict, FilterPeriods]] = None,
         **kwargs,
     ):
         """
-        Creates a TimeSeriesDataset backed by a provided dataprovider.
+        Creates a ``TimeSeriesDataset`` backed by a provided dataprovider.
 
-        A TimeSeriesDataset is a dataset backed by timeseries, but resampled,
+        A ``TimeSeriesDataset`` is a dataset backed by timeseries, but resampled,
         aligned, and (optionally) filtered.
 
         Parameters
         ----------
-        train_start_date: Union[datetime, str]
+        train_start_date
             Earliest possible point in the dataset (inclusive)
-        train_end_date: Union[datetime, str]
+        train_end_date
             Earliest possible point in the dataset (exclusive)
-        tag_list: Sequence[Union[str, dict, sensor_tag.SensorTag]]
+        tag_list
             List of tags to include in the dataset. The elements can be strings,
-            dictionaries or SensorTag namedtuples.
-        target_tag_list: Sequence[list[Union[str, dict, sensor_tag.SensorTag]]]
+            dictionaries or :class:`gordo_core.SensorTag`, :func:`tuple`.
+        target_tag_list
             List of tags to set as the dataset y. These will be treated the same as
             tag_list when fetching and pre-processing (resampling) but will be split
-            into the y return from ``.get_data()``
-        data_provider: Optional[GordoBaseDataProvider]
+            into the y return from :class:`~TimeSeriesDataset.get_data`
+        data_provider
             A dataprovider which can provide dataframes for tags from train_start_date to train_end_date
-        resolution: Optional[str]
+        resolution
             The bucket size for grouping all incoming time data (e.g. "10T").
             Available strings come from
-            https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#dateoffset-objects
-            **Note**: If this parameter is ``None`` or ``False``,
-            then _no_ aggregation/resampling is applied to the data.
-        row_filter: str or list
+            `timeseries <https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#dateoffset-objects>`_
+
+            .. note::
+                If this parameter is ``None`` or ``False``, then _no_ aggregation/resampling is applied to the data.
+        row_filter
             Filter on the rows. Only rows satisfying the filter will be in the dataset.
             See :func:`gordo_core.filter_rows.pandas_filter_rows` for
             further documentation of the filter format.
-        known_filter_periods: list
+        known_filter_periods
             List of periods to drop in the format
-            [~('2020-04-08 04:00:00+00:00' < index < '2020-04-08 10:00:00+00:00')].
+            ``[~('2020-04-08 04:00:00+00:00' < index < '2020-04-08 10:00:00+00:00')].``
             Note the time-zone suffix (+00:00), which is required.
         aggregation_methods
             Aggregation method(s) to use for the resampled buckets. If a single
             resample method is provided then the resulting dataframe will have names
             identical to the names of the series it got in. If several
             aggregation-methods are provided then the resulting dataframe will
             have a multi-level column index, with the series-name as the first level,
             and the aggregation method as the second level.
-            See :py:func::`pandas.core.resample.Resampler#aggregate` for more
+            See :func:`pandas.Series.resample` for more
             information on possible aggregation methods.
-        row_filter_buffer_size: int
+        row_filter_buffer_size
             Whatever elements are selected for removal based on the ``row_filter``, will also
             have this amount of elements removed fore and aft.
             Default is zero 0
-        asset: Optional[str]
+        asset
             Asset for which the tags are associated with.
-        n_samples_threshold: int = 0
+        n_samples_threshold
             The threshold at which the generated DataFrame is considered to have too few rows of data.
-        interpolation_method: str
-            How should missing values be interpolated. Either forward fill (`ffill`) or by linear
-            interpolation (default, `linear_interpolation`).
-        interpolation_limit: str
+        interpolation_method
+            How should missing values be interpolated. Either forward fill (``ffill``) or by linear
+            interpolation (default, ``linear_interpolation``).
+        interpolation_limit
             Parameter sets how long from last valid data point values will be interpolated/forward filled.
             If None, all missing values are interpolated/forward filled.
             Also, it's used as max time limit of point for look-back to find
             latest point before window's start (if needed).
-        filter_periods: dict
+        filter_periods
             Performs a series of algorithms that drops noisy data is specified.
-            See `filter_periods` class for details.
+            See ``filter_periods`` class for details.
         kwargs
             Deprecated arguments.
 
         .. deprecated::
             `asset` will be removed in the future.
         """
         self.train_start_date = self._validate_dt(train_start_date)
@@ -364,42 +365,42 @@
         interpolation_method: str = "linear_interpolation",
         interpolation_limit: str = DEFAULT_INTERPOLATION_LIMIT,
     ) -> Tuple[pd.DataFrame, dict]:
         """Resample, aggregate, join Series to Dataframe and drop Nans.
 
         Parameters
         ----------
-        series_iterable: Iterable[pd.Series]
+        series_iterable
             An iterator supplying series with time index
-        resampling_startpoint: datetime.datetime
+        resampling_startpoint
             The starting point for resampling. Most data frames will not have this
             in their datetime index, and it will be inserted with a NaN as the value.
             The resulting NaNs will be removed, so the only important requirement for this is
             that this resampling_startpoint datetime must be before or equal to the first
             (earliest) datetime in the data to be resampled.
-        resampling_endpoint: datetime.datetime
+        resampling_endpoint
             The end point for resampling. This datetime must be equal to or after the last datetime in the
             data to be resampled.
-        resolution: str
+        resolution
             The bucket size for grouping all incoming time data (e.g. "10T")
             Available strings come from
             https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#dateoffset-objects
-        aggregation_methods: Union[str, list[str], Callable]
+        aggregation_methods
             Aggregation method(s) to use for the resampled buckets. If a single
             resample method is provided then the resulting dataframe will have names
             identical to the names of the series it got in. If several
             aggregation-methods are provided then the resulting dataframe will
             have a multi-level column index, with the series-name as the first level,
             and the aggregation method as the second level.
             See :py:func::`pandas.core.resample.Resampler#aggregate` for more
             information on possible aggregation methods.
-        interpolation_method: str
+        interpolation_method
             How should missing values be interpolated. Either forward fill (`ffill`) or by linear
             interpolation (default, `linear_interpolation`).
-        interpolation_limit: str
+        interpolation_limit
             Parameter sets how long from last valid data point values will be interpolated/forward filled.
             Default is eight hours (`8H`).
             If None, all missing values are interpolated/forward filled.
 
         Returns
         -------
         pd.DataFrame
@@ -499,17 +500,16 @@
         interpolation_limit: str,
     ) -> pd.Series:
         """Try to fill Nans from look-back interpolated point.
 
         Only uses point from past to Nans filling if it was found not far then
         interpolation limit.
 
-        Returns:
+        Returns
         -------
-        pd.Series
             Same not changed Series or Series with attempt to fill Nans.
         """
         try:
             look_back_point = self.data_provider.get_closest_datapoint(
                 tag=tag,
                 before_time=resampling_startpoint,
                 point_max_look_back=pd.Timedelta(interpolation_limit),
@@ -743,15 +743,15 @@
     def get_metadata(self):
         return self._metadata.copy()
 
 
 class RandomDataset(TimeSeriesDataset):
     """
     Get a TimeSeriesDataset backed by
-    gordo_core.data_provider.providers.RandomDataProvider
+    :class:`gordo_core.data_provider.providers.RandomDataProvider`
     """
 
     @compat
     @capture_args
     def __init__(
         self,
         train_start_date: Union[datetime, str],
```

## gordo_core/utils.py

```diff
@@ -1,36 +1,36 @@
 import functools
 import inspect
 import logging
+import pkg_resources
 from collections import namedtuple
 from datetime import datetime
 from types import MappingProxyType
 from typing import Callable, Iterable, Mapping, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from influxdb import DataFrameClient, InfluxDBClient
 
 DEFAULT_INFLUX_PROXIES = MappingProxyType({"https": "", "http": ""})
 
 
 def capture_args_ext(ignore: Optional[Iterable[str]] = None):
     """
-    Decorator that captures args and kwargs passed to a given method.
+    Decorator that captures args and ``kwargs`` passed to a given method.
     This assumes the decorated method has a self, which has a dict of
-    kwargs assigned as an attribute named _params.
+    ``kwargs`` assigned as an attribute named ``_params``.
 
     Parameters
     ----------
-    ignore: Optional[Iterable[str]]
+    ignore
         List of arguments that need to be ignored during capturing
 
     Returns
     -------
-    Any
         Returns whatever the original method would return
     """
 
     def decorator(method: Callable):
         @functools.wraps(method)
         def wrapper(self, *args, **kwargs):
             sig_params = inspect.signature(method).parameters.items()
@@ -64,35 +64,36 @@
         return wrapper
 
     return decorator
 
 
 def capture_args(method: Callable):
     """
-    `capture_args_ext` without arguments
+    :func:`.capture_args_ext` without arguments
     """
     return capture_args_ext()(method)
 
 
-# Prediction result representation, name=str, predictions=dataframe, error_messages=list[str]
 PredictionResult = namedtuple("PredictionResult", "name predictions error_messages")
+"""
+Prediction result representation.
+"""
 
 
 def _parse_influx_uri(uri: str) -> Tuple[str, str, str, str, str, str]:
     """
     Parse an influx URI
 
     Parameters
     ----------
-    uri: str
-        Format: <username>:<password>@<host>:<port>/<optional-path>/<db_name>
+    uri
+        Format: ``<username>:<password>@<host>:<port>/<optional-path>/<db_name>``
 
     Returns
     -------
-    (str, str, str, str, str, str)
         username, password, host, port, path, database
     """
     username, password, host, port, *path, db_name = (
         uri.replace("/", ":").replace("@", ":").split(":")
     )
     path_str = "/".join(path) if path else ""
     return username, password, host, port, path_str, db_name
@@ -103,34 +104,30 @@
     api_key: Optional[str] = None,
     api_key_header: Optional[str] = "Ocp-Apim-Subscription-Key",
     recreate: bool = False,
     dataframe_client: bool = False,
     proxies: Mapping[str, str] = DEFAULT_INFLUX_PROXIES,
 ) -> Union[InfluxDBClient, DataFrameClient]:
     """
-    Get a InfluxDBClient or DataFrameClient from a SqlAlchemy like URI
+    Get a ``InfluxDBClient`` or ``DataFrameClient`` from a `SqlAlchemy <https://www.sqlalchemy.org/>`_ like URI
 
     Parameters
     ----------
-    uri: str
-        Connection string format: <username>:<password>@<host>:<port>/<optional-path>/<db_name>
-    api_key: str
+    uri
+        Connection string format: ``<username>:<password>@<host>:<port>/<optional-path>/<db_name>``
+    api_key
         Any api key required for the client connection
-    api_key_header: str
+    api_key_header
         The name of the header the api key should be assigned
-    recreate: bool
+    recreate
         Re/create the database named in the URI
-    dataframe_client: bool
-        Return a DataFrameClient instead of a standard InfluxDBClient
-    proxies: dict
+    dataframe_client
+        Return a DataFrameClient instead of a standard ``InfluxDBClient``
+    proxies
         A mapping of any proxies to pass to the influx client
-
-    Returns
-    -------
-    Union[InfluxDBClient, DataFrameClient]
     """
 
     username, password, host, port, path, db_name = _parse_influx_uri(uri)
 
     Client = DataFrameClient if dataframe_client else InfluxDBClient
 
     client = Client(
@@ -154,32 +151,31 @@
 def fill_series_with_look_back_points(
     series: pd.Series,
     look_back_point: pd.Series,
     end_time: datetime,
     interpolation_limit: str,
     resolution: Union[str, pd.Timedelta],
 ) -> pd.Series:
-    """Fill of Nans of given Series with interpolated look-back points.
+    """Fill of Nans of given ``Series`` with interpolated look-back points.
 
     Parameters
     ----------
-    series : pd.Series
+    series
         Series for Nans filling.
-    look_back_point : pd.Series
+    look_back_point
         Series with one closest point (with time) in past. Contains only one point.
-    end_time : datetime
+    end_time
         latest time of the Series till what points might be filled.
-    interpolation_limit : str
+    interpolation_limit
         time limit for interpolation.
-    resolution : str
+    resolution
         resolution of DatetimeIndex of the Series.
 
     Returns
     -------
-    pd.Series
         Newly copied and filled with Nans (if possible) Series.
         Given Series is not affected.
     """
     # round time of the look_back_point to match resolution, otherwise indexes won't match on 'filling'.
     look_back_point.index = look_back_point.index.round(resolution)
 
     series_copy = series.copy()
@@ -273,19 +269,18 @@
     resampling_endpoint: datetime,
     resolution: str,
     interpolation_limit: str,
     aggregation_methods: Union[str, list[str], Callable] = "mean",
     interpolation_method: str = "linear_interpolation",
 ):
     """Resample series accordingly to given parameters.
-
-    Note: Nans are NOT dropped in this function anymore after resampling.
-
     Takes a single series and resamples it.
-    See :class:`gordo_core.base.GordoBaseDataset.join_timeseries`
+
+    .. note::
+        Nans are NOT dropped in this function anymore after resampling.
     """
 
     startpoint_sametz = resampling_startpoint.astimezone(tz=series.index[0].tzinfo)
     endpoint_sametz = resampling_endpoint.astimezone(tz=series.index[0].tzinfo)
 
     if series.index[0] > startpoint_sametz:
         # Insert a NaN at the startpoint, to make sure that all resampled
@@ -358,20 +353,19 @@
 
 def _to_timestamps(column: list[pd.Timestamp]):
     return [v.timestamp() for v in column]
 
 
 def gaps_df_to_dict(df: pd.DataFrame) -> dict:
     """
-    Extract metadata information from `_find_gaps` DataFrame
+    Extract metadata information from :func:`find_gaps` DataFrame
 
-    Parameters
-    ----------
-    df: pd.DataFrame
-        Contains columns: start, end
+    Returns
+    -------
+        Contains columns ``start``, ``end``
     """
     if df.empty:
         return {}
     df_dict = df.to_dict("list")
     return {
         "start": _to_timestamps(df_dict["start"]),
         "end": _to_timestamps(df_dict["end"]),
@@ -402,7 +396,14 @@
     g = diff_[diff_ > td]
 
     # Output DataFrame
     gaps = pd.DataFrame(g, columns=["duration"], dtype="timedelta64[ns]")
     gaps["start"] = gaps.index - gaps["duration"]
     gaps = gaps.rename_axis("end").reset_index()
     return gaps[["start", "end"]]
+
+
+def get_version() -> Optional[str]:
+    try:
+        return pkg_resources.get_distribution("gordo-core").version
+    except ImportError:
+        return None
```

## gordo_core/validators.py

```diff
@@ -10,15 +10,15 @@
 logger = logging.getLogger(__name__)
 
 
 class BaseDescriptor:
     """
     Base descriptor class
 
-    New object should override __set__(self, instance, value) method to check
+    New object should override ``__set__(self, instance, value)`` method to check
     if 'value' meets required needs.
     """
 
     def __get__(self, instance, owner):
         return instance.__dict__[self.name]
 
     def __set_name__(self, owner, name):
@@ -26,15 +26,15 @@
 
     def __set__(self, instance, value):
         raise NotImplementedError("Setting value not implemented for this Validator!")
 
 
 class ValidDataset(BaseDescriptor):
     """
-    Descriptor for attributes requiring type :class:`gordo.workflow.config_elements.Dataset`
+    Descriptor for attributes requiring type :class:`gordo_core.base.GordoBaseDataset`
     """
 
     def __set__(self, instance, value):
 
         # Avoid circular dependency imports
         from gordo_core.base import GordoBaseDataset
 
@@ -43,15 +43,15 @@
                 f"Expected value to be an instance of GordoBaseDataset, found {value}"
             )
         instance.__dict__[self.name] = value
 
 
 class ValidDatasetKwargs(BaseDescriptor):
     """
-    Descriptor for attributes requiring type :class:`gordo.workflow.config_elements.Dataset`
+    Descriptor for attributes requiring type :class:`gordo_core.base.GordoBaseDataset`
     """
 
     def _verify_resolution(self, resolution: str):
         """
         Verifies that a resolution string is supported in pandas
         """
         try:
@@ -70,15 +70,15 @@
         if "resolution" in value:
             self._verify_resolution(value["resolution"])
         instance.__dict__[self.name] = value
 
 
 class ValidDataProvider(BaseDescriptor):
     """
-    Descriptor for DataProvider
+    Descriptor for attributes requiring type :class:`gordo_core.data_providers.base.GordoBaseDataProvider`
     """
 
     def __set__(self, instance, value):
 
         # Avoid circular dependency imports
         from gordo_core.data_providers.base import GordoBaseDataProvider
 
@@ -88,15 +88,15 @@
                 f"found {value} "
             )
         instance.__dict__[self.name] = value
 
 
 class ValidDatetime(BaseDescriptor):
     """
-    Descriptor for attributes requiring valid datetime.datetime attribute
+    Descriptor for attributes requiring valid :class:`datetime.datetime` attribute
     """
 
     def __set__(self, instance, value):
         datetime_value = None
         if isinstance(value, datetime.datetime):
             datetime_value = value
         elif isinstance(value, str):
```

## Comparing `gordo_core-0.3.0rc0.dist-info/LICENSE` & `gordo_core-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gordo_core-0.3.0rc0.dist-info/METADATA` & `gordo_core-0.3.1.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gordo-core
-Version: 0.3.0rc0
+Version: 0.3.1
 Summary: Gordo core library
 Home-page: https://github.com/equinor/gordo-core
 License: AGPLv3
 Keywords: gordo-core
 Author: Equinor ASA
 Author-email: fg_gpl@equinor.com
 Requires-Python: >=3.9,<4.0
@@ -25,41 +25,46 @@
 Requires-Dist: influxdb (>=5.3.0,<6.0.0)
 Requires-Dist: numexpr (>=2.7.1,<3.0.0)
 Requires-Dist: numpy (>=1.18.0,<2.0.0,!=1.20)
 Requires-Dist: pandas (>=1.1.0,<2.0.0)
 Requires-Dist: pyarrow (>=3.0.0,<11.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: xarray (>=0.16.2,<2024.0.0)
+Project-URL: Documentation, https://gordo-core.readthedocs.io/
 Project-URL: Repository, https://github.com/equinor/gordo-core
+Project-URL: Source, https://github.com/equinor/gordo-core
 Description-Content-Type: text/markdown
 
 # Gordo core library.
 
 The main component can be found [here](https://github.com/equinor/gordo).
 
+[Documentation is available on Read the Docs](https://gordo-core.readthedocs.io/)
+
 ## Installation
 
-Python 3.9 need to be installed in the system first.
+At least python 3.10 need to be installed in the system first.
 
 ```
 pip3 install gordo-core
 ```
 
 ## Developers Instructions
 
 ### Setup
 
 Install [poetry](https://python-poetry.org/docs/#installation).
 
 Setup and run development shell instance:
 
 ```console
-> poetry shell
 > poetry install
+> poetry shell
 ```
+### Pre-commit
 
 You could also install and apply [pre-commit](https://pre-commit.com/#usage) hooks.
 
 ### Run tests
 
 Install [docker](https://docs.docker.com/engine/install/) (or similar container manager) if you want to run test-suite.
 
@@ -70,7 +75,13 @@
 ```
 
 Run docker-related tests:
 ```console
 > poetry run pytest -m "dockertest"
 ```
 
+Build documentation:
+```console
+> cd docs/
+> poetry run make watch
+```
+
```

