# Comparing `tmp/ninjax-1.0.0.tar.gz` & `tmp/ninjax-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjax-1.0.0.tar", last modified: Wed Feb 22 13:34:45 2023, max compression
+gzip compressed data, was "ninjax-1.1.0.tar", last modified: Fri May 19 19:50:55 2023, max compression
```

## Comparing `ninjax-1.0.0.tar` & `ninjax-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-02-22 13:34:45.113261 ninjax-1.0.0/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1071 2022-08-08 16:14:32.000000 ninjax-1.0.0/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)     9671 2023-02-22 13:34:45.113261 ninjax-1.0.0/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)     9261 2023-02-22 13:32:36.000000 ninjax-1.0.0/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-02-22 13:34:45.113261 ninjax-1.0.0/ninjax/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      507 2022-11-24 15:49:52.000000 ninjax-1.0.0/ninjax/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    17684 2023-02-22 13:34:02.000000 ninjax-1.0.0/ninjax/ninjax.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-02-22 13:34:45.113261 ninjax-1.0.0/ninjax.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     9671 2023-02-22 13:34:45.000000 ninjax-1.0.0/ninjax.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      182 2023-02-22 13:34:45.000000 ninjax-1.0.0/ninjax.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2023-02-22 13:34:45.000000 ninjax-1.0.0/ninjax.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        7 2023-02-22 13:34:45.000000 ninjax-1.0.0/ninjax.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2023-02-22 13:34:45.113261 ninjax-1.0.0/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)      585 2022-11-24 15:49:52.000000 ninjax-1.0.0/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-19 19:50:55.316253 ninjax-1.1.0/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1071 2022-08-08 16:14:32.000000 ninjax-1.1.0/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     9671 2023-05-19 19:50:55.316253 ninjax-1.1.0/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     9261 2023-02-22 13:32:36.000000 ninjax-1.1.0/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-19 19:50:55.312253 ninjax-1.1.0/ninjax/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      507 2022-11-24 15:49:52.000000 ninjax-1.1.0/ninjax/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    17996 2023-05-19 19:50:00.000000 ninjax-1.1.0/ninjax/ninjax.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-05-19 19:50:55.312253 ninjax-1.1.0/ninjax.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     9671 2023-05-19 19:50:55.000000 ninjax-1.1.0/ninjax.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      182 2023-05-19 19:50:55.000000 ninjax-1.1.0/ninjax.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2023-05-19 19:50:55.000000 ninjax-1.1.0/ninjax.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        7 2023-05-19 19:50:55.000000 ninjax-1.1.0/ninjax.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2023-05-19 19:50:55.316253 ninjax-1.1.0/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      585 2022-11-24 15:49:52.000000 ninjax-1.1.0/setup.py
```

### Comparing `ninjax-1.0.0/LICENSE` & `ninjax-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjax-1.0.0/PKG-INFO` & `ninjax-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjax
-Version: 1.0.0
+Version: 1.1.0
 Summary: General Modules for JAX
 Home-page: http://github.com/danijar/ninjax
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
```

### Comparing `ninjax-1.0.0/README.md` & `ninjax-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ninjax-1.0.0/ninjax/ninjax.py` & `ninjax-1.1.0/ninjax/ninjax.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 import threading
 from functools import partial as bind
 
 import jax
 import jax.numpy as jnp
 
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 
 
 ###############################################################################
 # State
 ###############################################################################
 
 
@@ -37,35 +37,36 @@
     self.name = name
 
   def update(self, entries):
     for key, value in dict(entries).items():
       self[key] = value
 
   def __setitem__(self, key, value):
-    if not self.modify:
-      raise RuntimeError(
-          'Cannot modify state entries here. If you want to modify '
-          'state inside of scan() set modify=True. ' +
-          f'You were trying to set {key} to shape {value.shape} and ' +
-          f'dtype {value.dtype}.')
     if self.ignore and key in self:
       return  # Do not overwrite existing entries.
     if not self.create and key not in self:
       raise RuntimeError(
           'Can only create state entries during first call. ' +
           f'You were trying to set {key} to shape {value.shape} and ' +
           f'dtype {value.dtype}.')
+    if not self.modify:
+      raise RuntimeError(
+          'Cannot modify state entries here. If you want to modify '
+          'state inside of scan() set modify=True. ' +
+          f'You were trying to set {key} to shape {value.shape} and ' +
+          f'dtype {value.dtype}.')
     super().__setitem__(key, value)
 
 
 def pure(fun, nested=False):
   """Wrap an impure function that uses global state to explicitly pass the
   state in and out. The result is a pure function that is composable with JAX
   transformation. The pure function can be used as follows:
   `out, state = fun(state, rng, *args, **kwargs)`."""
+  @functools.wraps(fun)
   def purified(
       state, rng, *args, create=None, modify=None, ignore=None, **kwargs):
     context = CONTEXT.get(threading.get_ident(), None)
     if context:
       create = create if create is not None else context.create
       modify = modify if modify is not None else context.modify
       ignore = ignore if ignore is not None else context.ignore
@@ -165,90 +166,104 @@
     x2 = {k: v for k, v in context().items() if k not in strs}
     (y, (aux, state)), dx = backward(x1, x2, rng(), *args, **kwargs)
     context().update(state)
     return (y, x1, dx, aux) if has_aux else (y, x1, dx)
   return wrapper
 
 
-def jit(fun, static=None, **kwargs):
+def static_support(transform):
+  def new_transform(fun, *args, static=(), **kwargs):
+    assert isinstance(static, (list, tuple)), static
+    cache = {}
+    def new_function(*args2, **kwargs2):
+      sta = {k: v for k, v in kwargs2.items() if k in static}
+      dyn = {k: v for k, v in kwargs2.items() if k not in static}
+      key = hash(tuple(sta.get(n, '_default') for n in static))
+      if key not in cache:
+        specialized = bind(fun, **sta)
+        specialized.__name__ = fun.__name__
+        if hasattr(fun, 'pure'):
+          specialized.pure = fun.pure
+        cache[key] = transform(specialized, *args, **kwargs)
+      return cache[key](*args2, **dyn)
+    return new_function
+  return new_transform
+
+
+@static_support
+def jit(fun, **jitkw):
   """Compiles a pure function for fast execution. Only the first call of the
   function is allowed to create state entries."""
   if not getattr(fun, 'pure', False):
     raise ValueError('Use pure() before applying jit().')
-  static = static or ()
 
-  @bind(jax.jit, static_argnums=[0], **kwargs)
-  def init(statics, rng, *args, **kw):
-    # Return only state so JIT can remove dead code for fast initialization.
-    s = fun({}, rng, *args, ignore=True, **dict(statics), **kw)[1]
-    return s
-
-  @bind(jax.jit, static_argnums=[0], **kwargs)
-  def apply(statics, state, rng, *args, **kw):
-    return fun(state, rng, *args, create=False, **dict(statics), **kw)
+  def init(rng, *args, **kwargs):
+    @bind(jax.jit, **jitkw)
+    def jitted(rng, *args, **kwargs):
+      # Return only state so JIT can remove dead code for fast initialization.
+      return fun({}, rng, *args, ignore=True, **kwargs)[1]
+    state = jitted(rng, *args, **kwargs)
+    wrapper.keys = state.keys()
+    return state
+
+  def apply(state, rng, *args, **kwargs):
+    keys = wrapper.keys if hasattr(wrapper, 'keys') else state.keys()
+    selected = {k: v for k, v in state.items() if k in keys}
+    @bind(jax.jit, **jitkw)
+    def jitted(state, rng, *args, **kwargs):
+      return fun(state, rng, *args, create=False, **kwargs)
+    out, updated = jitted(selected, rng, *args, **kwargs)
+    return out, {**state, **updated}
 
   @functools.wraps(fun)
-  def wrapper(state, rng, *args, init_only=False, **kw):
-    if any([name not in kw for name in static]):
-      raise ValueError('Please pass all static arguments by keyword.')
-    state = state.copy()
-    statics = tuple(sorted([(k, v) for k, v in kw.items() if k in static]))
-    kw = {k: v for k, v in kw.items() if k not in static}
+  def wrapper(state, rng, *args, **kwargs):
     if not hasattr(wrapper, 'keys'):
-      created = init(statics, rng, *args, **kw)
-      wrapper.keys = set(created.keys())
-      for key, value in created.items():
-        if key not in state:
-          state[key] = value
-    if init_only:
-      return state
-    else:
-      selected = {k: v for k, v in state.items() if k in wrapper.keys}
-      out, updated = apply(statics, selected, rng, *args, **kw)
-      return out, {**state, **updated}
+      defaults = init(rng, *args, **kwargs)
+      state = {**defaults, **state}
+    return apply(state, rng, *args, **kwargs)
+
+  wrapper.init = init
+  wrapper.apply = apply
   return wrapper
 
 
-def pmap(fun, axis_name=None, static=None, **kwargs):
+@static_support
+def pmap(fun, axis_name=None, **pmapkw):
   """Compiles n pure function for fast execution across multiple devices. Only
   the first call of the function is allowed to create state entries."""
   if not getattr(fun, 'pure', False):
-    raise ValueError('Use pure() before applying jit().')
-  static = static or ()
+    raise ValueError('Use pure() before applying pmap().')
 
-  @bind(
-      jax.pmap, axis_name=axis_name, static_broadcasted_argnums=[0], **kwargs)
-  def init(statics, rng, *args, **kw):
-    # Return only state so JIT can remove dead code for fast initialization.
-    return fun({}, rng, *args, ignore=True, **dict(statics), **kw)[1]
-
-  @bind(
-      jax.pmap, axis_name=axis_name, static_broadcasted_argnums=[0], **kwargs)
-  def apply(statics, state, rng, *args, **kw):
-    return fun(state, rng, *args, create=False, **dict(statics), **kw)
+  def init(rng, *args, **kwargs):
+    @bind(jax.pmap, axis_name=axis_name, **pmapkw)
+    def pmapted(rng, *args, **kwargs):
+      # Return only state so pmap can remove dead code for fast initialization.
+      return fun({}, rng, *args, ignore=True, **kwargs)[1]
+    state = pmapted(rng, *args, **kwargs)
+    wrapper.keys = state.keys()
+    return state
+
+  def apply(state, rng, *args, **kwargs):
+    keys = wrapper.keys if hasattr(wrapper, 'keys') else state.keys()
+    selected = {k: v for k, v in state.items() if k in keys}
+    @bind(jax.pmap, axis_name=axis_name, **pmapkw)
+    def pmapted(state, rng, *args, **kwargs):
+      return fun(state, rng, *args, create=False, **kwargs)
+    out, updated = pmapted(selected, rng, *args, **kwargs)
+    return out, {**state, **updated}
 
   @functools.wraps(fun)
-  def wrapper(state, rng, *args, init_only=False, **kw):
-    if any([name not in kw for name in static]):
-      raise ValueError('Please pass all static arguments by keyword.')
-    state = state.copy()
-    statics = tuple(sorted([(k, v) for k, v in kw.items() if k in static]))
-    kw = {k: v for k, v in kw.items() if k not in static}
+  def wrapper(state, rng, *args, **kwargs):
     if not hasattr(wrapper, 'keys'):
-      created = init(statics, rng, *args, **kw)
-      wrapper.keys = set(created.keys())
-      for key, value in created.items():
-        if key not in state:
-          state[key] = value
-    if init_only:
-      return state
-    else:
-      selected = {k: v for k, v in state.items() if k in wrapper.keys}
-      out, updated = apply(statics, selected, rng, *args, **kw)
-      return out, {**state, **updated}
+      defaults = init(rng, *args, **kwargs)
+      state = {**defaults, **state}
+    return apply(state, rng, *args, **kwargs)
+
+  wrapper.init = init
+  wrapper.apply = apply
   return wrapper
 
 
 @jax.named_scope('cond')
 def cond(pred, true_fun, false_fun, *operands):
   true_fun = pure(true_fun, nested=True)
   false_fun = pure(false_fun, nested=True)
@@ -289,15 +304,14 @@
 
 
 @jax.named_scope('_prerun')
 def _prerun(fun, *args, **kwargs):
   if not context().create:
     return
   discarded, state = fun(dict(context()), rng(), *args, ignore=True, **kwargs)
-  del discarded
   context().update(state)
 
 
 ###############################################################################
 # Modules
 ###############################################################################
 
@@ -394,14 +408,15 @@
   @property
   def name(self):
     """The name of this module instance as a string."""
     return self._path.split('/')[-1]
 
   def get(self, name, *args, **kwargs):
     """Retrieve or create a state entry that belongs to this module."""
+    assert '{' not in name, 'Did you forget to format a string?'
     path = self.path + '/' + name
     if name in self._submodules:
       return self._submodules[name]
     if path in context():
       return context()[path]
     ctor, *args = args
     if 'name' in inspect.signature(ctor).parameters:
```

### Comparing `ninjax-1.0.0/ninjax.egg-info/PKG-INFO` & `ninjax-1.1.0/ninjax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjax
-Version: 1.0.0
+Version: 1.1.0
 Summary: General Modules for JAX
 Home-page: http://github.com/danijar/ninjax
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
```

### Comparing `ninjax-1.0.0/setup.py` & `ninjax-1.1.0/setup.py`

 * *Files identical despite different names*

