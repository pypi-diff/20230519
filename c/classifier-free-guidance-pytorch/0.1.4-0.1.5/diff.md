# Comparing `tmp/classifier-free-guidance-pytorch-0.1.4.tar.gz` & `tmp/classifier-free-guidance-pytorch-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classifier-free-guidance-pytorch-0.1.4.tar", last modified: Wed Mar  8 20:32:23 2023, max compression
+gzip compressed data, was "classifier-free-guidance-pytorch-0.1.5.tar", last modified: Fri May 19 18:13:00 2023, max compression
```

## Comparing `classifier-free-guidance-pytorch-0.1.4.tar` & `classifier-free-guidance-pytorch-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:32:23.194656 classifier-free-guidance-pytorch-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-08 20:32:13.000000 classifier-free-guidance-pytorch-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-08 20:32:13.000000 classifier-free-guidance-pytorch-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-08 20:32:23.194656 classifier-free-guidance-pytorch-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-03-08 20:32:13.000000 classifier-free-guidance-pytorch-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:32:23.190656 classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-08 20:32:13.000000 classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-03-08 20:32:13.000000 classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch/classifier_free_guidance_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:32:23.190656 classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch/data/
--rw-r--r--   0 runner    (1001) docker     (123)  3194984 2023-03-08 20:32:13.000000 classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch/data/bpe_simple_vocab_16e6.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-03-08 20:32:13.000000 classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-03-08 20:32:13.000000 classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-03-08 20:32:13.000000 classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:32:23.190656 classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-08 20:32:23.000000 classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-08 20:32:23.000000 classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 20:32:23.000000 classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-08 20:32:23.000000 classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-08 20:32:23.000000 classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 20:32:23.194656 classifier-free-guidance-pytorch-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-08 20:32:13.000000 classifier-free-guidance-pytorch-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:13:00.143517 classifier-free-guidance-pytorch-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-19 18:13:00.143517 classifier-free-guidance-pytorch-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:13:00.139517 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16690 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/classifier_free_guidance_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:13:00.139517 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  3194984 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/data/bpe_simple_vocab_16e6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:13:00.139517 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-19 18:13:00.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-19 18:13:00.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:13:00.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-19 18:13:00.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 18:13:00.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:13:00.143517 classifier-free-guidance-pytorch-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/setup.py
```

### Comparing `classifier-free-guidance-pytorch-0.1.4/LICENSE` & `classifier-free-guidance-pytorch-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.1.4/PKG-INFO` & `classifier-free-guidance-pytorch-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classifier-free-guidance-pytorch
-Version: 0.1.4
+Version: 0.1.5
 Summary: Classifier Free Guidance - Pytorch
 Home-page: https://github.com/lucidrains/classifier-free-guidance-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,classifier free guidance,text conditioning and guidance
 Classifier: Development Status :: 4 - Beta
```

### Comparing `classifier-free-guidance-pytorch-0.1.4/README.md` & `classifier-free-guidance-pytorch-0.1.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 If you wish to use cross attention based conditioning (each hidden feature in your network can attend to individual subword tokens), just import the `AttentionTextConditioner` instead. Rest is the same
 
 ```python
 from classifier_free_guidance_pytorch import AttentionTextConditioner
 
 text_conditioner = AttentionTextConditioner(
-    model_types = ('t5', 'clip'),   # something like in eDiff paper, where they used both T5 and Clip for even better results (Karras et al.)
+    model_types = ('t5', 'clip'),   # something like in eDiff paper, where they used both T5 and Clip for even better results (Balaji et al.)
     hidden_dims = (256, 512),
     cond_drop_prob = 0.2
 )
 ```
 
 ## Magic Decorator (wip)
 
@@ -185,7 +185,16 @@
     title   = {eDiff-I: Text-to-Image Diffusion Models with an Ensemble of Expert Denoisers},
     author  = {Yogesh Balaji and Seungjun Nah and Xun Huang and Arash Vahdat and Jiaming Song and Karsten Kreis and Miika Aittala and Timo Aila and Samuli Laine and Bryan Catanzaro and Tero Karras and Ming-Yu Liu},
     journal = {ArXiv},
     year    = {2022},
     volume  = {abs/2211.01324}
 }
 ```
+
+```bibtex
+@inproceedings{dao2022flashattention,
+    title   = {Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-Awareness},
+    author  = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+    booktitle = {Advances in Neural Information Processing Systems},
+    year    = {2022}
+}
+```
```

### Comparing `classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch/classifier_free_guidance_pytorch.py` & `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/classifier_free_guidance_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from beartype.typing import Callable, Tuple, Optional, List, Literal, Union
 from beartype.door import is_bearable
 
 from inspect import signature
 
 from classifier_free_guidance_pytorch.t5 import T5Adapter
 from classifier_free_guidance_pytorch.open_clip import OpenClipAdapter
+from classifier_free_guidance_pytorch.attend import Attend
 
 # constants
 
 COND_DROP_KEY_NAME = 'cond_drop_prob'
 
 TEXTS_KEY_NAME = 'texts'
 TEXT_EMBEDS_KEY_NAME = 'text_embeds'
@@ -134,26 +135,29 @@
     def __init__(
         self,
         dim,
         dim_head = 64,
         heads = 8,
         dim_context = None,
         norm_context = False,
-        num_null_kv = 0
+        num_null_kv = 0,
+        flash = False
     ):
         super().__init__()
         self.heads = heads
         self.scale = dim_head ** -0.5
         inner_dim = dim_head * heads
 
         dim_context = default(dim_context, dim)
 
         self.norm = nn.LayerNorm(dim)
         self.context_norm = nn.LayerNorm(dim_context) if norm_context else nn.Identity()
 
+        self.attend = Attend(flash = flash)        
+
         self.num_null_kv = num_null_kv
         self.null_kv = nn.Parameter(torch.randn(2, num_null_kv, dim_head))
 
         self.to_q = nn.Linear(dim, inner_dim, bias = False)
         self.to_kv = nn.Linear(dim_context, dim_head * 2, bias = False)
         self.to_out = nn.Linear(inner_dim, dim, bias = False)
 
@@ -175,28 +179,21 @@
         q, k, v = self.to_q(x), *self.to_kv(kv_input).chunk(2, dim = -1)
 
         if self.num_null_kv > 0:
             null_k, null_v = repeat(self.null_kv, 'kv n d -> kv b n d', b = b).unbind(dim = 0)
             k = torch.cat((null_k, k), dim = -2)
             v = torch.cat((null_v, v), dim = -2)
 
-        q = rearrange(q, 'b n (h d) -> b h n d', h = self.heads)
-
-        q = q * self.scale
-
-        sim = einsum('b h i d, b j d -> b h i j', q, k)
-
         if exists(mask):
             mask = F.pad(mask, (self.num_null_kv, 0), value = True)
             mask = rearrange(mask, 'b j -> b 1 1 j')
-            sim = sim.masked_fill(~mask, -torch.finfo(sim.dtype).max)
 
-        attn = sim.softmax(dim = -1)
+        q = rearrange(q, 'b n (h d) -> b h n d', h = self.heads)
 
-        out = einsum('b h i j, b j d -> b h i d', attn, v)
+        out = self.attend(q, k, v, mask = mask)
 
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
 # dimension adapters
 
 def rearrange_channel_last(fn):
@@ -246,24 +243,26 @@
 
 class CrossAttention(nn.Module):
     def __init__(
         self,
         dim,
         hidden_dim,
         heads = 8,
-        dim_head = 64
+        dim_head = 64,
+        flash = False
     ):
         super().__init__()
         self.attn = Attention(
             dim = hidden_dim,
             dim_context = dim,
             norm_context = True,
             num_null_kv = 1,
             dim_head = dim_head,
-            heads = heads
+            heads = heads,
+            flash = flash
         )
 
     def forward(
         self,
         condition,
         hiddens,
         mask = None
@@ -413,15 +412,16 @@
         hidden_dims: Tuple[int, ...],
         model_types = 't5',
         model_names = None,
         cond_drop_prob = 0.,
         hiddens_channel_first = True,
         dim_latent = None,
         attn_dim_head = 64,
-        attn_heads = 8
+        attn_heads = 8,
+        flash = True
     ):
         super().__init__()
         model_types = cast_tuple(model_types)
         model_names = cast_tuple(model_names, length = len(model_types))
 
         assert len(model_types) == len(model_names)
         assert all([model_type in MODEL_TYPES for model_type in model_types])
@@ -449,15 +449,15 @@
         self.hiddens_channel_first = cast_tuple(hiddens_channel_first, self.num_condition_fns) # whether hiddens to be conditioned is channel first or last
 
         assert len(self.hiddens_channel_first) == self.num_condition_fns
 
         self.cond_drop_prob = cond_drop_prob
 
         for hidden_dim in hidden_dims:
-            self.conditioners.append(CrossAttention(dim_latent, hidden_dim))
+            self.conditioners.append(CrossAttention(dim_latent, hidden_dim, flash = flash))
 
         self.register_buffer('_device_param', torch.tensor(0.), persistent = False)
 
     @property
     def device(self):
         return next(self.buffers()).device
```

### Comparing `classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch/data/bpe_simple_vocab_16e6.txt` & `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/data/bpe_simple_vocab_16e6.txt`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch/open_clip.py` & `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch/t5.py` & `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch/tokenizer.py` & `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/tokenizer.py`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch.egg-info/PKG-INFO` & `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classifier-free-guidance-pytorch
-Version: 0.1.4
+Version: 0.1.5
 Summary: Classifier Free Guidance - Pytorch
 Home-page: https://github.com/lucidrains/classifier-free-guidance-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,classifier free guidance,text conditioning and guidance
 Classifier: Development Status :: 4 - Beta
```

### Comparing `classifier-free-guidance-pytorch-0.1.4/classifier_free_guidance_pytorch.egg-info/SOURCES.txt` & `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 classifier_free_guidance_pytorch/__init__.py
+classifier_free_guidance_pytorch/attend.py
 classifier_free_guidance_pytorch/classifier_free_guidance_pytorch.py
 classifier_free_guidance_pytorch/open_clip.py
 classifier_free_guidance_pytorch/t5.py
 classifier_free_guidance_pytorch/tokenizer.py
 classifier_free_guidance_pytorch.egg-info/PKG-INFO
 classifier_free_guidance_pytorch.egg-info/SOURCES.txt
 classifier_free_guidance_pytorch.egg-info/dependency_links.txt
```

### Comparing `classifier-free-guidance-pytorch-0.1.4/setup.py` & `classifier-free-guidance-pytorch-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'classifier-free-guidance-pytorch',
   packages = find_packages(exclude=[]),
   include_package_data = True,
-  version = '0.1.4',
+  version = '0.1.5',
   license='MIT',
   description = 'Classifier Free Guidance - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/classifier-free-guidance-pytorch',
   keywords = [
```

