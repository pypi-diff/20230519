# Comparing `tmp/sketchlib-0.0.1.tar.gz` & `tmp/sketchlib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sketchlib-0.0.1.tar", last modified: Fri Apr 21 05:25:16 2023, max compression
+gzip compressed data, was "sketchlib-0.0.2.tar", last modified: Fri May 19 17:16:22 2023, max compression
```

## Comparing `sketchlib-0.0.1.tar` & `sketchlib-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 05:25:16.753268 sketchlib-0.0.1/
--rw-rw-rw-   0        0        0     1107 2023-04-20 19:32:39.000000 sketchlib-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2137 2023-04-21 05:25:16.752251 sketchlib-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-04-21 05:06:35.000000 sketchlib-0.0.1/README.md
--rw-rw-rw-   0        0        0     1238 2023-04-21 05:24:00.000000 sketchlib-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 05:25:16.753268 sketchlib-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 05:25:16.701661 sketchlib-0.0.1/sketchlib.egg-info/
--rw-rw-rw-   0        0        0     2137 2023-04-21 05:25:16.000000 sketchlib-0.0.1/sketchlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2023-04-21 05:25:16.000000 sketchlib-0.0.1/sketchlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 05:25:16.000000 sketchlib-0.0.1/sketchlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-21 05:25:16.000000 sketchlib-0.0.1/sketchlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-21 05:25:16.000000 sketchlib-0.0.1/sketchlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 05:25:16.734638 sketchlib-0.0.1/streamsketchlib/
--rw-rw-rw-   0        0        0        0 2023-03-27 18:18:54.000000 sketchlib-0.0.1/streamsketchlib/__init__.py
--rw-rw-rw-   0        0        0     1205 2023-04-18 22:00:01.000000 sketchlib-0.0.1/streamsketchlib/bloom_filter.py
--rw-rw-rw-   0        0        0     3493 2023-04-21 05:04:12.000000 sketchlib-0.0.1/streamsketchlib/cm_hh_cash_register.py
--rw-rw-rw-   0        0        0     2399 2023-04-14 18:07:20.000000 sketchlib-0.0.1/streamsketchlib/count_min.py
--rw-rw-rw-   0        0        0     2326 2023-03-27 17:31:29.000000 sketchlib-0.0.1/streamsketchlib/f0_bjkst.py
--rw-rw-rw-   0        0        0     3267 2023-04-13 23:38:23.000000 sketchlib-0.0.1/streamsketchlib/f0_estimate.py
--rw-rw-rw-   0        0        0     2104 2023-04-13 23:38:23.000000 sketchlib-0.0.1/streamsketchlib/f2_estimate.py
--rw-rw-rw-   0        0        0     1935 2023-04-14 19:30:34.000000 sketchlib-0.0.1/streamsketchlib/heavy_hitters_cm.py
--rw-rw-rw-   0        0        0     3690 2023-03-27 17:31:29.000000 sketchlib-0.0.1/streamsketchlib/minhash.py
--rw-rw-rw-   0        0        0     4296 2023-03-27 17:31:29.000000 sketchlib-0.0.1/streamsketchlib/misra_gries.py
--rw-rw-rw-   0        0        0      788 2023-03-30 20:22:20.000000 sketchlib-0.0.1/streamsketchlib/rsv_sampling.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:25:16.750254 sketchlib-0.0.1/tests/
--rw-rw-rw-   0        0        0     3134 2023-04-20 21:27:51.000000 sketchlib-0.0.1/tests/test_bloom_filter.py
--rw-rw-rw-   0        0        0     2197 2023-04-11 22:11:29.000000 sketchlib-0.0.1/tests/test_count_min.py
--rw-rw-rw-   0        0        0     1479 2023-03-30 20:16:29.000000 sketchlib-0.0.1/tests/test_f0_estimate.py
--rw-rw-rw-   0        0        0     1043 2023-03-30 22:04:32.000000 sketchlib-0.0.1/tests/test_f2_estimate.py
--rw-rw-rw-   0        0        0     4197 2023-04-14 18:07:20.000000 sketchlib-0.0.1/tests/test_hh_count_min.py
+drwxrwxrwx   0        0        0        0 2023-05-19 17:16:22.124473 sketchlib-0.0.2/
+-rw-rw-rw-   0        0        0     1107 2023-04-20 19:32:39.000000 sketchlib-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2126 2023-05-19 17:16:22.123504 sketchlib-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-21 05:06:35.000000 sketchlib-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1156 2023-05-19 17:15:04.000000 sketchlib-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 17:16:22.124473 sketchlib-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 17:16:22.079951 sketchlib-0.0.2/sketchlib.egg-info/
+-rw-rw-rw-   0        0        0     2126 2023-05-19 17:16:22.000000 sketchlib-0.0.2/sketchlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      753 2023-05-19 17:16:22.000000 sketchlib-0.0.2/sketchlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 17:16:22.000000 sketchlib-0.0.2/sketchlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-05-19 17:16:22.000000 sketchlib-0.0.2/sketchlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-19 17:16:22.000000 sketchlib-0.0.2/sketchlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 17:16:22.103462 sketchlib-0.0.2/streamsketchlib/
+-rw-rw-rw-   0        0        0        0 2023-03-27 18:18:54.000000 sketchlib-0.0.2/streamsketchlib/__init__.py
+-rw-rw-rw-   0        0        0     2431 2023-05-15 13:54:00.000000 sketchlib-0.0.2/streamsketchlib/bloom_filter.py
+-rw-rw-rw-   0        0        0     2467 2023-05-17 12:37:22.000000 sketchlib-0.0.2/streamsketchlib/count_min.py
+-rw-rw-rw-   0        0        0     1358 2023-05-15 13:54:00.000000 sketchlib-0.0.2/streamsketchlib/distinct_count.py
+-rw-rw-rw-   0        0        0     4415 2023-05-15 13:54:00.000000 sketchlib-0.0.2/streamsketchlib/distinct_count_algorithms.py
+-rw-rw-rw-   0        0        0     2858 2023-05-12 18:51:18.000000 sketchlib-0.0.2/streamsketchlib/f2_estimate.py
+-rw-rw-rw-   0        0        0     2059 2023-05-17 11:33:05.000000 sketchlib-0.0.2/streamsketchlib/heavy_hitters.py
+-rw-rw-rw-   0        0        0     8564 2023-05-17 12:37:22.000000 sketchlib-0.0.2/streamsketchlib/heavy_hitters_algorithms.py
+-rw-rw-rw-   0        0        0     1935 2023-04-14 19:30:34.000000 sketchlib-0.0.2/streamsketchlib/heavy_hitters_cm.py
+-rw-rw-rw-   0        0        0     3690 2023-03-27 17:31:29.000000 sketchlib-0.0.2/streamsketchlib/minhash.py
+-rw-rw-rw-   0        0        0     1444 2023-05-12 18:51:18.000000 sketchlib-0.0.2/streamsketchlib/rsv_sampling.py
+drwxrwxrwx   0        0        0        0 2023-05-19 17:16:22.120495 sketchlib-0.0.2/tests/
+-rw-rw-rw-   0        0        0     4159 2023-05-15 13:54:00.000000 sketchlib-0.0.2/tests/test_bloom_filter.py
+-rw-rw-rw-   0        0        0     2197 2023-04-11 22:11:29.000000 sketchlib-0.0.2/tests/test_count_min.py
+-rw-rw-rw-   0        0        0     2165 2023-05-12 18:51:18.000000 sketchlib-0.0.2/tests/test_distinct_count.py
+-rw-rw-rw-   0        0        0     2980 2023-05-12 18:51:18.000000 sketchlib-0.0.2/tests/test_f0_estimate.py
+-rw-rw-rw-   0        0        0     2368 2023-05-15 13:54:00.000000 sketchlib-0.0.2/tests/test_f2_estimate.py
+-rw-rw-rw-   0        0        0     5892 2023-05-17 12:40:20.000000 sketchlib-0.0.2/tests/test_heavyhitters.py
+-rw-rw-rw-   0        0        0     1059 2023-05-12 18:51:18.000000 sketchlib-0.0.2/tests/test_rsv_sampling.py
```

### Comparing `sketchlib-0.0.1/LICENSE` & `sketchlib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.1/PKG-INFO` & `sketchlib-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sketchlib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library of streaming algorithms for processing massive data.
 Author-email: "Dr. Hoa Vu and Daniel Barnas" <danielbarn90@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2023 Dr. Hoa Vu and Daniel Barnas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Project-URL: Homepage, https://github.com/db-gb/DataStreamSketches
+Project-URL: Homepage, https://datasketchlib.github.io/
 Keywords: streaming,algorithms,big,massive,data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `sketchlib-0.0.1/pyproject.toml` & `sketchlib-0.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sketchlib"
-version = "0.0.1"
+version = "0.0.2"
 description = "Library of streaming algorithms for processing massive data."
 readme = "README.md"
 authors = [{ name = "Dr. Hoa Vu and Daniel Barnas", email = "danielbarn90@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -23,26 +23,22 @@
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
-Homepage = "https://github.com/db-gb/DataStreamSketches"
+Homepage = "https://datasketchlib.github.io/"
 
 [tool.bumpver]
-current_version = "0.0.1"
+current_version = "0.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
-    'current_version = "{version}"',
-]
-"README.md" = [
-    "{version}",
-    "{pep440_version}",
+    'version = "{version}"',
 ]
```

### Comparing `sketchlib-0.0.1/sketchlib.egg-info/PKG-INFO` & `sketchlib-0.0.2/sketchlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sketchlib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library of streaming algorithms for processing massive data.
 Author-email: "Dr. Hoa Vu and Daniel Barnas" <danielbarn90@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2023 Dr. Hoa Vu and Daniel Barnas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Project-URL: Homepage, https://github.com/db-gb/DataStreamSketches
+Project-URL: Homepage, https://datasketchlib.github.io/
 Keywords: streaming,algorithms,big,massive,data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `sketchlib-0.0.1/sketchlib.egg-info/SOURCES.txt` & `sketchlib-0.0.2/sketchlib.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 sketchlib.egg-info/PKG-INFO
 sketchlib.egg-info/SOURCES.txt
 sketchlib.egg-info/dependency_links.txt
 sketchlib.egg-info/requires.txt
 sketchlib.egg-info/top_level.txt
 streamsketchlib/__init__.py
 streamsketchlib/bloom_filter.py
-streamsketchlib/cm_hh_cash_register.py
 streamsketchlib/count_min.py
-streamsketchlib/f0_bjkst.py
-streamsketchlib/f0_estimate.py
+streamsketchlib/distinct_count.py
+streamsketchlib/distinct_count_algorithms.py
 streamsketchlib/f2_estimate.py
+streamsketchlib/heavy_hitters.py
+streamsketchlib/heavy_hitters_algorithms.py
 streamsketchlib/heavy_hitters_cm.py
 streamsketchlib/minhash.py
-streamsketchlib/misra_gries.py
 streamsketchlib/rsv_sampling.py
 tests/test_bloom_filter.py
 tests/test_count_min.py
+tests/test_distinct_count.py
 tests/test_f0_estimate.py
 tests/test_f2_estimate.py
-tests/test_hh_count_min.py
+tests/test_heavyhitters.py
+tests/test_rsv_sampling.py
```

### Comparing `sketchlib-0.0.1/streamsketchlib/count_min.py` & `sketchlib-0.0.2/streamsketchlib/count_min.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         """ Compute the hash of a token. Converts hash value to a bin number
             based on k."""
         hash_value = mmh3.hash(token, seed, signed=False)/self.max_32_int
         bin_number = hash_value * self.width
         return int(bin_number)
 
     def insert(self, token, count):
+        # !!! Remember to put a guardrail against negative updates
         for row in range(self.depth):
             col = self._hash(token, self._hash_seeds[row])
             self.table[row][col] = self.table[row][col] + count
 
     def estimate_count(self, token):
         estimate = inf
         for row in range(self.depth):
```

### Comparing `sketchlib-0.0.1/streamsketchlib/f0_estimate.py` & `sketchlib-0.0.2/streamsketchlib/bloom_filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,70 @@
-import mmh3
+import mmh3 
 import math
-import bisect
-from bisect import bisect_left
-import statistics
+from copy import deepcopy
 
-
-class F0Estimate:
+class BloomFilter:
     """
-    Loglog algorithm: memory efficient data structure to estimate
-    the number of distinct elements in streams
+    Bloom Filter
     """
-    def __init__(self, epsilon=0.01, delta=0.01, c=2, hash_type="mmh3", seed=42):
-        """ epsilon: relative error
-        delta: failure probability
-        This is the first algorithm of [BJKST02]
+    def __init__(self, n=10000, delta=0.01, seed=42):
+        """ n: the maximum number of insertions
+        delta: false positive rate 
         """
-        self.epsilon = epsilon
-        self.hash_type = hash_type
-        self.max_128_int = pow(2, 128)-1
+        self.n = n
+        self.delta = delta
+        self.seed = seed
 
-        # width ~ c/eps^2 and depth ~ c log(1/delta)
-        self.width = c*int(math.pow(1/self.epsilon, 2))
-        self.depth = c*int(math.log(1/delta, 2))
-        self.seeds = [seed*i for i in range(self.depth)]
-
-        # data structure to store the smallest t hash values
-        self.table = [[] for i in range(self.depth)]
-
-        # a list to store all distinct values if F0 < t
-        self.naive_lst = set()
-
-    def _binary_search(self, a, x):
-        i = bisect_left(a, x)
-        if i != len(a) and a[i] == x:
-            return i
-        else:
-            return -1
+        self.m = math.ceil(self.n*math.log2(1/delta)/math.log(2))
+        self.k = math.ceil(math.log(1/delta))
+        self.max_128_int = pow(2, 128)-1
+        self.B = [0 for _ in range(self.m)]
+        self.seeds = [self.seed*i for i in range(self.k)]
 
     def _hash(self, token, seed):
-        """ Compute the hash of a token. """
-        if self.hash_type == "mmh3":
-            return mmh3.hash128(token, seed, signed=False)/self.max_128_int
-
-    def insert(self, token):
-        """ Insert a token into the sketch. Token must be byte-like objects. """
-        if len(self.naive_lst) < self.width:
-            self.naive_lst.add(token)
-
-        for i in range(self.depth):
-            hash_value = self._hash(token, self.seeds[i])
-            j = self._binary_search(self.table[i], hash_value)
-
-            if j == -1:
-                if len(self.table[i]) < self.width:
-                    bisect.insort(self.table[i], hash_value)
-                elif self.table[i][self.width-1] > hash_value:
-                    bisect.insort(self.table[i], hash_value)
-                    self.table[i].pop()
+        x = mmh3.hash128(token, seed, signed=False)/self.max_128_int
+        return int(x*(self.m-1))
+    
+    def delete(self, x):
+        """ Delete x from the data structure. To ensure correctness, remove the element x 
+        from the data structure only if it exists in the data structure.
+        """
+        for i in range(self.k):
+            self.B[self._hash(x, self.seeds[i])] -= 1
+
+    def insert(self, x):
+        """ Insert x to the data structure.
+        """
+        for i in range(self.k):
+            self.B[self._hash(x, self.seeds[i])] += 1
 
+    def membership(self, x):
+        """ Check if x is in the data structure. T
+        here is a probability of around delta for a false positive.
+        """
+        for i in range(self.k):
+            if self.B[self._hash(x, self.seeds[i])] == 0:
+                return False
+        return True
+    
     def merge(self, S):
-        """ Merge self and another sketch S that must have same seeds """
-        # merge the small lists
-        for x in S.naive_lst:
-            if len(self.naive_lst) < self.width:
-                self.naive_lst.add(x)
-            else:
-                break
-
-        # merge the smallest hash values
-        for i in range(self.depth):
-            for x in S.table[i]:
-                j = self._binary_search(self.table[i], x)
-                if j  == -1:
-                    if len(self.table[i]) < self.width:
-                        bisect.insort(self.table[i], x)
-                    elif self.table[i][self.width-1] > x:
-                        bisect.insort(self.table[i], x)
-                        self.table[i].pop()
-
-    def estimator(self):
-        """ Return the estimate for the number of distinct
-        elements inserted so far """
-        #start_time = time.time()
-        if len(self.naive_lst) < self.width:
-            result = len(self.naive_lst)
-            return result
-        est = [int(self.width/self.table[i][self.width-1]) for i in range(self.depth)]
-        median_of_est = statistics.median(est)
-        return int(median_of_est)
+        """ Combine self with Bloom filter S with the same n, delta, and seed to obtain 
+        a new Bloom filter that represents the union of the two sets.
+        """
+        for i in range(len(self.B)):
+            self.B[i] += S.B[i]
+
+    def __add__(self, S):
+        """ Return the merged Bloom filter of self and S.
+        """
+        merged_filter = BloomFilter.from_existing(self)
+        merged_filter.B = deepcopy(self.B)
+        for i in range(len(merged_filter.B)):
+            merged_filter.B[i] += S.B[i]
+        return merged_filter
+
+    @classmethod
+    def from_existing(cls, original):
+        """ Creates a new Bloom Filter based on existing Bloom Filter with similar parameters
+        so that they are mergeable."""
+        new_filter = cls(n = original.n, delta = original.delta, seed = original.seed)
+        return new_filter
```

### Comparing `sketchlib-0.0.1/streamsketchlib/heavy_hitters_cm.py` & `sketchlib-0.0.2/streamsketchlib/heavy_hitters_cm.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.1/streamsketchlib/minhash.py` & `sketchlib-0.0.2/streamsketchlib/minhash.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.1/tests/test_bloom_filter.py` & `sketchlib-0.0.2/tests/test_bloom_filter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 from streamsketchlib.bloom_filter import BloomFilter
 
 
-from streamsketchlib.bloom_filter import BloomFilter
-
-
 def test_bloom_filter_1():
     test_n = 1000000
-
     test_bf = BloomFilter(n=test_n)
+    result = True
+    false_positives = []
 
     for i in range(test_n):
         test_bf.insert(str(i))
 
-    result = True
     for i in range(test_n):
         if not test_bf.membership(str(i)):
             result = False
     assert result
 
-    false_positives = []
-
     for i in range(test_n, 2*test_n):
         if test_bf.membership(str(i)):
             false_positives.append(i)
-
     false_pos_count = len(false_positives)
     assert false_pos_count < (test_n * 0.012)
 
 
 def test_bloom_filter_2():
     delta = 0.0001
     n = 100
     B = BloomFilter(n = n, delta = delta)
+    result = True
+    false_positive = 0
+    
     for i in range(n):
         B.insert(str(i))
     
-    result = True
     for i in range(n):
         if B.membership(str(i)) == False:
             result = False
     assert(result == True)
 
-    false_positive = 0
     for i in range(n):
         if B.membership(str(i+n)) == True:
             false_positive += 1
     assert(false_positive <= 1.1*delta*n)
 
 
 def test_bloom_filter_3():
@@ -72,51 +67,48 @@
     # insert 0,...,n-1 to B
     # insert n/2-1,...,3n/2-1 to C
     # merge 
     delta = 0.1
     n = 1000
     B = BloomFilter(n = 2*n, delta = delta)
     C = BloomFilter(n = 2*n, delta = delta)
+    result = True
+    false_positive = 0
 
     for i in range(n):
         B.insert(str(i))
-
     for i in range(int(n/2), int((3/2)*n)):
         C.insert(str(i))
-
     B.merge(C)
     
-    result = True
     for i in range(int((3/2)*n)):
         if B.membership(str(i)) == False:
             result = False
     assert(result == True)
-
-    false_positive = 0
+   
     for i in range(2*n, 3*n):
         if B.membership(str(i)) == True:
             false_positive += 1
     assert(false_positive <= 1.1*n*delta)
 
 
 def test_bloom_filter_5():
     # insert 0,...,n-1 to B
     # insert n/2-1,...,3n/2-1 to C
     # merge C to B
     # delete n,...,3n/2-1 from B
     delta = 0.1
     n = 1000
     B = BloomFilter(n = 2*n, delta = delta)
-    C = BloomFilter(n = 2*n, delta = delta)
+    C = BloomFilter.from_existing(B)
     result = True
     false_positive = 0
 
     for i in range(n):
         B.insert(str(i))
-
     for i in range(int(n/2), int((3/2)*n)):
         C.insert(str(i))
 
     B.merge(C)
 
     for i in range(n, int((3/2)*n)):
         B.delete(str(i))
@@ -126,8 +118,48 @@
             result = False
     assert(result == True)
 
     for i in range(n, int((3/2)*n)):
         if B.membership(str(i)) == True:
             false_positive += 1
     assert(false_positive <= 1.1*delta*(1/2)*n)
-    
+
+def test_bloom_filter_6():
+    # insert 0,...,n-1 to B
+    # insert n/2-1,...,3n/2-1 to C
+    # D = C + B
+    # delete n,...,3n/2-1 from B
+    delta = 0.1
+    n = 1000
+    B = BloomFilter(n = 2*n, delta = delta)
+    C = BloomFilter.from_existing(B)
+    result = True
+    false_positive = 0
+
+    for i in range(n):
+        B.insert(str(i))
+    for i in range(int(n/2), int((3/2)*n)):
+        C.insert(str(i))
+    D = B + C
+    B = B + C
+
+    for i in range(n, int((3/2)*n)):
+        D.delete(str(i))
+        B.delete(str(i))
+
+    for i in range(n):
+        if D.membership(str(i)) == False or B.membership(str(i)) == False :
+            result = False
+    assert(result == True)
+
+    for i in range(n, int((3/2)*n)):
+        if D.membership(str(i)) == True or B.membership(str(i)) == True:
+            false_positive += 1
+    assert(false_positive <= 1.1*delta*(1/2)*n)
+    
+if __name__ == '__main__':
+    test_bloom_filter_1()
+    test_bloom_filter_2()
+    test_bloom_filter_3()
+    test_bloom_filter_4()
+    test_bloom_filter_5()
+    test_bloom_filter_6()
```

### Comparing `sketchlib-0.0.1/tests/test_count_min.py` & `sketchlib-0.0.2/tests/test_count_min.py`

 * *Files identical despite different names*

### Comparing `sketchlib-0.0.1/tests/test_f0_estimate.py` & `sketchlib-0.0.2/tests/test_distinct_count.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,87 @@
 import random
 import math
 import sys
 sys.path.insert(0, '..')
 
-from streamsketchlib.f0_estimate import F0Estimate
+from streamsketchlib.distinct_count import DistinctCount
 
 m = 1000000
 eps = 0.05
 delta = 0.05
 
 def test_f0_estimate_small():
     """ test case when F0 is large """
     l = 0
     u = 500000
     stream = []
-    f_0 = F0Estimate(epsilon = eps, delta = delta)
+    f_0 = DistinctCount(epsilon = eps, delta = delta)
 
     for i in range(m):
         x = random.randrange(l,u)
         stream.append(x)
         f_0.insert(str(x))
 
     ans = len(set(stream))
     assert (1-eps) * ans <= f_0.estimator() and  f_0.estimator() <= (1+eps) * ans
 
 def test_f0_estimate_medium():
     """ test case when F0 is medium """
     l = 0
     u = 2000000
     stream = []
-    f_0 = F0Estimate(epsilon = eps, delta = delta)
+    f_0 = DistinctCount(epsilon = eps, delta = delta)
 
     for i in range(m):
         x = random.randrange(l,u)
         stream.append(x)
         f_0.insert(str(x))
 
     ans = len(set(stream))
     assert (1-eps) * ans <= f_0.estimator() and  f_0.estimator() <= (1+eps) * ans
 
 def test_f0_estimate_large():
     """ test case when F0 is large """
     l = 0
     u = 1000000
     stream = []
-    f_0 = F0Estimate(epsilon = eps, delta = delta)
+    f_0 = DistinctCount(epsilon = eps, delta = delta)
 
     for i in range(m):
         x = random.randrange(l,u)
         stream.append(x)
         f_0.insert(str(x))
 
     ans = len(set(stream))
     assert (1-eps) * ans <= f_0.estimator() and  f_0.estimator() <= (1+eps) * ans
 
+def test_f0_estimate_merge():
+    """ test case when F0 is large """
+    l = 0
+    u = 1000000
+    l2 = int(1000000/2)
+    u2 = int(l2*2)
+
+    stream = []
+    f_0 = DistinctCount(epsilon = eps, delta = delta)
+    f_0_new = DistinctCount.from_existing(f_0)
+
+    for i in range(m):
+        x = random.randrange(l,u)
+        stream.append(x)
+        f_0.insert(str(x))
+    for i in range(m):
+        x = random.randrange(l2,u2)
+        stream.append(x)
+        f_0_new.insert(str(x))
+
+    f_0.merge(f_0_new)
+    ans = len(set(stream))
+
+    assert (1-eps) * ans <= f_0.estimator() and  f_0.estimator() <= (1+eps) * ans
+
 
 if __name__ == '__main__':
     test_f0_estimate_small()
     test_f0_estimate_medium()
     test_f0_estimate_large()
+    test_f0_estimate_merge()
```

### Comparing `sketchlib-0.0.1/tests/test_hh_count_min.py` & `sketchlib-0.0.2/tests/test_heavyhitters.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-from streamsketchlib.cm_hh_cash_register import HeavyHittersCMRegister
-
+from streamsketchlib.heavy_hitters import HeavyHittersFinder
 import pandas as pd
-from pympler.asizeof import asizeof
 from time import time
 
+def test_hh_small():
+    test_hh = HeavyHittersFinder(phi=0.01, epsilon=0.2)
+    # test = asizeof(test_hh_cm)
+
+    test_hh.insert("This", 1)
+    test_hh.insert("is", 1)
+    test_hh.insert("is", 3)
+    test_hh.insert("only", 1)
+    test_hh.insert("a", 1)
+    test_hh.insert("a", 2)
+    test_hh.insert("test.", 10000)
+    test_hh.insert("b", 1)
+    test_hh.insert("c", 1)
+    test_hh.insert("d", 1)
 
-def test_bidict_small():
-    test_hh_cm = HeavyHittersCMRegister(phi=0.01, epsilon=0.2)
-    test = asizeof(test_hh_cm)
-
-    test_hh_cm.insert("This", 1)
-    test_hh_cm.insert("is", 1)
-    test_hh_cm.insert("is", 3)
-    test_hh_cm.insert("only", 1)
-    test_hh_cm.insert("a", 1)
-    test_hh_cm.insert("a", 2)
-    test_hh_cm.insert("test.", 10000)
-    test_hh_cm.insert("b", 1)
-    test_hh_cm.insert("c", 1)
-    test_hh_cm.insert("d", 1)
-
-    test = asizeof(test_hh_cm)
+    #test = asizeof(test_hh_cm)
 
-    test = test_hh_cm.get_heavy_hitters()
-    assert test == ['test.']
+    test = test_hh.get_heavy_hitters()
+    assert test == {'test.': 10000}
 
 
-def test_bidict_large():
-    test_hh_cm = HeavyHittersCMRegister(phi=0.005, epsilon=0.2)
+def test_hh_large():
+    test_hh = HeavyHittersFinder(phi=0.005, epsilon=0.2)
     test_hh_dict = dict()
 
-    test_cm_size_start = asizeof(test_hh_cm)
-    test_dict_size_start = asizeof(test_hh_dict)
+    #test_cm_size_start = asizeof(test_hh_cm)
+    #test_dict_size_start = asizeof(test_hh_dict)
 
     try:
         test_data = pd.read_csv('item_sales_filtered.csv')
 
     except FileNotFoundError as e:
         print('Test files not found. Skipping test.')
         return
@@ -47,38 +44,38 @@
         if item[0] in test_hh_dict:
             test_hh_dict[item[0]] += item[1]
         else:
             test_hh_dict[item[0]] = item[1]
     end_dict = time()
 
     dict_time = end_dict - start_dict
-    test_dict_size_end = asizeof(test_hh_dict)
+    #test_dict_size_end = asizeof(test_hh_dict)
 
     start_cm = time()
     for item in item_sales:
-        test_hh_cm.insert(str(item[0]), item[1])
+        test_hh.insert(str(item[0]), item[1])
     end_cm = time()
 
     cm_time = end_cm - start_cm
-    test_cm_size_end = asizeof(test_hh_cm)
+    #test_cm_size_end = asizeof(test_hh_cm)
 
-    test = test_hh_cm.get_heavy_hitters()
+    test = test_hh.get_heavy_hitters()
     assert '1503844' in test
     assert '1473474' in test
     assert '2042941' in test
     assert '2042947' in test
     assert '819932' not in test
 
 
 def test_bidict_kindle():
-    test_hh_cm = HeavyHittersCMRegister(phi=0.01, epsilon=0.2)
+    test_hh_cm = HeavyHittersFinder(phi=0.01, epsilon=0.2)
     test_hh_dict = dict()
 
-    test_cm_size_start = asizeof(test_hh_cm)
-    test_dict_size_start = asizeof(test_hh_dict)
+    #test_cm_size_start = asizeof(test_hh_cm)
+    #test_dict_size_start = asizeof(test_hh_dict)
 
     try:
         test_data = pd.read_csv('kindle_reviews.csv')
 
     except FileNotFoundError as e:
         print('Test files not found. Skipping test.')
         return
@@ -91,32 +88,32 @@
         if reviewer in test_hh_dict:
             test_hh_dict[reviewer] += 1
         else:
             test_hh_dict[reviewer] = 1
     end_dict = time()
 
     dict_time = end_dict - start_dict
-    test_dict_size_end = asizeof(test_hh_dict)
+    #test_dict_size_end = asizeof(test_hh_dict)
 
     start_cm = time()
     for reviewer in reviewers:
         test_hh_cm.insert(str(reviewer), 1)
     end_cm = time()
     cm_time = end_cm - start_cm
 
-    test_cm_size_end = asizeof(test_hh_cm)
+    #test_cm_size_end = asizeof(test_hh_cm)
 
     test_hh = test_hh_cm.get_heavy_hitters()
     assert 'Amazon Customer' in test_hh
     assert 'Kindle Customer' in test_hh
 
 
 def test_small_merge():
-    test_hh_cm = HeavyHittersCMRegister(phi=0.01, epsilon=0.2)
-    test_hh_cm_2 = HeavyHittersCMRegister.from_existing(test_hh_cm)
+    test_hh_cm = HeavyHittersFinder(phi=0.01, epsilon=0.2)
+    test_hh_cm_2 = HeavyHittersFinder.from_existing(test_hh_cm)
 
     test_hh_cm.insert("This", 1)
     test_hh_cm.insert("is", 1)
     test_hh_cm.insert("is", 3)
     test_hh_cm.insert("only", 1)
     test_hh_cm.insert("a", 1)
     test_hh_cm.insert("a", 2)
@@ -145,7 +142,70 @@
 
     test_hh_cm.merge(test_hh_cm_2)
     merge_test = test_hh_cm.get_heavy_hitters()
 
     assert 'test.' in merge_test
     assert 'is' in merge_test
     assert 'only' not in merge_test
+
+def test_hh_mg_small():
+    test_hh = HeavyHittersFinder(phi=0.01, epsilon=0.2,
+                                 algorithm=HeavyHittersFinder.MISRAGRIES)
+    # test = asizeof(test_hh_cm)
+
+    test_hh.insert("This", 1)
+    test_hh.insert("is", 1)
+    test_hh.insert("is", 3)
+    test_hh.insert("only", 1)
+    test_hh.insert("a", 1)
+    test_hh.insert("a", 2)
+    test_hh.insert("test.", 10000)
+    test_hh.insert("b", 1)
+    test_hh.insert("c", 1)
+    test_hh.insert("d", 1)
+
+    # test = asizeof(test_hh_cm)
+
+    test = test_hh.get_heavy_hitters()
+    assert test == {'test.': 10000}
+
+
+def test_bidict_kindle_mg():
+    test_hh_cm = HeavyHittersFinder(phi=0.01, epsilon=0.2,
+                                    algorithm=HeavyHittersFinder.MISRAGRIES)
+    test_hh_dict = dict()
+
+    #test_cm_size_start = asizeof(test_hh_cm)
+    #test_dict_size_start = asizeof(test_hh_dict)
+
+    try:
+        test_data = pd.read_csv('kindle_reviews.csv')
+
+    except FileNotFoundError as e:
+        print('Test files not found. Skipping test.')
+        return
+
+    test_data = test_data['reviewerName']
+    reviewers = test_data.tolist()
+
+    start_dict = time()
+    for reviewer in reviewers:
+        if reviewer in test_hh_dict:
+            test_hh_dict[reviewer] += 1
+        else:
+            test_hh_dict[reviewer] = 1
+    end_dict = time()
+
+    dict_time = end_dict - start_dict
+    #test_dict_size_end = asizeof(test_hh_dict)
+
+    start_cm = time()
+    for reviewer in reviewers:
+        test_hh_cm.insert(str(reviewer), 1)
+    end_cm = time()
+    cm_time = end_cm - start_cm
+
+    #test_cm_size_end = asizeof(test_hh_cm)
+
+    test_hh = test_hh_cm.get_heavy_hitters()
+    assert 'Amazon Customer' in test_hh
+    assert 'Kindle Customer' in test_hh
```

