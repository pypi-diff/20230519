# Comparing `tmp/strawberry_django_plus-2.4.0.tar.gz` & `tmp/strawberry_django_plus-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-2.4.0.tar", max compression
+gzip compressed data, was "strawberry_django_plus-2.4.1.tar", max compression
```

## Comparing `strawberry_django_plus-2.4.0.tar` & `strawberry_django_plus-2.4.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1077 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/LICENSE
--rw-r--r--   0        0        0     3299 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/README.md
--rw-r--r--   0        0        0     4162 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     2950 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5554 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5751 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    26052 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3069 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1641 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1389 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0     6287 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/middlewares/debug_toolbar.py
--rw-r--r--   0        0        0        0 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    25062 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14819 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    24443 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1372 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    27509 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0    47551 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1107 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0     1445 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
--rw-r--r--   0        0        0        0 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2337 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    17876 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/type.py
--rw-r--r--   0        0        0    10174 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6924 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    12426 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     5865 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    13406 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      938 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     5169 1970-01-01 00:00:00.000000 strawberry_django_plus-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-19 15:14:15.513954 strawberry_django_plus-2.4.1/LICENSE
+-rw-r--r--   0        0        0     3299 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/README.md
+-rw-r--r--   0        0        0     4290 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2950 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5562 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5751 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    26052 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3069 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1657 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1389 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1168 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0     6304 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/middlewares/debug_toolbar.py
+-rw-r--r--   0        0        0        0 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    25062 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14825 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    24443 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1372 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    27526 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0    47560 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1107 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0     1445 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
+-rw-r--r--   0        0        0        0 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2337 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    18301 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0    10174 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6916 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    12426 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     5865 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    13142 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      938 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 strawberry_django_plus-2.4.1/PKG-INFO
```

### Comparing `strawberry_django_plus-2.4.0/LICENSE` & `strawberry_django_plus-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/README.md` & `strawberry_django_plus-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/pyproject.toml` & `strawberry_django_plus-2.4.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "2.4.0"
+version = "2.4.1"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
@@ -53,78 +53,84 @@
 django-debug-toolbar = "^4.0.0"
 django-choices-field = "^2.0"
 django-guardian = "^2.4.0"
 mkdocs = "^1.4.2"
 mkdocs-markdownextradata-plugin = "^0.2.5"
 mkdocs-material = "^9.0.9"
 mkdocs-minify-plugin = "^0.6.2"
-pymdown-extensions = "^9.5"
+pymdown-extensions = ">=9.5,<11.0"
 Markdown = "^3.3.7"
-ruff = "^0.0.261"
+ruff = "^0.0.269"
 
 
 [tool.poetry.extras]
 enum = ["django-choices-field"]
 debug-toolbar = ["django-debug-toolbar"]
 
 [tool.ruff]
 line-length = 100
 select = [
-  "E",
-  "F",
-  "W",
-  "I",
-  "N",
+  "A",
+  "ASYNC100",
+  "ASYNC101",
+  "ASYNC102",
+  "B",
+  "BLE",
+  "C4",
+  "COM",
   "D",
-  "UP",
-  "YTT",
   "D2",
   "D3",
   "D4",
-  "BLE",
-  "B",
-  "A",
-  "COM",
-  "C4",
   "DTZ",
-  "T10",
+  "E",
+  "ERA",
   "EXE",
-  "ISC",
-  "ICN001",
+  "F",
+  "FLY",
   "G",
+  "I",
+  "ICN001",
   "INP",
+  "INT",
+  "ISC",
+  "N",
+  "PGH",
   "PIE",
-  "T20",
-  "PYI",
+  "PL",
   "PT",
+  "PTH",
+  "PYI",
   "Q",
   "RET",
-  "SIM",
-  "TID",
-  "TCH",
-  "PTH",
-  "ERA",
-  "PGH",
-  "PL",
   "RSE",
   "RUF",
-  "TRY",
+  "TD",
+  "SIM",
   "SLF",
+  "T10",
+  "T20",
+  "TCH",
+  "TID",
+  "TRY",
+  "UP",
+  "W",
+  "YTT",
 ]
 ignore = [
   "D1",
   "D203",
   "D213",
-  "TCH001",
-  "TCH002",
-  "TCH003",
   "PGH003",
   "PLR09",
-  "PLR2004",
+  "RUF009",
   "SLF001",
+  "TD001",
+  "TD002",
+  "TD003",
   "TRY003",
 ]
 target-version = "py38"
 exclude = [
   ".eggs",
   ".git",
   ".hg",
@@ -134,15 +140,16 @@
   "__pycached__",
   "_build",
   "buck-out",
   "build",
   "dist",
 ]
 
-[tool.ruff.pyupgrade]
+[tool.ruff.per-file-ignores]
+"tests/*" = ["PLR2004"]
 
 [tool.ruff.isort]
 known-first-party = ["strawberry-django-plus"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
@@ -167,15 +174,15 @@
 '''
 
 [tool.pyright]
 pythonVersion = "3.8"
 useLibraryCodeForTypes = true
 venvPath = "."
 venv = ".venv"
-ignore = ["**/migrations"]
+exclude = [".venv", "**/migrations", "dist", "docs"]
 reportCallInDefaultInitializer = "warning"
 reportMatchNotExhaustive = "warning"
 reportMissingSuperCall = "warning"
 reportOverlappingOverload = "warning"
 reportUninitializedInstanceVariable = "none"
 reportUnnecessaryCast = "warning"
 reportUnnecessaryTypeIgnoreComment = "warning"
```

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/__init__.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/descriptors.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,21 @@
     Type,
     TypeVar,
     Union,
     overload,
 )
 
 from django.db.models.base import Model
-from django.db.models.query import Prefetch
 from typing_extensions import Self
 
-from .utils.typing import TypeOrSequence
-
 if TYPE_CHECKING:
+    from django.db.models.query import Prefetch
+
     from .optimizer import OptimizerStore, PrefetchType
+    from .utils.typing import TypeOrSequence
 
 __all__ = [
     "ModelProperty",
     "model_cached_property",
 ]
 
 _T = TypeVar("_T")
```

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/directives.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/field.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/field.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/filters.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/gql/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import TYPE_CHECKING
 
-import strawberry_django
+import strawberry_django  # noqa: TCH002
 from strawberry import (
     ID,
     UNSET,
     BasePermission,
     LazyType,
     Private,
     Schema,
```

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/middlewares/debug_toolbar.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/middlewares/debug_toolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         if not show_toolbar(request) or DebugToolbar.is_toolbar_request(request):
             return response
 
         content_type = response.get("Content-Type", "").split(";")[0]
         is_html = content_type in _HTML_TYPES
         is_graphiql = getattr(request, "_is_graphiql", False)
 
-        if is_html and is_graphiql and response.status_code == 200:
+        if is_html and is_graphiql and response.status_code == 200:  # noqa: PLR2004
             template = render_to_string("strawberry_django_plus/debug_toolbar.html")
             response.write(template)
             if "Content-Length" in response:
                 response["Content-Length"] = len(response.content)
 
         if is_html or not is_graphiql or content_type != "application/json":
             return response
```

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/mutations/fields.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/mutations/resolvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from django.db.models.fields.reverse_related import (
     ForeignObjectRel,
     ManyToManyRel,
     ManyToOneRel,
     OneToOneRel,
 )
 from strawberry import UNSET
-from strawberry.file_uploads.scalars import Upload
 from strawberry.types.info import Info
 from strawberry_django.fields.types import (
     ManyToManyInput,
     ManyToOneInput,
     OneToManyInput,
     OneToOneInput,
 )
@@ -41,14 +40,15 @@
 from strawberry_django_plus.types import ListInput, NodeInput
 from strawberry_django_plus.utils import aio
 from strawberry_django_plus.utils.inspect import get_model_fields
 from strawberry_django_plus.utils.resolvers import resolve_sync
 
 if TYPE_CHECKING:
     from django.db.models.manager import ManyToManyRelatedManager, RelatedManager
+    from strawberry.file_uploads.scalars import Upload
 
 _T = TypeVar("_T")
 _M = TypeVar("_M", bound=Model)
 _InputListTypes: TypeAlias = Union[strawberry.ID, "ParsedObject"]
 
 
 class FullCleanOptions(TypedDict, total=False):
@@ -252,15 +252,15 @@
 
     obj_models = [obj.__class__ for obj in instances]
     assert len(set(obj_models)) == 1
     fields = get_model_fields(obj_models[0])
     files: List[
         Tuple[
             models.FileField,
-            Union[Upload, Literal[False]],
+            Union["Upload", Literal[False]],
         ]
     ] = []
     m2m: List[Tuple[Union[ManyToManyField, ForeignObjectRel], Any]] = []
 
     if dataclasses.is_dataclass(data):
         data = vars(data)
```

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/optimizer.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/ordering.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/ordering.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/permissions.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -486,15 +486,15 @@
             "are checking for any permission for the given resource."
         ),
     )
 
     @classmethod
     def from_perm(cls, perm: str):
         parts = perm.split(".")
-        if len(parts) != 2:
+        if len(parts) != 2:  # noqa: PLR2004
             raise TypeError(
                 "Permissions need to be defined as `app_label.perm`, `app_label.` or `.perm`",
             )
         return cls(
             resource=parts[0].strip() or None,
             permission=parts[1].strip() or None,
         )
```

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/relay.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/relay.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
     """
     try:
         res = base64.b64decode(value.encode()).decode().split(":", 1)
     except Exception as e:  # noqa: BLE001
         raise ValueError(str(e)) from e
 
-    if len(res) != 2:
+    if len(res) != 2:  # noqa: PLR2004
         raise ValueError(f"{res} expected to contain only 2 items")
 
     return res[0], res[1]
 
 
 def to_base64(type_: Union[str, type, TypeDefinition], node_id: Any) -> str:
     """Encode the type name and node id to a base64 string.
@@ -167,19 +167,19 @@
 
     type_name: str
     node_id: str
 
     def __post_init__(self):
         if not isinstance(self.type_name, str):
             raise GlobalIDValueError(
-                f"type_name is expected to be a string, found {repr(self.type_name)}",
+                f"type_name is expected to be a string, found {self.type_name!r}",
             )
         if not isinstance(self.node_id, str):
             raise GlobalIDValueError(
-                f"node_id is expected to be a string, found {repr(self.node_id)}",
+                f"node_id is expected to be a string, found {self.node_id!r}",
             )
 
     def __str__(self):
         return to_base64(self.type_name, self.node_id)
 
     @classmethod
     def from_id(cls, value: Union[str, strawberry.ID]):
```

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/settings.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html` & `strawberry_django_plus-2.4.1/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/test/client.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/test/client.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/type.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/type.py`

 * *Files 4% similar despite different names*

```diff
@@ -323,14 +323,21 @@
 
         if not _has_own_node_resolver(cls, "resolve_id"):
             cls.resolve_id = types.MethodType(
                 lambda cls, root, *args, **kwargs: resolve_model_id(cls, root),
                 cls,
             )
 
+        # Adjust types that inherit from other types/interfaces that implement Node
+        # to make sure they pass themselves as the node type
+        for attr in ["resolve_node", "resolve_nodes", "resolve_id"]:
+            meth = getattr(cls, attr)
+            if isinstance(meth, types.MethodType) and meth.__self__ is not cls:
+                setattr(cls, attr, types.MethodType(cast(classmethod, meth).__func__, cls))
+
     strawberry.type(cls, **kwargs)
 
     # restore original annotations for further use
     cls.__annotations__ = original_annotations
     cls._django_type = django_type  # type: ignore
 
     return cls
```

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/types.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/utils/aio.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     while is_awaitable(ret, info=info):
         ret = await cast(Awaitable, ret)
 
     if ensure_type is not None:
         if (origin := get_origin(ensure_type)) and origin is Union:
             ensure_type = tuple(get_args(ensure_type))
         if not isinstance(ret, ensure_type):
-            raise TypeError(f"{ensure_type} expected, found {repr(ret)}")
+            raise TypeError(f"{ensure_type} expected, found {ret!r}")
 
     # FIXME: Remove cast once pyright resolves the negative TypeGuard form
     ret = cast(_R, ret)
 
     return ret
 
 
@@ -155,15 +155,15 @@
         return resolve_async(value, resolver, info=info, ensure_type=ensure_type)
 
     ret = resolver(value)
     if ensure_type is not None:
         if (origin := get_origin(ensure_type)) and origin is Union:
             ensure_type = tuple(get_args(ensure_type))
         if not isinstance(ret, ensure_type):
-            raise TypeError(f"{ensure_type} expected, found {repr(ret)}")
+            raise TypeError(f"{ensure_type} expected, found {ret!r}")
 
     return ret
 
 
 @overload
 def resolver(
     func: Callable[_P, AwaitableOrValue[_R]],
```

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/utils/resolvers.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import warnings
 from typing import (
     Any,
     Awaitable,
     Callable,
     Coroutine,
     Iterable,
-    List,
     Literal,
     Optional,
     Type,
     TypeVar,
     Union,
     cast,
     overload,
@@ -33,18 +32,20 @@
 from .inspect import get_django_type
 
 _T = TypeVar("_T")
 _M = TypeVar("_M", bound=Model)
 _R = TypeVar("_R")
 _P = ParamSpec("_P")
 _sentinel = object()
-_async_to_sync = cast(
-    Callable[[Callable[[Awaitable[_T]], Coroutine[Any, Any, _T]]], Callable[[Awaitable[_T]], _T]],
-    async_to_sync,
-)
+
+
+def _async_to_sync(
+    func: Callable[[Awaitable[_T]], Coroutine[Any, Any, _T]],
+) -> Callable[[Awaitable[_T]], _T]:
+    return async_to_sync(func)
 
 
 @overload
 def async_safe(
     func: Callable[_P, _R],
     /,
     *,
@@ -195,26 +196,17 @@
         inspect.iscoroutinefunction(resolver) or inspect.isasyncgenfunction(resolver)
     ):
         resolver = sync_to_async(resolver, thread_sensitive=True)
 
     return resolver(qs)
 
 
-resolve_qs_get_list = cast(
-    Callable[[AwaitableOrValue[QuerySet[_M]]], AwaitableOrValue[List[_M]]],
-    functools.partial(resolve_qs, resolver=list),
-)
-resolve_qs_get_first = cast(
-    Callable[[AwaitableOrValue[QuerySet[_M]]], AwaitableOrValue[Optional[_M]]],
-    functools.partial(resolve_qs, resolver=lambda qs: qs.first()),
-)
-resolve_qs_get_one = cast(
-    Callable[[AwaitableOrValue[QuerySet[_M]]], AwaitableOrValue[_M]],
-    functools.partial(resolve_qs, resolver=lambda qs: qs.get()),
-)
+resolve_qs_get_list = functools.partial(resolve_qs, resolver=list)
+resolve_qs_get_first = functools.partial(resolve_qs, resolver=lambda qs: qs.first())
+resolve_qs_get_one = functools.partial(resolve_qs, resolver=lambda qs: qs.get())
 
 
 @overload
 def resolve_result(
     res: AwaitableOrValue[Union[BaseManager[_M], QuerySet[_M]]],
     *,
     qs_resolver: None = ...,
@@ -414,15 +406,15 @@
 
     """
     if issubclass(source, Model):
         origin = None
     else:
         origin = source
         django_type = get_django_type(source, ensure_type=True)
-        source = cast(Type[_M], django_type.model)
+        source = cast(Type[Model], django_type.model)
 
     if isinstance(node_id, GlobalID):
         node_id = node_id.node_id
 
     id_attr = getattr(origin, "id_attr", "pk")
 
     qs = source._default_manager.filter(**{id_attr: node_id})
```

### Comparing `strawberry_django_plus-2.4.0/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-2.4.1/strawberry_django_plus/utils/typing.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.0/PKG-INFO` & `strawberry_django_plus-2.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 2.4.0
+Version: 2.4.1
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
@@ -20,19 +20,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: debug-toolbar
 Provides-Extra: enum
 Requires-Dist: django (>=3.2)
 Requires-Dist: django-choices-field (>=2.0) ; extra == "enum"
 Requires-Dist: django-debug-toolbar (>=3.4) ; extra == "debug-toolbar"
 Requires-Dist: strawberry-graphql (>=0.161.0)
 Requires-Dist: strawberry-graphql-django (>=0.8)
```

