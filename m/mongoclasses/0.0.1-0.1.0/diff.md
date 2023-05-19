# Comparing `tmp/mongoclasses-0.0.1.tar.gz` & `tmp/mongoclasses-0.1.0.tar.gz`

## Comparing `mongoclasses-0.0.1.tar` & `mongoclasses-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mongoclasses-0.0.1/src/mongoclasses/__about__.py
--rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 mongoclasses-0.0.1/src/mongoclasses/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoclasses-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 mongoclasses-0.0.1/tests/test_mongoclasses.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mongoclasses-0.0.1/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mongoclasses-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 mongoclasses-0.0.1/README.md
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 mongoclasses-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 mongoclasses-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/src/mongoclasses/__about__.py
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/src/mongoclasses/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/tests/test_mongoclasses.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/README.md
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 mongoclasses-0.1.0/PKG-INFO
```

### Comparing `mongoclasses-0.0.1/tests/test_mongoclasses.py` & `mongoclasses-0.1.0/tests/test_mongoclasses.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from dataclasses import dataclass, asdict
+
 from bson import ObjectId
 import pytest
 import pytest_asyncio
 from motor.motor_asyncio import AsyncIOMotorClient
+
 from mongoclasses import (
     mongoclass, insert_one, update_one, delete_one, find_one, find, fromdict
 )
 
 
 @pytest_asyncio.fixture
 async def database():
@@ -22,53 +25,64 @@
         name: str = ""
 
     return Foo
 
 
 def test_mongoclass_creation(database):
     # Missing a database.
-    with pytest.raises(AssertionError):
+    with pytest.raises(RuntimeError):
         @mongoclass
         class Foo:
             _id: ObjectId | None = None
 
     # Missing an _id field.
-    with pytest.raises(AssertionError):
+    with pytest.raises(AttributeError):
         @mongoclass(db=database)
         class Foo:
             ...
 
+    # Valid mongoclass
     @mongoclass(db=database)
     class Foo:
         _id: ObjectId | None = None
     
-    assert Foo.__mongomini_collection__.database == database
-    assert Foo.__mongomini_collection__.name == 'foo'
+    assert Foo.__mongoclasses_collection__.database == database
+    assert Foo.__mongoclasses_collection__.name == 'foo'
+
+    # Mongoclass being created from an already existing dataclass.
+    @dataclass
+    class Foo:
+        _id: ObjectId | None = None
+    
+    Foo = mongoclass(db=database)(Foo)
+    
+    assert Foo.__mongoclasses_collection__.database == database
+    assert Foo.__mongoclasses_collection__.name == 'foo'
 
 
 def test_mongoclass_collection_name(database):
     @mongoclass(db=database, collection_name='foobar')
     class Foo:
         _id: ObjectId | None = None
     
-    assert Foo.__mongomini_collection__.name == 'foobar'
+    assert Foo.__mongoclasses_collection__.name == 'foobar'
 
 
 def test_database_inheritance(database):
 
     @mongoclass(db=database)
     class Foo:
         _id: ObjectId | None = None
 
     @mongoclass
     class Bar(Foo):
         ...
 
-    assert Foo.__mongomini_collection__.database == database
-    assert Bar.__mongomini_collection__.database == database
+    assert Foo.__mongoclasses_collection__.database == database
+    assert Bar.__mongoclasses_collection__.database == database
 
 
 @pytest.mark.asyncio
 async def test_insert_one(Foo, database):    
     f = Foo()
     await insert_one(f)
 
@@ -100,15 +114,15 @@
 @pytest.mark.asyncio
 async def test_find_one(Foo):
     f = Foo()
     await insert_one(f)
 
     # Find document that exists
     result = await find_one(Foo, {'_id': f._id})
-    assert result['_id'] == f._id
+    assert result._id == f._id
 
     # find document that does not exist.
     result = await find_one(Foo, {'_id': "abcdef"})
     assert result is None
 
 
 @pytest.mark.asyncio
@@ -129,19 +143,15 @@
 
     assert len(l) == 3
 
 
 @pytest.mark.asyncio
 async def test_fromdict(Foo):
     f1 = Foo()
-    await insert_one(f1)
-
-    data = await find_one(Foo, {'_id': f1._id})
-    f2 = fromdict(Foo, data)
-
+    f2 = fromdict(Foo, asdict(f1))
     assert f1 == f2
 
 
 @pytest.mark.asyncio
 async def test_non_mongoclasses_in_mongoclass_functions():
     class Foo:
         ...
```

### Comparing `mongoclasses-0.0.1/.gitignore` & `mongoclasses-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mongoclasses-0.0.1/LICENSE.txt` & `mongoclasses-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mongoclasses-0.0.1/pyproject.toml` & `mongoclasses-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mongoclasses-0.0.1/PKG-INFO` & `mongoclasses-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongoclasses
-Version: 0.0.1
+Version: 0.1.0
 Project-URL: Documentation, https://github.com/rykroon/mongoclasses#readme
 Project-URL: Issues, https://github.com/rykroon/mongoclasses/issues
 Project-URL: Source, https://github.com/rykroon/mongoclasses
 Author-email: Ryan Kroon <rykroon.tech@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

