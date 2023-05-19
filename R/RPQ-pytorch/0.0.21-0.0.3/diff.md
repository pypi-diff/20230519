# Comparing `tmp/RPQ-pytorch-0.0.21.tar.gz` & `tmp/RPQ-pytorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RPQ-pytorch-0.0.21.tar", last modified: Thu Dec 22 16:19:02 2022, max compression
+gzip compressed data, was "RPQ-pytorch-0.0.3.tar", last modified: Fri May 19 21:50:33 2023, max compression
```

## Comparing `RPQ-pytorch-0.0.21.tar` & `RPQ-pytorch-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 16:19:02.543703 RPQ-pytorch-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2022-12-22 16:18:51.000000 RPQ-pytorch-0.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2022-12-22 16:19:02.543703 RPQ-pytorch-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2022-12-22 16:18:51.000000 RPQ-pytorch-0.0.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 16:19:02.543703 RPQ-pytorch-0.0.21/RPQ_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2022-12-22 16:19:02.000000 RPQ-pytorch-0.0.21/RPQ_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      304 2022-12-22 16:19:02.000000 RPQ-pytorch-0.0.21/RPQ_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 16:19:02.000000 RPQ-pytorch-0.0.21/RPQ_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-22 16:19:02.000000 RPQ-pytorch-0.0.21/RPQ_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-22 16:19:02.000000 RPQ-pytorch-0.0.21/RPQ_pytorch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 16:19:02.543703 RPQ-pytorch-0.0.21/rpq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 16:18:51.000000 RPQ-pytorch-0.0.21/rpq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 16:19:02.543703 RPQ-pytorch-0.0.21/rpq/models/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-22 16:18:51.000000 RPQ-pytorch-0.0.21/rpq/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57589 2022-12-22 16:18:51.000000 RPQ-pytorch-0.0.21/rpq/models/rpqopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2022-12-22 16:18:51.000000 RPQ-pytorch-0.0.21/rpq/models/rpqvit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2022-12-22 16:18:51.000000 RPQ-pytorch-0.0.21/rpq/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2022-12-22 16:18:51.000000 RPQ-pytorch-0.0.21/rpq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-22 16:19:02.543703 RPQ-pytorch-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2022-12-22 16:18:51.000000 RPQ-pytorch-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:33.404658 RPQ-pytorch-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-05-19 21:50:33.404658 RPQ-pytorch-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:33.404658 RPQ-pytorch-0.0.3/RPQ_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-05-19 21:50:33.000000 RPQ-pytorch-0.0.3/RPQ_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-19 21:50:33.000000 RPQ-pytorch-0.0.3/RPQ_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:50:33.000000 RPQ-pytorch-0.0.3/RPQ_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-19 21:50:33.000000 RPQ-pytorch-0.0.3/RPQ_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-19 21:50:33.000000 RPQ-pytorch-0.0.3/RPQ_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:33.404658 RPQ-pytorch-0.0.3/rpq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/rpq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:33.404658 RPQ-pytorch-0.0.3/rpq/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/rpq/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57773 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/rpq/models/rpqopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/rpq/models/rpqvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/rpq/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/rpq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:50:33.404658 RPQ-pytorch-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/setup.py
```

### Comparing `RPQ-pytorch-0.0.21/LICENSE` & `RPQ-pytorch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `RPQ-pytorch-0.0.21/PKG-INFO` & `RPQ-pytorch-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RPQ-pytorch
-Version: 0.0.21
+Version: 0.0.3
 Summary: Reverse Product Quantization (RPQ) of weights to reduce static memory usage.
 Home-page: https://github.com/a-kore/RPQ-pytorch
 Author: Ali Kore
 Author-email: akore654@gmail.com
 License: MIT
 Keywords: artificial intelligence,AI,machine learning,deep learning,pytorch,quantization,product quantization,reverse product quantization,memory reduction
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RPQ-pytorch
 Reverse Product Quantization (RPQ) of weights to reduce static memory usage.
 
-![](https://github.com/a-kore/RPQ-pytorch/raw/main/assets/rpq_diagram.gif)
+![](assets/rpq_diagram.gif)
 
 <!-- Go into how the method works. -->
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Installation](#installation)
@@ -31,15 +31,15 @@
 
 ## Introduction
 
 [Product quantization](https://www.pinecone.io/learn/product-quantization/) is a method for reducing the memory requirements for vector similarity search.  It reduces the memory footprint by chunking the vectors into subvectors that are each compressed into a set of codebooks with 256 codes each.  This allows us to have a set of codes that can be represented by uint8 indices instead of the full vector representation.
 
 If we reverse this process, we can dynamically spawn a larger set of vectors from a much smaller set of codebooks containing sub-vectors and a set of randomized uint8 indices, rather than having to persistently hold a much larger set of vectors.  This can be used during the forward pass to expand/compile the weight just-in-time in order to perform the operations on the input.  
 
-This creates a state for a model where the weights are "dormant" and expanded to their active state just before use.  This plays very well with methods like **gradient checkpointing** (and inference, similarly) where we can unpack the weights again rather then storing them.
+This creates a state for a model where the weights are "dormant" and expanded to their active state just before use.  This plays very well with methods like **gradient checkpointing** (and inference, similarly) where we can unpack the weights again rather then storing them.  In other words, the weights are part of the dynamic computational graph and can be forgotten/unpacked whenever they are needed.
 
 However, this doesn't come for free, the indices inherit from a set of shared codebooks, so the larger the weights, the more likelihood that vectors generated will share sub-vectors.  This can be prevented by increasing the number of codebooks, but requires more testing to see what the minimum number of codebooks required for each implementation should be.
 
 For instance, in the [Usage](#usage) section we define an RPQOPT model(OPT variant w/ RPQ weights) where the number of codebooks is set to the number of heads.  This is chosen abitrarily, but works well since the `hidden_dim` must be divisible by `num_codebooks`. 
 
 The effect of having a set of entangled vectors is unknown and would require rigorous testing with standard benchmarks for comparison.  Intuitively, this would have a different outcome depending on the way the final weight structure is used.  For a vector quantization module, it could be advantageous to have codes be entangled to avoid the issue of "dead codes" and increase codebook utilization.
 
@@ -48,22 +48,36 @@
 
 ```bash
 pip install rpq-pytorch
 ```
 
 ## Usage
 
-### Layers
+#### Standalone Weights
+
+A standalone module `RPQWeight` is available as an `nn.Module` wrapper that intializes a set of dynamic PQ weight and returns the expanded set of weight vectors.
+
+```python
+from rpq.nn import RPQWeight
+
+w = RPQWeight(num_codebooks=72, codebook_dim=128, num_vectors=9216) 
+
+print(w.codebooks.shape, w.indices.shape) # torch.Size([72, 256, 128]) torch.Size([72, 9216])
+
+print(w().shape) # torch.Size([9216, 9216])
+```
+
+#### Layers
 
 A set of common layers are re-implemented with quantized weights.  It follows the same usage as `torch.nn` modules with an extra argument for the `num_codebooks` for each layer.  For each layer, the `out_features`/`num_embeddings` must be divisible by the `num_codebooks`.
 
 ```python
 from rpq.nn import RPQLinear
 
-layer = RPQLinear(in_features=1024, out_features=4096, num_codebooks=16)
+layer = RPQLinear(in_features=1024, out_features=1024, num_codebooks=16)
 
 x = torch.randn(1, 1, 1024) # (b, n, d)
 y = layer(x) # (1, 1, 4096)
 
 ```
 
 Layers implemented:
@@ -77,19 +91,19 @@
 - [ ] `RPQConvTranspose1d`
 - [ ] `RPQConv3d`
 - [ ] `RPQConvTranspose3d`
 - [ ] `RPQBilinear`
 
 *Note: `Embedding` layers are a lookup table and therefore very fast, as such the operation to expand the weights for `RPQEmbedding` adds a lot of time to the operation especially for a small number of tokens (10s of $\mu s$ -> 10s of ms).
 
-### Models
+#### Models
 
 Using the layer implementations, we can implement models via drop-in replacement of their static weight counterparts.
 
-#### RPQViT (ViT Giant)
+##### RPQViT (ViT Giant)
 
 ```python
 from vit_pytorch import ViT
 from rpq.models.rpqvit import RPQViT
 from rpq.utils import model_size
 
 # vit_giant_patch14_336
@@ -123,15 +137,15 @@
 ```
 ```
 model size: 2252.157MB
 model size: 361.429MB  
 ```
 Approximately ~6x reduction in model size.
 
-#### RPQOPT (opt-66b)
+##### RPQOPT (opt-66b)
 
 ```python
 
 import torch
 from transformers.models.opt.modeling_opt import OPTConfig
 from transformers import GPT2Tokenizer
 from rpq.models.rpqopt import RPQOPTModel
@@ -148,34 +162,40 @@
     outputs = rpq_model(**inputs)
 
 model_size(rpq_model)
 ```
 ```
 model size: 5885.707MB 
 ```
-This is an RPQOPT-66b initialized at float32 precision, a static weight version (standard OPT-66b) would be **264 GB** in size. This amount to approximately ~44x reduction in size.
+This is an RPQOPT-66b initialized at float32 precision, a static weight version (standard OPT-66b) would be **264 GB** in size. This amounts to approximately ~44x reduction in size.
 
 
 ## Benchmarks
 
 Due to the entanglement of the weight matrix arising as result of the inheritance from a shared set of codebooks, testing the RPQ model variants against the original methods would be important to characterize issues/tradeoffs with training stability, especially at scale.  Those tests will be displayed in the table below:
-
+<!-- 93.6 93.4 43.0 57.2 -->
 | Model | Config | Model Size | Dataset | Validation Accuracy | Epochs |
 | --- | --- | --- | --- | --- | -- |
+| ViT | vit_base_patch16_224 | 330MB | MNIST | TBD | 90 |
+| RPQViT | vit_base_patch16_224 | 88MB | MINST | TBD | 90 |
+| ViT | vit_base_patch16_224 | 330MB | CIFAR10 | TBD | 90 |
+| RPQViT | vit_base_patch16_224 | 88MB | CIFAR10 | TBD | 90 |
 | ViT | vit_base_patch16_224 | 330MB | Imagenet | TBD | 90 |
 | RPQViT | vit_base_patch16_224 | 88MB | Imagenet | TBD | 90 |
 
+
 ## TODO
 
 - [ ] Implement `RPQConv1d` layer
 - [ ] Implement `RPQConv2d` layer
 - [ ] Implement `RPQConv3d` layer
 - [ ] Implement `RPQConvTranspose1d` layer
 - [ ] Implement `RPQConvTranspose2d` layer
 - [ ] Implement `RPQConvTranspose3d` layer
 - [ ] Implement `RPQBilinear` layer
-- [ ] Perform More benchmarks with LLMs (BERT, OPT, etc.,)
+- [ ] Perform benchmarks with ViTs (ViT vs RPQViT)
+- [ ] Perform benchmarks with LLMs (BERT, OPT, etc.,)
 - [ ] Explore methods of conversion from pre-trained static weights to dynamic RPQ weights
```

### Comparing `RPQ-pytorch-0.0.21/README.md` & `RPQ-pytorch-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # RPQ-pytorch
 Reverse Product Quantization (RPQ) of weights to reduce static memory usage.
 
-![](https://github.com/a-kore/RPQ-pytorch/raw/main/assets/rpq_diagram.gif)
+![](assets/rpq_diagram.gif)
 
 <!-- Go into how the method works. -->
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Installation](#installation)
@@ -14,15 +14,15 @@
 
 ## Introduction
 
 [Product quantization](https://www.pinecone.io/learn/product-quantization/) is a method for reducing the memory requirements for vector similarity search.  It reduces the memory footprint by chunking the vectors into subvectors that are each compressed into a set of codebooks with 256 codes each.  This allows us to have a set of codes that can be represented by uint8 indices instead of the full vector representation.
 
 If we reverse this process, we can dynamically spawn a larger set of vectors from a much smaller set of codebooks containing sub-vectors and a set of randomized uint8 indices, rather than having to persistently hold a much larger set of vectors.  This can be used during the forward pass to expand/compile the weight just-in-time in order to perform the operations on the input.  
 
-This creates a state for a model where the weights are "dormant" and expanded to their active state just before use.  This plays very well with methods like **gradient checkpointing** (and inference, similarly) where we can unpack the weights again rather then storing them.
+This creates a state for a model where the weights are "dormant" and expanded to their active state just before use.  This plays very well with methods like **gradient checkpointing** (and inference, similarly) where we can unpack the weights again rather then storing them.  In other words, the weights are part of the dynamic computational graph and can be forgotten/unpacked whenever they are needed.
 
 However, this doesn't come for free, the indices inherit from a set of shared codebooks, so the larger the weights, the more likelihood that vectors generated will share sub-vectors.  This can be prevented by increasing the number of codebooks, but requires more testing to see what the minimum number of codebooks required for each implementation should be.
 
 For instance, in the [Usage](#usage) section we define an RPQOPT model(OPT variant w/ RPQ weights) where the number of codebooks is set to the number of heads.  This is chosen abitrarily, but works well since the `hidden_dim` must be divisible by `num_codebooks`. 
 
 The effect of having a set of entangled vectors is unknown and would require rigorous testing with standard benchmarks for comparison.  Intuitively, this would have a different outcome depending on the way the final weight structure is used.  For a vector quantization module, it could be advantageous to have codes be entangled to avoid the issue of "dead codes" and increase codebook utilization.
 
@@ -31,22 +31,36 @@
 
 ```bash
 pip install rpq-pytorch
 ```
 
 ## Usage
 
-### Layers
+#### Standalone Weights
+
+A standalone module `RPQWeight` is available as an `nn.Module` wrapper that intializes a set of dynamic PQ weight and returns the expanded set of weight vectors.
+
+```python
+from rpq.nn import RPQWeight
+
+w = RPQWeight(num_codebooks=72, codebook_dim=128, num_vectors=9216) 
+
+print(w.codebooks.shape, w.indices.shape) # torch.Size([72, 256, 128]) torch.Size([72, 9216])
+
+print(w().shape) # torch.Size([9216, 9216])
+```
+
+#### Layers
 
 A set of common layers are re-implemented with quantized weights.  It follows the same usage as `torch.nn` modules with an extra argument for the `num_codebooks` for each layer.  For each layer, the `out_features`/`num_embeddings` must be divisible by the `num_codebooks`.
 
 ```python
 from rpq.nn import RPQLinear
 
-layer = RPQLinear(in_features=1024, out_features=4096, num_codebooks=16)
+layer = RPQLinear(in_features=1024, out_features=1024, num_codebooks=16)
 
 x = torch.randn(1, 1, 1024) # (b, n, d)
 y = layer(x) # (1, 1, 4096)
 
 ```
 
 Layers implemented:
@@ -60,19 +74,19 @@
 - [ ] `RPQConvTranspose1d`
 - [ ] `RPQConv3d`
 - [ ] `RPQConvTranspose3d`
 - [ ] `RPQBilinear`
 
 *Note: `Embedding` layers are a lookup table and therefore very fast, as such the operation to expand the weights for `RPQEmbedding` adds a lot of time to the operation especially for a small number of tokens (10s of $\mu s$ -> 10s of ms).
 
-### Models
+#### Models
 
 Using the layer implementations, we can implement models via drop-in replacement of their static weight counterparts.
 
-#### RPQViT (ViT Giant)
+##### RPQViT (ViT Giant)
 
 ```python
 from vit_pytorch import ViT
 from rpq.models.rpqvit import RPQViT
 from rpq.utils import model_size
 
 # vit_giant_patch14_336
@@ -106,15 +120,15 @@
 ```
 ```
 model size: 2252.157MB
 model size: 361.429MB  
 ```
 Approximately ~6x reduction in model size.
 
-#### RPQOPT (opt-66b)
+##### RPQOPT (opt-66b)
 
 ```python
 
 import torch
 from transformers.models.opt.modeling_opt import OPTConfig
 from transformers import GPT2Tokenizer
 from rpq.models.rpqopt import RPQOPTModel
@@ -131,34 +145,40 @@
     outputs = rpq_model(**inputs)
 
 model_size(rpq_model)
 ```
 ```
 model size: 5885.707MB 
 ```
-This is an RPQOPT-66b initialized at float32 precision, a static weight version (standard OPT-66b) would be **264 GB** in size. This amount to approximately ~44x reduction in size.
+This is an RPQOPT-66b initialized at float32 precision, a static weight version (standard OPT-66b) would be **264 GB** in size. This amounts to approximately ~44x reduction in size.
 
 
 ## Benchmarks
 
 Due to the entanglement of the weight matrix arising as result of the inheritance from a shared set of codebooks, testing the RPQ model variants against the original methods would be important to characterize issues/tradeoffs with training stability, especially at scale.  Those tests will be displayed in the table below:
-
+<!-- 93.6 93.4 43.0 57.2 -->
 | Model | Config | Model Size | Dataset | Validation Accuracy | Epochs |
 | --- | --- | --- | --- | --- | -- |
+| ViT | vit_base_patch16_224 | 330MB | MNIST | TBD | 90 |
+| RPQViT | vit_base_patch16_224 | 88MB | MINST | TBD | 90 |
+| ViT | vit_base_patch16_224 | 330MB | CIFAR10 | TBD | 90 |
+| RPQViT | vit_base_patch16_224 | 88MB | CIFAR10 | TBD | 90 |
 | ViT | vit_base_patch16_224 | 330MB | Imagenet | TBD | 90 |
 | RPQViT | vit_base_patch16_224 | 88MB | Imagenet | TBD | 90 |
 
+
 ## TODO
 
 - [ ] Implement `RPQConv1d` layer
 - [ ] Implement `RPQConv2d` layer
 - [ ] Implement `RPQConv3d` layer
 - [ ] Implement `RPQConvTranspose1d` layer
 - [ ] Implement `RPQConvTranspose2d` layer
 - [ ] Implement `RPQConvTranspose3d` layer
 - [ ] Implement `RPQBilinear` layer
-- [ ] Perform More benchmarks with LLMs (BERT, OPT, etc.,)
+- [ ] Perform benchmarks with ViTs (ViT vs RPQViT)
+- [ ] Perform benchmarks with LLMs (BERT, OPT, etc.,)
 - [ ] Explore methods of conversion from pre-trained static weights to dynamic RPQ weights
```

### Comparing `RPQ-pytorch-0.0.21/RPQ_pytorch.egg-info/PKG-INFO` & `RPQ-pytorch-0.0.3/RPQ_pytorch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RPQ-pytorch
-Version: 0.0.21
+Version: 0.0.3
 Summary: Reverse Product Quantization (RPQ) of weights to reduce static memory usage.
 Home-page: https://github.com/a-kore/RPQ-pytorch
 Author: Ali Kore
 Author-email: akore654@gmail.com
 License: MIT
 Keywords: artificial intelligence,AI,machine learning,deep learning,pytorch,quantization,product quantization,reverse product quantization,memory reduction
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RPQ-pytorch
 Reverse Product Quantization (RPQ) of weights to reduce static memory usage.
 
-![](https://github.com/a-kore/RPQ-pytorch/raw/main/assets/rpq_diagram.gif)
+![](assets/rpq_diagram.gif)
 
 <!-- Go into how the method works. -->
 
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Installation](#installation)
@@ -31,15 +31,15 @@
 
 ## Introduction
 
 [Product quantization](https://www.pinecone.io/learn/product-quantization/) is a method for reducing the memory requirements for vector similarity search.  It reduces the memory footprint by chunking the vectors into subvectors that are each compressed into a set of codebooks with 256 codes each.  This allows us to have a set of codes that can be represented by uint8 indices instead of the full vector representation.
 
 If we reverse this process, we can dynamically spawn a larger set of vectors from a much smaller set of codebooks containing sub-vectors and a set of randomized uint8 indices, rather than having to persistently hold a much larger set of vectors.  This can be used during the forward pass to expand/compile the weight just-in-time in order to perform the operations on the input.  
 
-This creates a state for a model where the weights are "dormant" and expanded to their active state just before use.  This plays very well with methods like **gradient checkpointing** (and inference, similarly) where we can unpack the weights again rather then storing them.
+This creates a state for a model where the weights are "dormant" and expanded to their active state just before use.  This plays very well with methods like **gradient checkpointing** (and inference, similarly) where we can unpack the weights again rather then storing them.  In other words, the weights are part of the dynamic computational graph and can be forgotten/unpacked whenever they are needed.
 
 However, this doesn't come for free, the indices inherit from a set of shared codebooks, so the larger the weights, the more likelihood that vectors generated will share sub-vectors.  This can be prevented by increasing the number of codebooks, but requires more testing to see what the minimum number of codebooks required for each implementation should be.
 
 For instance, in the [Usage](#usage) section we define an RPQOPT model(OPT variant w/ RPQ weights) where the number of codebooks is set to the number of heads.  This is chosen abitrarily, but works well since the `hidden_dim` must be divisible by `num_codebooks`. 
 
 The effect of having a set of entangled vectors is unknown and would require rigorous testing with standard benchmarks for comparison.  Intuitively, this would have a different outcome depending on the way the final weight structure is used.  For a vector quantization module, it could be advantageous to have codes be entangled to avoid the issue of "dead codes" and increase codebook utilization.
 
@@ -48,22 +48,36 @@
 
 ```bash
 pip install rpq-pytorch
 ```
 
 ## Usage
 
-### Layers
+#### Standalone Weights
+
+A standalone module `RPQWeight` is available as an `nn.Module` wrapper that intializes a set of dynamic PQ weight and returns the expanded set of weight vectors.
+
+```python
+from rpq.nn import RPQWeight
+
+w = RPQWeight(num_codebooks=72, codebook_dim=128, num_vectors=9216) 
+
+print(w.codebooks.shape, w.indices.shape) # torch.Size([72, 256, 128]) torch.Size([72, 9216])
+
+print(w().shape) # torch.Size([9216, 9216])
+```
+
+#### Layers
 
 A set of common layers are re-implemented with quantized weights.  It follows the same usage as `torch.nn` modules with an extra argument for the `num_codebooks` for each layer.  For each layer, the `out_features`/`num_embeddings` must be divisible by the `num_codebooks`.
 
 ```python
 from rpq.nn import RPQLinear
 
-layer = RPQLinear(in_features=1024, out_features=4096, num_codebooks=16)
+layer = RPQLinear(in_features=1024, out_features=1024, num_codebooks=16)
 
 x = torch.randn(1, 1, 1024) # (b, n, d)
 y = layer(x) # (1, 1, 4096)
 
 ```
 
 Layers implemented:
@@ -77,19 +91,19 @@
 - [ ] `RPQConvTranspose1d`
 - [ ] `RPQConv3d`
 - [ ] `RPQConvTranspose3d`
 - [ ] `RPQBilinear`
 
 *Note: `Embedding` layers are a lookup table and therefore very fast, as such the operation to expand the weights for `RPQEmbedding` adds a lot of time to the operation especially for a small number of tokens (10s of $\mu s$ -> 10s of ms).
 
-### Models
+#### Models
 
 Using the layer implementations, we can implement models via drop-in replacement of their static weight counterparts.
 
-#### RPQViT (ViT Giant)
+##### RPQViT (ViT Giant)
 
 ```python
 from vit_pytorch import ViT
 from rpq.models.rpqvit import RPQViT
 from rpq.utils import model_size
 
 # vit_giant_patch14_336
@@ -123,15 +137,15 @@
 ```
 ```
 model size: 2252.157MB
 model size: 361.429MB  
 ```
 Approximately ~6x reduction in model size.
 
-#### RPQOPT (opt-66b)
+##### RPQOPT (opt-66b)
 
 ```python
 
 import torch
 from transformers.models.opt.modeling_opt import OPTConfig
 from transformers import GPT2Tokenizer
 from rpq.models.rpqopt import RPQOPTModel
@@ -148,34 +162,40 @@
     outputs = rpq_model(**inputs)
 
 model_size(rpq_model)
 ```
 ```
 model size: 5885.707MB 
 ```
-This is an RPQOPT-66b initialized at float32 precision, a static weight version (standard OPT-66b) would be **264 GB** in size. This amount to approximately ~44x reduction in size.
+This is an RPQOPT-66b initialized at float32 precision, a static weight version (standard OPT-66b) would be **264 GB** in size. This amounts to approximately ~44x reduction in size.
 
 
 ## Benchmarks
 
 Due to the entanglement of the weight matrix arising as result of the inheritance from a shared set of codebooks, testing the RPQ model variants against the original methods would be important to characterize issues/tradeoffs with training stability, especially at scale.  Those tests will be displayed in the table below:
-
+<!-- 93.6 93.4 43.0 57.2 -->
 | Model | Config | Model Size | Dataset | Validation Accuracy | Epochs |
 | --- | --- | --- | --- | --- | -- |
+| ViT | vit_base_patch16_224 | 330MB | MNIST | TBD | 90 |
+| RPQViT | vit_base_patch16_224 | 88MB | MINST | TBD | 90 |
+| ViT | vit_base_patch16_224 | 330MB | CIFAR10 | TBD | 90 |
+| RPQViT | vit_base_patch16_224 | 88MB | CIFAR10 | TBD | 90 |
 | ViT | vit_base_patch16_224 | 330MB | Imagenet | TBD | 90 |
 | RPQViT | vit_base_patch16_224 | 88MB | Imagenet | TBD | 90 |
 
+
 ## TODO
 
 - [ ] Implement `RPQConv1d` layer
 - [ ] Implement `RPQConv2d` layer
 - [ ] Implement `RPQConv3d` layer
 - [ ] Implement `RPQConvTranspose1d` layer
 - [ ] Implement `RPQConvTranspose2d` layer
 - [ ] Implement `RPQConvTranspose3d` layer
 - [ ] Implement `RPQBilinear` layer
-- [ ] Perform More benchmarks with LLMs (BERT, OPT, etc.,)
+- [ ] Perform benchmarks with ViTs (ViT vs RPQViT)
+- [ ] Perform benchmarks with LLMs (BERT, OPT, etc.,)
 - [ ] Explore methods of conversion from pre-trained static weights to dynamic RPQ weights
```

### Comparing `RPQ-pytorch-0.0.21/rpq/models/rpqopt.py` & `RPQ-pytorch-0.0.3/rpq/models/rpqopt.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,16 +286,16 @@
         self.do_layer_norm_before = config.do_layer_norm_before
         self.dropout = config.dropout
         self.activation_fn = ACT2FN[config.activation_function]
 
         self.self_attn_layer_norm = nn.LayerNorm(
             self.embed_dim, elementwise_affine=config.layer_norm_elementwise_affine
         )
-        self.fc1 = RPQLinear(self.embed_dim, config.ffn_dim, config.num_attention_heads*(config.ffn_dim//self.embed_dim), bias=config.enable_bias)
-        self.fc2 = RPQLinear(config.ffn_dim, self.embed_dim, config.num_attention_heads, bias=config.enable_bias)
+        self.fc1 = RPQLinear(self.embed_dim, config.ffn_dim, config.num_attention_heads, bias=config.enable_bias)
+        self.fc2 = RPQLinear(config.ffn_dim, self.embed_dim, config.num_attention_heads*(config.ffn_dim//self.embed_dim), bias=config.enable_bias)
         self.final_layer_norm = nn.LayerNorm(self.embed_dim, elementwise_affine=config.layer_norm_elementwise_affine)
 
     def forward(
         self,
         hidden_states: torch.Tensor,
         attention_mask: Optional[torch.Tensor] = None,
         layer_head_mask: Optional[torch.Tensor] = None,
@@ -403,14 +403,18 @@
 
     def _init_weights(self, module):
         std = self.config.init_std
         if isinstance(module, RPQLinear):
             module.codebooks.data.normal_(mean=0.0, std=std)
             if module.bias is not None:
                 module.bias.data.zero_()
+        elif isinstance (module, nn.Linear):
+            module.weight.data.normal_(mean=0.0, std=std)
+            if module.bias is not None:
+                module.bias.data.zero_()
         elif isinstance(module, RPQEmbedding):
             module.codebooks.data.normal_(mean=0.0, std=std)
             if module.padding_idx is not None:
                 module.get_weight().data[module.padding_idx].zero_()
 
     def _set_gradient_checkpointing(self, module, value=False):
         if isinstance(module, (RPQOPTDecoder)):
```

### Comparing `RPQ-pytorch-0.0.21/rpq/models/rpqvit.py` & `RPQ-pytorch-0.0.3/rpq/models/rpqvit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
-Implementation of ViT model with standard modules replaced with their RPQ counterparts.
+Implementation of ViT model with standard linear modules replaced with their RPQ counterparts.
 
 This is a modified version of the ViT model from the https://github.com/lucidrains/vit-pytorch repository.
 """
 import torch
 from torch import nn
 from einops import rearrange, repeat
 from einops.layers.torch import Rearrange
 from torch.nn.modules.utils import _pair
 from rpq.nn import RPQLinear
-from functools import partial
 
 
 class PreNorm(nn.Module):
     def __init__(self, dim, fn):
         super().__init__()
         self.norm = nn.LayerNorm(dim)
         self.fn = fn
@@ -23,15 +22,15 @@
 class FeedForward(nn.Module):
     def __init__(self, dim, hidden_dim, num_codebooks, dropout = 0.):
         super().__init__()
         self.net = nn.Sequential(
             RPQLinear(dim, hidden_dim, num_codebooks),
             nn.GELU(),
             nn.Dropout(dropout),
-            RPQLinear(hidden_dim, dim, num_codebooks),
+            RPQLinear(hidden_dim, dim, (hidden_dim//dim)*num_codebooks),
             nn.Dropout(dropout)
         )
     def forward(self, x):
         return self.net(x)
 
 class Attention(nn.Module):
     def __init__(self, dim, heads = 8, dim_head = 64, dropout = 0.):
@@ -41,15 +40,15 @@
 
         self.heads = heads
         self.scale = dim_head ** -0.5
 
         self.attend = nn.Softmax(dim = -1)
         self.dropout = nn.Dropout(dropout)
 
-        self.to_qkv = RPQLinear(dim, inner_dim * 3, heads * 3, bias = False)
+        self.to_qkv = RPQLinear(dim, inner_dim * 3, heads, bias = False)
 
         self.to_out = nn.Sequential(
             RPQLinear(inner_dim, dim, heads),
             nn.Dropout(dropout)
         ) if project_out else nn.Identity()
 
     def forward(self, x):
@@ -90,15 +89,15 @@
 
         num_patches = (image_height // patch_height) * (image_width // patch_width)
         patch_dim = channels * patch_height * patch_width
         assert pool in {'cls', 'mean'}, 'pool type must be either cls (cls token) or mean (mean pooling)'
 
         self.to_patch_embedding = nn.Sequential(
             Rearrange('b c (h p1) (w p2) -> b (h w) (p1 p2 c)', p1 = patch_height, p2 = patch_width),
-            RPQLinear(patch_dim, dim, num_codebooks = heads * (dim//patch_dim)),
+            nn.Linear(patch_dim, dim),
         )
 
         self.pos_embedding = nn.Parameter(torch.randn(1, num_patches + 1, dim))
         self.cls_token = nn.Parameter(torch.randn(1, 1, dim))
         self.dropout = nn.Dropout(emb_dropout)
 
         self.transformer = Transformer(dim, depth, heads, dim_head, mlp_dim, dropout)
```

### Comparing `RPQ-pytorch-0.0.21/setup.py` & `RPQ-pytorch-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'RPQ-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.21',
+  version = '0.0.3',
   license='MIT',
   description = 'Reverse Product Quantization (RPQ) of weights to reduce static memory usage.',
   author = 'Ali Kore',
   author_email = 'akore654@gmail.com',
   long_description=open('README.md', 'r').read(),
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/a-kore/RPQ-pytorch',
@@ -23,14 +23,15 @@
     'memory reduction',
   ],
   install_requires=[
     'torch>=1.6',
     'einops>=0.6',
     'transformers>=4.0',
     'vit-pytorch>=0.40',
+    'routing-transformer>=1.6',
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.10',
```

