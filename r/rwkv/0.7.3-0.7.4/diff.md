# Comparing `tmp/rwkv-0.7.3.tar.gz` & `tmp/rwkv-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwkv-0.7.3.tar", last modified: Tue Apr  4 01:55:06 2023, max compression
+gzip compressed data, was "rwkv-0.7.4.tar", last modified: Fri May 19 16:15:22 2023, max compression
```

## Comparing `rwkv-0.7.3.tar` & `rwkv-0.7.4.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-04-04 01:55:06.000000 rwkv-0.7.3/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    11357 2023-03-01 07:25:16.000000 rwkv-0.7.3/LICENSE
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       24 2023-03-01 07:52:12.000000 rwkv-0.7.3/MANIFEST.in
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4770 2023-04-04 01:55:06.000000 rwkv-0.7.3/PKG-INFO
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4300 2023-03-18 18:39:01.000000 rwkv-0.7.3/README.md
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      499 2023-04-04 01:46:44.000000 rwkv-0.7.3/pyproject.toml
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       38 2023-04-04 01:55:06.000000 rwkv-0.7.3/setup.cfg
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-04-04 01:55:05.000000 rwkv-0.7.3/src/
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-04-04 01:55:06.000000 rwkv-0.7.3/src/rwkv/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-02-28 12:56:58.000000 rwkv-0.7.3/src/rwkv/__init__.py
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-04-04 01:55:06.000000 rwkv-0.7.3/src/rwkv/cuda/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5001 2023-03-22 08:26:52.000000 rwkv-0.7.3/src/rwkv/cuda/operators.cu
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     2955 2023-04-04 01:45:51.000000 rwkv-0.7.3/src/rwkv/cuda/wrapper.cpp
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    32491 2023-03-30 08:32:56.000000 rwkv-0.7.3/src/rwkv/model.py
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4850 2023-03-22 08:27:06.000000 rwkv-0.7.3/src/rwkv/utils.py
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-04-04 01:55:06.000000 rwkv-0.7.3/src/rwkv.egg-info/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4770 2023-04-04 01:55:05.000000 rwkv-0.7.3/src/rwkv.egg-info/PKG-INFO
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      313 2023-04-04 01:55:05.000000 rwkv-0.7.3/src/rwkv.egg-info/SOURCES.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        1 2023-04-04 01:55:05.000000 rwkv-0.7.3/src/rwkv.egg-info/dependency_links.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       19 2023-04-04 01:55:05.000000 rwkv-0.7.3/src/rwkv.egg-info/requires.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        5 2023-04-04 01:55:05.000000 rwkv-0.7.3/src/rwkv.egg-info/top_level.txt
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-05-19 16:15:22.000000 rwkv-0.7.4/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    11357 2023-03-01 07:25:16.000000 rwkv-0.7.4/LICENSE
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       47 2023-05-19 16:15:03.000000 rwkv-0.7.4/MANIFEST.in
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4770 2023-05-19 16:15:22.000000 rwkv-0.7.4/PKG-INFO
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4300 2023-03-18 18:39:01.000000 rwkv-0.7.4/README.md
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      499 2023-05-19 16:11:03.000000 rwkv-0.7.4/pyproject.toml
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       38 2023-05-19 16:15:22.000000 rwkv-0.7.4/setup.cfg
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-05-19 16:15:22.000000 rwkv-0.7.4/src/
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-05-19 16:15:22.000000 rwkv-0.7.4/src/rwkv/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-02-28 12:56:58.000000 rwkv-0.7.4/src/rwkv/__init__.py
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-05-19 16:15:22.000000 rwkv-0.7.4/src/rwkv/cuda/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     8677 2023-04-27 19:18:02.000000 rwkv-0.7.4/src/rwkv/cuda/operators.cu
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4702 2023-04-27 19:18:02.000000 rwkv-0.7.4/src/rwkv/cuda/wrapper.cpp
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    33248 2023-04-27 19:18:02.000000 rwkv-0.7.4/src/rwkv/model.py
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3224 2023-05-19 10:04:58.000000 rwkv-0.7.4/src/rwkv/rwkv_tokenizer.py
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)  1093733 2023-05-18 04:00:58.000000 rwkv-0.7.4/src/rwkv/rwkv_vocab_v20230424.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5141 2023-05-19 16:11:52.000000 rwkv-0.7.4/src/rwkv/utils.py
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-05-19 16:15:22.000000 rwkv-0.7.4/src/rwkv.egg-info/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4770 2023-05-19 16:15:22.000000 rwkv-0.7.4/src/rwkv.egg-info/PKG-INFO
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      374 2023-05-19 16:15:22.000000 rwkv-0.7.4/src/rwkv.egg-info/SOURCES.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        1 2023-05-19 16:15:22.000000 rwkv-0.7.4/src/rwkv.egg-info/dependency_links.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       19 2023-05-19 16:15:22.000000 rwkv-0.7.4/src/rwkv.egg-info/requires.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        5 2023-05-19 16:15:22.000000 rwkv-0.7.4/src/rwkv.egg-info/top_level.txt
```

### Comparing `rwkv-0.7.3/LICENSE` & `rwkv-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rwkv-0.7.3/PKG-INFO` & `rwkv-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv
-Version: 0.7.3
+Version: 0.7.4
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `rwkv-0.7.3/README.md` & `rwkv-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `rwkv-0.7.3/src/rwkv/model.py` & `rwkv-0.7.4/src/rwkv/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,44 +32,47 @@
         verbose=True,
         extra_cuda_cflags=["-t 4", "-std=c++17", "--use_fast_math", "-O3", "--extra-device-vectorization"],
         is_python_module=False)
 
     @MyStatic
     def cuda_wkv(T: int, C: int, w, u, k, v, aa, bb, pp):
         assert 1 * C % min(C, 32) == 0
-        assert k.dtype == torch.float16
+        assert k.dtype == v.dtype == torch.float16 or k.dtype == v.dtype == torch.float32
+        assert w.dtype == u.dtype == aa.dtype == bb.dtype == pp.dtype == torch.float32
         w = w.contiguous()
         u = u.contiguous()
         k = k.contiguous()
         v = v.contiguous()
-        y = torch.empty((T, C), device=w.device, memory_format=torch.contiguous_format, dtype=torch.float16)
+        y = torch.empty((T, C), device=w.device, memory_format=torch.contiguous_format, dtype=k.dtype)
         torch.ops.rwkv.wkv_forward(1, T, C, w, u, k, v, y, aa, bb, pp)
         return y, aa, bb, pp
     @MyStatic
     def cuda_mm8_seq(B: int, N: int, M: int, x, w, mx, rx, my, ry):
-        assert x.dtype == mx.dtype == rx.dtype == my.dtype == ry.dtype == torch.float16
+        assert x.dtype == mx.dtype == rx.dtype == my.dtype == ry.dtype
+        assert x.dtype == torch.float32 or x.dtype == torch.float16
         assert w.dtype == torch.uint8
         assert x.shape == [B, N]
         assert w.shape == [N, M]
         assert rx.shape == mx.shape == [M]
         assert ry.shape == my.shape == [N, 1]
-        y = torch.empty((B, M), device=w.device, dtype=torch.float16)
+        y = torch.empty((B, M), device=w.device, dtype=x.dtype)
         torch.ops.rwkv.mm8_seq(B, N, M, x, w, mx, rx, my, ry, y)
         return y
     @MyStatic
     def cuda_mm8_one(N: int, M: int, x, w, mx, rx, my, ry):
-        assert x.dtype == mx.dtype == rx.dtype == my.dtype == ry.dtype == torch.float16
+        assert x.dtype == mx.dtype == rx.dtype == my.dtype == ry.dtype
+        assert x.dtype == torch.float32 or x.dtype == torch.float16
         assert w.dtype == torch.uint8
         assert x.shape == [N]
         assert w.shape == [N, M]
         assert rx.shape == mx.shape == [M]
         assert ry.shape == my.shape == [N, 1]
         y = torch.zeros((M,), device=w.device, dtype=torch.float32)
         torch.ops.rwkv.mm8_one(N, M, x, w, mx, rx, my, ry, y)
-        return y.to(dtype=torch.float16)
+        return y.to(dtype=x.dtype)
 else:
     os.environ["RWKV_CUDA_ON"] = '0'
 
 ########################################################################################################
 
 class RWKV(MyModule):
     def __init__(self, model, strategy, verbose = True, convert_and_save_and_exit = None):
@@ -313,31 +316,44 @@
                 prxxx(f'Converted and saved. Now this will exit.')
                 exit(0)
             
             gc.collect()
             if 'cuda' in args.strategy_string:
                 torch.cuda.empty_cache()
 
+    @MyFunction
+    def torch_mm8_seq(self, x, w, mx, rx, my, ry):
+        return x @ ((w.to(dtype=x.dtype) + 0.5) * ry * rx + my + mx)
+
+    @MyFunction
+    def torch_mm8_one(self, x, w, mx, rx, my, ry):
+        return x @ ((w.to(dtype=x.dtype) + 0.5) * ry * rx + my + mx)
+
     if os.environ.get('RWKV_CUDA_ON') == '1':
         @MyFunction
         def mm8_seq(self, x, w, mx, rx, my, ry):
-            B, N, M = x.shape[0], w.shape[0], w.shape[1]
-            return cuda_mm8_seq(B, N, M, x, w, mx, rx, my, ry)
+            if w.device.type == 'cuda' and x.dtype == torch.float16:
+                B, N, M = x.shape[0], w.shape[0], w.shape[1]
+                return cuda_mm8_seq(B, N, M, x, w, mx, rx, my, ry)
+            else:
+                return self.torch_mm8_seq(x, w, mx, rx, my, ry)
         @MyFunction
         def mm8_one(self, x, w, mx, rx, my, ry):
-            N, M = w.shape[0], w.shape[1]
-            return cuda_mm8_one(N, M, x, w, mx, rx, my, ry)
+            if w.device.type == 'cuda':
+                N, M = w.shape[0], w.shape[1]
+                return cuda_mm8_one(N, M, x, w, mx, rx, my, ry)
+            else:
+                return self.torch_mm8_one(x, w, mx, rx, my, ry)
     else:
         @MyFunction
         def mm8_seq(self, x, w, mx, rx, my, ry):
-            return x @ ((w.to(dtype=x.dtype) + 0.5) * ry * rx + my + mx)
-
+            return self.torch_mm8_seq(x, w, mx, rx, my, ry)
         @MyFunction
         def mm8_one(self, x, w, mx, rx, my, ry):
-            return x @ ((w.to(dtype=x.dtype) + 0.5) * ry * rx + my + mx)
+            return self.torch_mm8_one(x, w, mx, rx, my, ry)
 
     ########################################################################################################
 
     @MyFunction
     def ffn_one(self, x, sx, ln_w, ln_b, k_mix, r_mix, kw, vw, rw, kmx, krx, kmy, kry, vmx, vrx, vmy, vry, rmx, rrx, rmy, rry):
         xx = F.layer_norm(x, (x.shape[-1],), weight=ln_w, bias=ln_b)
         kx = xx * k_mix + sx * (1 - k_mix)
```

### Comparing `rwkv-0.7.3/src/rwkv/utils.py` & `rwkv-0.7.4/src/rwkv/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ########################################################################################################
 # The RWKV Language Model - https://github.com/BlinkDL/RWKV-LM
 ########################################################################################################
 
-import json, time, random, os
+import os, sys
 import numpy as np
 import torch
 from torch.nn import functional as F
 
 class PIPELINE_ARGS():
     def __init__(self, temperature=1.0, top_p=0.85, top_k=0, alpha_frequency=0.2, alpha_presence=0.2, token_ban=[], token_stop=[], chunk_len=256):
         self.temperature = temperature
@@ -20,14 +20,18 @@
 
 class PIPELINE():
     def __init__(self, model, WORD_NAME):
         self.model = model
         if WORD_NAME == 'cl100k_base':
             import tiktoken
             self.tokenizer = tiktoken.get_encoding(WORD_NAME)
+        elif WORD_NAME == 'rwkv_vocab_v20230424':
+            sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
+            from rwkv_tokenizer import TRIE_TOKENIZER
+            self.tokenizer = TRIE_TOKENIZER(os.path.dirname(os.path.abspath(__file__)) + '/rwkv_vocab_v20230424.txt')        
         else:
             from tokenizers import Tokenizer
             self.tokenizer = Tokenizer.from_file(WORD_NAME)
 
     def refine_context(self, context):
         context = context.strip().split('\n')
         for c in range(len(context)):
@@ -35,18 +39,18 @@
         context = list(filter(lambda c: c != '', context))
         context = '\n' + ('\n'.join(context)).strip()
         if context == '':
             context = '\n'
         return context
 
     def encode(self, x):
-        if 'tiktoken' in str(type(self.tokenizer)):
-            return self.tokenizer.encode(x)
-        else:
+        if 'Tokenizer' in str(type(self.tokenizer)):
             return self.tokenizer.encode(x).ids
+        else:
+            return self.tokenizer.encode(x)
     
     def decode(self, x):
         return self.tokenizer.decode(x)
 
     def sample_logits(self, logits, temperature=1.0, top_p=0.85, top_k=0):
         probs = F.softmax(logits.float(), dim=-1)
         top_k = int(top_k)
```

### Comparing `rwkv-0.7.3/src/rwkv.egg-info/PKG-INFO` & `rwkv-0.7.4/src/rwkv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv
-Version: 0.7.3
+Version: 0.7.4
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

