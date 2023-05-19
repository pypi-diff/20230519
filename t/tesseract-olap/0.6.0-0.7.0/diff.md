# Comparing `tmp/tesseract_olap-0.6.0.tar.gz` & `tmp/tesseract_olap-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesseract_olap-0.6.0.tar", max compression
+gzip compressed data, was "tesseract_olap-0.7.0.tar", max compression
```

## Comparing `tesseract_olap-0.6.0.tar` & `tesseract_olap-0.7.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     2221 2022-09-13 02:26:29.134849 tesseract_olap-0.6.0/PACKAGE.md
--rw-r--r--   0        0        0      840 2023-03-24 01:27:03.260612 tesseract_olap-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      291 2023-03-24 01:31:31.773632 tesseract_olap-0.6.0/tesseract_olap/__init__.py
--rw-r--r--   0        0        0       92 2022-09-08 19:06:02.193244 tesseract_olap-0.6.0/tesseract_olap/backend/__init__.py
--rw-r--r--   0        0        0       79 2021-11-28 03:30:02.170791 tesseract_olap-0.6.0/tesseract_olap/backend/clickhouse/__init__.py
--rw-r--r--   0        0        0     5382 2023-03-24 00:38:03.868174 tesseract_olap-0.6.0/tesseract_olap/backend/clickhouse/backend.py
--rw-r--r--   0        0        0     1776 2023-03-24 00:42:44.291191 tesseract_olap-0.6.0/tesseract_olap/backend/clickhouse/dialect.py
--rw-r--r--   0        0        0     1221 2021-11-28 03:39:55.555792 tesseract_olap-0.6.0/tesseract_olap/backend/clickhouse/enums.py
--rw-r--r--   0        0        0       67 2022-02-08 01:50:06.630491 tesseract_olap-0.6.0/tesseract_olap/backend/clickhouse/growth.py
--rw-r--r--   0        0        0    19835 2023-03-24 00:46:15.636659 tesseract_olap-0.6.0/tesseract_olap/backend/clickhouse/sqlbuild.py
--rw-r--r--   0        0        0     1734 2023-03-03 22:06:57.931744 tesseract_olap-0.6.0/tesseract_olap/backend/exceptions.py
--rw-r--r--   0        0        0     3375 2023-03-23 23:39:59.358616 tesseract_olap-0.6.0/tesseract_olap/backend/models.py
--rw-r--r--   0        0        0      204 2022-09-13 02:25:25.476112 tesseract_olap-0.6.0/tesseract_olap/common/__init__.py
--rw-r--r--   0        0        0      951 2023-02-28 21:54:06.732282 tesseract_olap-0.6.0/tesseract_olap/common/captions.py
--rw-r--r--   0        0        0      204 2023-02-28 22:55:53.201991 tesseract_olap-0.6.0/tesseract_olap/common/exceptions.py
--rw-r--r--   0        0        0      399 2022-09-13 02:25:25.485798 tesseract_olap-0.6.0/tesseract_olap/common/types.py
--rw-r--r--   0        0        0      263 2023-02-28 22:55:45.464971 tesseract_olap-0.6.0/tesseract_olap/exceptions.py
--rw-r--r--   0        0        0      511 2022-03-10 15:33:40.890581 tesseract_olap-0.6.0/tesseract_olap/logiclayer/__init__.py
--rw-r--r--   0        0        0     6665 2022-08-19 20:46:44.427219 tesseract_olap-0.6.0/tesseract_olap/logiclayer/dependencies.py
--rw-r--r--   0        0        0     5313 2023-03-03 22:34:01.690917 tesseract_olap-0.6.0/tesseract_olap/logiclayer/module.py
--rw-r--r--   0        0        0     1198 2023-03-01 16:54:43.595549 tesseract_olap-0.6.0/tesseract_olap/logiclayer/response.py
--rw-r--r--   0        0        0     1129 2022-08-19 20:52:45.954437 tesseract_olap-0.6.0/tesseract_olap/query/__init__.py
--rw-r--r--   0        0        0     2262 2022-04-18 23:12:59.462564 tesseract_olap-0.6.0/tesseract_olap/query/calculations.py
--rw-r--r--   0        0        0     2848 2022-08-17 20:43:46.760168 tesseract_olap-0.6.0/tesseract_olap/query/enums.py
--rw-r--r--   0        0        0     2747 2023-03-01 01:27:28.563738 tesseract_olap-0.6.0/tesseract_olap/query/exceptions.py
--rw-r--r--   0        0        0    10504 2023-03-23 22:03:42.102103 tesseract_olap-0.6.0/tesseract_olap/query/models.py
--rw-r--r--   0        0        0    10811 2023-03-21 18:59:53.094892 tesseract_olap-0.6.0/tesseract_olap/query/queries.py
--rw-r--r--   0        0        0     7613 2022-08-19 20:54:16.492156 tesseract_olap-0.6.0/tesseract_olap/query/requests.py
--rw-r--r--   0        0        0     1406 2023-03-23 22:31:12.320685 tesseract_olap-0.6.0/tesseract_olap/query/results.py
--rw-r--r--   0        0        0      990 2023-03-02 22:59:25.384644 tesseract_olap-0.6.0/tesseract_olap/schema/__init__.py
--rw-r--r--   0        0        0     5410 2023-03-17 20:51:44.464943 tesseract_olap-0.6.0/tesseract_olap/schema/aggregators.py
--rw-r--r--   0        0        0     2502 2023-03-22 18:48:30.780846 tesseract_olap-0.6.0/tesseract_olap/schema/csv.py
--rw-r--r--   0        0        0     3117 2023-03-17 21:03:53.342792 tesseract_olap-0.6.0/tesseract_olap/schema/enums.py
--rw-r--r--   0        0        0     3323 2023-02-28 22:55:23.141709 tesseract_olap-0.6.0/tesseract_olap/schema/exceptions.py
--rw-r--r--   0        0        0     3122 2022-08-09 18:20:00.702530 tesseract_olap-0.6.0/tesseract_olap/schema/json.py
--rw-r--r--   0        0        0     7874 2023-03-21 18:39:17.877077 tesseract_olap-0.6.0/tesseract_olap/schema/models.py
--rw-r--r--   0        0        0     4786 2021-08-19 20:44:25.627000 tesseract_olap-0.6.0/tesseract_olap/schema/schema.xsd
--rw-r--r--   0        0        0    23345 2023-03-21 19:40:50.286511 tesseract_olap-0.6.0/tesseract_olap/schema/traverse.py
--rw-r--r--   0        0        0    17275 2023-03-17 21:14:00.924689 tesseract_olap-0.6.0/tesseract_olap/schema/xml.py
--rw-r--r--   0        0        0       64 2021-11-28 03:02:26.025135 tesseract_olap-0.6.0/tesseract_olap/server/__init__.py
--rw-r--r--   0        0        0     1053 2023-02-28 22:55:51.560682 tesseract_olap-0.6.0/tesseract_olap/server/exceptions.py
--rw-r--r--   0        0        0     6979 2023-03-23 23:40:48.895350 tesseract_olap-0.6.0/tesseract_olap/server/server.py
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 tesseract_olap-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2221 2023-05-19 01:51:12.794118 tesseract_olap-0.7.0/PACKAGE.md
+-rw-r--r--   0        0        0      862 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/__init__.py
+-rw-r--r--   0        0        0       92 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/__init__.py
+-rw-r--r--   0        0        0       79 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/__init__.py
+-rw-r--r--   0        0        0     5868 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/backend.py
+-rw-r--r--   0        0        0     1762 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/dialect.py
+-rw-r--r--   0        0        0     1221 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/enums.py
+-rw-r--r--   0        0        0    19408 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/sqlbuild.py
+-rw-r--r--   0        0        0     1734 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/exceptions.py
+-rw-r--r--   0        0        0     3248 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/models.py
+-rw-r--r--   0        0        0      243 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/common/__init__.py
+-rw-r--r--   0        0        0      219 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/common/exceptions.py
+-rw-r--r--   0        0        0     1570 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/common/strings.py
+-rw-r--r--   0        0        0      385 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/common/types.py
+-rw-r--r--   0        0        0      380 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/exceptions.py
+-rw-r--r--   0        0        0      511 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/logiclayer/__init__.py
+-rw-r--r--   0        0        0     6665 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/logiclayer/dependencies.py
+-rw-r--r--   0        0        0     5677 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/logiclayer/module.py
+-rw-r--r--   0        0        0     1198 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/logiclayer/response.py
+-rw-r--r--   0        0        0     1129 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/__init__.py
+-rw-r--r--   0        0        0     2262 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/calculations.py
+-rw-r--r--   0        0        0     2848 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/enums.py
+-rw-r--r--   0        0        0     3104 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/exceptions.py
+-rw-r--r--   0        0        0    10377 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/models.py
+-rw-r--r--   0        0        0    11603 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/queries.py
+-rw-r--r--   0        0        0     7990 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/requests.py
+-rw-r--r--   0        0        0     1539 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/results.py
+-rw-r--r--   0        0        0     1145 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/__init__.py
+-rw-r--r--   0        0        0     5400 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/aggregators.py
+-rw-r--r--   0        0        0     3391 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/csv.py
+-rw-r--r--   0        0        0     2908 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/enums.py
+-rw-r--r--   0        0        0     3323 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/exceptions.py
+-rw-r--r--   0        0        0     2500 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/json.py
+-rw-r--r--   0        0        0     8559 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/models.py
+-rw-r--r--   0        0        0     4645 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/schema.xsd
+-rw-r--r--   0        0        0    23574 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/traverse.py
+-rw-r--r--   0        0        0    18440 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/xml.py
+-rw-r--r--   0        0        0       64 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/server/__init__.py
+-rw-r--r--   0        0        0      898 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/server/exceptions.py
+-rw-r--r--   0        0        0     4269 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/server/schema.py
+-rw-r--r--   0        0        0     4260 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/server/server.py
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 tesseract_olap-0.7.0/PKG-INFO
```

### Comparing `tesseract_olap-0.6.0/PACKAGE.md` & `tesseract_olap-0.7.0/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.6.0/pyproject.toml` & `tesseract_olap-0.7.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tesseract-olap"
-version = "0.6.0"
+version = "0.7.0"
 description = "A simple OLAP library."
 authors = ["Francisco Abarzua <francisco@datawheel.us>"]
 license = "MIT"
 readme = "PACKAGE.md"
 repository = "https://github.com/Datawheel/tesseract-python"
 
 [tool.poetry.dependencies]
@@ -20,14 +20,15 @@
 [tool.poetry.extras]
 clickhouse = ["asynch"]
 
 [tool.poetry.group.dev.dependencies]
 asynch = "^0.2.1"
 fastapi = ">=0.70.0"
 logiclayer = "^0.2.0"
+lxml-stubs = "^0.4.0"
 pytest = "^7.2.0"
 pytest-asyncio = "^0.20.0"
 requests = "^2.27.1"
 ruff = "^0.0.237"
 sqlparse = "^0.4.0"
 tomli = "^2.0.1"
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/backend/clickhouse/backend.py` & `tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/backend.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from contextlib import asynccontextmanager
-from typing import AsyncGenerator, List, Type, TypeVar, Union
+from typing import AsyncGenerator, List, Optional, Type, TypeVar, Union
 
 import asynch
 from asynch.cursors import Cursor
 from asynch.errors import ClickHouseException
 from asynch.proto.result import IterQueryResult
 
 from tesseract_olap.backend import Backend
@@ -143,7 +143,23 @@
 
         if isinstance(self._rows, IterQueryResult):
             async for row in self._rows:
                 yield dict(zip(columns, row))
 
         else:
             raise ValueError("Streaming result not enabled")
+
+    async def execute(self, query: str, args: Optional[dict]=None, context=None):
+        self._check_cursor_closed()
+        self._check_query_executing()
+        self._begin_query()
+
+        execute, kwargs = self._prepare(context)
+
+        del kwargs["settings"]["max_block_size"]
+
+        response = await execute(query, args=args, with_column_types=True, **kwargs)
+
+        await self._process_response(response)
+        self._end_query()
+
+        return self._rowcount
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/backend/clickhouse/enums.py` & `tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.6.0/tesseract_olap/backend/clickhouse/sqlbuild.py` & `tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/sqlbuild.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 """ClickHouse SQL generation module.
 
 Comprises all the functions which generate SQL code, through the pypika library.
 """
 
 from itertools import chain
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Set, Tuple, Union
 
 from pypika import functions as fn
 from pypika.dialects import ClickHouseQuery, QueryBuilder
-from pypika.enums import Order
+from pypika.enums import Arithmetic, Order
 from pypika.queries import Selectable, Table
-from pypika.terms import Criterion, Field, Function, PyformatParameter
+from pypika.terms import ArithmeticExpression, Criterion, Field, Function, PyformatParameter
 
 from tesseract_olap.backend import ParamManager
+from tesseract_olap.common.strings import shorthash
 from tesseract_olap.query import (Comparison, DataQuery, HierarchyField,
                                   LogicOperator, MeasureField, MembersQuery,
                                   NumericConstraint, RestrictionAge)
+from tesseract_olap.query.models import LevelField
 from tesseract_olap.schema import MemberType, models
 
-from .dialect import TopK, ArrayElement
+from .dialect import ArrayElement, AverageWeighted, Power, TopK
 
 
 def dataquery_sql(
     query: DataQuery,
-) -> Tuple[QueryBuilder, Dict[str, str], List[models.InlineTable]]:
+) -> Tuple[Selectable, Dict[str, str], List[models.InlineTable]]:
     """Build the query which will retrieve an aggregated dataset from the
     database.
 
-    The construction of this query has three main parts:
+    The construction of this query has two main parts:
     - The Core Query,
-        which retrieves the primary keys and data rows needed for later steps
+        which retrieves all the columns needed for later steps, and applies the
+        filter on the qualitative fields (cuts)
     - The Grouping Query,
-        which applies the calculations/aggregations over the data
-    - The Enriching Query,
-        which retrieves the IDs, labels and extra data for the grouped data
+        which applies the calculations/aggregations over the data, filters on
+        quantitative fields (filters), applies pagination, sorting and the
+        aliases over the columns
 
-    The returned query is the third, which contains the other two as subqueries.
+    The returned query is composed by the Grouping query on the Core query as
+    subquery.
     """
     pman = ParamManager()
     external_tables: List[models.InlineTable] = []
 
     def _convert_table(table: Union[models.Table, models.InlineTable], alias: Optional[str]):
         if isinstance(table, models.Table):
             return Table(table.name, schema=table.schema, alias=alias)
@@ -52,273 +56,258 @@
         *,
         alias: Optional[str] = None,
     ) -> Table:
         return table_fact if table is None else _convert_table(table, alias)
 
     locale = query.locale
     table_fact = _convert_table(query.cube.table, "tfact")
+    tfact_is_subset = query.cube.subset_table
 
-    def dataquery_tcore_sql() -> QueryBuilder:
+    def dataquery_tcore_sql() -> Selectable:
         """
         Build the query which will create the `core_table`, an intermediate query
         which contains all data from the Dimension Tables and the Fact Table the
         cube is associated to.
 
         This query also retrieves the row for all associated dimensions used in
         drilldowns and cuts, through a LEFT JOIN using the foreign key.
         """
         qb: QueryBuilder = ClickHouseQuery.from_(table_fact)
 
-        def _get_closest_field(field: HierarchyField):
-            """Prevents SELECTing fields from table_dim if the column used as
-            primary key is the same one being SELECTed, thus avoiding an
-            unnecessary LEFT JOIN operation.
-            """
-            column = field.deepest_level.key_column
-            alias = f"lv_{field.deepest_level.alias}"
-            table_dim = _get_table(field.table)
-            if table_dim is not table_fact and column == field.primary_key:
-                return Field(field.foreign_key, alias=alias, table=table_fact)
-            return Field(column, alias=alias, table=table_dim)
-
-        select_fields = chain((
+        qb = qb.select(*(
             # from the fact table, get the fields which contain the values
             # to aggregate and filter; ensure to not duplicate key_columns
-            Field(item.measure.key_column, alias=f"ms_{item.key_alias}", table=table_fact)
+            Field(item.measure.key_column, alias=f"ms_{item.alias_key}", table=table_fact)
             for item in dict(
-                (obj.key_alias, obj) for obj in query.fields_quantitative
+                (obj.alias_key, obj) for obj in query.fields_quantitative
             ).values()
-        ), (
-            # from the dimension tables, get the fields which contain the primary
-            # key of the lowest level in each hierarchy, whether it's used as a
-            # drilldown or as a cut
-            _get_closest_field(item) for item in query.fields_qualitative
         ))
 
-        qb = qb.select(*select_fields)
+        for hiefi in query.fields_qualitative:
+            table_dim = _get_table(hiefi.table)
 
-        for field in query.fields_qualitative:
-            table = _get_table(field.table)
-            if (
-                table is table_fact or \
-                # if optimized by _get_closest_field()
-                field.deepest_level.key_column == field.primary_key
-            ):
-                continue
+            field_fkey = table_fact.field(hiefi.foreign_key)
 
-            qb = qb.left_join(table)\
-                   .on(table_fact.field(field.foreign_key)\
-                       == table.field(field.primary_key))
+            columns: Set[Field] = set()
 
-        return qb.as_("tcore")
+            for lvlfi in hiefi.levels:
+                # apply cuts to fact table to reduce amount of data to aggregate later
+                caster = lvlfi.level.type_caster
+                members_include = sorted(caster(mem) for mem in lvlfi.members_include)
+                members_exclude = sorted(caster(mem) for mem in lvlfi.members_exclude)
 
-    def dataquery_tgroup_sql(tcore: QueryBuilder) -> QueryBuilder:
-        """
-        Builds the query which will perform the grouping by drilldown members, and
-        then the aggregation over the resulting groups.
-        """
-        qb: QueryBuilder = ClickHouseQuery.from_(tcore)
+                lvl_columns = [
+                    Field(column, alias=f"lv_{alias}", table=table_dim)
+                    for column, _, alias in _yield_lvlfi_columns(lvlfi, locale)
+                ]
 
-        select_fields = chain(
-            # Apply aggregations over quantitative fields to get measures
-            (_get_aggregate(tcore, item) for item in query.fields_quantitative),
+                if table_dim is table_fact:
+                    if len(members_include) > 0:
+                        qb = qb.where(
+                            table_fact.field(lvlfi.key_column).isin(members_include)
+                        )
 
-            # Pass the representative level columns to later use to enrich
-            (Field(f"lv_{field.deepest_level.alias}",
-                   alias=f"dd_{field.deepest_level.alias}", table=tcore)
-            for field in query.fields_qualitative
-            if field.is_drilldown),
-        )
-        qb = qb.select(*select_fields)
+                    if len(members_exclude) > 0:
+                        qb = qb.where(
+                            table_fact.field(lvlfi.key_column).notin(members_exclude)
+                        )
 
-        # Use the representative levels, so the data gets aggregated
-        groupby_fields = (
-            tcore.field(f"lv_{field.deepest_level.alias}")
-            for field in query.fields_qualitative
-            if field.is_drilldown
-        )
-        qb = qb.groupby(*groupby_fields)
+                elif lvlfi.key_column == hiefi.primary_key:
+                    lvl_columns[0] = Field(hiefi.foreign_key, alias=lvl_columns[0].alias, table=table_fact)
+
+                    if len(members_include) > 0:
+                        qb = qb.where(field_fkey.isin(members_include))
+
+                    if len(members_exclude) > 0:
+                        qb = qb.where(field_fkey.notin(members_exclude))
+
+                elif lvlfi.is_cut:
+                    subq = ClickHouseQuery.from_(table_dim).select(hiefi.primary_key)
+
+                    if len(members_include) > 0:
+                        subq = subq.where(
+                            table_dim.field(lvlfi.key_column).isin(members_include)
+                        )
+
+                    if len(members_exclude) > 0:
+                        subq = subq.where(
+                            table_dim.field(lvlfi.key_column).notin(members_exclude)
+                        )
+
+                    qb = qb.where(field_fkey.isin(subq))
+
+                columns.update(lvl_columns)
 
-        for field in query.fields_qualitative:
-            for item in field.columns:
-                # transform the member keys to their MemberType set by the user
-                caster = item.level.key_type.get_caster()
-                # apply cuts' include/exclude restrictions
-                if len(item.members_include) > 0:
-                    members = sorted(caster(mem) for mem in item.members_include)
-                    qb = qb.where(
-                        tcore.field(f"lv_{item.alias}").isin(members)
-                    )
-                if len(item.members_exclude) > 0:
-                    members = sorted(caster(mem) for mem in item.members_exclude)
-                    qb = qb.where(
-                        tcore.field(f"lv_{item.alias}").notin(members)
-                    )
                 # apply arbitrary time restrictions
-                if item.time_restriction is not None:
+                # can't be handled as a cut because depends on a value we don't know
+                if lvlfi.time_restriction is not None:
                     # this is equivalent to having a cut set on this level,
                     # for the members that match the time scale
-                    table_time = _get_table(field.table, alias=f"ttime_{item.alias}")
                     order = Order.asc \
-                            if item.time_restriction.age == RestrictionAge.OLDEST else \
+                            if lvlfi.time_restriction.age == RestrictionAge.OLDEST else \
                             Order.desc
 
                     # we intend to create a subquery on the fact table for all
                     # possible members of the relevant level/timescale, using
                     # distinct unify, and get the first in the defined order
                     # which translates into latest/oldest
+
                     # TODO: use EXPLAIN to see if DISTINCT improves or worsens the query
-                    qb_time: QueryBuilder = ClickHouseQuery.from_(table_fact)\
-                                                           .distinct()\
-                                                           .limit(1)
-                    if table_time is table_fact:
+                    qb_time: QueryBuilder = \
+                        ClickHouseQuery.from_(table_fact).distinct().limit(1)
+                    field_time = table_dim.field(lvlfi.key_column)
+
+                    if table_dim is table_fact:
                         # Hierarchy is defined in the fact table -> direct query
-                        qb_time = qb_time\
-                            .select(table_fact.field(item.key_column))\
-                            .orderby(table_fact.field(item.key_column), order=order)
+                        qb = qb.where(
+                            field_time == qb_time
+                                .select(table_fact.field(lvlfi.key_column))
+                                .orderby(table_fact.field(lvlfi.key_column), order=order)
+                        )
+
+                    elif lvlfi.key_column == hiefi.primary_key:
+                        qb = qb.where(
+                            field_fkey == qb_time
+                                .select(table_fact.field(hiefi.primary_key))
+                                .orderby(table_fact.field(hiefi.primary_key), order=order)
+                        )
+
                     else:
-                        # Hierarchy lives in its own dimension table -> innerjoin
-                        qb_time = qb_time\
-                            .select(table_time.field(item.key_column))\
-                            .inner_join(table_time).on(
-                                table_fact.field(field.foreign_key)\
-                                == table_time.field(field.primary_key)
-                            )\
-                            .orderby(table_time.field(item.key_column), order=order)
-                    # apply the time restriction cut
-                    qb = qb.where(
-                        tcore.field(f"lv_{item.alias}").isin(qb_time)
+                        qb = qb.where(
+                            field_time == qb_time
+                                .left_join(table_dim).on(
+                                    field_fkey == table_dim.field(hiefi.primary_key)
+                                )
+                                .select(table_dim.field(lvlfi.key_column))
+                                .orderby(table_dim.field(lvlfi.key_column), order=order)
+                        )
+
+            qb = qb.select(*sorted(columns, key=lambda x: x.name))
+
+            # we must do LEFT JOIN if the request needs a column from a table
+            # other than fact table
+            if any(field.table is not table_fact for field in columns):
+                qb = qb.left_join(table_dim).on(
+                    table_dim.field(hiefi.primary_key) == field_fkey
+                )
+
+            # if the hierarchy is not stored on the fact table and the fact table
+            # combines facts for multiple levels, apply a filter over the
+            # foreign keys matching the members of the requested level
+            if table_dim is not table_fact and tfact_is_subset:
+                qb = qb.where(
+                    field_fkey.isin(
+                        ClickHouseQuery.from_(table_dim)\
+                            .select(hiefi.primary_key)\
+                            .distinct()
                     )
+                )
 
-        return qb.as_("tgroup")
+        return qb.as_("tcore")
 
-    def dataquery_tdata_sql(tgroup: QueryBuilder) -> QueryBuilder:
+    def dataquery_tgroup_sql(tcore: Selectable) -> Selectable:
         """
-        Enriches the table to final outcome, using the primary keys of the associated
-        dimensions to get the relevant columns.
+        Builds the query which will perform the grouping by drilldown members, and
+        then the aggregation over the resulting groups.
         """
-        qb: QueryBuilder = ClickHouseQuery.from_(tgroup)
+        qb: QueryBuilder = ClickHouseQuery.from_(tcore)
+
+        select_fields = chain(
+            # Apply aggregations over quantitative fields to get measures
+            (_get_aggregate(tcore, item) for item in query.fields_quantitative),
+
+            # Pass the representative level columns to later use to enrich
+            (Field(f"lv_{alias}", alias=name, table=tcore)
+            for hiefi in query.fields_qualitative
+            for _, name, alias in _yield_hiefi_columns(hiefi, locale)
+            if hiefi.has_drilldowns),
+        )
+        qb = qb.select(*select_fields)
+
+        # Use the representative levels, so the data gets aggregated
+        groupby_fields = (
+            tcore.field(f"lv_{alias}")
+            for hiefi in query.fields_qualitative
+            for _, _, alias in _yield_hiefi_columns(hiefi, locale)
+            if hiefi.has_drilldowns
+        )
+        qb = qb.groupby(*groupby_fields)
 
         # Default sorting directions
         # The results are sorted by the ID column of each drilldown
         order = Order.asc
         orderby = (
-            tgroup.field(f"dd_{field.deepest_level.alias}")
-            for field in query.fields_qualitative
-            if field.is_drilldown
+            tcore.field(f"lv_{hiefi.deepest_level.alias}")
+            for hiefi in query.fields_qualitative
+            if hiefi.has_drilldowns
         )
         # Flag to know an user-defined sorting field hasn't been set
         sort_field = None
 
-        # Select Measure columns from tgroup
-        measure_fields = (
-            Field(f"ag_{item.alias}", alias=item.measure.name, table=tgroup)
-            for item in query.fields_quantitative
-        )
-        qb = qb.select(*measure_fields).distinct()
-
         # Apply user-defined filters on aggregated data
-        for field in query.fields_quantitative:
+        for msrfi in query.fields_quantitative:
             # skip field if no filter is defined
-            if not field.constraint1:
+            if not msrfi.constraint1:
                 continue
 
             # create criterion for first constraint
-            column = Field(f"ag_{field.alias}", table=tgroup)
-            criterion = _get_filter_criterion(column, field.constraint1)
+            column = Field(msrfi.name)
+            criterion = _get_filter_criterion(column, msrfi.constraint1)
             # add second constraint to criterion if defined
-            if field.constraint2:
-                criterion2 = _get_filter_criterion(column, field.constraint2)
-                if field.joint == LogicOperator.AND:
+            if msrfi.constraint2:
+                criterion2 = _get_filter_criterion(column, msrfi.constraint2)
+                if msrfi.joint == LogicOperator.AND:
                     criterion &= criterion2
-                elif field.joint == LogicOperator.OR:
+                elif msrfi.joint == LogicOperator.OR:
                     criterion |= criterion2
-            qb = qb.where(criterion)
+            qb = qb.having(criterion)
 
-        # Apply enrichment LEFT JOIN for drilldown labels
-        for field in query.fields_qualitative:
+        for hiefi in query.fields_qualitative:
             # skip field if is not a drilldown
-            if not field.is_drilldown:
+            if not hiefi.has_drilldowns:
                 continue
 
-            # enrichment LEFT JOIN is done against a DISTINCT,
-            # column-specified subquery to reduce memory usage
-            field_columns = tuple(_yield_drilldown_columns(field, locale))
-
-            # don't do LEFT JOIN if this field only requests the column for its PK
-            if len(field_columns) == 1 and (
-                field_columns[0][0] == field.deepest_level.key_column and
-                field_columns[0][1] == field.deepest_level.name
-            ):
-                column, alias = field_columns[0]
-                qb = qb.select(
-                    Field(f"dd_{field.deepest_level.alias}", alias=alias, table=tgroup)
-                )
-
-            # do LEFT JOIN with dim_table if this field is requesting properties,
-            # parents, or the level has a name_column defined
-            else:
-                table_target = _get_table(field.table)
-                fields_left = (table_target.field(item) for item, _ in field_columns)
-                table_left: QueryBuilder = \
-                    ClickHouseQuery.from_(table_target)\
-                                   .select(*fields_left)\
-                                   .distinct()
-                # replace fact_table with subquery
-                table_enrich = table_left
-
-                # compose the pypika.Field list for each drilldown, drilldown ID & propty
-                drilldown_fields = (Field(column, alias=alias, table=table_enrich)
-                                    for column, alias in field_columns)
-
-                qb = qb.select(*drilldown_fields)\
-                       .left_join(table_left).on(
-                    tgroup.field(f"dd_{field.deepest_level.alias}")
-                    == table_left.field(field.deepest_level.key_column)
-                )
-
-                # User-defined sorting directions for Properties
-                if sort_field is None and query.sorting:
-                    sort_field, sort_order = query.sorting
-                    # TODO: this method could still use a drilldown for sorting, check
-                    field_finder = (Field(column, table=table_enrich)
-                                    for column, alias in field_columns
-                                    if alias == sort_field)
-                    sort_field = next(field_finder, None)
-                    if sort_field is not None:
-                        order = Order.asc if sort_order == "asc" else Order.desc
-                        orderby = chain((sort_field,), orderby)
+            # User-defined sorting directions for Properties
+            if sort_field is None and query.sorting:
+                sort_field, sort_order = query.sorting
+                # TODO: this method could still use a drilldown for sorting, check
+                field_finder = (tcore.field(f"lv_{alias}")
+                                for column, name, alias in _yield_hiefi_columns(hiefi, locale)
+                                if name == sort_field)
+                sort_field = next(field_finder, None)
+                if sort_field is not None:
+                    order = Order.asc if sort_order == "asc" else Order.desc
+                    orderby = chain((sort_field,), orderby)
 
         # User-defined sorting directions for Measures
         if sort_field is None and query.sorting:
             sort_field, sort_order = query.sorting
-            field_finder = (Field(f"ag_{field.alias}", table=tgroup)
-                            for field in query.fields_quantitative
-                            if field.name == sort_field)
+            field_finder = (Field(msrfi.name)
+                            for msrfi in query.fields_quantitative
+                            if msrfi.name == sort_field)
             sort_field = next(field_finder, None)
             if sort_field is not None:
                 order = Order.asc if sort_order == "asc" else Order.desc
                 orderby = chain((sort_field,), orderby)
 
         qb = qb.orderby(*orderby, order=order)
 
         # apply pagination parameters if values are higher than zero
         pag_limit, pag_offset = query.pagination
         if pag_limit > 0:
             qb = qb.limit(pag_limit)
         if pag_offset > 0:
             qb = qb.offset(pag_offset)
 
-        return qb.as_("tdata")
+        return qb.as_("tgroup")
 
     table_core = dataquery_tcore_sql()
     table_group = dataquery_tgroup_sql(table_core)
-    table_data = dataquery_tdata_sql(table_group)
 
-    return table_data, pman.params, external_tables
+    return table_group, pman.params, external_tables
 
 
 def membersquery_sql(
     query: MembersQuery,
 ) -> Tuple[QueryBuilder, Dict[str, str], List[models.InlineTable]]:
     """Build the query which will list all the members of a Level in a dimension
     table.
@@ -343,15 +332,15 @@
 
     table_dim = table_fact \
                 if field.table is None else \
                 _convert_table(field.table, "tdim")
 
     level_columns = tuple(
         (alias, column_name)
-        for column in field.columns
+        for column in field.levels
         for alias, column_name in (
             ("ID", column.level.key_column),
             ("Label", column.level.get_name_column(locale)),
         )
         if column_name is not None
     )
 
@@ -382,72 +371,80 @@
         qb = qb.offset(pagination.offset)
 
     if query.search is not None:
         pname = pman.register(f"%{query.search}%")
         param = PyformatParameter(pname)
         search_criterion = Criterion.any(
             Field(field).ilike(param) # type: ignore
-            for lvlfield in query.hiefield.columns
+            for lvlfield in query.hiefield.levels
             for field in (
-                lvlfield.level.key_column if lvlfield.level.key_type == MemberType.STRING else None,
+                lvlfield.level.key_column
+                    if lvlfield.level.key_type == MemberType.STRING else
+                    None,
                 lvlfield.level.get_name_column(locale),
             )
             if field is not None
         )
         qb = qb.where(search_criterion)
 
     return qb, pman.params, external_tables
 
 
-def _get_aggregate(table: Selectable, item: MeasureField) -> Function:
+def _get_aggregate(table: Selectable, msrfi: MeasureField) -> Union[Function, ArithmeticExpression]:
     """Generates an AggregateFunction instance from a measure, including all its
     parameters, to be used in the SQL query.
     """
-    field = table.field(f"ms_{item.key_alias}")
-    alias = f"ag_{item.alias}"
+    field = table.field(f"ms_{msrfi.alias_key}")
+    # alias = f"ag_{msrfi.alias_name}"
+    alias = msrfi.name
 
-    if item.aggregator_type == "Sum":
+    if msrfi.aggregator_type == "Sum":
         return fn.Sum(field, alias=alias)
 
-    elif item.aggregator_type == "Count":
+    elif msrfi.aggregator_type == "Count":
         return fn.Count(field, alias=alias)
 
-    elif item.aggregator_type == "Average":
+    elif msrfi.aggregator_type == "Average":
         return fn.Avg(field, alias=alias)
 
-    elif item.aggregator_type == "Max":
+    elif msrfi.aggregator_type == "Max":
         return fn.Max(field, alias=alias)
 
-    elif item.aggregator_type == "Min":
+    elif msrfi.aggregator_type == "Min":
         return fn.Min(field, alias=alias)
 
-    elif item.aggregator_type == "Mode":
+    elif msrfi.aggregator_type == "Mode":
         return ArrayElement(TopK(1, field), 1, alias=alias)
 
-    # elif item.aggregator_type == "BasicGroupedMedian":
+    # elif msrfi.aggregator_type == "BasicGroupedMedian":
     #     return fn.Abs()
 
-    # elif item.aggregator_type == "WeightedSum":
+    # elif msrfi.aggregator_type == "WeightedSum":
     #     return fn.Abs()
 
-    # elif item.aggregator_type == "WeightedAverage":
-    #     return fn.Abs()
+    elif msrfi.aggregator_type == "WeightedAverage":
+        params = msrfi.aggregator_params
+        weight_field = params["weight_column"]
+        return AverageWeighted(field, weight_field, alias=alias)
 
-    # elif item.aggregator_type == "ReplicateWeightMoe":
+    # elif msrfi.aggregator_type == "ReplicateWeightMoe":
     #     return fn.Abs()
 
-    # elif item.aggregator_type == "CalculatedMoe":
-    #     return fn.Abs()
+    elif msrfi.aggregator_type == "CalculatedMoe":
+        params = msrfi.aggregator_params
+        critical_value = params["critical_value"]
+        term = fn.Sqrt(fn.Sum(Power(field / critical_value, 2)))
+        return ArithmeticExpression(Arithmetic.mul, term, critical_value, alias=alias)
 
-    # elif item.aggregator_type == "WeightedAverageMoe":
+    # elif msrfi.aggregator_type == "WeightedAverageMoe":
     #     return fn.Abs()
 
     raise NameError(
         f"Clickhouse module not prepared to handle aggregation type: "
-        f"{item.aggregator_type}"
+        f"{msrfi.aggregator_type}"
     )
 
 
 def _get_filter_criterion(field: Field, constr: NumericConstraint):
     comparison, scalar = constr
 
     if comparison == Comparison.GT:
@@ -462,25 +459,29 @@
         return field.eq(scalar)
     elif comparison == Comparison.NEQ:
         return field.ne(scalar)
 
     raise NameError(f"Invalid criterion type: {comparison}")
 
 
-def _yield_drilldown_columns(field: HierarchyField, locale: str):
+def _yield_hiefi_columns(hiefi: HierarchyField, locale: str):
     """Generates pairs of (column name, column alias) for all fields related to
     a HierarchyField object.
 
     This comprises Drilldown Labels and IDs, and its requested Properties.
     """
-    for item in field.columns_drilldown:
-        name = item.level.name
-        key_column = item.level.key_column
-        name_column = item.level.get_name_column(locale)
-        if name_column is None:
-            yield key_column, name
-        else:
-            yield key_column, f"{name} ID"
-            yield name_column, name
-        for propty in item.properties:
-            propty_column = propty.get_key_column(locale)
-            yield propty_column, propty.name
+    for lvlfi in hiefi.drilldown_levels:
+        yield from _yield_lvlfi_columns(lvlfi, locale)
+
+
+def _yield_lvlfi_columns(lvlfi: LevelField, locale: str):
+    name = lvlfi.level.name
+    key_column = lvlfi.level.key_column
+    name_column = lvlfi.level.get_name_column(locale)
+    if name_column is None:
+        yield key_column, name, shorthash(name + key_column)
+    else:
+        yield key_column, f"{name} ID", shorthash(name + key_column)
+        yield name_column, name, shorthash(name + name_column)
+    for propty in lvlfi.properties:
+        propty_column = propty.get_key_column(locale)
+        yield propty_column, propty.name, shorthash(propty.name + propty_column)
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/backend/exceptions.py` & `tesseract_olap-0.7.0/tesseract_olap/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.6.0/tesseract_olap/backend/models.py` & `tesseract_olap-0.7.0/tesseract_olap/backend/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,28 +2,23 @@
 
 This module contains abstract definitions for the interfaces of the Backend
 class. Tesseract is compatible with any kind of data source as long as there's a
 backend class that adapts the Query and the Results to the defined interface.
 """
 
 import abc
-import uuid
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, AsyncGenerator, Dict, Optional, Union
 
-from tesseract_olap.common import AnyDict
+from tesseract_olap.common import AnyDict, shorthash
 
 if TYPE_CHECKING:
     from tesseract_olap.query import DataQuery, MembersQuery
     from tesseract_olap.schema import SchemaTraverser
 
-def random_string():
-    """Generates a string composed from 8 random numbers and letters."""
-    return str(uuid.uuid4())[:8]
-
 
 class Backend(abc.ABC):
     """Base class for database backends compatible with Tesseract."""
 
     @abc.abstractmethod
     async def connect(self, **kwargs):
         """Establishes the connection to the backend server.
@@ -86,10 +81,10 @@
     """
     params: Dict[str, str] = field(default_factory=dict)
 
     def register(self, value: str, key: Optional[str] = None) -> str:
         """Stores a new named parameter value.
         If not provided, also generates the parameter name.
         """
-        key = f"p{random_string()}" if key is None else key
+        key = f"p_{shorthash(value)}" if key is None else key
         self.params[key] = value
         return key
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/logiclayer/dependencies.py` & `tesseract_olap-0.7.0/tesseract_olap/logiclayer/dependencies.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.6.0/tesseract_olap/logiclayer/module.py` & `tesseract_olap-0.7.0/tesseract_olap/logiclayer/module.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 from typing import Optional, Union
 
 import logiclayer as ll
 from fastapi import Depends, HTTPException, Request
 from fastapi.responses import FileResponse, RedirectResponse
 
 from tesseract_olap import __version__ as tesseract_version
-from tesseract_olap.backend.exceptions import BackendError
+from tesseract_olap.exceptions import TesseractError
 from tesseract_olap.query import DataRequest, MembersRequest
-from tesseract_olap.query.exceptions import QueryError
 from tesseract_olap.server import OlapServer
 
 from .dependencies import dataquery_params, membersquery_params
 from .response import StreamingJSONResponse
 
 
 class TesseractModule(ll.LogicLayerModule):
@@ -41,103 +40,138 @@
         """Creates a new :class:`TesseractModule` instance from the strings with
         the path to the schema file (or the schema content itself), and with the
         connection string to the backend.
         """
         server = OlapServer(connection, schema)
         return cls(server)
 
+
     @ll.healthcheck
     def healthcheck(self):
         return self.server.ping()
 
     @ll.on_startup
     async def event_startup(self):
         await self.server.connect()
 
     @ll.on_shutdown
     async def event_shutdown(self):
         await self.server.disconnect()
 
+
     @ll.route("GET", "/")
     async def status(self):
         """Pings the backend configured in the tesseract server."""
         beat = await self.server.ping()
         return {
             "status": "ok" if beat else "error",
             "software": "tesseract-olap[python]",
             "version": tesseract_version,
         }
 
+
     @ll.route("GET", "/cubes")
-    def public_schema(self, locale: Optional[str] = None):
+    def public_schema(
+        self,
+        locale: Optional[str] = None,
+    ):
+        """Returns the public schema with all the available cubes."""
         return self.server.schema.get_public_schema(locale=locale)
 
     @ll.route("GET", "/cubes/{cube_name}")
-    def public_schema_cube(self, cube_name: str, locale: Optional[str] = None):
+    def public_schema_cube(
+        self,
+        cube_name: str,
+        locale: Optional[str] = None,
+    ):
+        """Returns the public schema for the single specified cube."""
         locale = self.server.schema.default_locale if locale is None else locale
         cube = self.server.schema.get_cube(cube_name)
         return cube.get_public_schema(locale=locale)
 
-    @ll.route(["HEAD", "GET"], "/data", response_class=RedirectResponse)
-    def query_data_default(self, request: Request):
+
+    @ll.route(["HEAD", "GET"], "/data",
+        name="redirect_data",
+        response_class=RedirectResponse)
+    def query_data_default(
+        self,
+        request: Request,
+    ):
+        """Redirects the request to the canonical endpoint in jsonrecords format."""
         return f"{request.url.path}.jsonrecords?{request.url.query}"
 
-    @ll.route(["HEAD", "GET"], "/members", response_class=RedirectResponse)
-    def query_members_default(self, request: Request):
+    @ll.route(["HEAD", "GET"], "/members",
+        name="redirect_members",
+        response_class=RedirectResponse)
+    def query_members_default(
+        self,
+        request: Request,
+    ):
+        """Redirects the request to the canonical endpoint in jsonrecords format."""
         return f"{request.url.path}.jsonrecords?{request.url.query}"
 
-    @ll.route("GET", "/data.{filetype}", response_class=StreamingJSONResponse)
+
+    @ll.route("GET", "/data.{filetype}",
+        name="route_data",
+        response_class=StreamingJSONResponse)
     async def query_data(
         self,
-        filetype: str = "jsonrecords",
+        filetype: str,
         query: DataRequest = Depends(dataquery_params),
     ):
         try:
             result = await self.server.execute(query)
-        except QueryError as exc:
-            raise HTTPException(status_code=400, detail=exc.message) from None
-        except BackendError as exc:
+        except TesseractError as exc:
             raise HTTPException(status_code=exc.code, detail=exc.message) from None
-        return StreamingJSONResponse({
-            "data": result,
-            "format": filetype,
-            "sources": result.sources,
-        })
-
-    @ll.route("GET", "/members.{filetype}", response_class=StreamingJSONResponse)
+        else:
+            return StreamingJSONResponse({
+                "data": result,
+                "format": filetype,
+                "sources": result.sources,
+            })
+
+    @ll.route("GET", "/members.{filetype}",
+        name="route_members",
+        response_class=StreamingJSONResponse)
     async def query_members(
         self,
-        filetype: str = "jsonrecords",
+        filetype: str,
         query: MembersRequest = Depends(membersquery_params),
     ):
         try:
             result = await self.server.execute(query)
-        except QueryError as exc:
-            raise HTTPException(status_code=400, detail=exc.message) from None
-        except BackendError as exc:
+        except TesseractError as exc:
             raise HTTPException(status_code=exc.code, detail=exc.message) from None
-        return StreamingJSONResponse({
-            "data": result,
-            "format": filetype,
-        })
+        else:
+            return StreamingJSONResponse({
+                "data": result,
+                "format": filetype,
+            })
+
 
     @ll.route("GET", "/debug/schema", debug=True)
     def debug_schema(self):
         return dataclasses.asdict(self.server.raw_schema)
 
     @ll.route("GET", "/debug/download_logs", debug=True)
-    def debug_logs_download(self, filename: str):
+    def debug_logs_download(
+        self,
+        filename: str,
+    ):
         filename = Path(filename).name
         if not filename.endswith(".log"):
             raise HTTPException(401, "File not allowed")
         filepath = Path.cwd().joinpath(filename).resolve()
         return FileResponse(filepath, media_type="text/plain", filename=filename)
 
     @ll.route("GET", "/debug/clear_logs", debug=True)
-    def debug_logs_clear(self, filename: str):
+    def debug_logs_clear(
+        self,
+        filename: str,
+    ):
         filename = Path(filename).name
         if not filename.endswith(".log"):
             raise HTTPException(401, "File not allowed")
         filepath = Path.cwd().joinpath(filename).resolve()
         with filepath.open("w", encoding="utf-8") as fileio:
             fileio.write("")
         return
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/logiclayer/response.py` & `tesseract_olap-0.7.0/tesseract_olap/logiclayer/response.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.6.0/tesseract_olap/query/__init__.py` & `tesseract_olap-0.7.0/tesseract_olap/query/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.6.0/tesseract_olap/query/calculations.py` & `tesseract_olap-0.7.0/tesseract_olap/query/calculations.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.6.0/tesseract_olap/query/enums.py` & `tesseract_olap-0.7.0/tesseract_olap/query/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.6.0/tesseract_olap/query/exceptions.py` & `tesseract_olap-0.7.0/tesseract_olap/query/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Optional
 
 from tesseract_olap.common import BaseError
 
 
 class QueryError(BaseError):
     """Base class for exceptions in `tesseract_olap.query` module."""
+    code = 400
 
 
 class InvalidQuery(QueryError):
     """This error occurs when a query is misconstructed.
 
     Can be raised before or after a request is made against a data server.
     """
@@ -73,15 +74,26 @@
         )
 
 
 class InvalidFormat(QueryError):
     """This error occurs when a format used to retrieve data is not supported by
     the upstream server.
 
-    Should be raised before the target url to contact with the upstream server
-    is built.
+    Should be raised before the query is executed against the upstream server.
     """
 
     def __init__(self, extension: str) -> None:
         super().__init__(
             f"Format '{extension}' is not supported by the server."
         )
+
+
+class NotAuthorized(QueryError):
+    """The roles provided don't match the roles needed to access some of the
+    requested parameters.
+
+    Should be raised before the query is executed against the upstream server.
+    """
+    code = 403
+
+    def __init__(self) -> None:
+        super().__init__("Request doesn't count with the necessary permissions.")
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/query/models.py` & `tesseract_olap-0.7.0/tesseract_olap/query/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """Query-related internal structs module.
 
 This module contains data-storing structs, used mainly on the query and backend
 modules.
 """
 
 import dataclasses
-from functools import lru_cache
-from hashlib import md5
 from typing import (Dict, FrozenSet, Iterable, NamedTuple, Optional, Set,
                     Tuple, Union)
 
 from typing_extensions import Literal
 
-from tesseract_olap.common import Array, Prim
+from tesseract_olap.common import Array, Prim, shorthash
 from tesseract_olap.schema import (DimensionTraverser, HierarchyTraverser,
                                    LevelTraverser, Measure, PropertyTraverser)
 
 from .enums import (Comparison, LogicOperator, Membership, Order,
                     RestrictionAge, RestrictionScale)
 
 NumericConstraint = Tuple[Union[Comparison, str], float]
@@ -174,43 +172,43 @@
 @dataclasses.dataclass(eq=True, frozen=True, order=False)
 class HierarchyField:
     """Contains the parameters associated to a slicing operation on the data,
     based on a single Hierarchy from a Cube's Dimension.
     """
     dimension: "DimensionTraverser"
     hierarchy: "HierarchyTraverser"
-    columns: Tuple["LevelField", ...]
+    levels: Tuple["LevelField", ...]
 
     @property
-    def columns_cut(self) -> Iterable["LevelField"]:
-        return (item for item in self.columns if item.is_cut)
+    def cut_levels(self) -> Iterable["LevelField"]:
+        return (item for item in self.levels if item.is_cut)
 
     @property
-    def columns_drilldown(self) -> Iterable["LevelField"]:
-        return (item for item in self.columns if item.is_drilldown)
+    def drilldown_levels(self) -> Iterable["LevelField"]:
+        return (item for item in self.levels if item.is_drilldown)
 
     @property
     def deepest_level(self) -> "LevelField":
         """Returns the deepest LevelField requested in this Hierarchy, for this
         query operation."""
         # TODO: check if is needed to force this to use drilldowns only
-        return self.columns[-1]
+        return self.levels[-1]
 
     @property
     def foreign_key(self) -> str:
         """Returns the column in the fact table of the Cube this Dimension
         belongs to, that matches the primary key of the items in the dim_table.
         """
         return self.dimension.foreign_key  # type: ignore
 
     @property
-    def is_drilldown(self) -> bool:
+    def has_drilldowns(self) -> bool:
         """Verifies if any of the contained LevelFields is being used as a
         drilldown."""
-        return any(self.columns_drilldown)
+        return any(self.drilldown_levels)
 
     @property
     def primary_key(self) -> str:
         """Returns the column in the dimension table for the parent Dimension,
         which is used as primary key for the whole set of levels in the chosen
         Hierarchy."""
         return self.hierarchy.primary_key
@@ -234,15 +232,15 @@
     members_include: Set[str] = dataclasses.field(default_factory=set)
     properties: FrozenSet["PropertyTraverser"] = dataclasses.field(default_factory=frozenset)
     time_restriction: Optional[TimeRestriction] = None
 
     @property
     def alias(self):
         """Returns a deterministic short hash of the name of the entity."""
-        return shorthash(self.level.name)
+        return shorthash(self.level.name + self.level.key_column)
 
     @property
     def is_cut(self) -> bool:
         return len(self.members_exclude) + len(self.members_include) > 0
 
     @property
     def key_column(self) -> str:
@@ -263,20 +261,20 @@
     measure: "Measure"
     is_measure: bool = False
     constraint1: Optional[NumericConstraint] = None
     constraint2: Optional[NumericConstraint] = None
     joint: LogicOperator = LogicOperator.AND
 
     @property
-    def alias(self):
+    def alias_name(self):
         """Returns a deterministic short hash of the name of the entity."""
         return shorthash(self.measure.name)
 
     @property
-    def key_alias(self):
+    def alias_key(self):
         """Returns a deterministic hash of the key column of the entity."""
         return shorthash(self.measure.key_column)
 
     @property
     def is_filter(self) -> bool:
         return self.constraint1 is not None
 
@@ -295,12 +293,7 @@
         """Quick method to retrieve the measure aggregator type."""
         return str(self.measure.aggregator)
 
     def get_source(self):
         # TODO add locale compatibility
         """Quick method to obtain the source information of the measure."""
         return self.measure.annotations.get("source")
-
-
-@lru_cache(128)
-def shorthash(string: str):
-    return str(md5(string.encode("utf-8")).hexdigest())[:8]
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/query/queries.py` & `tesseract_olap-0.7.0/tesseract_olap/query/queries.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 This module contains data structs used to carry and compose objects used during
 a Query. The elements are agnostic to the type of backend used, and its primary
 purpose is organize and easily obtain the data needed for later steps.
 """
 
 from collections import defaultdict
 from dataclasses import dataclass, field
+from itertools import chain
 from typing import List, Mapping, Optional, Set, Tuple, Union
 
 import immutables as immu
 
 from tesseract_olap.common import AnyDict
 from tesseract_olap.schema import (CubeTraverser, DimensionTraverser,
-                                   HierarchyTraverser, LevelTraverser,
+                                   HierarchyTraverser, LevelTraverser, Measure,
                                    SchemaTraverser)
 
 from .enums import LogicOperator, RestrictionScale
-from .exceptions import InvalidEntityName
+from .exceptions import InvalidEntityName, NotAuthorized
 from .models import (CutIntent, HierarchyField, LevelField, MeasureField,
                      PaginationIntent, SortingIntent)
 from .requests import DataRequest, MembersRequest
 
 
 @dataclass(eq=False, order=False)
 class DataQuery:
@@ -47,14 +48,17 @@
         in a :class:`DataRequest` object.
 
         If any of the parameters can't be found on the Schema, raises a derivate
         of the :class:`InvalidQuery` error.
         """
         cube = schema.get_cube(request.cube)
 
+        if not cube.is_authorized(request.roles):
+            raise NotAuthorized()
+
         return cls(
             cube=cube,
             fields_qualitative=_get_data_hierarfields(cube, request),
             fields_quantitative=_get_data_measurefields(cube, request),
             locale=schema.default_locale \
                    if request.locale is None else \
                    request.locale,
@@ -137,15 +141,18 @@
     # the 'single dimension, same hierarchy' rule
     dimension_store: Mapping[DimensionTraverser, HierarchyTraverser] = {}
     hierarchy_store: Mapping[HierarchyTraverser, List[LevelTraverser]] = defaultdict(list)
 
     for name in involved_levels:
         dimension, hierarchy, level = level_map[name]
         if dimension_store.get(dimension, hierarchy) != hierarchy:
-            raise ValueError("Multiple Hierarchies from the same Dimension are being requested. Only a single Hierarchy can be used at a time for a query.")
+            raise ValueError(
+                "Multiple Hierarchies from the same Dimension are being requested. "
+                "Only a single Hierarchy can be used at a time for a query."
+            )
         dimension_store[dimension] = hierarchy
         hierarchy_store[hierarchy].append(level)
 
     # Apply default members
     for dimension in cube.dimensions:
         hierarchy = dimension_store.get(dimension, dimension.default_hierarchy)
 
@@ -210,37 +217,54 @@
                 (with_parents is not False and level.name in with_parents)
             )
 
         fields.reverse()
         return tuple(fields)
 
     return tuple(
-        HierarchyField(dimension, hierarchy, columns=_resolve_fields(hierarchy))
+        HierarchyField(dimension, hierarchy, levels=_resolve_fields(hierarchy))
         for dimension, hierarchy in (
             sorted(dimension_store.items(), key=lambda item: item[0].name)
         )
     )
 
 
 def _get_data_measurefields(cube: "CubeTraverser", req: "DataRequest"):
     """Regroups query parameters related to a Measure, to simplify contextual use.
     """
     measure_set = req.measures
 
-    involved_measures = req.measures.copy()
-    involved_measures.update(item.field for item in req.filters.values())
+    measure_map = immu.Map(
+        (item.name, item)
+        for measure in cube.measure_map.values()
+        for item in _yield_all_measures(measure)
+    )
+
+    try:
+        involved_measures = set(measure_map[name] for name in chain(
+            req.measures,
+            (item.field for item in req.filters.values()),
+        ))
+    except KeyError as exc:
+        raise InvalidEntityName("Measure", exc.args[0]) from None
+
+    involved_submeasures = set(
+        submeasure
+        for measure in involved_measures
+        for submeasure in measure.submeasures.values()
+    )
+    involved_measures.update(involved_submeasures)
 
-    def _compose_field(measure_name: str) -> "MeasureField":
-        measure = cube.get_measure(measure_name)
+    def _compose_field(measure: "Measure") -> "MeasureField":
         kwargs = {
-            "is_measure": measure_name in measure_set,
+            "is_measure": measure.name in measure_set,
             "constraint1": None,
         }
 
-        fltr = req.filters.get(measure_name)
+        fltr = req.filters.get(measure.name)
         if fltr is None:
             pass
         elif len(fltr.condition) == 1: # is (NumConstr)
             kwargs["constraint1"] = fltr.condition[0]
         elif len(fltr.condition) == 3: # is (NumConstr, LogicOp, NumConstr)
             kwargs["constraint1"] = fltr.condition[0]
             kwargs["joint"] = LogicOperator.from_str(fltr.condition[1])
@@ -268,8 +292,14 @@
     if with_parents:
         levels = tuple(hierarchy.levels)
         last_index = levels.index(level)
         fields = tuple(LevelField(level) for level in levels[0:last_index])
     else:
         fields = LevelField(level),
 
-    return HierarchyField(dimension, hierarchy, columns=fields)
+    return HierarchyField(dimension, hierarchy, levels=fields)
+
+
+def _yield_all_measures(measure: "Measure"):
+    yield measure
+    for submeasure in measure.submeasures.values():
+        yield submeasure
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/query/requests.py` & `tesseract_olap-0.7.0/tesseract_olap/query/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     cuts_exclude: Mapping[str, Array[str]]
     cuts_include: Mapping[str, Array[str]]
     filters: Mapping[str, Union[SingleFilterCondition, DoubleFilterCondition]]
     locale: str
     pagination: Union[str, Tuple[int, int]]
     parents: Union[bool, Array[str]]
     properties: Array[str]
+    roles: Array[str]
     sorting: Tuple[str, Literal["asc", "desc"]]
     time: str
 
 
 class DataRequestParams(DataRequestOptionalParams, total=True):
     """DataRequestParams interface.
 
@@ -72,14 +73,15 @@
     cuts: Mapping[str, "CutIntent"] = field(default_factory=dict)
     filters: Mapping[str, "FilterIntent"] = field(default_factory=dict)
     locale: Optional[str] = None
     options: Mapping[str, bool] = field(default_factory=dict)
     pagination: "PaginationIntent" = field(default_factory=PaginationIntent)
     parents: Union[bool, Set[str]] = False
     properties: Set[str] = field(default_factory=set)
+    roles: Set[str] = field(default_factory=set)
     sorting: Optional["SortingIntent"] = None
     time_restriction: Optional["TimeRestriction"] = None
 
     @classmethod
     def new(cls, cube: str, request: DataRequestParams):
         """Creates a new :class:`DataRequest` instance from a set of parameters
         defined in a dict.
@@ -88,14 +90,15 @@
         require the use of internal dataclasses and the setup of internal
         structures and unique conditions.
         """
 
         cuts_include = request.get("cuts_include", {})
         cuts_exclude = request.get("cuts_exclude", {})
         filters = request.get("filters", {})
+        roles = request.get("roles", [])
 
         kwargs = {
             "locale": request.get("locale"),
             "cuts": {
                 item: CutIntent.new(level=item,
                                     incl=cuts_include.get(item, []),
                                     excl=cuts_exclude.get(item, []))
@@ -106,29 +109,30 @@
             "filters": {
                 item: FilterIntent.new(field=item, condition=condition)
                 for item, condition in filters.items()
             },
             "captions": set(request.get("captions", [])),
             "properties": set(request.get("properties", [])),
             "options": {},
+            "roles": set(roles) if isinstance(roles, (list, tuple)) else roles
         }
 
         item = request.get("pagination", (0, 0))
         if isinstance(item, str):
             kwargs["pagination"] = PaginationIntent.from_str(item)
         elif isinstance(item, (list, tuple)):
             kwargs["pagination"] = PaginationIntent(*item)
 
         item = request.get("parents", False)
         if isinstance(item, (set, bool)):
             kwargs["parents"] = item
-        elif isinstance(item, str):
-            kwargs["parents"] = {item}
         elif isinstance(item, (list, tuple)):
             kwargs["parents"] = set(item)
+        elif isinstance(item, str):
+            kwargs["parents"] = {item}
 
         item = request.get("sorting")
         if isinstance(item, str):
             kwargs["sorting"] = SortingIntent.from_str(item)
         elif isinstance(item, (list, tuple)):
             kwargs["sorting"] = SortingIntent.new(*item)
 
@@ -179,14 +183,15 @@
     """
 
     cube: str
     level: str
     locale: Optional[str] = None
     options: Mapping[str, bool] = field(default_factory=dict)
     pagination: "PaginationIntent" = field(default_factory=PaginationIntent)
+    roles: Set[str] = field(default_factory=set)
     search: Optional[str] = None
 
     @classmethod
     def new(cls, cube: str, request: MembersRequestParams):
         """Creates a new :class:`MembersRequest` instance from a set of parameters
         defined in a dict.
 
@@ -194,18 +199,22 @@
         require the use of internal dataclasses and the setup of internal
         structures and unique conditions.
         """
 
         item = request.get("pagination", (0, 0))
         pagination = PaginationIntent(*item)
 
+        item = request.get("roles", [])
+        roles = set(item) if isinstance(item, (list, tuple)) else item
+
         return cls(
             cube=cube,
             level=request["level"],
             locale=request.get("locale"),
             options={
                 "parents": request.get("parents", False),
                 "children": request.get("children", False),
             },
             pagination=pagination,
+            roles=roles,
             search=request.get("search"),
         )
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/query/results.py` & `tesseract_olap-0.7.0/tesseract_olap/query/results.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 """Result structs module
 
 This module contains wrapper classes for the resulting data of queries obtained
 for structs in the requests module.
 """
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import AsyncIterator, Optional
 
 from tesseract_olap.common import AnyDict, Array
 
 from .requests import DataRequest, MembersRequest
 
 
 @dataclass(eq=False, order=False)
 class DataResult:
     """Container class for results to :class:`DataRequest`."""
     first: Optional[AnyDict]
     iterator: AsyncIterator[AnyDict]
     sources: Array[AnyDict]
     query: DataRequest
+    _use_iterator: bool = field(default=False, init=False, repr=False, compare=False)
 
     def __aiter__(self):
         return self
 
     async def __anext__(self):
-        if hasattr(self, "_use_iterator"):
+        if self._use_iterator:
             return await self.iterator.__anext__()
 
-        setattr(self, "_use_iterator", True)
+        self._use_iterator = True
 
         if self.first is None:
             raise StopAsyncIteration()
 
         return self.first
 
 
 @dataclass(eq=False, order=False)
 class MembersResult:
     """Container class for results to :class:`MembersRequest`."""
     first: Optional[AnyDict]
     iterator: AsyncIterator[AnyDict]
     query: MembersRequest
+    _use_iterator: bool = field(default=False, init=False, repr=False, compare=False)
 
     def __aiter__(self):
         return self
 
     async def __anext__(self):
-        if hasattr(self, "_use_iterator"):
+        if self._use_iterator:
             return await self.iterator.__anext__()
 
-        setattr(self, "_use_iterator", True)
+        self._use_iterator = True
 
         if self.first is None:
             raise StopAsyncIteration()
 
         return self.first
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/schema/__init__.py` & `tesseract_olap-0.7.0/tesseract_olap/schema/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from .aggregators import Aggregator
+from .csv import parse_csv_schema
 from .enums import AggregatorType, DimensionType, MemberType
-from .models import (Cube, Dimension, DimensionUsage, Entity, Hierarchy,
-                     HierarchyUsage, InlineTable, Level, LevelUsage, Measure,
-                     Property, PropertyUsage, Schema, Table)
+from .json import parse_json_schema
+from .models import (AccessControl, Cube, Dimension, DimensionUsage, Entity,
+                     Hierarchy, HierarchyUsage, InlineTable, Level, LevelUsage,
+                     Measure, Property, PropertyUsage, Schema, Table)
 from .traverse import (CubeTraverser, DimensionTraverser, HierarchyTraverser,
                        LevelTraverser, PropertyTraverser, SchemaTraverser)
 from .xml import parse_xml_schema
 
 __all__ = (
+    "AccessControl",
     "Aggregator",
     "AggregatorType",
     "Cube",
     "CubeTraverser",
     "Dimension",
     "DimensionTraverser",
     "DimensionType",
@@ -22,14 +25,16 @@
     "HierarchyUsage",
     "InlineTable",
     "Level",
     "LevelTraverser",
     "LevelUsage",
     "Measure",
     "MemberType",
+    "parse_csv_schema",
+    "parse_json_schema",
     "parse_xml_schema",
     "Property",
     "PropertyTraverser",
     "PropertyUsage",
     "Schema",
     "SchemaTraverser",
     "Table",
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/schema/aggregators.py` & `tesseract_olap-0.7.0/tesseract_olap/schema/aggregators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Schema Aggregators module.
 
 Contains the different types of aggregator that can be used in the definition of
 a Measure in the Schema.
 """
 
-import abc
 import dataclasses
 from typing import Dict, List, Set
 
 from .enums import AggregatorType
 
 
-class Aggregator(abc.ABC):
+class Aggregator:
     """Base class for aggregator methods.
 
     The instances contain parameters to compose the associated SQL query.
     Backend packages should extend these according to support, and implement
     the methods needed for conversion to string.
     """
     def __init__(self) -> None:
@@ -42,15 +41,15 @@
         """Returns a dict with the serialized params of the instance.
 
         Base class just returns an empty dict. More complex subclasses must
         override this method."""
         return {}
 
     @classmethod
-    def new(cls, kwargs: dict) -> "Aggregator":
+    def new(cls, kwargs: Dict[str, str]) -> "Aggregator":
         field_names = cls.get_fields()
         return cls(**{k: v for k, v in kwargs.items() if k in field_names})
 
     @staticmethod
     def from_enum(enum: AggregatorType) -> "Aggregator":
         agg_classes = {
             AggregatorType.SUM: Sum,
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/schema/csv.py` & `tesseract_olap-0.7.0/tesseract_olap/schema/csv.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,68 @@
 import csv
 from email.message import Message
-from typing import Generator, Iterable, List, Sequence, Tuple, Union
+from pathlib import Path
+from typing import Generator, Iterable, List, Sequence, TextIO, Tuple, Union
 
-DELIMITER_TRANSLATE = {
+import immutables as immu
+
+from tesseract_olap.common import is_numeric, numerify
+
+from . import models
+
+DELIMITER_TRANSLATE = immu.Map({
     "comma": ",",
     "semicolon": ";",
     "tab": "\t",
     "space": " ",
-}
+})
+
+
+class ColumnTypeInferrer:
+    def __init__(self, iterable: Iterable[str], csv_params: dict):
+        self.csv_params = csv_params
+        self.headers = ""
+        self.iterator = iter(iterable)
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        row = next(self.iterator)
+        if self.headers:
+            row_items = next(csv.reader([row], **self.csv_params))
+            self.types = [
+                itype and is_numeric(item)
+                for item, itype in zip(row_items, self.types)
+            ]
+        else:
+            self.headers = list(csv.reader(row))
+            self.types = [True for item in self.headers]
+        return row
+
+    def cast(
+        self, table: Iterable[Sequence[str]],
+    ) -> Generator[Tuple[Union[float, str],...], None, None]:
+        iterator = iter(table)
+        yield tuple(next(iterator))
+        yield from (
+            tuple(
+                numerify(item) if is_num else item
+                for item, is_num in zip(row, self.types)
+            )
+            for row in iterator
+        )
+
+
+class CSVSchema(models.Schema):
+    pass
+
+
+class CSVInlineTable(models.InlineTable):
+    pass
 
 
 def parse_csv(
     content: Iterable[str],
     *,
     dialect: Union[str, csv.Dialect] = "",
     mimetype: str = "",
@@ -42,45 +93,32 @@
         kwargs["delimiter"] = DELIMITER_TRANSLATE.get(delimiter, delimiter)
 
     content = ColumnTypeInferrer(content, kwargs)
     table = tuple(csv.reader(content, **kwargs))
     return list(content.cast(table))
 
 
-class ColumnTypeInferrer:
-    def __init__(self, iterable: Iterable[str], csv_params: dict):
-        self.csv_params = csv_params
-        self.headers = ""
-        self.iterator = iter(iterable)
-
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        row = next(self.iterator)
-        if self.headers:
-            row_items = next(csv.reader([row], **self.csv_params))
-            self.types = [
-                itype and item.isnumeric()
-                for item, itype in zip(row_items, self.types)
-            ]
-        else:
-            self.headers = list(csv.reader(row))
-            self.types = [True for item in self.headers]
-        return row
-
-    def cast(
-        self, table: Iterable[Sequence[str]],
-    ) -> Generator[Tuple[Union[float, str],...], None, None]:
-        iterator = iter(table)
-        yield tuple(next(iterator))
-        yield from (
-            tuple(
-                numerify(item) if is_num else item
-                for item, is_num in zip(row, self.types)
-            )
-            for row in iterator
-        )
-
-
-def numerify(string: str):
-    return int(string) if int(string) == float(string) else float(string)
+def parse_csv_schema(source: Union[str, Path, TextIO], name: str = "") -> "CSVSchema":
+    if isinstance(source, Path):
+        name = source.name.replace(source.suffix, "")
+        with source.open("r") as io:
+            headers, *rows = parse_csv(line for line in io)
+
+    elif isinstance(source, TextIO):
+        name = source.name
+        headers, *rows = parse_csv(source.readlines())
+        source.close()
+
+    else:
+        headers, *rows = parse_csv(source)
+
+    table = CSVInlineTable(
+        name=name,
+        headers=tuple(str(item) for item in headers),
+        types=CSVInlineTable.infer_types(rows),
+        rows=rows,
+    )
+
+    return CSVSchema(
+        name="",
+        shared_table_map=immu.Map([(table.name, table)])
+    )
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/schema/enums.py` & `tesseract_olap-0.7.0/tesseract_olap/schema/enums.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,30 +72,24 @@
         if value is None:
             return cls.INT64
         value = value.lower()
         return next((item for item in cls if item.value == value), cls.INT64)
 
     @classmethod
     def from_values(cls, values: Sequence[Any]):
-        value = values[0]
+        types = frozenset(type(value) for value in values)
 
-        if isinstance(value, bool):
+        if len(types) == 1 and bool in types:
             return MemberType.BOOLEAN
 
-        if isinstance(value, int):
-            return cls.from_int_values(values)
-
-        if isinstance(value, float):
+        if float in types:
             return MemberType.FLOAT64
 
-        if isinstance(value, str):
-            if value.isnumeric():
-                if int(value) == float(value):
-                    return cls.from_int_values([int(i) for i in values])
-                return MemberType.FLOAT64
+        if int in types:
+            return cls.from_int_values(values)
 
         return MemberType.STRING
 
     @classmethod
     def from_int_values(cls, values: Sequence[int]):
         mini = min(values)
         maxi = max(values)
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/schema/exceptions.py` & `tesseract_olap-0.7.0/tesseract_olap/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.6.0/tesseract_olap/schema/json.py` & `tesseract_olap-0.7.0/tesseract_olap/schema/json.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from functools import lru_cache
 from pathlib import Path
-from typing import Callable, Dict, TextIO, TypeVar, Union
+from typing import Callable, Dict, TextIO, Union
 
-import httpx
 import orjson
 
+from tesseract_olap.common import T
+
 from . import models
 
 
 class JSONSchema(models.Schema):
     @classmethod
     def parse(cls, root: dict):
+        raise NotImplementedError("Parsing for JSONSchema is not yet available.")
 
         cubes_mapper = _mapper_factory("cubes", "name", JSONCube.parse)
         dimensions_mapper = _mapper_factory("dimensions", "name", JSONDimension.parse)
         tables_mapper = _mapper_factory("inline_tables", "name", JSONInlineTable.parse)
 
         return cls(
             name=root["name"],
@@ -26,36 +28,27 @@
             default_locale=root.get("default_locale", "xx"),
         )
 
 
 class JSONCube(models.Cube):
     @classmethod
     def parse(cls, root: dict):
-        return cls(
-            name
-        )
+        raise NotImplementedError()
 
 
 class JSONDimension(models.Dimension):
     @classmethod
     def parse(cls, root: dict):
-        return cls(
-            name
-        )
+        raise NotImplementedError()
 
 
 class JSONInlineTable(models.InlineTable):
     @classmethod
     def parse(cls, root: dict):
-        return cls(
-            name
-        )
-
-
-T = TypeVar('T')
+        raise NotImplementedError()
 
 
 @lru_cache(10)
 def _mapper_factory(
     parent_obj: str,
     property_name: str,
     reducer: Callable[[dict], T],
@@ -67,47 +60,32 @@
             item[property_name]: reducer(item)
             for item in root.get(parent_obj, [])
         }
 
     return mapper_func
 
 
-def _parse_pathlib_path(path: Path) -> JSONSchema:
-    pass
+def parse_json_schema(source: Union[str, Path, TextIO]) -> JSONSchema:
+    """Attempts to parse an object into a JSONSchema.
 
+    This function accepts:
+    - A raw JSON :class:`str`
+    - A local path (as a :class:`pathlib.Path`) to a JSON file
+    - A not-binary read-only :class:`TextIO` instance for a file-like object
+    """
+    contents: Union[str, bytes]
 
-async def parse_json_schema(source: Union[str, Path, TextIO]) -> JSONSchema:
-    if isinstance(source, str):
-        # Check if argument is a URL and fetch the file
-        if source.lstrip().startswith("http"):
-            with httpx.AsyncClient() as client:
-                response = await client.get(source)
-                response.raise_for_status()
-
-            root = orjson.loads(response.content)
-
-        # Check if argument is a file path and load the file
-        elif source.rstrip().endswith(".json"):
-            path = Path(source).resolve()
-            if not path.exists():
-                raise FileNotFoundError("JSON schema: Path '{}' does not exist".format(path))
-
-            if path.is_file():
-                with path.open("rb") as f:
-                    root = orjson.loads(f.read())
-            else:
-                # TODO: enable traversing all JSON files in a directory
-                raise IsADirectoryError("JSON schema: Path must point to a single file")
-
-        # Check if argument is a raw XML string
-        elif source.lstrip().startswith("{"):
-            root = orjson.loads(source)
-
-        else:
-            raise ValueError("JSON schema: Source can't be recognized")
+    # if argument is pathlib.Path, resolve its contents
+    if isinstance(source, Path):
+        contents = source.read_bytes()
+
+    # if argument is a file-like, attempt to read it
+    elif isinstance(source, TextIO):
+        contents = source.read()
+        source.close()
 
-    # if argument is not a string, attempt to use it like a file-like object
+    # if argument is str, parse its contents directly
     else:
-        with source as f:
-            root = orjson.loads(f.read())
+        contents = source
 
+    root = orjson.loads(contents)
     return JSONSchema.parse(root)
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/schema/models.py` & `tesseract_olap-0.7.0/tesseract_olap/schema/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from dataclasses import dataclass, field
-from typing import List, Mapping, Optional, Tuple, Union
+from typing import Iterable, List, Mapping, Optional, Sequence, Tuple, Union
 
 import immutables as immu
 
 from tesseract_olap.common import get_localization
 
 from .aggregators import Aggregator, Count
 from .enums import DimensionType, MemberType
@@ -20,15 +20,14 @@
 class Schema:
     """Base Schema class."""
 
     name: str
     annotations: Annotations = field(default_factory=immu.Map)
     cube_map: Mapping[str, "Cube"] = field(default_factory=immu.Map)
     default_locale: str = "xx"
-    # TODO: implement role permissions model
     shared_dimension_map: Mapping[str, "Dimension"] = field(default_factory=immu.Map)
     shared_table_map: Mapping[str, "InlineTable"] = field(default_factory=immu.Map)
 
     @classmethod
     def join(cls, *args: "Schema"):
         annotations = {}
         cube_map = {}
@@ -48,28 +47,46 @@
             cube_map=cube_map,
             shared_dimension_map=shared_dimension_map,
             shared_table_map=shared_table_map,
         )
 
 
 @dataclass(eq=True, frozen=True, repr=False)
+class AccessControl:
+    public: bool = True
+    rules: Mapping[str, bool] = field(default_factory=immu.Map)
+
+    def __repr__(self) -> str:
+        return 'Public' if self.public else 'Private(%d)' % len(self.rules)
+
+    def is_authorized(self, roles: Iterable[str]) -> bool:
+        rules = self.rules
+        return self.public or any(rules.get(role, False) for role in roles)
+
+
+@dataclass(eq=True, frozen=True, repr=False)
 class InlineTable:
     name: str
     headers: Tuple[str, ...]
     types: Tuple[MemberType, ...]
-    rows: List[Tuple[str, ...]]
+    rows: List[Tuple[Union[str, float], ...]]
 
     def __repr__(self) -> str:
         return "{0.__class__.__name__}(name='{0.name}')".format(self)
 
+    @staticmethod
+    def infer_types(rows: Sequence[Tuple[Union[float, str], ...]]):
+        return tuple(MemberType.from_values(column) for column in zip(*rows))
+
 
 class Entity:
     name: str
     annotations: Annotations
     captions: CaptionSet
+    acl: AccessControl = field(default_factory=AccessControl)
 
     def get_annotation(self, name: str) -> Optional[str]:
         """Retrieves an annotation for the entity.
         If the annotation is not defined, raises a :class:`KeyError`.
         """
         return self.annotations[name]
 
@@ -84,30 +101,37 @@
 
     def get_locale_available(self) -> List[str]:
         """Retrieves the list of locales for whose a caption has been defined in
         this entity.
         """
         return sorted(self.captions.keys())
 
+    def is_authorized(self, role: Iterable[str]) -> bool:
+        role = {role} if isinstance(role, str) else role
+        return self.acl.is_authorized(role)
+
 
 @dataclass(eq=True, frozen=True)
 class Cube(Entity):
     name: str
     table: Union["InlineTable", "Table", str]
+    acl: AccessControl = field(default_factory=AccessControl)
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     dimension_map: Mapping[str, Union["Dimension", "DimensionUsage"]] \
         = field(default_factory=immu.Map)
     measure_map: Mapping[str, "Measure"] = field(default_factory=immu.Map)
+    subset_table: bool = False
+    visible: bool = True
 
 
 @dataclass(eq=True, frozen=True)
 class Table:
     name: str
-    primary_key: str = "id"
+    primary_key: str
     schema: Optional[str] = None
 
 
 @dataclass(eq=True, frozen=True)
 class Dimension(Entity):
     name: str
     annotations: Annotations = field(default_factory=immu.Map)
@@ -168,70 +192,63 @@
 @dataclass(eq=True, frozen=True)
 class Measure(Entity):
     name: str
     key_column: str
     aggregator: Aggregator = field(default_factory=Count)
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
-    submeasures: Mapping[str, "SubMeasure"] = field(default_factory=immu.Map)
-
-
-@dataclass(eq=True, frozen=True)
-class SubMeasure(Entity):
-    name: str
-    aggregator: Aggregator = field(default_factory=Count)
-    captions: CaptionSet = field(default_factory=immu.Map)
+    submeasures: Mapping[str, "Measure"] = field(default_factory=immu.Map)
 
 
 class Usage(Entity):
     """Defines a base class for Usage entities, so the type checker can enforce
     a bound class as a parameter.
     """
     source: str
 
 
 @dataclass(eq=True, frozen=True)
 class DimensionUsage(Usage):
-    """Defines an usage of a :class:`Schema`-level :class:`SharedDimension`
+    """Establishes the usage of a :class:`Schema`-level :class:`SharedDimension`
     inside a :class:`Cube`.
     """
     name: str
     source: str
     foreign_key: str
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     hierarchy_map: Mapping[str, "HierarchyUsage"] = field(default_factory=immu.Map)
 
 
 @dataclass(eq=True, frozen=True)
 class HierarchyUsage(Usage):
-    """Defines an usage of a :class:`Hierarchy` from a inside of a
-    :class:`SharedDimension`, in a :class:`DimensionUsage`.
+    """Establishes the usage of a :class:`Hierarchy` defined in a
+    :class:`SharedDimension`.
     """
     name: str
     source: str
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     level_map: Mapping[str, "LevelUsage"] = field(default_factory=immu.Map)
 
 
 @dataclass(eq=True, frozen=True)
 class LevelUsage(Usage):
-    """Defines an usage of a :class:`Level` from a inside of a
-    :class:`SharedDimension`, in a :class:`HierarchyUsage`.
+    """Establishes the usage of a :class:`Level` defined in a :class:`Hierarchy`
+    under a :class:`SharedDimension`.
     """
     name: str
     source: str
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
     property_map: Mapping[str, "PropertyUsage"] = field(default_factory=immu.Map)
 
 
 @dataclass(eq=True, frozen=True)
 class PropertyUsage(Usage):
-    """Defines an usage of a :class:`Property` from a inside of a
-    :class:`SharedDimension`, in a :class:`LevelUsage`.
+    """Establishes the usage of a :class:`Property` defined in a :class:`Level`
+    under a :class:`SharedDimension`.
     """
     name: str
     source: str
     annotations: Annotations = field(default_factory=immu.Map)
     captions: CaptionSet = field(default_factory=immu.Map)
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/schema/schema.xsd` & `tesseract_olap-0.7.0/tesseract_olap/schema/schema.xsd`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with CRLF line terminators*

 * *Files 19% similar despite different names*

```diff
@@ -1,300 +1,291 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0d0a 3c78 733a 7363 6865  F-8"?>..<xs:sche
-00000030: 6d61 2078 6d6c 6e73 3a78 733d 2268 7474  ma xmlns:xs="htt
-00000040: 703a 2f2f 7777 772e 7733 2e6f 7267 2f32  p://www.w3.org/2
-00000050: 3030 312f 584d 4c53 6368 656d 6122 3e0d  001/XMLSchema">.
-00000060: 0a0d 0a3c 7873 3a61 7474 7269 6275 7465  ...<xs:attribute
-00000070: 206e 616d 653d 226e 616d 6522 2074 7970   name="name" typ
-00000080: 653d 2278 733a 7374 7269 6e67 222f 3e0d  e="xs:string"/>.
-00000090: 0a0d 0a3c 7873 3a73 696d 706c 6554 7970  ...<xs:simpleTyp
-000000a0: 6520 6e61 6d65 3d22 6469 6d65 6e73 696f  e name="dimensio
-000000b0: 6e54 7970 6522 3e0d 0a20 203c 7873 3a72  nType">..  <xs:r
-000000c0: 6573 7472 6963 7469 6f6e 2062 6173 653d  estriction base=
-000000d0: 2278 733a 7374 7269 6e67 223e 0d0a 2020  "xs:string">..  
-000000e0: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
-000000f0: 6e20 7661 6c75 653d 2267 656f 222f 3e0d  n value="geo"/>.
-00000100: 0a20 2020 203c 7873 3a65 6e75 6d65 7261  .    <xs:enumera
-00000110: 7469 6f6e 2076 616c 7565 3d22 7469 6d65  tion value="time
-00000120: 222f 3e0d 0a20 2020 203c 7873 3a65 6e75  "/>..    <xs:enu
-00000130: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-00000140: 7374 6422 2f3e 0d0a 2020 3c2f 7873 3a72  std"/>..  </xs:r
-00000150: 6573 7472 6963 7469 6f6e 3e0d 0a3c 2f78  estriction>..</x
-00000160: 733a 7369 6d70 6c65 5479 7065 3e0d 0a0d  s:simpleType>...
-00000170: 0a3c 7873 3a73 696d 706c 6554 7970 6520  .<xs:simpleType 
-00000180: 6e61 6d65 3d22 6b65 7954 7970 6522 3e0d  name="keyType">.
-00000190: 0a20 203c 7873 3a72 6573 7472 6963 7469  .  <xs:restricti
-000001a0: 6f6e 2062 6173 653d 2278 733a 7374 7269  on base="xs:stri
-000001b0: 6e67 223e 0d0a 2020 2020 3c78 733a 656e  ng">..    <xs:en
-000001c0: 756d 6572 6174 696f 6e20 7661 6c75 653d  umeration value=
-000001d0: 2274 6578 7422 2f3e 0d0a 2020 2020 3c78  "text"/>..    <x
-000001e0: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
-000001f0: 6c75 653d 226e 6f6e 7465 7874 222f 3e0d  lue="nontext"/>.
-00000200: 0a20 203c 2f78 733a 7265 7374 7269 6374  .  </xs:restrict
-00000210: 696f 6e3e 0d0a 3c2f 7873 3a73 696d 706c  ion>..</xs:simpl
-00000220: 6554 7970 653e 0d0a 0d0a 3c78 733a 636f  eType>....<xs:co
-00000230: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
-00000240: 416e 6e6f 7461 7469 6f6e 456c 656d 656e  AnnotationElemen
-00000250: 7422 3e0d 0a20 203c 7873 3a73 696d 706c  t">..  <xs:simpl
-00000260: 6543 6f6e 7465 6e74 3e0d 0a20 2020 203c  eContent>..    <
-00000270: 7873 3a65 7874 656e 7369 6f6e 2062 6173  xs:extension bas
-00000280: 653d 2278 733a 7374 7269 6e67 223e 0d0a  e="xs:string">..
-00000290: 2020 2020 2020 3c78 733a 6174 7472 6962        <xs:attrib
-000002a0: 7574 6520 7265 663d 226e 616d 6522 2075  ute ref="name" u
-000002b0: 7365 3d22 7265 7175 6972 6564 222f 3e0d  se="required"/>.
-000002c0: 0a20 2020 203c 2f78 733a 6578 7465 6e73  .    </xs:extens
-000002d0: 696f 6e3e 0d0a 2020 3c2f 7873 3a73 696d  ion>..  </xs:sim
-000002e0: 706c 6543 6f6e 7465 6e74 3e0d 0a3c 2f78  pleContent>..</x
-000002f0: 733a 636f 6d70 6c65 7854 7970 653e 0d0a  s:complexType>..
-00000300: 0d0a 3c78 733a 636f 6d70 6c65 7854 7970  ..<xs:complexTyp
-00000310: 6520 6e61 6d65 3d22 4375 6265 456c 656d  e name="CubeElem
-00000320: 656e 7422 3e0d 0a20 203c 7873 3a73 6571  ent">..  <xs:seq
-00000330: 7565 6e63 653e 0d0a 2020 2020 3c78 733a  uence>..    <xs:
-00000340: 656c 656d 656e 7420 6e61 6d65 3d22 416e  element name="An
-00000350: 6e6f 7461 7469 6f6e 2220 7479 7065 3d22  notation" type="
-00000360: 416e 6e6f 7461 7469 6f6e 456c 656d 656e  AnnotationElemen
-00000370: 7422 206d 6178 4f63 6375 7273 3d22 756e  t" maxOccurs="un
-00000380: 626f 756e 6465 6422 2f3e 0d0a 2020 2020  bounded"/>..    
-00000390: 3c78 733a 656c 656d 656e 7420 6e61 6d65  <xs:element name
-000003a0: 3d22 5461 626c 6522 2074 7970 653d 2254  ="Table" type="T
-000003b0: 6162 6c65 456c 656d 656e 7422 2f3e 0d0a  ableElement"/>..
-000003c0: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
-000003d0: 6e61 6d65 3d22 4469 6d65 6e73 696f 6e55  name="DimensionU
-000003e0: 7361 6765 2220 7479 7065 3d22 4469 6d65  sage" type="Dime
-000003f0: 6e73 696f 6e55 7361 6765 456c 656d 656e  nsionUsageElemen
-00000400: 7422 206d 6178 4f63 6375 7273 3d22 756e  t" maxOccurs="un
-00000410: 626f 756e 6465 6422 2f3e 0d0a 2020 2020  bounded"/>..    
-00000420: 3c78 733a 656c 656d 656e 7420 6e61 6d65  <xs:element name
-00000430: 3d22 4469 6d65 6e73 696f 6e22 2074 7970  ="Dimension" typ
-00000440: 653d 2244 696d 656e 7369 6f6e 456c 656d  e="DimensionElem
-00000450: 656e 7422 206d 6178 4f63 6375 7273 3d22  ent" maxOccurs="
-00000460: 756e 626f 756e 6465 6422 2f3e 0d0a 2020  unbounded"/>..  
-00000470: 3c2f 7873 3a73 6571 7565 6e63 653e 0d0a  </xs:sequence>..
-00000480: 0d0a 2020 3c78 733a 6174 7472 6962 7574  ..  <xs:attribut
-00000490: 6520 7265 663d 226e 616d 6522 2075 7365  e ref="name" use
-000004a0: 3d22 7265 7175 6972 6564 222f 3e0d 0a3c  ="required"/>..<
-000004b0: 2f78 733a 636f 6d70 6c65 7854 7970 653e  /xs:complexType>
-000004c0: 0d0a 0d0a 3c78 733a 636f 6d70 6c65 7854  ....<xs:complexT
-000004d0: 7970 6520 6e61 6d65 3d22 4469 6d65 6e73  ype name="Dimens
-000004e0: 696f 6e45 6c65 6d65 6e74 223e 0d0a 2020  ionElement">..  
-000004f0: 3c78 733a 7365 7175 656e 6365 3e0d 0a20  <xs:sequence>.. 
-00000500: 2020 203c 7873 3a65 6c65 6d65 6e74 206e     <xs:element n
-00000510: 616d 653d 2248 6965 7261 7263 6879 2220  ame="Hierarchy" 
-00000520: 7479 7065 3d22 4869 6572 6172 6368 7945  type="HierarchyE
-00000530: 6c65 6d65 6e74 2220 6d61 784f 6363 7572  lement" maxOccur
-00000540: 733d 2275 6e62 6f75 6e64 6564 222f 3e0d  s="unbounded"/>.
-00000550: 0a20 203c 2f78 733a 7365 7175 656e 6365  .  </xs:sequence
-00000560: 3e0d 0a20 200d 0a20 203c 7873 3a61 7474  >..  ..  <xs:att
-00000570: 7269 6275 7465 2072 6566 3d22 6e61 6d65  ribute ref="name
-00000580: 2220 7573 653d 2272 6571 7569 7265 6422  " use="required"
-00000590: 2f3e 0d0a 2020 3c78 733a 6174 7472 6962  />..  <xs:attrib
-000005a0: 7574 6520 6e61 6d65 3d22 6465 6661 756c  ute name="defaul
-000005b0: 745f 6869 6572 6172 6368 7922 2074 7970  t_hierarchy" typ
-000005c0: 653d 2278 733a 7374 7269 6e67 2220 2f3e  e="xs:string" />
-000005d0: 0d0a 2020 3c78 733a 6174 7472 6962 7574  ..  <xs:attribut
-000005e0: 6520 6e61 6d65 3d22 666f 7265 6967 6e5f  e name="foreign_
-000005f0: 6b65 7922 2074 7970 653d 2278 733a 7374  key" type="xs:st
-00000600: 7269 6e67 2220 2f3e 0d0a 2020 3c78 733a  ring" />..  <xs:
-00000610: 6174 7472 6962 7574 6520 6e61 6d65 3d22  attribute name="
-00000620: 7479 7065 2220 7479 7065 3d22 6469 6d65  type" type="dime
-00000630: 6e73 696f 6e54 7970 6522 2064 6566 6175  nsionType" defau
-00000640: 6c74 3d22 7374 6422 202f 3e0d 0a3c 2f78  lt="std" />..</x
-00000650: 733a 636f 6d70 6c65 7854 7970 653e 0d0a  s:complexType>..
-00000660: 0d0a 3c78 733a 636f 6d70 6c65 7854 7970  ..<xs:complexTyp
-00000670: 6520 6e61 6d65 3d22 4469 6d65 6e73 696f  e name="Dimensio
-00000680: 6e55 7361 6765 456c 656d 656e 7422 3e0d  nUsageElement">.
-00000690: 0a20 203c 7873 3a61 7474 7269 6275 7465  .  <xs:attribute
-000006a0: 2072 6566 3d22 6e61 6d65 2220 7573 653d   ref="name" use=
-000006b0: 2272 6571 7569 7265 6422 2f3e 0d0a 2020  "required"/>..  
-000006c0: 3c78 733a 6174 7472 6962 7574 6520 6e61  <xs:attribute na
-000006d0: 6d65 3d22 666f 7265 6967 6e5f 6b65 7922  me="foreign_key"
-000006e0: 2074 7970 653d 2278 733a 7374 7269 6e67   type="xs:string
-000006f0: 2220 7573 653d 2272 6571 7569 7265 6422  " use="required"
-00000700: 2f3e 0d0a 2020 3c78 733a 6174 7472 6962  />..  <xs:attrib
-00000710: 7574 6520 6e61 6d65 3d22 736f 7572 6365  ute name="source
-00000720: 2220 7479 7065 3d22 7873 3a73 7472 696e  " type="xs:strin
-00000730: 6722 2075 7365 3d22 7265 7175 6972 6564  g" use="required
-00000740: 222f 3e0d 0a3c 2f78 733a 636f 6d70 6c65  "/>..</xs:comple
-00000750: 7854 7970 653e 0d0a 0d0a 3c78 733a 636f  xType>....<xs:co
-00000760: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
-00000770: 4869 6572 6172 6368 7945 6c65 6d65 6e74  HierarchyElement
-00000780: 223e 0d0a 2020 3c78 733a 7365 7175 656e  ">..  <xs:sequen
-00000790: 6365 3e0d 0a20 2020 203c 7873 3a63 686f  ce>..    <xs:cho
-000007a0: 6963 653e 0d0a 2020 2020 2020 3c78 733a  ice>..      <xs:
-000007b0: 656c 656d 656e 7420 6e61 6d65 3d22 5461  element name="Ta
-000007c0: 626c 6522 2074 7970 653d 2254 6162 6c65  ble" type="Table
-000007d0: 456c 656d 656e 7422 2f3e 0d0a 2020 2020  Element"/>..    
-000007e0: 2020 3c78 733a 656c 656d 656e 7420 6e61    <xs:element na
-000007f0: 6d65 3d22 496e 6c69 6e65 5461 626c 6522  me="InlineTable"
-00000800: 2074 7970 653d 2249 6e6c 696e 6554 6162   type="InlineTab
-00000810: 6c65 456c 656d 656e 7422 2f3e 0d0a 2020  leElement"/>..  
-00000820: 2020 3c2f 7873 3a63 686f 6963 653e 0d0a    </xs:choice>..
-00000830: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
-00000840: 6e61 6d65 3d22 4c65 7665 6c22 2074 7970  name="Level" typ
-00000850: 653d 224c 6576 656c 456c 656d 656e 7422  e="LevelElement"
-00000860: 206d 6178 4f63 6375 7273 3d22 756e 626f   maxOccurs="unbo
-00000870: 756e 6465 6422 2f3e 0d0a 2020 3c2f 7873  unded"/>..  </xs
-00000880: 3a73 6571 7565 6e63 653e 0d0a 2020 0d0a  :sequence>..  ..
-00000890: 2020 3c78 733a 6174 7472 6962 7574 6520    <xs:attribute 
-000008a0: 7265 663d 226e 616d 6522 2075 7365 3d22  ref="name" use="
-000008b0: 7265 7175 6972 6564 222f 3e0d 0a20 203c  required"/>..  <
-000008c0: 7873 3a61 7474 7269 6275 7465 206e 616d  xs:attribute nam
-000008d0: 653d 2270 7269 6d61 7279 5f6b 6579 2220  e="primary_key" 
-000008e0: 7479 7065 3d22 7873 3a73 7472 696e 6722  type="xs:string"
-000008f0: 2f3e 0d0a 3c2f 7873 3a63 6f6d 706c 6578  />..</xs:complex
-00000900: 5479 7065 3e0d 0a0d 0a3c 7873 3a63 6f6d  Type>....<xs:com
-00000910: 706c 6578 5479 7065 206e 616d 653d 2249  plexType name="I
-00000920: 6e6c 696e 6554 6162 6c65 456c 656d 656e  nlineTableElemen
-00000930: 7422 3e0d 0a20 203c 7873 3a73 6571 7565  t">..  <xs:seque
-00000940: 6e63 653e 0d0a 2020 2020 3c78 733a 656c  nce>..    <xs:el
-00000950: 656d 656e 7420 6e61 6d65 3d22 436f 6c75  ement name="Colu
-00000960: 6d6e 4465 6622 2074 7970 653d 2249 6e6c  mnDef" type="Inl
-00000970: 696e 6554 6162 6c65 436f 6c75 6d6e 456c  ineTableColumnEl
-00000980: 656d 656e 7422 206d 6178 4f63 6375 7273  ement" maxOccurs
-00000990: 3d22 756e 626f 756e 6465 6422 2f3e 0d0a  ="unbounded"/>..
-000009a0: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
-000009b0: 6e61 6d65 3d22 526f 7722 2074 7970 653d  name="Row" type=
-000009c0: 2249 6e6c 696e 6554 6162 6c65 526f 7745  "InlineTableRowE
-000009d0: 6c65 6d65 6e74 2220 6d61 784f 6363 7572  lement" maxOccur
-000009e0: 733d 2275 6e62 6f75 6e64 6564 222f 3e0d  s="unbounded"/>.
-000009f0: 0a20 203c 2f78 733a 7365 7175 656e 6365  .  </xs:sequence
-00000a00: 3e0d 0a0d 0a20 203c 7873 3a61 7474 7269  >....  <xs:attri
-00000a10: 6275 7465 206e 616d 653d 2261 6c69 6173  bute name="alias
-00000a20: 2220 7479 7065 3d22 7873 3a73 7472 696e  " type="xs:strin
-00000a30: 6722 2075 7365 3d22 7265 7175 6972 6564  g" use="required
-00000a40: 222f 3e0d 0a3c 2f78 733a 636f 6d70 6c65  "/>..</xs:comple
-00000a50: 7854 7970 653e 0d0a 0d0a 3c78 733a 636f  xType>....<xs:co
-00000a60: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
-00000a70: 496e 6c69 6e65 5461 626c 6543 6f6c 756d  InlineTableColum
-00000a80: 6e45 6c65 6d65 6e74 223e 0d0a 2020 3c78  nElement">..  <x
-00000a90: 733a 6174 7472 6962 7574 6520 7265 663d  s:attribute ref=
-00000aa0: 226e 616d 6522 2075 7365 3d22 7265 7175  "name" use="requ
-00000ab0: 6972 6564 222f 3e0d 0a20 203c 7873 3a61  ired"/>..  <xs:a
-00000ac0: 7474 7269 6275 7465 206e 616d 653d 226b  ttribute name="k
-00000ad0: 6579 5f74 7970 6522 2074 7970 653d 226b  ey_type" type="k
-00000ae0: 6579 5479 7065 2220 7573 653d 2272 6571  eyType" use="req
-00000af0: 7569 7265 6422 2f3e 0d0a 3c2f 7873 3a63  uired"/>..</xs:c
-00000b00: 6f6d 706c 6578 5479 7065 3e0d 0a0d 0a3c  omplexType>....<
-00000b10: 7873 3a63 6f6d 706c 6578 5479 7065 206e  xs:complexType n
-00000b20: 616d 653d 2249 6e6c 696e 6554 6162 6c65  ame="InlineTable
-00000b30: 526f 7745 6c65 6d65 6e74 223e 0d0a 2020  RowElement">..  
-00000b40: 3c78 733a 7365 7175 656e 6365 3e0d 0a20  <xs:sequence>.. 
-00000b50: 2020 203c 7873 3a65 6c65 6d65 6e74 206e     <xs:element n
-00000b60: 616d 653d 2256 616c 7565 2220 7479 7065  ame="Value" type
-00000b70: 3d22 496e 6c69 6e65 5461 626c 6556 616c  ="InlineTableVal
-00000b80: 7565 456c 656d 656e 7422 206d 6178 4f63  ueElement" maxOc
-00000b90: 6375 7273 3d22 756e 626f 756e 6465 6422  curs="unbounded"
-00000ba0: 2f3e 0d0a 2020 3c2f 7873 3a73 6571 7565  />..  </xs:seque
-00000bb0: 6e63 653e 0d0a 3c2f 7873 3a63 6f6d 706c  nce>..</xs:compl
-00000bc0: 6578 5479 7065 3e0d 0a0d 0a3c 7873 3a63  exType>....<xs:c
-00000bd0: 6f6d 706c 6578 5479 7065 206e 616d 653d  omplexType name=
-00000be0: 2249 6e6c 696e 6554 6162 6c65 5661 6c75  "InlineTableValu
-00000bf0: 6545 6c65 6d65 6e74 223e 0d0a 2020 3c78  eElement">..  <x
-00000c00: 733a 7369 6d70 6c65 436f 6e74 656e 743e  s:simpleContent>
-00000c10: 0d0a 2020 2020 3c78 733a 6578 7465 6e73  ..    <xs:extens
-00000c20: 696f 6e20 6261 7365 3d22 7873 3a73 7472  ion base="xs:str
-00000c30: 696e 6722 3e0d 0a20 2020 2020 203c 7873  ing">..      <xs
-00000c40: 3a61 7474 7269 6275 7465 206e 616d 653d  :attribute name=
-00000c50: 2263 6f6c 756d 6e22 2074 7970 653d 2278  "column" type="x
-00000c60: 733a 7374 7269 6e67 2220 7573 653d 2272  s:string" use="r
-00000c70: 6571 7569 7265 6422 2f3e 0d0a 2020 2020  equired"/>..    
-00000c80: 3c2f 7873 3a65 7874 656e 7369 6f6e 3e0d  </xs:extension>.
-00000c90: 0a20 203c 2f78 733a 7369 6d70 6c65 436f  .  </xs:simpleCo
-00000ca0: 6e74 656e 743e 0d0a 3c2f 7873 3a63 6f6d  ntent>..</xs:com
-00000cb0: 706c 6578 5479 7065 3e0d 0a0d 0a3c 7873  plexType>....<xs
-00000cc0: 3a63 6f6d 706c 6578 5479 7065 206e 616d  :complexType nam
-00000cd0: 653d 224c 6576 656c 456c 656d 656e 7422  e="LevelElement"
-00000ce0: 3e0d 0a20 203c 7873 3a73 6571 7565 6e63  >..  <xs:sequenc
-00000cf0: 653e 0d0a 2020 2020 3c78 733a 656c 656d  e>..    <xs:elem
-00000d00: 656e 7420 6e61 6d65 3d22 5072 6f70 6572  ent name="Proper
-00000d10: 7479 2220 7479 7065 3d22 5072 6f70 6572  ty" type="Proper
-00000d20: 7479 456c 656d 656e 7422 206d 696e 4f63  tyElement" minOc
-00000d30: 6375 7273 3d22 3022 206d 6178 4f63 6375  curs="0" maxOccu
-00000d40: 7273 3d22 756e 626f 756e 6465 6422 2f3e  rs="unbounded"/>
-00000d50: 0d0a 2020 3c2f 7873 3a73 6571 7565 6e63  ..  </xs:sequenc
-00000d60: 653e 0d0a 2020 0d0a 2020 3c78 733a 6174  e>..  ..  <xs:at
-00000d70: 7472 6962 7574 6520 7265 663d 226e 616d  tribute ref="nam
-00000d80: 6522 2075 7365 3d22 7265 7175 6972 6564  e" use="required
-00000d90: 222f 3e0d 0a20 203c 7873 3a61 7474 7269  "/>..  <xs:attri
-00000da0: 6275 7465 206e 616d 653d 226b 6579 5f63  bute name="key_c
-00000db0: 6f6c 756d 6e22 2074 7970 653d 2278 733a  olumn" type="xs:
-00000dc0: 7374 7269 6e67 2220 7573 653d 2272 6571  string" use="req
-00000dd0: 7569 7265 6422 2f3e 0d0a 2020 3c78 733a  uired"/>..  <xs:
-00000de0: 6174 7472 6962 7574 6520 6e61 6d65 3d22  attribute name="
-00000df0: 6e61 6d65 5f63 6f6c 756d 6e22 2074 7970  name_column" typ
-00000e00: 653d 2278 733a 7374 7269 6e67 222f 3e0d  e="xs:string"/>.
-00000e10: 0a20 203c 7873 3a61 7474 7269 6275 7465  .  <xs:attribute
-00000e20: 206e 616d 653d 226b 6579 5f74 7970 6522   name="key_type"
-00000e30: 2074 7970 653d 226b 6579 5479 7065 222f   type="keyType"/
-00000e40: 3e0d 0a3c 2f78 733a 636f 6d70 6c65 7854  >..</xs:complexT
-00000e50: 7970 653e 0d0a 0d0a 3c78 733a 636f 6d70  ype>....<xs:comp
-00000e60: 6c65 7854 7970 6520 6e61 6d65 3d22 5072  lexType name="Pr
-00000e70: 6f70 6572 7479 456c 656d 656e 7422 3e0d  opertyElement">.
-00000e80: 0a20 203c 7873 3a61 7474 7269 6275 7465  .  <xs:attribute
-00000e90: 2072 6566 3d22 6e61 6d65 2220 7573 653d   ref="name" use=
-00000ea0: 2272 6571 7569 7265 6422 2f3e 0d0a 2020  "required"/>..  
-00000eb0: 3c78 733a 6174 7472 6962 7574 6520 6e61  <xs:attribute na
-00000ec0: 6d65 3d22 636f 6c75 6d6e 2220 7479 7065  me="column" type
-00000ed0: 3d22 7873 3a73 7472 696e 6722 2075 7365  ="xs:string" use
-00000ee0: 3d22 7265 7175 6972 6564 222f 3e0d 0a20  ="required"/>.. 
-00000ef0: 203c 7873 3a61 7474 7269 6275 7465 206e   <xs:attribute n
-00000f00: 616d 653d 2263 6170 7469 6f6e 5f73 6574  ame="caption_set
-00000f10: 2220 7479 7065 3d22 7873 3a73 7472 696e  " type="xs:strin
-00000f20: 6722 2f3e 0d0a 3c2f 7873 3a63 6f6d 706c  g"/>..</xs:compl
-00000f30: 6578 5479 7065 3e0d 0a0d 0a3c 7873 3a63  exType>....<xs:c
-00000f40: 6f6d 706c 6578 5479 7065 206e 616d 653d  omplexType name=
-00000f50: 224d 6561 7375 7265 456c 656d 656e 7422  "MeasureElement"
-00000f60: 3e0d 0a20 203c 7873 3a73 6571 7565 6e63  >..  <xs:sequenc
-00000f70: 653e 0d0a 2020 2020 3c78 733a 656c 656d  e>..    <xs:elem
-00000f80: 656e 7420 6e61 6d65 3d22 416e 6e6f 7461  ent name="Annota
-00000f90: 7469 6f6e 2220 7479 7065 3d22 416e 6e6f  tion" type="Anno
-00000fa0: 7461 7469 6f6e 456c 656d 656e 7422 206d  tationElement" m
-00000fb0: 6178 4f63 6375 7273 3d22 756e 626f 756e  axOccurs="unboun
-00000fc0: 6465 6422 2f3e 0d0a 2020 3c2f 7873 3a73  ded"/>..  </xs:s
-00000fd0: 6571 7565 6e63 653e 0d0a 0d0a 2020 3c78  equence>....  <x
-00000fe0: 733a 6174 7472 6962 7574 6520 7265 663d  s:attribute ref=
-00000ff0: 226e 616d 6522 2075 7365 3d22 7265 7175  "name" use="requ
-00001000: 6972 6564 222f 3e0d 0a20 203c 7873 3a61  ired"/>..  <xs:a
-00001010: 7474 7269 6275 7465 206e 616d 653d 2261  ttribute name="a
-00001020: 6767 7265 6761 746f 7222 2074 7970 653d  ggregator" type=
-00001030: 2278 733a 7374 7269 6e67 2220 7573 653d  "xs:string" use=
-00001040: 2272 6571 7569 7265 6422 2f3e 0d0a 2020  "required"/>..  
-00001050: 3c78 733a 6174 7472 6962 7574 6520 6e61  <xs:attribute na
-00001060: 6d65 3d22 636f 6c75 6d6e 2220 7479 7065  me="column" type
-00001070: 3d22 7873 3a73 7472 696e 6722 2075 7365  ="xs:string" use
-00001080: 3d22 7265 7175 6972 6564 222f 3e0d 0a3c  ="required"/>..<
-00001090: 2f78 733a 636f 6d70 6c65 7854 7970 653e  /xs:complexType>
-000010a0: 0d0a 0d0a 3c78 733a 636f 6d70 6c65 7854  ....<xs:complexT
-000010b0: 7970 6520 6e61 6d65 3d22 5461 626c 6545  ype name="TableE
-000010c0: 6c65 6d65 6e74 223e 0d0a 2020 3c78 733a  lement">..  <xs:
-000010d0: 6174 7472 6962 7574 6520 7265 663d 226e  attribute ref="n
-000010e0: 616d 6522 2075 7365 3d22 7265 7175 6972  ame" use="requir
-000010f0: 6564 222f 3e0d 0a20 203c 7873 3a61 7474  ed"/>..  <xs:att
-00001100: 7269 6275 7465 206e 616d 653d 2270 7269  ribute name="pri
-00001110: 6d61 7279 5f6b 6579 2220 7479 7065 3d22  mary_key" type="
-00001120: 7873 3a73 7472 696e 6722 2f3e 0d0a 3c2f  xs:string"/>..</
-00001130: 7873 3a63 6f6d 706c 6578 5479 7065 3e0d  xs:complexType>.
-00001140: 0a0d 0a3c 7873 3a65 6c65 6d65 6e74 206e  ...<xs:element n
-00001150: 616d 653d 2253 6368 656d 6122 3e0d 0a20  ame="Schema">.. 
-00001160: 203c 7873 3a63 6f6d 706c 6578 5479 7065   <xs:complexType
-00001170: 3e0d 0a20 2020 203c 7873 3a73 6571 7565  >..    <xs:seque
-00001180: 6e63 653e 0d0a 2020 2020 2020 3c78 733a  nce>..      <xs:
-00001190: 656c 656d 656e 7420 6e61 6d65 3d22 5368  element name="Sh
-000011a0: 6172 6564 4469 6d65 6e73 696f 6e22 2074  aredDimension" t
-000011b0: 7970 653d 2244 696d 656e 7369 6f6e 456c  ype="DimensionEl
-000011c0: 656d 656e 7422 206d 696e 4f63 6375 7273  ement" minOccurs
-000011d0: 3d22 3022 206d 6178 4f63 6375 7273 3d22  ="0" maxOccurs="
-000011e0: 756e 626f 756e 6465 6422 2f3e 0d0a 2020  unbounded"/>..  
-000011f0: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
-00001200: 6e61 6d65 3d22 4375 6265 2220 7479 7065  name="Cube" type
-00001210: 3d22 4375 6265 456c 656d 656e 7422 206d  ="CubeElement" m
-00001220: 6178 4f63 6375 7273 3d22 756e 626f 756e  axOccurs="unboun
-00001230: 6465 6422 2f3e 0d0a 2020 2020 3c2f 7873  ded"/>..    </xs
-00001240: 3a73 6571 7565 6e63 653e 0d0a 0d0a 2020  :sequence>....  
-00001250: 2020 3c78 733a 6174 7472 6962 7574 6520    <xs:attribute 
-00001260: 7265 663d 226e 616d 6522 2075 7365 3d22  ref="name" use="
-00001270: 7265 7175 6972 6564 222f 3e0d 0a20 203c  required"/>..  <
-00001280: 2f78 733a 636f 6d70 6c65 7854 7970 653e  /xs:complexType>
-00001290: 0d0a 3c2f 7873 3a65 6c65 6d65 6e74 3e0d  ..</xs:element>.
-000012a0: 0a0d 0a3c 2f78 733a 7363 6865 6d61 3e20  ...</xs:schema> 
-000012b0: 0d0a                                     ..
+00000020: 462d 3822 3f3e 0a3c 7873 3a73 6368 656d  F-8"?>.<xs:schem
+00000030: 6120 786d 6c6e 733a 7873 3d22 6874 7470  a xmlns:xs="http
+00000040: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
+00000050: 3031 2f58 4d4c 5363 6865 6d61 223e 0a0a  01/XMLSchema">..
+00000060: 3c78 733a 6174 7472 6962 7574 6520 6e61  <xs:attribute na
+00000070: 6d65 3d22 6e61 6d65 2220 7479 7065 3d22  me="name" type="
+00000080: 7873 3a73 7472 696e 6722 2f3e 0a0a 3c78  xs:string"/>..<x
+00000090: 733a 7369 6d70 6c65 5479 7065 206e 616d  s:simpleType nam
+000000a0: 653d 2264 696d 656e 7369 6f6e 5479 7065  e="dimensionType
+000000b0: 223e 0a20 203c 7873 3a72 6573 7472 6963  ">.  <xs:restric
+000000c0: 7469 6f6e 2062 6173 653d 2278 733a 7374  tion base="xs:st
+000000d0: 7269 6e67 223e 0a20 2020 203c 7873 3a65  ring">.    <xs:e
+000000e0: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+000000f0: 3d22 6765 6f22 2f3e 0a20 2020 203c 7873  ="geo"/>.    <xs
+00000100: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
+00000110: 7565 3d22 7469 6d65 222f 3e0a 2020 2020  ue="time"/>.    
+00000120: 3c78 733a 656e 756d 6572 6174 696f 6e20  <xs:enumeration 
+00000130: 7661 6c75 653d 2273 7464 222f 3e0a 2020  value="std"/>.  
+00000140: 3c2f 7873 3a72 6573 7472 6963 7469 6f6e  </xs:restriction
+00000150: 3e0a 3c2f 7873 3a73 696d 706c 6554 7970  >.</xs:simpleTyp
+00000160: 653e 0a0a 3c78 733a 7369 6d70 6c65 5479  e>..<xs:simpleTy
+00000170: 7065 206e 616d 653d 226b 6579 5479 7065  pe name="keyType
+00000180: 223e 0a20 203c 7873 3a72 6573 7472 6963  ">.  <xs:restric
+00000190: 7469 6f6e 2062 6173 653d 2278 733a 7374  tion base="xs:st
+000001a0: 7269 6e67 223e 0a20 2020 203c 7873 3a65  ring">.    <xs:e
+000001b0: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+000001c0: 3d22 7465 7874 222f 3e0a 2020 2020 3c78  ="text"/>.    <x
+000001d0: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
+000001e0: 6c75 653d 226e 6f6e 7465 7874 222f 3e0a  lue="nontext"/>.
+000001f0: 2020 3c2f 7873 3a72 6573 7472 6963 7469    </xs:restricti
+00000200: 6f6e 3e0a 3c2f 7873 3a73 696d 706c 6554  on>.</xs:simpleT
+00000210: 7970 653e 0a0a 3c78 733a 636f 6d70 6c65  ype>..<xs:comple
+00000220: 7854 7970 6520 6e61 6d65 3d22 416e 6e6f  xType name="Anno
+00000230: 7461 7469 6f6e 456c 656d 656e 7422 3e0a  tationElement">.
+00000240: 2020 3c78 733a 7369 6d70 6c65 436f 6e74    <xs:simpleCont
+00000250: 656e 743e 0a20 2020 203c 7873 3a65 7874  ent>.    <xs:ext
+00000260: 656e 7369 6f6e 2062 6173 653d 2278 733a  ension base="xs:
+00000270: 7374 7269 6e67 223e 0a20 2020 2020 203c  string">.      <
+00000280: 7873 3a61 7474 7269 6275 7465 2072 6566  xs:attribute ref
+00000290: 3d22 6e61 6d65 2220 7573 653d 2272 6571  ="name" use="req
+000002a0: 7569 7265 6422 2f3e 0a20 2020 203c 2f78  uired"/>.    </x
+000002b0: 733a 6578 7465 6e73 696f 6e3e 0a20 203c  s:extension>.  <
+000002c0: 2f78 733a 7369 6d70 6c65 436f 6e74 656e  /xs:simpleConten
+000002d0: 743e 0a3c 2f78 733a 636f 6d70 6c65 7854  t>.</xs:complexT
+000002e0: 7970 653e 0a0a 3c78 733a 636f 6d70 6c65  ype>..<xs:comple
+000002f0: 7854 7970 6520 6e61 6d65 3d22 4375 6265  xType name="Cube
+00000300: 456c 656d 656e 7422 3e0a 2020 3c78 733a  Element">.  <xs:
+00000310: 7365 7175 656e 6365 3e0a 2020 2020 3c78  sequence>.    <x
+00000320: 733a 656c 656d 656e 7420 6e61 6d65 3d22  s:element name="
+00000330: 416e 6e6f 7461 7469 6f6e 2220 7479 7065  Annotation" type
+00000340: 3d22 416e 6e6f 7461 7469 6f6e 456c 656d  ="AnnotationElem
+00000350: 656e 7422 206d 6178 4f63 6375 7273 3d22  ent" maxOccurs="
+00000360: 756e 626f 756e 6465 6422 2f3e 0a20 2020  unbounded"/>.   
+00000370: 203c 7873 3a65 6c65 6d65 6e74 206e 616d   <xs:element nam
+00000380: 653d 2254 6162 6c65 2220 7479 7065 3d22  e="Table" type="
+00000390: 5461 626c 6545 6c65 6d65 6e74 222f 3e0a  TableElement"/>.
+000003a0: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
+000003b0: 6e61 6d65 3d22 4469 6d65 6e73 696f 6e55  name="DimensionU
+000003c0: 7361 6765 2220 7479 7065 3d22 4469 6d65  sage" type="Dime
+000003d0: 6e73 696f 6e55 7361 6765 456c 656d 656e  nsionUsageElemen
+000003e0: 7422 206d 6178 4f63 6375 7273 3d22 756e  t" maxOccurs="un
+000003f0: 626f 756e 6465 6422 2f3e 0a20 2020 203c  bounded"/>.    <
+00000400: 7873 3a65 6c65 6d65 6e74 206e 616d 653d  xs:element name=
+00000410: 2244 696d 656e 7369 6f6e 2220 7479 7065  "Dimension" type
+00000420: 3d22 4469 6d65 6e73 696f 6e45 6c65 6d65  ="DimensionEleme
+00000430: 6e74 2220 6d61 784f 6363 7572 733d 2275  nt" maxOccurs="u
+00000440: 6e62 6f75 6e64 6564 222f 3e0a 2020 3c2f  nbounded"/>.  </
+00000450: 7873 3a73 6571 7565 6e63 653e 0a0a 2020  xs:sequence>..  
+00000460: 3c78 733a 6174 7472 6962 7574 6520 7265  <xs:attribute re
+00000470: 663d 226e 616d 6522 2075 7365 3d22 7265  f="name" use="re
+00000480: 7175 6972 6564 222f 3e0a 3c2f 7873 3a63  quired"/>.</xs:c
+00000490: 6f6d 706c 6578 5479 7065 3e0a 0a3c 7873  omplexType>..<xs
+000004a0: 3a63 6f6d 706c 6578 5479 7065 206e 616d  :complexType nam
+000004b0: 653d 2244 696d 656e 7369 6f6e 456c 656d  e="DimensionElem
+000004c0: 656e 7422 3e0a 2020 3c78 733a 7365 7175  ent">.  <xs:sequ
+000004d0: 656e 6365 3e0a 2020 2020 3c78 733a 656c  ence>.    <xs:el
+000004e0: 656d 656e 7420 6e61 6d65 3d22 4869 6572  ement name="Hier
+000004f0: 6172 6368 7922 2074 7970 653d 2248 6965  archy" type="Hie
+00000500: 7261 7263 6879 456c 656d 656e 7422 206d  rarchyElement" m
+00000510: 6178 4f63 6375 7273 3d22 756e 626f 756e  axOccurs="unboun
+00000520: 6465 6422 2f3e 0a20 203c 2f78 733a 7365  ded"/>.  </xs:se
+00000530: 7175 656e 6365 3e0a 2020 0a20 203c 7873  quence>.  .  <xs
+00000540: 3a61 7474 7269 6275 7465 2072 6566 3d22  :attribute ref="
+00000550: 6e61 6d65 2220 7573 653d 2272 6571 7569  name" use="requi
+00000560: 7265 6422 2f3e 0a20 203c 7873 3a61 7474  red"/>.  <xs:att
+00000570: 7269 6275 7465 206e 616d 653d 2264 6566  ribute name="def
+00000580: 6175 6c74 5f68 6965 7261 7263 6879 2220  ault_hierarchy" 
+00000590: 7479 7065 3d22 7873 3a73 7472 696e 6722  type="xs:string"
+000005a0: 202f 3e0a 2020 3c78 733a 6174 7472 6962   />.  <xs:attrib
+000005b0: 7574 6520 6e61 6d65 3d22 666f 7265 6967  ute name="foreig
+000005c0: 6e5f 6b65 7922 2074 7970 653d 2278 733a  n_key" type="xs:
+000005d0: 7374 7269 6e67 2220 2f3e 0a20 203c 7873  string" />.  <xs
+000005e0: 3a61 7474 7269 6275 7465 206e 616d 653d  :attribute name=
+000005f0: 2274 7970 6522 2074 7970 653d 2264 696d  "type" type="dim
+00000600: 656e 7369 6f6e 5479 7065 2220 6465 6661  ensionType" defa
+00000610: 756c 743d 2273 7464 2220 2f3e 0a3c 2f78  ult="std" />.</x
+00000620: 733a 636f 6d70 6c65 7854 7970 653e 0a0a  s:complexType>..
+00000630: 3c78 733a 636f 6d70 6c65 7854 7970 6520  <xs:complexType 
+00000640: 6e61 6d65 3d22 4469 6d65 6e73 696f 6e55  name="DimensionU
+00000650: 7361 6765 456c 656d 656e 7422 3e0a 2020  sageElement">.  
+00000660: 3c78 733a 6174 7472 6962 7574 6520 7265  <xs:attribute re
+00000670: 663d 226e 616d 6522 2075 7365 3d22 7265  f="name" use="re
+00000680: 7175 6972 6564 222f 3e0a 2020 3c78 733a  quired"/>.  <xs:
+00000690: 6174 7472 6962 7574 6520 6e61 6d65 3d22  attribute name="
+000006a0: 666f 7265 6967 6e5f 6b65 7922 2074 7970  foreign_key" typ
+000006b0: 653d 2278 733a 7374 7269 6e67 2220 7573  e="xs:string" us
+000006c0: 653d 2272 6571 7569 7265 6422 2f3e 0a20  e="required"/>. 
+000006d0: 203c 7873 3a61 7474 7269 6275 7465 206e   <xs:attribute n
+000006e0: 616d 653d 2273 6f75 7263 6522 2074 7970  ame="source" typ
+000006f0: 653d 2278 733a 7374 7269 6e67 2220 7573  e="xs:string" us
+00000700: 653d 2272 6571 7569 7265 6422 2f3e 0a3c  e="required"/>.<
+00000710: 2f78 733a 636f 6d70 6c65 7854 7970 653e  /xs:complexType>
+00000720: 0a0a 3c78 733a 636f 6d70 6c65 7854 7970  ..<xs:complexTyp
+00000730: 6520 6e61 6d65 3d22 4869 6572 6172 6368  e name="Hierarch
+00000740: 7945 6c65 6d65 6e74 223e 0a20 203c 7873  yElement">.  <xs
+00000750: 3a73 6571 7565 6e63 653e 0a20 2020 203c  :sequence>.    <
+00000760: 7873 3a63 686f 6963 653e 0a20 2020 2020  xs:choice>.     
+00000770: 203c 7873 3a65 6c65 6d65 6e74 206e 616d   <xs:element nam
+00000780: 653d 2254 6162 6c65 2220 7479 7065 3d22  e="Table" type="
+00000790: 5461 626c 6545 6c65 6d65 6e74 222f 3e0a  TableElement"/>.
+000007a0: 2020 2020 2020 3c78 733a 656c 656d 656e        <xs:elemen
+000007b0: 7420 6e61 6d65 3d22 496e 6c69 6e65 5461  t name="InlineTa
+000007c0: 626c 6522 2074 7970 653d 2249 6e6c 696e  ble" type="Inlin
+000007d0: 6554 6162 6c65 456c 656d 656e 7422 2f3e  eTableElement"/>
+000007e0: 0a20 2020 203c 2f78 733a 6368 6f69 6365  .    </xs:choice
+000007f0: 3e0a 2020 2020 3c78 733a 656c 656d 656e  >.    <xs:elemen
+00000800: 7420 6e61 6d65 3d22 4c65 7665 6c22 2074  t name="Level" t
+00000810: 7970 653d 224c 6576 656c 456c 656d 656e  ype="LevelElemen
+00000820: 7422 206d 6178 4f63 6375 7273 3d22 756e  t" maxOccurs="un
+00000830: 626f 756e 6465 6422 2f3e 0a20 203c 2f78  bounded"/>.  </x
+00000840: 733a 7365 7175 656e 6365 3e0a 2020 0a20  s:sequence>.  . 
+00000850: 203c 7873 3a61 7474 7269 6275 7465 2072   <xs:attribute r
+00000860: 6566 3d22 6e61 6d65 2220 7573 653d 2272  ef="name" use="r
+00000870: 6571 7569 7265 6422 2f3e 0a20 203c 7873  equired"/>.  <xs
+00000880: 3a61 7474 7269 6275 7465 206e 616d 653d  :attribute name=
+00000890: 2270 7269 6d61 7279 5f6b 6579 2220 7479  "primary_key" ty
+000008a0: 7065 3d22 7873 3a73 7472 696e 6722 2f3e  pe="xs:string"/>
+000008b0: 0a3c 2f78 733a 636f 6d70 6c65 7854 7970  .</xs:complexTyp
+000008c0: 653e 0a0a 3c78 733a 636f 6d70 6c65 7854  e>..<xs:complexT
+000008d0: 7970 6520 6e61 6d65 3d22 496e 6c69 6e65  ype name="Inline
+000008e0: 5461 626c 6545 6c65 6d65 6e74 223e 0a20  TableElement">. 
+000008f0: 203c 7873 3a73 6571 7565 6e63 653e 0a20   <xs:sequence>. 
+00000900: 2020 203c 7873 3a65 6c65 6d65 6e74 206e     <xs:element n
+00000910: 616d 653d 2243 6f6c 756d 6e44 6566 2220  ame="ColumnDef" 
+00000920: 7479 7065 3d22 496e 6c69 6e65 5461 626c  type="InlineTabl
+00000930: 6543 6f6c 756d 6e45 6c65 6d65 6e74 2220  eColumnElement" 
+00000940: 6d61 784f 6363 7572 733d 2275 6e62 6f75  maxOccurs="unbou
+00000950: 6e64 6564 222f 3e0a 2020 2020 3c78 733a  nded"/>.    <xs:
+00000960: 656c 656d 656e 7420 6e61 6d65 3d22 526f  element name="Ro
+00000970: 7722 2074 7970 653d 2249 6e6c 696e 6554  w" type="InlineT
+00000980: 6162 6c65 526f 7745 6c65 6d65 6e74 2220  ableRowElement" 
+00000990: 6d61 784f 6363 7572 733d 2275 6e62 6f75  maxOccurs="unbou
+000009a0: 6e64 6564 222f 3e0a 2020 3c2f 7873 3a73  nded"/>.  </xs:s
+000009b0: 6571 7565 6e63 653e 0a0a 2020 3c78 733a  equence>..  <xs:
+000009c0: 6174 7472 6962 7574 6520 6e61 6d65 3d22  attribute name="
+000009d0: 616c 6961 7322 2074 7970 653d 2278 733a  alias" type="xs:
+000009e0: 7374 7269 6e67 2220 7573 653d 2272 6571  string" use="req
+000009f0: 7569 7265 6422 2f3e 0a3c 2f78 733a 636f  uired"/>.</xs:co
+00000a00: 6d70 6c65 7854 7970 653e 0a0a 3c78 733a  mplexType>..<xs:
+00000a10: 636f 6d70 6c65 7854 7970 6520 6e61 6d65  complexType name
+00000a20: 3d22 496e 6c69 6e65 5461 626c 6543 6f6c  ="InlineTableCol
+00000a30: 756d 6e45 6c65 6d65 6e74 223e 0a20 203c  umnElement">.  <
+00000a40: 7873 3a61 7474 7269 6275 7465 2072 6566  xs:attribute ref
+00000a50: 3d22 6e61 6d65 2220 7573 653d 2272 6571  ="name" use="req
+00000a60: 7569 7265 6422 2f3e 0a20 203c 7873 3a61  uired"/>.  <xs:a
+00000a70: 7474 7269 6275 7465 206e 616d 653d 226b  ttribute name="k
+00000a80: 6579 5f74 7970 6522 2074 7970 653d 226b  ey_type" type="k
+00000a90: 6579 5479 7065 2220 7573 653d 2272 6571  eyType" use="req
+00000aa0: 7569 7265 6422 2f3e 0a3c 2f78 733a 636f  uired"/>.</xs:co
+00000ab0: 6d70 6c65 7854 7970 653e 0a0a 3c78 733a  mplexType>..<xs:
+00000ac0: 636f 6d70 6c65 7854 7970 6520 6e61 6d65  complexType name
+00000ad0: 3d22 496e 6c69 6e65 5461 626c 6552 6f77  ="InlineTableRow
+00000ae0: 456c 656d 656e 7422 3e0a 2020 3c78 733a  Element">.  <xs:
+00000af0: 7365 7175 656e 6365 3e0a 2020 2020 3c78  sequence>.    <x
+00000b00: 733a 656c 656d 656e 7420 6e61 6d65 3d22  s:element name="
+00000b10: 5661 6c75 6522 2074 7970 653d 2249 6e6c  Value" type="Inl
+00000b20: 696e 6554 6162 6c65 5661 6c75 6545 6c65  ineTableValueEle
+00000b30: 6d65 6e74 2220 6d61 784f 6363 7572 733d  ment" maxOccurs=
+00000b40: 2275 6e62 6f75 6e64 6564 222f 3e0a 2020  "unbounded"/>.  
+00000b50: 3c2f 7873 3a73 6571 7565 6e63 653e 0a3c  </xs:sequence>.<
+00000b60: 2f78 733a 636f 6d70 6c65 7854 7970 653e  /xs:complexType>
+00000b70: 0a0a 3c78 733a 636f 6d70 6c65 7854 7970  ..<xs:complexTyp
+00000b80: 6520 6e61 6d65 3d22 496e 6c69 6e65 5461  e name="InlineTa
+00000b90: 626c 6556 616c 7565 456c 656d 656e 7422  bleValueElement"
+00000ba0: 3e0a 2020 3c78 733a 7369 6d70 6c65 436f  >.  <xs:simpleCo
+00000bb0: 6e74 656e 743e 0a20 2020 203c 7873 3a65  ntent>.    <xs:e
+00000bc0: 7874 656e 7369 6f6e 2062 6173 653d 2278  xtension base="x
+00000bd0: 733a 7374 7269 6e67 223e 0a20 2020 2020  s:string">.     
+00000be0: 203c 7873 3a61 7474 7269 6275 7465 206e   <xs:attribute n
+00000bf0: 616d 653d 2263 6f6c 756d 6e22 2074 7970  ame="column" typ
+00000c00: 653d 2278 733a 7374 7269 6e67 2220 7573  e="xs:string" us
+00000c10: 653d 2272 6571 7569 7265 6422 2f3e 0a20  e="required"/>. 
+00000c20: 2020 203c 2f78 733a 6578 7465 6e73 696f     </xs:extensio
+00000c30: 6e3e 0a20 203c 2f78 733a 7369 6d70 6c65  n>.  </xs:simple
+00000c40: 436f 6e74 656e 743e 0a3c 2f78 733a 636f  Content>.</xs:co
+00000c50: 6d70 6c65 7854 7970 653e 0a0a 3c78 733a  mplexType>..<xs:
+00000c60: 636f 6d70 6c65 7854 7970 6520 6e61 6d65  complexType name
+00000c70: 3d22 4c65 7665 6c45 6c65 6d65 6e74 223e  ="LevelElement">
+00000c80: 0a20 203c 7873 3a73 6571 7565 6e63 653e  .  <xs:sequence>
+00000c90: 0a20 2020 203c 7873 3a65 6c65 6d65 6e74  .    <xs:element
+00000ca0: 206e 616d 653d 2250 726f 7065 7274 7922   name="Property"
+00000cb0: 2074 7970 653d 2250 726f 7065 7274 7945   type="PropertyE
+00000cc0: 6c65 6d65 6e74 2220 6d69 6e4f 6363 7572  lement" minOccur
+00000cd0: 733d 2230 2220 6d61 784f 6363 7572 733d  s="0" maxOccurs=
+00000ce0: 2275 6e62 6f75 6e64 6564 222f 3e0a 2020  "unbounded"/>.  
+00000cf0: 3c2f 7873 3a73 6571 7565 6e63 653e 0a20  </xs:sequence>. 
+00000d00: 200a 2020 3c78 733a 6174 7472 6962 7574   .  <xs:attribut
+00000d10: 6520 7265 663d 226e 616d 6522 2075 7365  e ref="name" use
+00000d20: 3d22 7265 7175 6972 6564 222f 3e0a 2020  ="required"/>.  
+00000d30: 3c78 733a 6174 7472 6962 7574 6520 6e61  <xs:attribute na
+00000d40: 6d65 3d22 6b65 795f 636f 6c75 6d6e 2220  me="key_column" 
+00000d50: 7479 7065 3d22 7873 3a73 7472 696e 6722  type="xs:string"
+00000d60: 2075 7365 3d22 7265 7175 6972 6564 222f   use="required"/
+00000d70: 3e0a 2020 3c78 733a 6174 7472 6962 7574  >.  <xs:attribut
+00000d80: 6520 6e61 6d65 3d22 6e61 6d65 5f63 6f6c  e name="name_col
+00000d90: 756d 6e22 2074 7970 653d 2278 733a 7374  umn" type="xs:st
+00000da0: 7269 6e67 222f 3e0a 2020 3c78 733a 6174  ring"/>.  <xs:at
+00000db0: 7472 6962 7574 6520 6e61 6d65 3d22 6b65  tribute name="ke
+00000dc0: 795f 7479 7065 2220 7479 7065 3d22 6b65  y_type" type="ke
+00000dd0: 7954 7970 6522 2f3e 0a3c 2f78 733a 636f  yType"/>.</xs:co
+00000de0: 6d70 6c65 7854 7970 653e 0a0a 3c78 733a  mplexType>..<xs:
+00000df0: 636f 6d70 6c65 7854 7970 6520 6e61 6d65  complexType name
+00000e00: 3d22 5072 6f70 6572 7479 456c 656d 656e  ="PropertyElemen
+00000e10: 7422 3e0a 2020 3c78 733a 6174 7472 6962  t">.  <xs:attrib
+00000e20: 7574 6520 7265 663d 226e 616d 6522 2075  ute ref="name" u
+00000e30: 7365 3d22 7265 7175 6972 6564 222f 3e0a  se="required"/>.
+00000e40: 2020 3c78 733a 6174 7472 6962 7574 6520    <xs:attribute 
+00000e50: 6e61 6d65 3d22 636f 6c75 6d6e 2220 7479  name="column" ty
+00000e60: 7065 3d22 7873 3a73 7472 696e 6722 2075  pe="xs:string" u
+00000e70: 7365 3d22 7265 7175 6972 6564 222f 3e0a  se="required"/>.
+00000e80: 2020 3c78 733a 6174 7472 6962 7574 6520    <xs:attribute 
+00000e90: 6e61 6d65 3d22 6361 7074 696f 6e5f 7365  name="caption_se
+00000ea0: 7422 2074 7970 653d 2278 733a 7374 7269  t" type="xs:stri
+00000eb0: 6e67 222f 3e0a 3c2f 7873 3a63 6f6d 706c  ng"/>.</xs:compl
+00000ec0: 6578 5479 7065 3e0a 0a3c 7873 3a63 6f6d  exType>..<xs:com
+00000ed0: 706c 6578 5479 7065 206e 616d 653d 224d  plexType name="M
+00000ee0: 6561 7375 7265 456c 656d 656e 7422 3e0a  easureElement">.
+00000ef0: 2020 3c78 733a 7365 7175 656e 6365 3e0a    <xs:sequence>.
+00000f00: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
+00000f10: 6e61 6d65 3d22 416e 6e6f 7461 7469 6f6e  name="Annotation
+00000f20: 2220 7479 7065 3d22 416e 6e6f 7461 7469  " type="Annotati
+00000f30: 6f6e 456c 656d 656e 7422 206d 6178 4f63  onElement" maxOc
+00000f40: 6375 7273 3d22 756e 626f 756e 6465 6422  curs="unbounded"
+00000f50: 2f3e 0a20 203c 2f78 733a 7365 7175 656e  />.  </xs:sequen
+00000f60: 6365 3e0a 0a20 203c 7873 3a61 7474 7269  ce>..  <xs:attri
+00000f70: 6275 7465 2072 6566 3d22 6e61 6d65 2220  bute ref="name" 
+00000f80: 7573 653d 2272 6571 7569 7265 6422 2f3e  use="required"/>
+00000f90: 0a20 203c 7873 3a61 7474 7269 6275 7465  .  <xs:attribute
+00000fa0: 206e 616d 653d 2261 6767 7265 6761 746f   name="aggregato
+00000fb0: 7222 2074 7970 653d 2278 733a 7374 7269  r" type="xs:stri
+00000fc0: 6e67 2220 7573 653d 2272 6571 7569 7265  ng" use="require
+00000fd0: 6422 2f3e 0a20 203c 7873 3a61 7474 7269  d"/>.  <xs:attri
+00000fe0: 6275 7465 206e 616d 653d 2263 6f6c 756d  bute name="colum
+00000ff0: 6e22 2074 7970 653d 2278 733a 7374 7269  n" type="xs:stri
+00001000: 6e67 2220 7573 653d 2272 6571 7569 7265  ng" use="require
+00001010: 6422 2f3e 0a3c 2f78 733a 636f 6d70 6c65  d"/>.</xs:comple
+00001020: 7854 7970 653e 0a0a 3c78 733a 636f 6d70  xType>..<xs:comp
+00001030: 6c65 7854 7970 6520 6e61 6d65 3d22 5461  lexType name="Ta
+00001040: 626c 6545 6c65 6d65 6e74 223e 0a20 203c  bleElement">.  <
+00001050: 7873 3a61 7474 7269 6275 7465 2072 6566  xs:attribute ref
+00001060: 3d22 6e61 6d65 2220 7573 653d 2272 6571  ="name" use="req
+00001070: 7569 7265 6422 2f3e 0a20 203c 7873 3a61  uired"/>.  <xs:a
+00001080: 7474 7269 6275 7465 206e 616d 653d 2270  ttribute name="p
+00001090: 7269 6d61 7279 5f6b 6579 2220 7479 7065  rimary_key" type
+000010a0: 3d22 7873 3a73 7472 696e 6722 2f3e 0a3c  ="xs:string"/>.<
+000010b0: 2f78 733a 636f 6d70 6c65 7854 7970 653e  /xs:complexType>
+000010c0: 0a0a 3c78 733a 656c 656d 656e 7420 6e61  ..<xs:element na
+000010d0: 6d65 3d22 5363 6865 6d61 223e 0a20 203c  me="Schema">.  <
+000010e0: 7873 3a63 6f6d 706c 6578 5479 7065 3e0a  xs:complexType>.
+000010f0: 2020 2020 3c78 733a 7365 7175 656e 6365      <xs:sequence
+00001100: 3e0a 2020 2020 2020 3c78 733a 656c 656d  >.      <xs:elem
+00001110: 656e 7420 6e61 6d65 3d22 5368 6172 6564  ent name="Shared
+00001120: 4469 6d65 6e73 696f 6e22 2074 7970 653d  Dimension" type=
+00001130: 2244 696d 656e 7369 6f6e 456c 656d 656e  "DimensionElemen
+00001140: 7422 206d 696e 4f63 6375 7273 3d22 3022  t" minOccurs="0"
+00001150: 206d 6178 4f63 6375 7273 3d22 756e 626f   maxOccurs="unbo
+00001160: 756e 6465 6422 2f3e 0a20 2020 2020 203c  unded"/>.      <
+00001170: 7873 3a65 6c65 6d65 6e74 206e 616d 653d  xs:element name=
+00001180: 2243 7562 6522 2074 7970 653d 2243 7562  "Cube" type="Cub
+00001190: 6545 6c65 6d65 6e74 2220 6d61 784f 6363  eElement" maxOcc
+000011a0: 7572 733d 2275 6e62 6f75 6e64 6564 222f  urs="unbounded"/
+000011b0: 3e0a 2020 2020 3c2f 7873 3a73 6571 7565  >.    </xs:seque
+000011c0: 6e63 653e 0a0a 2020 2020 3c78 733a 6174  nce>..    <xs:at
+000011d0: 7472 6962 7574 6520 7265 663d 226e 616d  tribute ref="nam
+000011e0: 6522 2075 7365 3d22 7265 7175 6972 6564  e" use="required
+000011f0: 222f 3e0a 2020 3c2f 7873 3a63 6f6d 706c  "/>.  </xs:compl
+00001200: 6578 5479 7065 3e0a 3c2f 7873 3a65 6c65  exType>.</xs:ele
+00001210: 6d65 6e74 3e0a 0a3c 2f78 733a 7363 6865  ment>..</xs:sche
+00001220: 6d61 3e20 0a                             ma> .
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/schema/traverse.py` & `tesseract_olap-0.7.0/tesseract_olap/schema/traverse.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,24 +61,25 @@
         for item in self.cube_map.values():
             locales.update(item.get_locale_available())
         # TODO: add from shared_dimension_map and shared_table_map
         locales.discard("xx")
         locales.add(self.schema.default_locale)
         return sorted(locales)
 
-    def get_public_schema(self, locale: Optional[str] = None):
+    def get_public_schema(self, roles: List[str] = [], locale: Optional[str] = None):
         """Generates a JSON-encodeable schema describing this entity."""
         default_locale = self.schema.default_locale
         locale = default_locale if locale is None else locale
         return {
             "name": self.schema.name,
             # "locales": self.get_locale_available(),
             "default_locale": default_locale,
             "cubes": [cube.get_public_schema(locale)
-                      for cube in self.cube_map.values()],
+                      for cube in self.cube_map.values()
+                      if cube.visible and cube.is_authorized(roles)],
             "annotations": self.schema.annotations,
         }
 
     def validate(self):
         """Performs some verifications on the resulting data structure, after
         parsing the schema file."""
 
@@ -105,14 +106,19 @@
     The relationships are made via the :class:`EntityUsageTraverser` subclasses,
     initialized upon creation.
     """
 
     _cube: "Cube"
     _dimension_map: Mapping[str, "DimensionTraverser"]
     _table: Union["Table", "InlineTable"]
+    annotations: Annotations
+    captions: CaptionSet
+    name: str
+    subset_table: bool
+    visible: bool
 
     def __init__(
         self,
         cube: "Cube",
         *,
         dimension_map: Mapping[str, "Dimension"],
         table_map: Mapping[str, "InlineTable"],
@@ -129,25 +135,16 @@
         self._table = table_map[cube.table] \
                       if isinstance(cube.table, str) else \
                       cube.table
 
     def __repr__(self) -> str:
         return f"CubeTraverser(name='{self._cube.name}', table={self.table})"
 
-    @property
-    def name(self) -> str:
-        return self._cube.name
-
-    @property
-    def annotations(self) -> Annotations:
-        return self._cube.annotations
-
-    @property
-    def captions(self) -> CaptionSet:
-        return self._cube.captions
+    def __getattr__(self, _name: str):
+        return getattr(self._cube, _name)
 
     @property
     def table(self) -> Union["Table", "InlineTable"]:
         return self._table
 
     @property
     def measures(self) -> Iterable["Measure"]:
@@ -304,14 +301,17 @@
                     "annotations": measure.annotations,
                 }
                 for measure in self.measures
             ],
             "annotations": self._cube.annotations,
         }
 
+    def is_authorized(self, roles: Iterable[str]):
+        return self._cube.is_authorized(roles)
+
 
 class EntityUsageTraverser(Generic[EntityType, UsageType]):
     """Wrapper class to unify an usage with its entity.
 
     Its properties are looked on the usage, then on the entity if not found.
     The usage instance is optional, as this wrapper also standardizes the
     properties and traversing methods across entities in the codebase.
@@ -578,19 +578,23 @@
         else:
             self.property_map = OrderedDict(
                 (name, PropertyTraverser(entity.property_map[item.source], item))
                 for name, item in usage.property_map.items()
             )
 
     @property
+    def type_caster(self):
+        return self.key_type.get_caster()
+
+    @property
     def properties(self) -> Iterable["PropertyTraverser"]:
         """Returns a generator that yields all Properties under this Level."""
         return self.property_map.values()
 
-    def get_name_column(self, locale: str = "xx"):
+    def get_name_column(self, locale: str = "xx") -> Union[str, None]:
         return self._entity.get_name_column(locale)
 
     def get_public_schema(self, locale: str):
         """Generates a JSON-encodeable schema describing this entity."""
         return {
             "name": self.name,
             "caption": self.get_caption(locale),
```

### Comparing `tesseract_olap-0.6.0/tesseract_olap/schema/xml.py` & `tesseract_olap-0.7.0/tesseract_olap/schema/xml.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 
 Defines subclasses for the core Entity classes, parsed from an XML document.
 """
 
 import logging
 from ast import literal_eval as eval_tuple
 from collections import OrderedDict
+from itertools import chain
 from pathlib import Path
 from typing import (Generator, Iterable, List, Optional, TextIO, Tuple, Type,
                     TypeVar, Union)
 
-import httpx
 import immutables as immu
 from lxml import etree
 
 from . import models
 from .aggregators import Aggregator
 from .csv import parse_csv
 from .enums import AggregatorType, DimensionType, MemberType
-from .exceptions import InvalidXMLAttributeValue, MissingXMLAttribute, MissingXMLNode
+from .exceptions import (InvalidXMLAttributeValue, MissingXMLAttribute,
+                         MissingXMLNode)
 
 logger = logging.getLogger(__name__)
 
 XMLEntity = Union[
     "XMLSharedDimension",
     "XMLHierarchy",
     "XMLLevel",
@@ -40,174 +41,220 @@
 AnyXMLEntity = TypeVar("AnyXMLEntity", bound=XMLEntity)
 
 
 class XMLSchema(models.Schema):
     tag = "Schema"
 
     @classmethod
-    def parse(cls, node: etree._Element):
+    def parse(cls, node: etree._Element, index: int = 0):
         """Parse a <Schema> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+
         cube_gen = _yield_children_nodes(node, XMLCube)
         shareddim_gen = _yield_children_nodes(node, XMLSharedDimension)
         sharedtbl_gen = _yield_children_nodes(node, XMLInlineTable)
 
         return cls(
-            name=_get_attr(node, "name"),
+            name=name,
             cube_map=OrderedDict(cube_gen),
             shared_dimension_map=immu.Map(shareddim_gen),
             shared_table_map=immu.Map(sharedtbl_gen),
             default_locale=node.get("default_locale", "xx"),
             annotations=immu.Map(_yield_annotations(node)),
         )
 
 
+class XMLAccessControl(models.AccessControl):
+    tag = "Access"
+
+    @classmethod
+    def parse(cls, node: etree._Element):
+        """Parse all <Access> XML node that are directly under this node."""
+
+        rules_gen = (
+            (role, _get_attr(item, "rule") == "allow")
+            for item in node.iterchildren(cls.tag)
+            for role in _get_attr(item, "roles").split(",")
+        )
+
+        return cls(
+            public=node.get("public", "true") == "true",
+            rules=immu.Map(rules_gen),
+        )
+
+
 class XMLCube(models.Cube):
     tag = "Cube"
 
     @classmethod
-    def parse(cls, node: etree._Element, _: int):
+    def parse(cls, node: etree._Element, index: int):
         """Parse a <Cube> XML node."""
-        cube_name = _get_attr(node, "name")
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
 
         table = _find_table_ref(node)
         if table is None:
-            raise MissingXMLNode(node.tag, cube_name, "Table")
+            raise MissingXMLNode(node.tag, name, "Table")
 
         dimension_map = OrderedDict(
             _yield_children_nodes(node, XMLPrivateDimension, XMLDimensionUsage)
         )
         if len(dimension_map) == 0:
-            raise MissingXMLNode(node.tag, cube_name, "Dimension")
+            raise MissingXMLNode(node.tag, name, "Dimension")
 
         measure_map = OrderedDict(_yield_children_nodes(node, XMLMeasure))
         if len(measure_map) == 0:
-            raise MissingXMLNode(node.tag, cube_name, "Measure")
+            raise MissingXMLNode(node.tag, name, "Measure")
 
         return cls(
-            name=cube_name,
+            name=name,
             captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            acl=XMLAccessControl.parse(node),
             dimension_map=dimension_map,
             measure_map=measure_map,
             table=table,
             annotations=immu.Map(_yield_annotations(node)),
+            subset_table=node.get("subset_table", "false").lower() != "false",
+            visible=node.get("visible", "true").lower() != "false",
         )
 
 
 class XMLDimensionUsage(models.DimensionUsage):
     tag = "DimensionUsage"
 
     @classmethod
-    def parse(cls, node: etree._Element, _: int):
+    def parse(cls, node: etree._Element, index: int):
         """Parse a <DimensionUsage> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+
         return cls(
-            name=_get_attr(node, "name"),
+            name=name,
             source=_get_attr(node, "source"),
-            foreign_key=node.get("foreign_key"),
+            foreign_key=_get_attr(node, "foreign_key"),
             annotations=immu.Map(_yield_annotations(node)),
             captions=immu.Map(_yield_locale_pairs(node, "caption")),
             hierarchy_map=OrderedDict(
                 _yield_children_nodes(node, XMLHierarchyUsage, attr="source")
             ),
         )
 
 
 class XMLHierarchyUsage(models.HierarchyUsage):
     tag = "HierarchyUsage"
 
     @classmethod
-    def parse(cls, node: etree._Element, _: int):
+    def parse(cls, node: etree._Element, index: int):
         """Parse a <HierarchyUsage> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+
         return cls(
-            name=_get_attr(node, "name"),
+            name=name,
             source=_get_attr(node, "source"),
             annotations=immu.Map(_yield_annotations(node)),
             captions=immu.Map(_yield_locale_pairs(node, "caption")),
             level_map=OrderedDict(
                 _yield_children_nodes(node, XMLLevelUsage, attr="source")
             ),
         )
 
 
 class XMLLevelUsage(models.LevelUsage):
     tag = "LevelUsage"
 
     @classmethod
-    def parse(cls, node: etree._Element, _: int):
+    def parse(cls, node: etree._Element, index: int):
         """Parse a <LevelUsage> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+
         return cls(
-            name=_get_attr(node, "name"),
+            name=name,
             source=_get_attr(node, "source"),
             annotations=immu.Map(_yield_annotations(node)),
             captions=immu.Map(_yield_locale_pairs(node, "caption")),
             property_map=OrderedDict(
                 _yield_children_nodes(node, XMLPropertyUsage, attr="source")
             ),
         )
 
 
 class XMLPropertyUsage(models.PropertyUsage):
     tag = "PropertyUsage"
 
     @classmethod
-    def parse(cls, node: etree._Element, _: int):
+    def parse(cls, node: etree._Element, index: int):
         """Parse a <PropertyUsage> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+
         return cls(
-            name=_get_attr(node, "name"),
+            name=name,
             source=_get_attr(node, "source"),
             annotations=immu.Map(_yield_annotations(node)),
             captions=immu.Map(_yield_locale_pairs(node, "caption")),
         )
 
 
 class XMLTable(models.Table):
     tag = "Table"
 
     @classmethod
-    def parse(cls, node: etree._Element, _: int):
+    def parse(cls, node: etree._Element, index: int):
         """Parse a <Table> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+
         return cls(
-            name=_get_attr(node, "name"),
+            name=name,
             schema=node.get("schema"),
-            primary_key=node.get("primary_key"),
+            primary_key=node.get("primary_key", "id"),
         )
 
 
 class XMLInlineTable(models.InlineTable):
     tag = "InlineTable"
 
     @classmethod
-    def parse(cls, node: etree._Element, _: int):
+    def parse(cls, node: etree._Element, index: int):
         """Parse a <InlineTable> XML node."""
-        node_name = _get_attr(node, "name")
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+
         node_format = _get_attr(node, "format")
 
         if node_format == "csv":
             node_format = "text/csv"
 
         if node_format == "tuples":
             headers, rows = cls.parse_tuples(node)
         elif node_format.startswith("text/csv"):
             content = [] if node.text is None else node.text.strip().splitlines()
             headers, *rows = parse_csv(content, mimetype=node_format)
+            headers = tuple(str(item) for item in headers)
         else:
-            raise InvalidXMLAttributeValue(node.tag, node_name, "format", node_format)
+            raise InvalidXMLAttributeValue(node.tag, name, "format", node_format)
 
         return cls(
-            name=node_name,
+            name=name,
             headers=headers,
-            types=tuple(MemberType.from_values(column) for column in zip(*rows)),
+            types=cls.infer_types(rows),
             rows=rows,
         )
 
     @staticmethod
-    def parse_tuples(node: etree._Element):
+    def parse_tuples(
+        node: etree._Element,
+    ) -> Tuple[Tuple[str, ...], List[Tuple[Union[str, float], ...]]]:
         """Parse the child nodes from an InlineTable with `tuples` format."""
         try:
             # try parsing literal tuples with ast.eval()
-            children: List[Tuple[str, ...]] = [
+            children: List[Tuple[Union[str, float], ...]] = [
                 eval_tuple(line)
                 for line in (item.text for item in node.iterchildren("Row"))
                 if line
             ]
         except SyntaxError:
             # Python `tuples` looks similar to CSV, so let's try with it
             row_iter = (
@@ -215,27 +262,31 @@
                 for line in (item.text for item in node.iterchildren("Row"))
                 if line is not None
             )
             children = parse_csv(row_iter, skipinitialspace=True)
         # at least 2 rows must be present: a header list and a data row
         if len(children) < 2:
             raise MissingXMLNode(node.tag, _get_attr(node, "name"), "Row")
-        return children[0], children[1:]
+        headers = tuple(str(item) for item in children[0])
+        return headers, children[1:]
 
 
 class XMLSharedDimension(models.Dimension):
     tag = "SharedDimension"
 
     @classmethod
-    def parse(cls, node: etree._Element, _: int):
+    def parse(cls, node: etree._Element, index: int):
         """Parse a Shared <Dimension> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+
         dim_type = node.get("type")
 
         return cls(
-            name=_get_attr(node, "name"),
+            name=name,
             captions=immu.Map(_yield_locale_pairs(node, "caption")),
             dim_type=DimensionType.from_str(dim_type),
             foreign_key=node.get("foreign_key"),
             hierarchy_map=OrderedDict(_yield_children_nodes(node, XMLHierarchy)),
             annotations=immu.Map(_yield_annotations(node)),
         )
 
@@ -255,28 +306,29 @@
         return dimension
 
 
 class XMLHierarchy(models.Hierarchy):
     tag = "Hierarchy"
 
     @classmethod
-    def parse(cls, node: etree._Element, _: int):
+    def parse(cls, node: etree._Element, index: int):
         """Parse a <Hierarchy> XML node."""
-        node_name = _get_attr(node, "name")
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
 
         level_map = OrderedDict(_yield_children_nodes(node, XMLLevel))
         if len(level_map) == 0:
-            raise MissingXMLNode(node.tag, node_name, "Level")
+            raise MissingXMLNode(node.tag, name, "Level")
 
         default_pk = ""
         for item in level_map.values():
             default_pk = item.key_column
 
         return cls(
-            name=node_name,
+            name=name,
             primary_key=node.get("primary_key", default_pk),
             captions=immu.Map(_yield_locale_pairs(node, "caption")),
             table=_find_table_ref(node),
             level_map=level_map,
             default_member=cls._parse_default_member(node),
             annotations=immu.Map(_yield_annotations(node)),
         )
@@ -289,72 +341,99 @@
 
 class XMLLevel(models.Level):
     tag = "Level"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a <Level> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+
         key_type = node.get("key_type")
 
         return cls(
-            name=_get_attr(node, "name"),
+            name=name,
             depth=index + 1,
             key_column=_get_attr(node, "key_column"),
             key_type=MemberType.from_str(key_type),
             captions=immu.Map(_yield_locale_pairs(node, "caption")),
             name_column_map=immu.Map(_yield_locale_pairs(node, "name_column")),
             property_map=OrderedDict(_yield_children_nodes(node, XMLProperty)),
             annotations=immu.Map(_yield_annotations(node)),
         )
 
 
 class XMLProperty(models.Property):
     tag = "Property"
 
     @classmethod
-    def parse(cls, node: etree._Element, _: int):
+    def parse(cls, node: etree._Element, index: int):
         """Parse a <Property> XML node."""
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+
         key_type = node.get("key_type")
 
         keycol_map = immu.Map(_yield_locale_pairs(node, "key_column"))
         if len(keycol_map) == 0:
             raise MissingXMLAttribute(node.tag, "key_column")
 
         return cls(
-            name=_get_attr(node, "name"),
+            name=name,
             annotations=immu.Map(_yield_annotations(node)),
             captions=immu.Map(_yield_locale_pairs(node, "caption")),
             key_column_map=keycol_map,
             key_type=MemberType.from_str(key_type),
         )
 
 
 class XMLMeasure(models.Measure):
     tag = "Measure"
 
     @classmethod
-    def parse(cls, node: etree._Element, _: int):
+    def parse(cls, node: etree._Element, index: int):
         """Parse a <Measure> XML node."""
-        submeasures = (
+        name = _get_attr(node, "name")
+        logger.debug("Parsing node <{} name='{}' />", cls.tag, name)
+
+        aggregator = cls._get_aggregator(node)
+        captions = immu.Map(_yield_locale_pairs(node, "caption"))
+
+        def _parse_column(node: etree._Element):
+            coltype = _get_attr(node, "type").upper()
+            colname = node.get("name", f"{name} {coltype}")
+            colcapt = immu.Map(_yield_locale_pairs(node, "caption"))
+            return cls(
+                name=colname,
+                key_column=_get_attr(node, "key_column"),
+                aggregator=aggregator,
+                annotations=immu.Map(_yield_annotations(node)),
+                captions=immu.Map(
+                    (locale, colcapt.get(locale, f"{caption} {coltype}"))
+                    for locale, caption in captions.items()
+                ),
+            )
+
+        measurecols = (
             (item.name, item)
             for item in (
-                models.SubMeasure(
-                    name=_get_attr(item, "name"),
-                    aggregator=cls._get_aggregator(item),
-                )
-                for item in node.iterchildren("Submeasure")
+                _parse_column(item)
+                for item in node.iterchildren("MeasureColumn")
             )
         )
+
+        submeasures = _yield_children_nodes(node, cls)
+
         return cls(
-            name=_get_attr(node, "name"),
+            name=name,
             key_column=_get_attr(node, "key_column"),
-            aggregator=cls._get_aggregator(node),
+            aggregator=aggregator,
             annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            submeasures=immu.Map(submeasures),
+            captions=captions,
+            submeasures=immu.Map(chain(measurecols, submeasures)),
         )
 
     @staticmethod
     def _get_aggregator(mea_node: etree._Element) -> Aggregator:
         """
         Raises:
             :class:`MissingXMLAttribute` --
@@ -375,42 +454,49 @@
         try:
             agg_type = AggregatorType.from_str(value)
         except ValueError:
             node_name = _get_attr(mea_node, "name")
             raise InvalidXMLAttributeValue(node.tag, node_name, attr, value)
         else:
             agg_cls = Aggregator.from_enum(agg_type)
-            return agg_cls.new(node.attrib)
+            agg_args = {str(k).replace("-", "_"): str(v) for k, v in node.attrib.items()}
+            return agg_cls.new(agg_args)
 
 
 def _find_table_ref(node: etree._Element):
-    table_node = next(node.iterchildren("InlineTable", "Table", "TableUsage"), None)
+    gen_tables = (item for item in node.iterchildren("InlineTable", "Table", "TableUsage"))
+    table_node = next(gen_tables, None)
 
     if table_node is None:
         return None
     elif table_node.tag == "InlineTable":
         return XMLInlineTable.parse(table_node, 0)
     elif table_node.tag == "Table":
         return XMLTable.parse(table_node, 0)
     elif table_node.tag == "TableUsage":
         return _get_attr(table_node, "source")
 
     raise MissingXMLNode(node.tag, _get_attr(node, "name"), "Table")
 
 
 def _get_attr(node: etree._Element, attr: str) -> str:
+    """Retrieves an attribute from a node.
+
+    If the attribute is not present, raises :class:`MissingXMLAttribute`.
+    """
     try:
         value = node.attrib[attr]
-    except KeyError:
-        raise MissingXMLAttribute(node.tag, attr)
+    except KeyError as exc:
+        raise MissingXMLAttribute(node.tag, attr) from exc
     else:
-        return value
+        return str(value)
 
 
 def _yield_annotations(node: etree._Element) -> Iterable[Tuple[str, Optional[str]]]:
+    """Yields a pair of (name, value) for each Annotation in the node."""
     return (
         (_get_attr(item, "name"), item.text)
         for item in node.iterchildren("Annotation")
     )
 
 
 def _yield_children_nodes(
@@ -437,82 +523,29 @@
             continue
 
         child_value = child_node.get("value", child_node.text)
         if child_value is not None:
             yield (_get_attr(child_node, "locale"), child_value)
 
 
-def _parse_pathlib_path(path: Path, parser: etree.XMLParser) -> XMLSchema:
-    """Parses an XML schema from the content of a specific pathlib.Path instance.
-
-    This function is able to parse a single file, or all files in a directory.
-    """
-    if not path.exists():
-        raise FileNotFoundError("XML source: Path {} does not exist".format(path))
-
-    def read_xml_path(path: Path) -> XMLSchema:
-        with path.open("r") as fileio:
-            tree = etree.parse(fileio, parser)
-        root = tree.getroot()
-        return XMLSchema.parse(root)
-
-    # If path is directory, load all XMLs and combine them
-    if path.is_dir():
-        schemas = (read_xml_path(item)
-                  for item in path.glob("**/*.xml") if item.is_file())
-        return XMLSchema.join(*schemas)
-
-    # If path is file, load and parse it
-    if path.is_file():
-        return read_xml_path(path)
-
-    raise ValueError("XML source: Path can't be interpreted")
-
-
 def parse_xml_schema(source: Union[str, Path, TextIO]) -> XMLSchema:
     """Attempts to parse an object into a XMLSchema.
 
     This function accepts:
-    - An URL (as a :class:`str`)
-    - A local path (as a :class:`str` or :class:`pathlib.Path`) to a XML file,
-      or a directory containing XML files
     - A raw XML :class:`str`
+    - A local path (as a :class:`pathlib.Path`) to a XML file
     - A not-binary read-only :class:`TextIO` instance for a file-like object
     """
     parser = etree.XMLParser(encoding="utf-8",
                              remove_blank_text=True,
                              remove_comments=True)
 
-    # if argument is string...
+    # if argument is str, is assumed to be a raw XML string
     if isinstance(source, str):
-        source = source.strip()
-
-        # Check if argument is a URL and fetch the file
-        if source.startswith(("http://", "https://", "ftp://")):
-            response = httpx.get(source)
-            response.raise_for_status()
-
-            root = etree.fromstring(response.text, parser)
-            return XMLSchema.parse(root)
-
-        # Check if argument is a path and load the file(s)
-        elif source.endswith((".xml", "/", "\\")):
-            path = Path(source).resolve()
-            return _parse_pathlib_path(path, parser)
-
-        # Check if argument is a raw XML string
-        elif source.startswith("<Schema "):
-            root = etree.fromstring(source, parser)
-            return XMLSchema.parse(root)
-
-        raise ValueError("XML source: Value can't be recognized")
-
-    # if argument is a pathlib.Path, open it and parse contents
-    elif isinstance(source, Path):
-        path = source.resolve()
-        return _parse_pathlib_path(path, parser)
+        root = etree.fromstring(source, parser)
+        return XMLSchema.parse(root)
 
-    # if argument is not a string, attempt to use it like a file-like object
+    # if argument is pathlib.Path or TextIO, open it and parse contents
     else:
         tree = etree.parse(source, parser)
         root = tree.getroot()
         return XMLSchema.parse(root)
```

### Comparing `tesseract_olap-0.6.0/PKG-INFO` & `tesseract_olap-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesseract-olap
-Version: 0.6.0
+Version: 0.7.0
 Summary: A simple OLAP library.
 Home-page: https://github.com/Datawheel/tesseract-python
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

