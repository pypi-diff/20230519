# Comparing `tmp/typodoo-0.2.tar.gz` & `tmp/typodoo-0.3.tar.gz`

## Comparing `typodoo-0.2.tar` & `typodoo-0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 typodoo-0.2/typodoo.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 typodoo-0.2/typodoo_activate.pth
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 typodoo-0.2/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 typodoo-0.2/LICENSE.txt
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 typodoo-0.2/README.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 typodoo-0.2/pyproject.toml
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 typodoo-0.2/PKG-INFO
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 typodoo-0.3/typodoo.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 typodoo-0.3/typodoo_activate.pth
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 typodoo-0.3/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 typodoo-0.3/LICENSE.txt
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 typodoo-0.3/README.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 typodoo-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 typodoo-0.3/PKG-INFO
```

### Comparing `typodoo-0.2/typodoo.py` & `typodoo-0.3/typodoo.py`

 * *Files 17% similar despite different names*

```diff
@@ -49,15 +49,18 @@
                     return True
             return False
 
         # if '_original_module' is into attrs, the metaclass is called
         # from the method BaseModel._build_model when the class hierarchy
         # is build from the graph. We must only take care of the first call
         # to the metaclass when the original module is imported.
-        if "_original_module" not in attrs:
+        # We must take care of a special case where Odoo define a Mocked
+        # implementation of IrQweb by python inheritance to allows the rendition
+        # of views while no database is selected
+        if "_original_module" not in attrs and name != "MockIrQWeb":
             if _extends(bases):
                 # TODO support delegation inheritance too ?
                 # TODO Merge with existing _inherit field, or error if already set.
                 attrs["_inherit"] = list(_inherit(bases))
                 bases = tuple(_bases(bases))  # TODO Deduplicate.
 
         return _orig_new(meta, name, bases, attrs)
@@ -70,14 +73,17 @@
         return _orig_init(self, name, bases, attrs)
 
     model.MetaModel.__init__ = _typodoo_init
 
     _orig_call = model.MetaModel.__call__
 
     def _typodoo_call(cls, env, *args):
+        if not hasattr(env, "registry"):
+            # no DB selected -> no registry initialized
+            return _orig_call(cls, env, *args)
         registry_cls = env.registry[cls._name]
         if cls is registry_cls:
             # cls is in registry, we likely come from api.Environment.__get_item__
             # and we want to call the regular constructor.
             return _orig_call(cls, env, *args)
         else:
             # We are instanciating a class that is not in the registry so
```

### Comparing `typodoo-0.2/.gitignore` & `typodoo-0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `typodoo-0.2/LICENSE.txt` & `typodoo-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `typodoo-0.2/README.md` & `typodoo-0.3/README.md`

 * *Files identical despite different names*

### Comparing `typodoo-0.2/pyproject.toml` & `typodoo-0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typodoo-0.2/PKG-INFO` & `typodoo-0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: typodoo
-Version: 0.2
+Version: 0.3
 Summary: Towards idiomatic Python with types for the Odoo ORM
 Project-URL: Documentation, https://github.com/sbidoul/typodoo#readme
 Project-URL: Issues, https://github.com/sbidoul/typodoo/issues
 Project-URL: Source, https://github.com/sbidoul/typodoo
 Author-email: Stéphane Bidoul <stephane.bidoul@acsone.eu>
+License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Odoo
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Requires-Dist: wrapt
```

