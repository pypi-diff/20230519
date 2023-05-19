# Comparing `tmp/audiolm-pytorch-1.0.2.tar.gz` & `tmp/audiolm-pytorch-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm-pytorch-1.0.2.tar", last modified: Thu May 18 19:09:10 2023, max compression
+gzip compressed data, was "audiolm-pytorch-1.0.4.tar", last modified: Fri May 19 18:21:06 2023, max compression
```

## Comparing `audiolm-pytorch-1.0.2.tar` & `audiolm-pytorch-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:09:10.734339 audiolm-pytorch-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 19:09:10.734339 audiolm-pytorch-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:09:10.730339 audiolm-pytorch-1.0.2/audiolm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65627 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/audiolm_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/encodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/hubert_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30000 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/soundstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/audiolm_pytorch/vq_wav2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:09:10.734339 audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 19:09:10.000000 audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-18 19:09:10.000000 audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:09:10.000000 audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-18 19:09:10.000000 audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 19:09:10.000000 audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:09:10.734339 audiolm-pytorch-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-18 19:08:58.000000 audiolm-pytorch-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:21:06.071267 audiolm-pytorch-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 18:21:06.071267 audiolm-pytorch-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:21:06.071267 audiolm-pytorch-1.0.4/audiolm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/audiolm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65656 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/audiolm_pytorch/audiolm_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/audiolm_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/audiolm_pytorch/encodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/audiolm_pytorch/hubert_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/audiolm_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30000 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/audiolm_pytorch/soundstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/audiolm_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/audiolm_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/audiolm_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/audiolm_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/audiolm_pytorch/vq_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:21:06.071267 audiolm-pytorch-1.0.4/audiolm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 18:21:06.000000 audiolm-pytorch-1.0.4/audiolm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-19 18:21:06.000000 audiolm-pytorch-1.0.4/audiolm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:21:06.000000 audiolm-pytorch-1.0.4/audiolm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-19 18:21:06.000000 audiolm-pytorch-1.0.4/audiolm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 18:21:06.000000 audiolm-pytorch-1.0.4/audiolm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:21:06.071267 audiolm-pytorch-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-19 18:20:54.000000 audiolm-pytorch-1.0.4/setup.py
```

### Comparing `audiolm-pytorch-1.0.2/LICENSE` & `audiolm-pytorch-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.2/PKG-INFO` & `audiolm-pytorch-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.0.2
+Version: 1.0.4
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.0.2/README.md` & `audiolm-pytorch-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.2/audiolm_pytorch/__init__.py` & `audiolm-pytorch-1.0.4/audiolm_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.2/audiolm_pytorch/audiolm_pytorch.py` & `audiolm-pytorch-1.0.4/audiolm_pytorch/audiolm_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
 
         self.norm = LayerNorm(dim)
         self.context_norm = LayerNorm(dim_context) if norm_context else nn.Identity()
 
         self.attn_dropout = nn.Dropout(dropout)
 
         self.num_null_kv = num_null_kv
-        self.null_kv = nn.Parameter(torch.randn(2, num_null_kv, dim_head))
+        self.null_kv = nn.Parameter(torch.randn(2, num_null_kv, dim_head)) if num_null_kv > 0 else None
 
         self.to_q = nn.Linear(dim, inner_dim, bias = False)
         self.to_kv = nn.Linear(dim_context, dim_head * 2, bias = False)
 
         self.q_scale = nn.Parameter(torch.ones(dim_head))
         self.k_scale = nn.Parameter(torch.ones(dim_head))
```

### Comparing `audiolm-pytorch-1.0.2/audiolm_pytorch/data.py` & `audiolm-pytorch-1.0.4/audiolm_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.2/audiolm_pytorch/encodec.py` & `audiolm-pytorch-1.0.4/audiolm_pytorch/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.2/audiolm_pytorch/hubert_kmeans.py` & `audiolm-pytorch-1.0.4/audiolm_pytorch/hubert_kmeans.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.2/audiolm_pytorch/optimizer.py` & `audiolm-pytorch-1.0.4/audiolm_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.2/audiolm_pytorch/soundstream.py` & `audiolm-pytorch-1.0.4/audiolm_pytorch/soundstream.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.2/audiolm_pytorch/t5.py` & `audiolm-pytorch-1.0.4/audiolm_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.2/audiolm_pytorch/trainer.py` & `audiolm-pytorch-1.0.4/audiolm_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.2/audiolm_pytorch/vq_wav2vec.py` & `audiolm-pytorch-1.0.4/audiolm_pytorch/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/PKG-INFO` & `audiolm-pytorch-1.0.4/audiolm_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.0.2
+Version: 1.0.4
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.0.2/audiolm_pytorch.egg-info/SOURCES.txt` & `audiolm-pytorch-1.0.4/audiolm_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.0.2/setup.py` & `audiolm-pytorch-1.0.4/setup.py`

 * *Files identical despite different names*

