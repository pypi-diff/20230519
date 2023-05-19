# Comparing `tmp/vector_quantize_pytorch-1.4.1.tar.gz` & `tmp/vector_quantize_pytorch-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.4.1.tar", last modified: Sat May  6 16:42:47 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.5.0.tar", last modified: Fri May 19 21:30:17 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.4.1.tar` & `vector_quantize_pytorch-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:42:47.267129 vector_quantize_pytorch-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-06 16:42:34.000000 vector_quantize_pytorch-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-06 16:42:47.267129 vector_quantize_pytorch-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-06 16:42:34.000000 vector_quantize_pytorch-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:42:47.267129 vector_quantize_pytorch-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-06 16:42:34.000000 vector_quantize_pytorch-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:42:47.267129 vector_quantize_pytorch-1.4.1/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-06 16:42:34.000000 vector_quantize_pytorch-1.4.1/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-06 16:42:34.000000 vector_quantize_pytorch-1.4.1/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-06 16:42:34.000000 vector_quantize_pytorch-1.4.1/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-05-06 16:42:34.000000 vector_quantize_pytorch-1.4.1/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:42:47.267129 vector_quantize_pytorch-1.4.1/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-06 16:42:47.000000 vector_quantize_pytorch-1.4.1/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-06 16:42:47.000000 vector_quantize_pytorch-1.4.1/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:42:47.000000 vector_quantize_pytorch-1.4.1/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 16:42:47.000000 vector_quantize_pytorch-1.4.1/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-06 16:42:47.000000 vector_quantize_pytorch-1.4.1/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:17.043879 vector_quantize_pytorch-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-19 21:30:07.000000 vector_quantize_pytorch-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-19 21:30:17.043879 vector_quantize_pytorch-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-19 21:30:07.000000 vector_quantize_pytorch-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:30:17.043879 vector_quantize_pytorch-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-19 21:30:07.000000 vector_quantize_pytorch-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:17.043879 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-19 21:30:07.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-19 21:30:07.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-19 21:30:07.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23261 2023-05-19 21:30:07.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:17.043879 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-19 21:30:16.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-19 21:30:17.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:30:16.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-19 21:30:16.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 21:30:16.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.4.1/LICENSE` & `vector_quantize_pytorch-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.4.1/PKG-INFO` & `vector_quantize_pytorch-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.4.1
+Version: 1.5.0
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.4.1/README.md` & `vector_quantize_pytorch-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.4.1/setup.py` & `vector_quantize_pytorch-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.4.1',
+  version = '1.5.0',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.4.1/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.4.1/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.4.1/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,14 +354,15 @@
 
         self.sample_fn = sample_vectors_distributed if use_ddp and sync_kmeans else batched_sample_vectors
         self.kmeans_all_reduce_fn = distributed.all_reduce if use_ddp and sync_kmeans else noop
         self.all_reduce_fn = distributed.all_reduce if use_ddp else noop
 
         self.register_buffer('initted', torch.Tensor([not kmeans_init]))
         self.register_buffer('cluster_size', torch.zeros(num_codebooks, codebook_size))
+        self.register_buffer('embed_avg', embed.clone())
 
         self.learnable_codebook = learnable_codebook
         if learnable_codebook:
             self.embed = nn.Parameter(embed)
         else:
             self.register_buffer('embed', embed)
 
@@ -376,29 +377,31 @@
             self.kmeans_iters,
             use_cosine_sim = True,
             sample_fn = self.sample_fn,
             all_reduce_fn = self.kmeans_all_reduce_fn
         )
 
         self.embed.data.copy_(embed)
+        self.embed_avg.data.copy_(embed.clone())
         self.cluster_size.data.copy_(cluster_size)
         self.initted.data.copy_(torch.Tensor([True]))
 
     def replace(self, batch_samples, batch_mask):
         batch_samples = l2norm(batch_samples)
 
         for ind, (samples, mask) in enumerate(zip(batch_samples.unbind(dim = 0), batch_mask.unbind(dim = 0))):
             if not torch.any(mask):
                 continue
 
             sampled = self.sample_fn(rearrange(samples, '... -> 1 ...'), mask.sum().item())
             sampled = rearrange(sampled, '1 ... -> ...')
 
             self.embed.data[ind][mask] = sampled
-            self.cluster_size.data[ind][mask] = self.reset_cluster_size            
+            self.embed_avg.data[ind][mask] = sampled * self.reset_cluster_size
+            self.cluster_size.data[ind][mask] = self.reset_cluster_size
 
     def expire_codes_(self, batch_samples):
         if self.threshold_ema_dead_code == 0:
             return
 
         expired_codes = self.cluster_size < self.threshold_ema_dead_code
 
@@ -441,25 +444,30 @@
             self.cluster_size.data.lerp_(bins, 1 - self.decay)
 
             zero_mask = (bins == 0)
             bins = bins.masked_fill(zero_mask, 1.)
 
             embed_sum = einsum('h n d, h n c -> h c d', flatten, embed_onehot)
             self.all_reduce_fn(embed_sum)
+            self.embed_avg.data.lerp_(embed_sum, 1 - self.decay)
 
-            embed_normalized = embed_sum / rearrange(bins, '... -> ... 1')
+            cluster_size = laplace_smoothing(self.cluster_size, self.codebook_size, self.eps) * self.cluster_size.sum()
+
+            embed_normalized = self.embed_avg / rearrange(cluster_size, '... -> ... 1')
             embed_normalized = l2norm(embed_normalized)
 
             embed_normalized = torch.where(
                 rearrange(zero_mask, '... -> ... 1'),
                 embed,
                 embed_normalized
             )
 
             self.embed.data.lerp_(embed_normalized, 1 - self.decay)
+            self.embed.data.copy_(l2norm(self.embed))
+
             self.expire_codes_(x)
 
         if needs_codebook_dim:
             quantize, embed_ind = map(lambda t: rearrange(t, '1 ... -> ...'), (quantize, embed_ind))
 
         dist = unpack_one(dist, ps, 'h * d')
         return quantize, embed_ind, dist
```

### Comparing `vector_quantize_pytorch-1.4.1/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.5.0/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.4.1
+Version: 1.5.0
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

