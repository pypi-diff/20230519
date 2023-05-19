# Comparing `tmp/vector_quantize_pytorch-1.5.0.tar.gz` & `tmp/vector_quantize_pytorch-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.5.0.tar", last modified: Fri May 19 21:30:17 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.5.1.tar", last modified: Fri May 19 21:39:41 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.5.0.tar` & `vector_quantize_pytorch-1.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:17.043879 vector_quantize_pytorch-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-19 21:30:07.000000 vector_quantize_pytorch-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-19 21:30:17.043879 vector_quantize_pytorch-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-19 21:30:07.000000 vector_quantize_pytorch-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:30:17.043879 vector_quantize_pytorch-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-19 21:30:07.000000 vector_quantize_pytorch-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:17.043879 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-19 21:30:07.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-19 21:30:07.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-19 21:30:07.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    23261 2023-05-19 21:30:07.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:30:17.043879 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-19 21:30:16.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-19 21:30:17.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:30:16.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-19 21:30:16.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 21:30:16.000000 vector_quantize_pytorch-1.5.0/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:39:41.737601 vector_quantize_pytorch-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-19 21:39:26.000000 vector_quantize_pytorch-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-19 21:39:41.737601 vector_quantize_pytorch-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-19 21:39:26.000000 vector_quantize_pytorch-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:39:41.737601 vector_quantize_pytorch-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-19 21:39:26.000000 vector_quantize_pytorch-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:39:41.737601 vector_quantize_pytorch-1.5.1/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-19 21:39:26.000000 vector_quantize_pytorch-1.5.1/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-19 21:39:26.000000 vector_quantize_pytorch-1.5.1/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-19 21:39:26.000000 vector_quantize_pytorch-1.5.1/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23362 2023-05-19 21:39:26.000000 vector_quantize_pytorch-1.5.1/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:39:41.737601 vector_quantize_pytorch-1.5.1/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-19 21:39:41.000000 vector_quantize_pytorch-1.5.1/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-19 21:39:41.000000 vector_quantize_pytorch-1.5.1/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:39:41.000000 vector_quantize_pytorch-1.5.1/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-19 21:39:41.000000 vector_quantize_pytorch-1.5.1/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 21:39:41.000000 vector_quantize_pytorch-1.5.1/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.5.0/LICENSE` & `vector_quantize_pytorch-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.0/PKG-INFO` & `vector_quantize_pytorch-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.5.0
+Version: 1.5.1
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.5.0/README.md` & `vector_quantize_pytorch-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.0/setup.py` & `vector_quantize_pytorch-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.5.0',
+  version = '1.5.1',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.5.1/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.5.1/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.5.0/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.5.1/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,16 +39,17 @@
 
 def gumbel_sample(t, temperature = 1., dim = -1):
     if temperature == 0:
         return t.argmax(dim = dim)
 
     return ((t / temperature) + gumbel_noise(t)).argmax(dim = dim)
 
-def laplace_smoothing(x, n_categories, eps = 1e-5):
-    return (x + eps) / (x.sum() + n_categories * eps)
+def laplace_smoothing(x, n_categories, eps = 1e-5, dim = -1):
+    denom = x.sum(dim = dim, keepdim = True)
+    return (x + eps) / (denom + n_categories * eps)
 
 def sample_vectors(samples, num):
     num_samples, device = samples.shape[0], samples.device
     if num_samples >= num:
         indices = torch.randperm(num_samples, device = device)[:num]
     else:
         indices = torch.randint(0, num_samples, (num,), device = device)
@@ -301,15 +302,15 @@
             self.all_reduce_fn(cluster_size)
             self.cluster_size.data.lerp_(cluster_size, 1 - self.decay)
 
             embed_sum = einsum('h n d, h n c -> h c d', flatten, embed_onehot)
             self.all_reduce_fn(embed_sum.contiguous())
             self.embed_avg.data.lerp_(embed_sum, 1 - self.decay)
 
-            cluster_size = laplace_smoothing(self.cluster_size, self.codebook_size, self.eps) * self.cluster_size.sum()
+            cluster_size = laplace_smoothing(self.cluster_size, self.codebook_size, self.eps) * self.cluster_size.sum(dim = -1, keepdim = True)
 
             embed_normalized = self.embed_avg / rearrange(cluster_size, '... -> ... 1')
             self.embed.data.copy_(embed_normalized)
             self.expire_codes_(x)
 
         if needs_codebook_dim:
             quantize, embed_ind = map(lambda t: rearrange(t, '1 ... -> ...'), (quantize, embed_ind))
@@ -446,15 +447,15 @@
             zero_mask = (bins == 0)
             bins = bins.masked_fill(zero_mask, 1.)
 
             embed_sum = einsum('h n d, h n c -> h c d', flatten, embed_onehot)
             self.all_reduce_fn(embed_sum)
             self.embed_avg.data.lerp_(embed_sum, 1 - self.decay)
 
-            cluster_size = laplace_smoothing(self.cluster_size, self.codebook_size, self.eps) * self.cluster_size.sum()
+            cluster_size = laplace_smoothing(self.cluster_size, self.codebook_size, self.eps) * self.cluster_size.sum(dim = -1, keepdim = True)
 
             embed_normalized = self.embed_avg / rearrange(cluster_size, '... -> ... 1')
             embed_normalized = l2norm(embed_normalized)
 
             embed_normalized = torch.where(
                 rearrange(zero_mask, '... -> ... 1'),
                 embed,
```

### Comparing `vector_quantize_pytorch-1.5.0/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.5.1/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.5.0
+Version: 1.5.1
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

