# Comparing `tmp/arroba-0.1.tar.gz` & `tmp/arroba-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arroba-0.1.tar", last modified: Mon May  1 01:31:59 2023, max compression
+gzip compressed data, was "arroba-0.2.tar", last modified: Thu May 18 22:15:39 2023, max compression
```

## Comparing `arroba-0.1.tar` & `arroba-0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-05-01 01:31:59.691130 arroba-0.1/
--rw-r--r--   0 ryan       (501) staff       (20)     4309 2023-05-01 01:31:59.691007 arroba-0.1/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     3605 2023-05-01 01:30:47.000000 arroba-0.1/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-05-01 01:31:59.690272 arroba-0.1/arroba/
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-05-01 00:25:12.000000 arroba-0.1/arroba/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     8299 2023-05-01 00:32:18.000000 arroba-0.1/arroba/diff.py
--rw-r--r--   0 ryan       (501) staff       (20)    32113 2023-05-01 00:32:18.000000 arroba-0.1/arroba/mst.py
--rw-r--r--   0 ryan       (501) staff       (20)     5593 2023-05-01 00:40:24.000000 arroba-0.1/arroba/util.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-05-01 01:31:59.690843 arroba-0.1/arroba.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     4309 2023-05-01 01:31:59.000000 arroba-0.1/arroba.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      236 2023-05-01 01:31:59.000000 arroba-0.1/arroba.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-05-01 01:31:59.000000 arroba-0.1/arroba.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       56 2023-05-01 01:31:59.000000 arroba-0.1/arroba.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        7 2023-05-01 01:31:59.000000 arroba-0.1/arroba.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)     1020 2023-05-01 00:33:55.000000 arroba-0.1/pyproject.toml
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-05-01 01:31:59.691175 arroba-0.1/setup.cfg
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-05-18 22:15:39.942837 arroba-0.2/
+-rw-r--r--   0 ryan       (501) staff       (20)     4581 2023-05-18 22:15:39.942715 arroba-0.2/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     3822 2023-05-18 22:09:06.000000 arroba-0.2/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-05-18 22:15:39.941949 arroba-0.2/arroba/
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-05-01 00:25:12.000000 arroba-0.2/arroba/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     8236 2023-05-18 02:58:36.000000 arroba-0.2/arroba/diff.py
+-rw-r--r--   0 ryan       (501) staff       (20)    34206 2023-05-18 21:57:54.000000 arroba-0.2/arroba/mst.py
+-rw-r--r--   0 ryan       (501) staff       (20)     9171 2023-05-18 21:57:33.000000 arroba-0.2/arroba/repo.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4157 2023-05-17 23:33:24.000000 arroba-0.2/arroba/storage.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6206 2023-05-17 23:45:14.000000 arroba-0.2/arroba/util.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-05-18 22:15:39.942537 arroba-0.2/arroba.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     4581 2023-05-18 22:15:39.000000 arroba-0.2/arroba.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      269 2023-05-18 22:15:39.000000 arroba-0.2/arroba.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-05-18 22:15:39.000000 arroba-0.2/arroba.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       56 2023-05-18 22:15:39.000000 arroba-0.2/arroba.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        7 2023-05-18 22:15:39.000000 arroba-0.2/arroba.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)     1067 2023-05-18 22:06:44.000000 arroba-0.2/pyproject.toml
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-05-18 22:15:39.942882 arroba-0.2/setup.cfg
```

### Comparing `arroba-0.1/PKG-INFO` & `arroba-0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: arroba
-Version: 0.1
-Summary: Python implementation of Bluesky's low level AT Protocol, including repo, MST, and sync methods
+Version: 0.2
+Summary: Python implementation of Bluesky PDS and AT Protocol, including repo, MST, and sync methods
 Author-email: Ryan Barrett <arroba@ryanb.org>
 Project-URL: Homepage, https://github.com/snarfed/arroba
+Project-URL: Documentation, https://arroba.readthedocs.io/
 Keywords: arroba,AT Protocol,ATP,Bluesky
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 arroba [![Circle CI](https://circleci.com/gh/snarfed/arroba.svg?style=svg)](https://circleci.com/gh/snarfed/arroba) [![Coverage Status](https://coveralls.io/repos/github/snarfed/arroba/badge.svg?branch=main)](https://coveralls.io/github/snarfed/arroba?branch=master)
 ===
 
-Python implementation of [Bluesky](https://blueskyweb.xyz/)'s low level [AT Protocol](https://atproto.com/), including [data repository](https://atproto.com/guides/data-repos), [Merkle search tree](https://atproto.com/guides/data-repos), and [com.atproto.sync XRPC methods](https://atproto.com/lexicons/com-atproto-sync).
+Python implementation of [Bluesky](https://blueskyweb.xyz/) [PDS](https://atproto.com/guides/data-repos) and [AT Protocol](https://atproto.com/specs/atp), including data repository, Merkle search tree, and [com.atproto.sync XRPC methods](https://atproto.com/lexicons/com-atproto-sync).
 
 _Arroba_ is the Spanish word for the [@ character](https://en.wikipedia.org/wiki/At_sign) ("at sign").
 
 Install from [PyPI](https://pypi.org/project/arroba/) with `pip install arroba`.
 
 License: This project is placed into the public domain.
 
@@ -34,14 +35,18 @@
 ## Usage
 
 TODO
 
 
 ## Changelog
 
+### 0.2 - 2023-05-18
+
+Implement repo and commit chain in new Repo class, including pluggable storage. This completes the first pass at all PDS data structures. Next release will include initial implementations of the `com.atproto.sync.*` XRPC methods.
+
 ### 0.1 - 2023-04-30
 
 Initial release! Still very in progress. MST, Walker, and Diff classes are mostly complete and working. Repo, commits, and sync XRPC methods are still in progress.
 
 
 Release instructions
 ---
```

### Comparing `arroba-0.1/README.md` & `arroba-0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 arroba [![Circle CI](https://circleci.com/gh/snarfed/arroba.svg?style=svg)](https://circleci.com/gh/snarfed/arroba) [![Coverage Status](https://coveralls.io/repos/github/snarfed/arroba/badge.svg?branch=main)](https://coveralls.io/github/snarfed/arroba?branch=master)
 ===
 
-Python implementation of [Bluesky](https://blueskyweb.xyz/)'s low level [AT Protocol](https://atproto.com/), including [data repository](https://atproto.com/guides/data-repos), [Merkle search tree](https://atproto.com/guides/data-repos), and [com.atproto.sync XRPC methods](https://atproto.com/lexicons/com-atproto-sync).
+Python implementation of [Bluesky](https://blueskyweb.xyz/) [PDS](https://atproto.com/guides/data-repos) and [AT Protocol](https://atproto.com/specs/atp), including data repository, Merkle search tree, and [com.atproto.sync XRPC methods](https://atproto.com/lexicons/com-atproto-sync).
 
 _Arroba_ is the Spanish word for the [@ character](https://en.wikipedia.org/wiki/At_sign) ("at sign").
 
 Install from [PyPI](https://pypi.org/project/arroba/) with `pip install arroba`.
 
 License: This project is placed into the public domain.
 
@@ -17,14 +17,18 @@
 ## Usage
 
 TODO
 
 
 ## Changelog
 
+### 0.2 - 2023-05-18
+
+Implement repo and commit chain in new Repo class, including pluggable storage. This completes the first pass at all PDS data structures. Next release will include initial implementations of the `com.atproto.sync.*` XRPC methods.
+
 ### 0.1 - 2023-04-30
 
 Initial release! Still very in progress. MST, Walker, and Diff classes are mostly complete and working. Repo, commits, and sync XRPC methods are still in progress.
 
 
 Release instructions
 ---
```

### Comparing `arroba-0.1/arroba/diff.py` & `arroba-0.2/arroba/diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 Huge thanks to the Bluesky team for working in the public, in open source, and to
 Daniel Holmgren and Devin Ivy for this code specifically!
 """
 from collections import namedtuple
 import logging
 
-from arroba.mst import Leaf, MST, Walker
+from .mst import Leaf, MST, Walker
 
 logger = logging.getLogger(__name__)
 
 
 def mst_diff(cur, prev=None):
     """Generates a diff between two MSTs.
 
@@ -30,15 +30,14 @@
 
     prev.get_pointer()
     diff = Diff()
 
     left_walker = Walker(prev)
     right_walker = Walker(cur)
     while not left_walker.status.done or not right_walker.status.done:
-        # print(left_walker.status, right_walker.status)
         # if one walker is finished, continue walking the other & logging all nodes
         if left_walker.status.done and not right_walker.status.done:
             node = right_walker.status.cur
             if isinstance(node, Leaf):
                 diff.record_add(node.key, node.value)
             else:
                 diff.record_new_cid(node.pointer)
```

### Comparing `arroba-0.1/arroba/mst.py` & `arroba-0.2/arroba/mst.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 """Bluesky / AT Protocol Merkle search tree implementation.
 
 * https://atproto.com/guides/data-repos
 * https://atproto.com/lexicons/com-atproto-sync
 * https://hal.inria.fr/hal-02303490/document
 
 Heavily based on:
-https://github.com/bluesky/atproto/blob/main/packages/repo/src/mst/mst.ts
+https://github.com/bluesky-social/atproto/blob/main/packages/repo/src/mst/mst.ts
 
 Huge thanks to the Bluesky team for working in the public, in open source, and to
 Daniel Holmgren and Devin Ivy for this code specifically!
 
-Notable differences:
-* All in memory, no block storage (yet)
-
 From that file:
 
 This is an implementation of a Merkle Search Tree (MST)
 The data structure is described here: https://hal.inria.fr/hal-02303490/document
 The MST is an ordered, insert-order-independent, deterministic tree.
 Keys are laid out in alphabetic order.
 The key insight of an MST is that each key is hashed and starting 0s are counted
@@ -46,20 +43,24 @@
 `bsky/posts/abcdehi` Then the first will be described as `prefix: 0, key:
 'bsky/posts/abcdefg'`, and the second will be described as `prefix: 16, key:
 'hi'.`
 """
 from collections import namedtuple
 import copy
 from hashlib import sha256
+import logging
 from os.path import commonprefix
 import re
 
 from multiformats import CID
 
-from arroba.util import dag_cbor_cid
+from .storage import BlockMap, Storage
+from .util import dag_cbor_cid
+
+logger = logging.getLogger(__name__)
 
 # this is treeEntry in mst.ts
 Entry = namedtuple('Entry', [
     'p',  # int, length of prefix that this key shares with the prev key
     'k',  # bytes, the rest of the key outside the shared prefix
     'v',  # str CID, value
     't',  # str CID, next subtree (to the right of leaf), or None
@@ -76,70 +77,96 @@
 ])
 
 
 class MST:
     """Merkle search tree class.
 
     Attributes:
+      storage: :class:`Storage`
       entries: sequence of :class:`MST` and :class:`Leaf`
       layer: int, this MST's layer in the root MST
       pointer: :class:`CID`
       outdated_pointer: boolean, whether pointer needs to be recalculated
     """
+    storage = None
     entries = None
     layer = None
     pointer = None
     outdated_pointer = False
 
-    def __init__(self, entries=None, pointer=None, layer=None):
+    def __init__(self, *, storage=None, entries=None, pointer=None, layer=None):
         """Constructor.
+
         Args:
-            entries: sequence of :class:`MST` and :class:`Leaf`
-            pointer: :class:`CID`
-            layer: int
+          storage: :class:`Storage`
+          entries: sequence of :class:`MST` and :class:`Leaf`
+          pointer: :class:`CID`
+          layer: int
 
         Returns:
-            :class:`MST`
+          :class:`MST`
         """
-        self.entries = entries or []
-        self.pointer = pointer or cid_for_entries(self.entries)
+        self.storage = storage
+        self.entries = entries
+        self.pointer = pointer
         self.layer = layer
 
-#     def from_data(data: NodeData, opts?: Partial<MstOpts>):
+    @classmethod
+    def load(cls, *, storage=None, cid=None):
+        return MST(storage=storage, entries=None, pointer=cid, layer=None)
+
+    @classmethod
+    def create(cls, *, storage=None, entries=None, layer=None):
+        """
+
+        Args:
+          storage: :class:`Storage`
+          entries: sequence of :class:`MST` and :class:`Leaf`
+          layer: int
+
+        Returns:
+          :class:`MST`
+        """
+        if not entries:
+            entries = []
+        pointer = cid_for_entries(entries)
+        return MST(storage=storage, entries=entries, pointer=pointer, layer=layer)
+
+#     def from_data(storage, data, opts):
 #         """
 #         Returns:
 #           :class:`MST`
 #         """
-#         { layer = None } = opts or {}
-#         entries = deserialize_node_data(data, opts)
+#         entries = deserialize_node_data(data)
 #         pointer = cid_for_cbor(data)
 #         return MST(entries=entries, pointer=pointer)
 
     def __eq__(self, other):
         if isinstance(other, MST):
             return self.get_pointer() == other.get_pointer()
 
     def __unicode__(self):
         return f'MST with pointer {self.get_pointer()}'
 
     def __repr__(self):
-        return f'MST(entries=..., pointer={self.get_pointer()}, layer={self.get_layer()})'
+        return f'MST(storage={self.storage}, entries=..., pointer={self.get_pointer()}, layer={self.get_layer()})'
 
     # Immutability
     # -------------------
     def new_tree(self, entries):
         """We never mutate an MST, we just return a new MST with updated values.
 
         Args:
             entries: sequence of :class:`MST` and :class:`Leaf`
 
         Returns:
             :class:`MST`
         """
-        mst = MST(entries=entries, pointer=self.pointer, layer=self.layer)
+        mst = MST(storage=self.storage, entries=entries, pointer=self.pointer,
+                  layer=self.layer)
         mst.outdated_pointer = True
         return mst
 
 
 #     Getters (lazy load)
 #     -------------------
 
@@ -147,22 +174,24 @@
         """
 
         We don't want to load entries of every subtree, just the ones we need.
 
         Returns:
           sequence of :class:`MST` and :class:`Leaf`
         """
-        if self.entries:
+        if self.entries is not None:
             return copy.copy(self.entries)
 
         if self.pointer:
-            data = self.storage.read_obj(self.pointer, node_data_def)
-            first_leaf = data.e[0]
-            layer = leading_zeros_on_hash(first_leaf.k) if first_leaf else None
-            self.entries = deserialize_node_data(self.storage, data, {layer})
+            data = Data(**self.storage.read(self.pointer))
+            first_leaf = layer = None
+            if data.e:
+                layer = leading_zeros_on_hash(data.e[0]['k'])
+            self.entries = deserialize_node_data(storage=self.storage, data=data,
+                                                 layer=layer)
             return self.entries
 
         raise RuntimeError('No entries or CID provided')
 
     def get_pointer(self):
         """Returns this MST's root CID pointer. Calculates it if necessary.
 
@@ -172,19 +201,25 @@
 
         Returns:
           :class:`CID`
         """
         if not self.outdated_pointer:
             return self.pointer
 
-        for e in self.entries:
+        outdated = False
+        entries = self.get_entries()
+        for e in entries:
             if isinstance(e, MST) and e.outdated_pointer:
+                outdated = True
                 e.get_pointer()
 
-        self.pointer = cid_for_entries(self.entries)
+        if outdated:
+            entries = self.get_entries()
+
+        self.pointer = cid_for_entries(entries)
         self.outdated_pointer = False
         return self.pointer
 
     def get_layer(self):
         """Returns this MST's layer, and sets self.layer.
 
         In most cases, we get the layer of a node from a hint on creation. In the
@@ -207,17 +242,18 @@
 
         Returns:
           int or None
         """
         if self.layer is not None:
             return self.layer
 
-        layer = layer_for_entries(self.entries)
+        entries = self.get_entries()
+        layer = layer_for_entries(entries)
         if layer is None:
-            for entry in self.entries:
+            for entry in entries:
                 if isinstance(entry, MST):
                     child_layer = entry.attempt_get_layer()
                     if child_layer is not None:
                         layer = child_layer + 1
                         break
 
         if layer is not None:
@@ -225,14 +261,37 @@
 
         return layer
 
 
     # Core functionality
     # -------------------
 
+    def get_unstored_blocks(self):
+        """Return the necessary blocks to persist the MST to repo storage.
+
+        Returns:
+          (:class:`CID` root, :class:`BlockMap`) tuple
+        """
+        unstored = BlockMap()
+        pointer = self.get_pointer()
+
+        if self.storage.has(pointer):
+            return pointer, unstored
+
+        entries = self.get_entries()
+        data = serialize_node_data(entries)
+        unstored.add(data._asdict())
+
+        for entry in entries:
+            if isinstance(entry, MST):
+                _, blocks = entry.get_unstored_blocks()
+                unstored.update(blocks)
+
+        return pointer, unstored
+
     def add(self, key, value=None, known_zeros=None):
         """Adds a new leaf for the given key/value pair.
 
         Args:
           key: str
           value: :class:`CID`
           known_zeros: int
@@ -293,15 +352,15 @@
             updated = []
             if left:
                 updated.append(left)
             updated.append(Leaf(key=key, value=value))
             if right:
                 updated.append(right)
 
-            new_root = MST(entries=updated, layer=key_zeros)
+            new_root = MST.create(storage=self.storage, entries=updated, layer=key_zeros)
             new_root.outdated_pointer = True
             return new_root
 
     def get(self, key):
         """Gets the value at the given key.
 
         Args:
@@ -316,15 +375,15 @@
             return found.value
 
         prev = self.at_index(index - 1)
         if prev and isinstance(prev, MST):
             return prev.get(key)
 
     def update(self, key, value):
-        """Edits the value at the given key
+        """Edits the value at the given key.
 
         Args:
           key: str
           value: :class:`CID`
 
         Returns:
           :class:`MST`
@@ -384,18 +443,18 @@
             else:
                 return self.remove_entry(index)
 
         # else recurse down to find it
         prev = self.at_index(index - 1)
         if isinstance(prev, MST):
             subtree = prev.delete_recurse(key)
-            if subtree.entries == 0:
-                return self.remove_entry(index - 1)
-            else:
+            if subtree.get_entries():
                 return self.update_entry(index - 1, subtree)
+            else:
+                return self.remove_entry(index - 1)
 
         raise KeyError(f'Could not find a record with key: {key}')
 
 
 #     Simple Operations
 #     -------------------
 
@@ -428,50 +487,51 @@
 
         Args:
           entry: :class:`MST` or :class:`Leaf`
 
         Returns:
           :class:`MST`
         """
-        return self.new_tree(self.entries + [entry])
+        return self.new_tree(self.get_entries() + [entry])
 
     def prepend(self, entry):
         """Prepends an entry to the start of the node.
 
         Args:
           entry: :class:`MST` or :class:`Leaf`
 
         Returns:
           :class:`MST`
         """
-        return self.new_tree([entry] + self.entries)
+        return self.new_tree([entry] + self.get_entries())
 
     def at_index(self, index):
         """Returns the entry at a given index.
 
         Args:
           index: int
 
         Returns:
           :class:`MST` or :class:`Leaf` or None
         """
-        if 0 <= index < len(self.entries):
-            return self.entries[index]
+        entries = self.get_entries()
+        if 0 <= index < len(entries):
+            return entries[index]
 
     def slice(self, start=None, end=None):
         """Returns a slice of this node.
 
         Args:
           start: int, optional, inclusive
           end: int, optional, exclusive
 
         Returns:
           sequence of :class:`MST` and :class:`Leaf`
         """
-        return self.entries[start:end]
+        return self.get_entries()[start:end]
 
     def splice_in(self, entry, index):
         """Inserts an entry at a given index.
 
         Args:
           entry: :class:`MST` or :class:`Leaf`
           index: int
@@ -507,16 +567,17 @@
 
         Only if the topmost node in the tree only points to another tree.
         Otherwise, does nothing.
 
         Returns:
           :class:`MST`
         """
-        if len(self.entries) == 1 and isinstance(self.entries[0], MST):
-            return self.entries[0].trim_top()
+        entries = self.get_entries()
+        if len(entries) == 1 and isinstance(entries[0], MST):
+            return entries[0].trim_top()
         else:
             return self
 
 
 #     Subtree & Splits
 #     -------------------
 
@@ -544,16 +605,16 @@
             split = last_in_left.split_around(key)
             if split[0]:
                 left = left.append(split[0])
             if split[1]:
                 right = right.prepend(split[1])
 
         return [
-            left if left.entries else None,
-            right if right.entries else None,
+            left if left.get_entries() else None,
+            right if right.get_entries() else None,
         ]
 
     def append_merge(self, to_merge):
         """Merges another tree with this one.
 
         The simple merge case where every key in the right tree is greater than
         every key in the left tree. Used primarily for deletes.
@@ -563,41 +624,45 @@
 
         Returns:
           :class:`MST`
         """
         assert self.get_layer() == to_merge.get_layer(), \
             'Trying to merge two nodes from different layers of the MST'
 
-        last_in_left = self.entries[-1]
-        first_in_right = to_merge.entries[0]
+        self_entries = self.get_entries()
+        to_merge_entries = to_merge.get_entries()
+        last_in_left = self_entries[-1]
+        first_in_right = to_merge_entries[0]
 
         if isinstance(last_in_left, MST) and isinstance(first_in_right, MST):
             merged = last_in_left.append_merge(first_in_right)
             return self.new_tree(
-                list(self.entries[:-1]) + [merged] + to_merge.entries[1:])
+                list(self_entries[:-1]) + [merged] + to_merge_entries[1:])
         else:
-            return self.new_tree(self.entries + to_merge.entries)
+            return self.new_tree(self_entries + to_merge_entries)
 
 
     # Create relatives
     # -------------------
 
     def create_child(self):
         """
         Returns:
           :class:`MST`
         """
-        return MST(entries=[], layer=self.get_layer() - 1)
+        return MST.create(storage=self.storage, entries=[],
+                          layer=self.get_layer() - 1)
 
     def create_parent(self):
         """
         Returns:
           :class:`MST`
         """
-        parent = MST(entries=[self], layer=self.get_layer() + 1)
+        parent = MST.create(storage=self.storage, entries=[self],
+                            layer=self.get_layer() + 1)
         parent.outdated_pointer = True
         return parent
 
 
 #     Finding insertion points
 #     -------------------
 
@@ -606,108 +671,124 @@
 
         Args:
           key: str
 
         Returns:
           int
         """
-        for i, entry in enumerate(self.entries):
+        entries = self.get_entries()
+        for i, entry in enumerate(entries):
             if isinstance(entry, Leaf) and entry.key >= key:
                 return i
 
         # if we can't find it, we're on the end
-        return len(self.entries)
+        return len(entries)
 
 
 #     List operations (partial tree traversal)
 #     -------------------
 
-#     @TODO write tests for these
+    def walk_leaves_from(self, key):
+        """Walk tree starting at key.
 
-#     Walk tree starting at key
-#     def walk_leaves_from(key: string): AsyncIterable<Leaf>:
-#         index = self.find_gt_or_equal_leaf_index(key)
-#         prev = self.entries[index - 1]
-#         if prev and isinstance(prev, MST):
-#             for e in prev.walk_leaves_from(key):
-#                 yield e
-#         for entry in self.entries[index:]:
-#             if isinstance(entry, Leaf):
-#                 yield entry
-#             else:
-#                 for e in entry.walk_leaves_from(key):
-#                     yield e
+        Generator for leaves in the tree, starting at a given rkey.
 
-#     def list(
-#         count = Number.MAX_SAFE_INTEGER,
-#         after?: string,
-#         before?: string,
-#     ):
-#     """
-#     Returns:
-#       Leaf[]
-#     """
-#         vals: Leaf[] = []
-#         for leaf in self.walk_leaves_from(after or ''):
-#             if leaf.key == after:
-#                 continue
-#             if len(vals) >= count:
-#                 break
-#             if before and leaf.key >= before:
-#                 break
-#             vals.append(leaf)
-#         return vals
-
-#     def list_with_prefix(
-#         prefix: string,
-#         count = Number.MAX_SAFE_INTEGER,
-#     ):
-#     """
-#     Returns:
-#       Leaf[]
-#     """
-#         vals: Leaf[] = []
-#         for leaf in self.walk_leaves_from(prefix):
-#             if len(vals) >= count or not leaf.key.startswith(prefix):
-#                 break
-#             vals.append(leaf)
-#         return vals
+        Args:
+          key: str
+
+        Generates:
+          :class:`Leaf`
+        """
+        index = self.find_gt_or_equal_leaf_index(key)
+        entries = self.get_entries()
+
+        if index > 0:
+            prev = entries[index - 1]
+            if prev and isinstance(prev, MST):
+                for e in prev.walk_leaves_from(key):
+                    yield e
+
+        for entry in entries[index:]:
+            if isinstance(entry, Leaf):
+                yield entry
+            else:
+                for e in entry.walk_leaves_from(key):
+                    yield e
+
+    def list(self, after=None, before=None):
+        """Returns entries, optionally bounded within an rkey range.
+
+        Args:
+          after: str rkey, optional
+          before: str rkey, optional
+
+        Returns:
+          sequence of :class:`Leaf`
+        """
+        vals = []
+
+        for leaf in self.walk_leaves_from(after or ''):
+            if leaf.key == after:
+                continue
+            if before and leaf.key >= before:
+                break
+            vals.append(leaf)
+
+        return vals
+
+    def list_with_prefix(self, prefix):
+        """Returns entries with a given rkey prefix.
+
+        Args:
+          prefix: str, rkey prefix
+
+        Returns:
+          sequence of :class:`Leaf`
+        """
+        vals = []
+
+        for leaf in self.walk_leaves_from(prefix):
+            if not leaf.key.startswith(prefix):
+                break
+            vals.append(leaf)
 
+        return vals
 
 #     Full tree traversal
 #     -------------------
 
     def walk(self):
         """Walk full tree, depth first, and emit nodes.
 
         Returns:
           generator of :class:`MST` and :class:`Leaf`
         """
         yield self
 
-        for entry in self.entries:
+        for entry in self.get_entries():
             if isinstance(entry, MST):
                 for e in entry.walk():
                     yield e
             else:
                 yield entry
 
 #     Walk full tree & emit nodes, consumer can bail at any point by returning False
 #     def paths():
 #     """
 #     Returns:
 #       sequence of :class:`MST` and :class:`Leaf`
 #     """
-#         paths: NodeEntry[][] = []
-#         for entry in self.entries:
+#         paths = []
+#         for entry in self.get_entries():
 #             if isinstance(entry, Leaf):
 #                 paths.append([entry])
 #             if isinstance(entry, MST):
 #                 sub_paths = entry.paths()
-#                 paths = paths + sub_paths.map((p) => ([entry] + p))
+#                 paths.extend([entry] + p for p in sub_paths)
+#
 #         return paths
 
     def all_nodes(self):
         """Walks the tree and returns all nodes.
 
         Returns:
           sequence of :class:`MST` and :class:`Leaf`
@@ -717,15 +798,15 @@
 #     Walks tree & returns all cids
 #     def all_cids():
 #     """
 #     Returns:
 #       CidSet
 #     """
 #         cids = CidSet()
-#         for entry in self.entries:
+#         for entry in self.get_entries():
 #             if isinstance(entry, Leaf):
 #                 cids.add(entry.value)
 #             else:
 #                 subtree_cids = entry.all_cids()
 #                 cids.add_set(subtree_cids)
 #         cids.add(self.get_pointer())
 #         return cids
@@ -751,15 +832,15 @@
 #     -------------------
 
     # Walk reachable branches of tree & emit nodes, consumer can bail at any
     # point by returning False
 
 #     def walk_reachable(): AsyncIterable<NodeEntry>:
 #         yield self
-#         for entry in self.entries:
+#         for entry in self.get_entries():
 #             if isinstance(entry, MST):
 #                 try:
 #                     for e in entry.walk_reachable():
 #                         yield e
 #                 catch (err):
 #                     if err instanceof MissingBlockError:
 #                         continue
@@ -785,15 +866,15 @@
 #     """
 #     Returns:
 #       void
 #     """
 #         leaves = CidSet()
 #         to_fetch = CidSet()
 #         to_fetch.add(self.get_pointer())
-#         for entry in self.entries:
+#         for entry in self.get_entries():
 #             if isinstance(entry, Leaf):
 #                 leaves.add(entry.value)
 #             else:
 #                 to_fetch.add(entry.get_pointer())
 #         while (to_fetch.size() > 0):
 #             next_layer = CidSet()
 #             fetched = self.storage.get_blocks(to_fetch.to_list())
@@ -867,54 +948,52 @@
             break
 
     return leading_zeros
 
 
 def layer_for_entries(entries):
     """
-    sequence of :class:`MST` and :class:`Leaf`
+    Args:
+      entries: sequence of :class:`MST` and :class:`Leaf`
+
     Returns:
       number | None
     """
     for entry in entries:
         if isinstance(entry, Leaf):
             return leading_zeros_on_hash(first_leaf.key)
 
 
-# def deserialize_node_data = (
-#     storage: ReadableBlockstore,
-#     data: NodeData,
-#     opts?: Partial<MstOpts>,
-# ):
-#     """
-#     Returns:
-#       sequence of :class:`MST` and :class:`Leaf`
-#     """
-#     { layer } = opts or {}
-#     entries = []
-#     if (data.l is not None):
-#         entries.append(
-#             MST.load(storage, data.l,:
-#                 layer: layer ? layer - 1 : undefined,
-#             )
-
-#     last_key = ''
-#     for entry in data.e:
-#         key_str = uint8arrays.to_string(entry.k, 'ascii')
-#         key = last_key.slice(0, entry.p) + key_str
-#         ensure_valid_key(key)
-#         entries.append(Leaf(key, entry.v))
-#         last_key = key
-#         if entry.t is not None:
-#             entries.append(
-#                 MST.load(storage, entry.t,:
-#                     layer: layer ? layer - 1 : undefined,
-#                 )
+def deserialize_node_data(*, storage=None, data=None, layer=None):
+    """
+    Args:
+      storage: :class:`Storage`
+      data: :class:`Data`
+
+    Returns:
+      sequence of :class:`MST` and :class:`Leaf`
+    """
+    entries = []
+    if (data.l is not None):
+        entries.append(MST(storage=storage, pointer=data.l,
+                           layer=layer - 1 if layer else None))
+
+    last_key = ''
+    for entry_data in data.e:
+        entry = Entry(**entry_data)
+        key_str = entry.k.decode()
+        key = last_key[:entry.p] + key_str
+        ensure_valid_key(key)
+        entries.append(Leaf(key, entry.v))
+        last_key = key
+        if entry.t is not None:
+            entries.append(MST(storage=storage, pointer=entry.t,
+                               layer=layer - 1 if layer else None))
 
-#     return entries
+    return entries
 
 
 def serialize_node_data(entries):
     """
     Args:
       entries: sequence of :class:`MST` and :class:`Leaf`
```

### Comparing `arroba-0.1/arroba/util.py` & `arroba-0.2/arroba/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Misc AT Protocol utils. TIDs, CIDs, etc."""
 import copy
 from datetime import datetime, timezone
 import logging
 from numbers import Integral
 import random
+import time
 
 from Crypto.Hash import SHA256
 from Crypto.PublicKey import ECC
 from Crypto.Signature import DSS
 import dag_cbor.encoding
 from multiformats import CID, multicodec, multihash
 
@@ -17,19 +18,29 @@
 # pycryptodome's internal RNG. This constant is overridden in tests to use
 # random.randbytes with a fixed seed.
 _randfunc = None
 
 # the bottom 32 clock ids can be randomized & are not guaranteed to be collision
 # resistant. we use the same clockid for all TIDs coming from this runtime.
 _clockid = random.randint(0, 31)
-# _tid_last = time.time_ns() // 1000  # microseconds
+_tid_last = 0  # microseconds
 
 S32_CHARS = '234567abcdefghijklmnopqrstuvwxyz'
 
 
+def now(tz=timezone.utc, **kwargs):
+    """Wrapper for datetime.now that allows us to mock it out in tests."""
+    return datetime.now(tz=tz, **kwargs)
+
+
+def time_ns():
+    """Wrapper for time.time_ns that allows us to mock it out in tests."""
+    return time.time_ns()
+
+
 def dag_cbor_cid(obj):
     """Returns the DAG-CBOR CID for a given object.
 
     Args:
       obj: CBOR-compatible native object or value
 
     Returns:
@@ -114,26 +125,32 @@
     if not isinstance(tid, (str, bytes)) or len(tid) != 13:
         raise ValueError(f'Expected 13-character str or bytes; got {tid}')
 
     encoded = tid.replace('-', '')[:-2]  # strip clock id
     return datetime.fromtimestamp(s32decode(encoded) / 1000 / 1000, timezone.utc)
 
 
-# TODO
-# def next_tid():
-#     global _tid_last
-
-#     # enforce that we're at least 1us after the last TID to prevent TIDs moving
-#     # backwards if system clock drifts backwards
-#     now = time.time_ns() // 1000
-#     if now > _tid_last:
-#         _tid_last = now
-#     else:
-#         _tid_last += 1
-#         now = _tid_last
+def next_tid():
+    """Returns the TID corresponding to the current time.
+
+    A TID is UNIX timestamp (ie time since the epoch) in microseconds.
+    Returned tids are guaranteed to monotonically increase across calls.
+
+    https://atproto.com/specs/atp#timestamp-ids-tid
+    https://github.com/bluesky-social/atproto/blob/main/packages/common-web/src/tid.ts
+
+    Returns:
+      str, TID
+    """
+    global _tid_last
+
+    # enforce that we're at least 1us after the last TID to prevent TIDs moving
+    # backwards if system clock drifts backwards
+    _tid_last = max(time_ns() // 1000, _tid_last + 1)
+    return str(_tid_last)
 
 
 def new_p256_key():
     """Generates a new ECC P-256 keypair.
 
     Returns:
       :class:`Crypto.PublicKey.ECC.EccKey`
@@ -159,19 +176,23 @@
     keypairs. Context:
     * Go supports P-256, ED25519, SECP256K1 keys
     * TS supports P-256, SECP256K1 keys
     * this recommends ED25519, then P-256:
       https://soatok.blog/2022/05/19/guidance-for-choosing-an-elliptic-curve-signature-algorithm-in-2022/
 
     Args:
-      commit: dict repo commit
+      commit: dict, repo commit
       key: :class:`Crypto.PublicKey.ECC.EccKey`
+
+    Returns:
+      dict, repo commit
     """
     signer = DSS.new(key, 'fips-186-3', randfunc=_randfunc)
     commit['sig'] = signer.sign(SHA256.new(dag_cbor.encoding.encode(commit)))
+    return commit
 
 
 def verify_commit_sig(commit, key):
     """Returns true if the commit's signature is valid, False otherwise.
 
     See :func:`sign_commit` for more background.
```

### Comparing `arroba-0.1/arroba.egg-info/PKG-INFO` & `arroba-0.2/arroba.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: arroba
-Version: 0.1
-Summary: Python implementation of Bluesky's low level AT Protocol, including repo, MST, and sync methods
+Version: 0.2
+Summary: Python implementation of Bluesky PDS and AT Protocol, including repo, MST, and sync methods
 Author-email: Ryan Barrett <arroba@ryanb.org>
 Project-URL: Homepage, https://github.com/snarfed/arroba
+Project-URL: Documentation, https://arroba.readthedocs.io/
 Keywords: arroba,AT Protocol,ATP,Bluesky
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 arroba [![Circle CI](https://circleci.com/gh/snarfed/arroba.svg?style=svg)](https://circleci.com/gh/snarfed/arroba) [![Coverage Status](https://coveralls.io/repos/github/snarfed/arroba/badge.svg?branch=main)](https://coveralls.io/github/snarfed/arroba?branch=master)
 ===
 
-Python implementation of [Bluesky](https://blueskyweb.xyz/)'s low level [AT Protocol](https://atproto.com/), including [data repository](https://atproto.com/guides/data-repos), [Merkle search tree](https://atproto.com/guides/data-repos), and [com.atproto.sync XRPC methods](https://atproto.com/lexicons/com-atproto-sync).
+Python implementation of [Bluesky](https://blueskyweb.xyz/) [PDS](https://atproto.com/guides/data-repos) and [AT Protocol](https://atproto.com/specs/atp), including data repository, Merkle search tree, and [com.atproto.sync XRPC methods](https://atproto.com/lexicons/com-atproto-sync).
 
 _Arroba_ is the Spanish word for the [@ character](https://en.wikipedia.org/wiki/At_sign) ("at sign").
 
 Install from [PyPI](https://pypi.org/project/arroba/) with `pip install arroba`.
 
 License: This project is placed into the public domain.
 
@@ -34,14 +35,18 @@
 ## Usage
 
 TODO
 
 
 ## Changelog
 
+### 0.2 - 2023-05-18
+
+Implement repo and commit chain in new Repo class, including pluggable storage. This completes the first pass at all PDS data structures. Next release will include initial implementations of the `com.atproto.sync.*` XRPC methods.
+
 ### 0.1 - 2023-04-30
 
 Initial release! Still very in progress. MST, Walker, and Diff classes are mostly complete and working. Repo, commits, and sync XRPC methods are still in progress.
 
 
 Release instructions
 ---
```

### Comparing `arroba-0.1/pyproject.toml` & `arroba-0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 build-backend = 'setuptools.build_meta'
 
 [tool.setuptools]
 packages = ['arroba']
 
 [project]
 name = 'arroba'
-version = '0.1'
+version = '0.2'
 authors = [
     { name='Ryan Barrett', email='arroba@ryanb.org' },
 ]
-description = "Python implementation of Bluesky's low level AT Protocol, including repo, MST, and sync methods"
+description = "Python implementation of Bluesky PDS and AT Protocol, including repo, MST, and sync methods"
 readme = 'README.md'
 requires-python = '>=3.9'
 keywords = ['arroba', 'AT Protocol', 'ATP', 'Bluesky']
 dependencies = [
     'dag-cbor',
     'dag-json',
     'multiformats>=0.2.0',
@@ -31,7 +31,8 @@
     'Intended Audience :: Developers',
     'Development Status :: 3 - Alpha',
     'Topic :: Software Development :: Libraries :: Python Modules',
 ]
 
 [project.urls]
 'Homepage' = 'https://github.com/snarfed/arroba'
+'Documentation' = 'https://arroba.readthedocs.io/'
```

