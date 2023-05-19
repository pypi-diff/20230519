# Comparing `tmp/pytorch_optimizer-2.9.0.tar.gz` & `tmp/pytorch_optimizer-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_optimizer-2.9.0.tar", max compression
+gzip compressed data, was "pytorch_optimizer-2.9.1.tar", max compression
```

## Comparing `pytorch_optimizer-2.9.0.tar` & `pytorch_optimizer-2.9.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    11357 2023-05-06 08:07:56.335615 pytorch_optimizer-2.9.0/LICENSE
--rw-r--r--   0        0        0    60156 2023-05-06 08:07:56.335615 pytorch_optimizer-2.9.0/README.rst
--rw-r--r--   0        0        0     4383 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pyproject.toml
--rw-r--r--   0        0        0     7354 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/base/__init__.py
--rw-r--r--   0        0        0     1583 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/base/exception.py
--rw-r--r--   0        0        0     6913 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/base/optimizer.py
--rw-r--r--   0        0        0     2761 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/base/scheduler.py
--rw-r--r--   0        0        0      491 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/base/types.py
--rw-r--r--   0        0        0      131 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/__init__.py
--rw-r--r--   0        0        0      971 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/chebyshev.py
--rw-r--r--   0        0        0     4034 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py
--rw-r--r--   0        0        0        0 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/experimental/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/experimental/deberta_v3_lr_scheduler.py
--rw-r--r--   0        0        0     1255 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/linear_warmup.py
--rw-r--r--   0        0        0     1400 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/proportion.py
--rw-r--r--   0        0        0        0 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/__init__.py
--rw-r--r--   0        0        0     4437 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/a2grad.py
--rw-r--r--   0        0        0     6701 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adabelief.py
--rw-r--r--   0        0        0     5470 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adabound.py
--rw-r--r--   0        0        0     3573 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adadelta.py
--rw-r--r--   0        0        0     8782 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adafactor.py
--rw-r--r--   0        0        0     6122 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adai.py
--rw-r--r--   0        0        0     4976 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adamax.py
--rw-r--r--   0        0        0     4664 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adamod.py
--rw-r--r--   0        0        0     6501 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adamp.py
--rw-r--r--   0        0        0     6417 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adams.py
--rw-r--r--   0        0        0     6274 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adan.py
--rw-r--r--   0        0        0     5253 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adanorm.py
--rw-r--r--   0        0        0     6014 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adapnm.py
--rw-r--r--   0        0        0     4169 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adashift.py
--rw-r--r--   0        0        0     4138 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adasmooth.py
--rw-r--r--   0        0        0      781 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/agc.py
--rw-r--r--   0        0        0     3172 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/aggmo.py
--rw-r--r--   0        0        0     3618 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/alig.py
--rw-r--r--   0        0        0     5290 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/apollo.py
--rw-r--r--   0        0        0     4803 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/avagrad.py
--rw-r--r--   0        0        0    25140 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/dadapt.py
--rw-r--r--   0        0        0     6749 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/diffgrad.py
--rw-r--r--   0        0        0    10702 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/fp16.py
--rw-r--r--   0        0        0     2764 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/fromage.py
--rw-r--r--   0        0        0      474 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/gc.py
--rw-r--r--   0        0        0     2517 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/gravity.py
--rw-r--r--   0        0        0     7544 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/gsam.py
--rw-r--r--   0        0        0     8316 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lamb.py
--rw-r--r--   0        0        0     3546 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lars.py
--rw-r--r--   0        0        0     4106 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lion.py
--rw-r--r--   0        0        0     4113 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lookahead.py
--rw-r--r--   0        0        0     6466 2023-05-06 08:07:56.343615 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/madgrad.py
--rw-r--r--   0        0        0     3172 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/msvag.py
--rw-r--r--   0        0        0     3595 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/nero.py
--rw-r--r--   0        0        0     4520 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/novograd.py
--rw-r--r--   0        0        0     4214 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/pcgrad.py
--rw-r--r--   0        0        0     4233 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/pid.py
--rw-r--r--   0        0        0     3741 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/pnm.py
--rw-r--r--   0        0        0     4827 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/qhadam.py
--rw-r--r--   0        0        0     3249 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/qhm.py
--rw-r--r--   0        0        0     5622 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/radam.py
--rw-r--r--   0        0        0     6744 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/ranger.py
--rw-r--r--   0        0        0    12772 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/ranger21.py
--rw-r--r--   0        0        0    15565 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/rotograd.py
--rw-r--r--   0        0        0     4638 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sam.py
--rw-r--r--   0        0        0    10375 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sgd.py
--rw-r--r--   0        0        0     4276 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sgdp.py
--rw-r--r--   0        0        0    16132 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/shampoo.py
--rw-r--r--   0        0        0    20625 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/shampoo_utils.py
--rw-r--r--   0        0        0     5081 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sm3.py
--rw-r--r--   0        0        0     2852 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/srmm.py
--rw-r--r--   0        0        0     7165 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/swats.py
--rw-r--r--   0        0        0     8832 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/utils.py
--rw-r--r--   0        0        0     5306 2023-05-06 08:07:56.347616 pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/yogi.py
--rw-r--r--   0        0        0    62650 1970-01-01 00:00:00.000000 pytorch_optimizer-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-19 12:09:37.191772 pytorch_optimizer-2.9.1/LICENSE
+-rw-r--r--   0        0        0    60156 2023-05-19 12:09:37.191772 pytorch_optimizer-2.9.1/README.rst
+-rw-r--r--   0        0        0     4305 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0     7354 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/base/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/base/exception.py
+-rw-r--r--   0        0        0     5633 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/base/optimizer.py
+-rw-r--r--   0        0        0     2761 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/base/scheduler.py
+-rw-r--r--   0        0        0      491 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/base/types.py
+-rw-r--r--   0        0        0      131 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0      971 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/chebyshev.py
+-rw-r--r--   0        0        0     4034 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/cosine_anealing.py
+-rw-r--r--   0        0        0        0 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/experimental/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/experimental/deberta_v3_lr_scheduler.py
+-rw-r--r--   0        0        0     1255 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/linear_warmup.py
+-rw-r--r--   0        0        0     1400 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/proportion.py
+-rw-r--r--   0        0        0        0 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/__init__.py
+-rw-r--r--   0        0        0     4464 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/a2grad.py
+-rw-r--r--   0        0        0     6701 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adabelief.py
+-rw-r--r--   0        0        0     5470 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adabound.py
+-rw-r--r--   0        0        0     3573 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adadelta.py
+-rw-r--r--   0        0        0     8782 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adafactor.py
+-rw-r--r--   0        0        0     6115 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adai.py
+-rw-r--r--   0        0        0     4976 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adamax.py
+-rw-r--r--   0        0        0     4664 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adamod.py
+-rw-r--r--   0        0        0     6494 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adamp.py
+-rw-r--r--   0        0        0     6417 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adams.py
+-rw-r--r--   0        0        0     6267 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adan.py
+-rw-r--r--   0        0        0     5253 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adanorm.py
+-rw-r--r--   0        0        0     6014 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adapnm.py
+-rw-r--r--   0        0        0     4169 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adashift.py
+-rw-r--r--   0        0        0     4138 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adasmooth.py
+-rw-r--r--   0        0        0      784 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/agc.py
+-rw-r--r--   0        0        0     3172 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/aggmo.py
+-rw-r--r--   0        0        0     3618 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/alig.py
+-rw-r--r--   0        0        0     5367 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/apollo.py
+-rw-r--r--   0        0        0     4803 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/avagrad.py
+-rw-r--r--   0        0        0    25140 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/dadapt.py
+-rw-r--r--   0        0        0     6749 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/diffgrad.py
+-rw-r--r--   0        0        0    10702 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/fp16.py
+-rw-r--r--   0        0        0     2764 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/fromage.py
+-rw-r--r--   0        0        0      396 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/gc.py
+-rw-r--r--   0        0        0     2517 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/gravity.py
+-rw-r--r--   0        0        0     7544 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/gsam.py
+-rw-r--r--   0        0        0     8316 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lamb.py
+-rw-r--r--   0        0        0     3546 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lars.py
+-rw-r--r--   0        0        0     4099 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lion.py
+-rw-r--r--   0        0        0     4155 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lookahead.py
+-rw-r--r--   0        0        0     6466 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/madgrad.py
+-rw-r--r--   0        0        0     3172 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/msvag.py
+-rw-r--r--   0        0        0     3595 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/nero.py
+-rw-r--r--   0        0        0     4520 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/novograd.py
+-rw-r--r--   0        0        0     4242 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/pcgrad.py
+-rw-r--r--   0        0        0     4233 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/pid.py
+-rw-r--r--   0        0        0     3741 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/pnm.py
+-rw-r--r--   0        0        0     4827 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/qhadam.py
+-rw-r--r--   0        0        0     3249 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/qhm.py
+-rw-r--r--   0        0        0     5622 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/radam.py
+-rw-r--r--   0        0        0     6737 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/ranger.py
+-rw-r--r--   0        0        0    12385 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/ranger21.py
+-rw-r--r--   0        0        0    15565 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/rotograd.py
+-rw-r--r--   0        0        0     4638 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sam.py
+-rw-r--r--   0        0        0    10375 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sgd.py
+-rw-r--r--   0        0        0     4276 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sgdp.py
+-rw-r--r--   0        0        0    16137 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/shampoo.py
+-rw-r--r--   0        0        0    20625 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/shampoo_utils.py
+-rw-r--r--   0        0        0     5081 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sm3.py
+-rw-r--r--   0        0        0     2852 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/srmm.py
+-rw-r--r--   0        0        0     7165 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/swats.py
+-rw-r--r--   0        0        0     8755 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/utils.py
+-rw-r--r--   0        0        0     5306 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/yogi.py
+-rw-r--r--   0        0        0    62572 1970-01-01 00:00:00.000000 pytorch_optimizer-2.9.1/PKG-INFO
```

### Comparing `pytorch_optimizer-2.9.0/LICENSE` & `pytorch_optimizer-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/README.rst` & `pytorch_optimizer-2.9.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -125,17 +125,17 @@
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
 | Nero         | *Learning by Turning: Neural Architecture Aware Optimisation*                                     | `github <https://github.com/jxbz/nero>`__                                         | `https://arxiv.org/abs/2102.07227 <https://arxiv.org/abs/2102.07227>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2021arXiv210207227L/exportcitation>`__                                      |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
 | Adan         | *Adaptive Nesterov Momentum Algorithm for Faster Optimizing Deep Models*                          | `github <https://github.com/sail-sg/Adan>`__                                      | `https://arxiv.org/abs/2208.06677 <https://arxiv.org/abs/2208.06677>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2022arXiv220806677X/exportcitation>`__                                      |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
 | Adai         | *Disentangling the Effects of Adaptive Learning Rate and Momentum*                                | `github <https://github.com/zeke-xie/adaptive-inertia-adai>`__                    | `https://arxiv.org/abs/2006.15815 <https://arxiv.org/abs/2006.15815>`__                       | `cite <https://github.com/zeke-xie/adaptive-inertia-adai#citing>`__                                                  |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| SAM          | *Sharpness-Aware Minimization*                                                                    | `github <https://github.com/davda54/sam>`__                                       | `https://arxiv.org/abs/2010.01412 <https://arxiv.org/abs/2010.01412>`__     | `cite <https://ui.adsabs.harvard.edu/abs/2020arXiv201001412F/exportcitation>`__                                                        |
+| SAM          | *Sharpness-Aware Minimization*                                                                    | `github <https://github.com/davda54/sam>`__                                       | `https://arxiv.org/abs/2010.01412 <https://arxiv.org/abs/2010.01412>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2020arXiv201001412F/exportcitation>`__                                      |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| ASAM         | *Adaptive Sharpness-Aware Minimization*                                                           | `github <https://github.com/davda54/sam>`__                                       | `https://arxiv.org/abs/2102.11600 <https://arxiv.org/abs/2102.11600>`__     | `cite <https://ui.adsabs.harvard.edu/abs/2021arXiv210211600K/exportcitation>`__                                                        |
+| ASAM         | *Adaptive Sharpness-Aware Minimization*                                                           | `github <https://github.com/davda54/sam>`__                                       | `https://arxiv.org/abs/2102.11600 <https://arxiv.org/abs/2102.11600>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2021arXiv210211600K/exportcitation>`__                                      |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
 | GSAM         | *Surrogate Gap Guided Sharpness-Aware Minimization*                                               | `github <https://github.com/juntang-zhuang/GSAM>`__                               | `https://openreview.net/pdf?id=edONMAnhLu- <https://openreview.net/pdf?id=edONMAnhLu->`__     | `cite <https://github.com/juntang-zhuang/GSAM#citation>`__                                                           |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
 | D-Adaptation | *Learning-Rate-Free Learning by D-Adaptation*                                                     | `github <https://github.com/facebookresearch/dadaptation>`__                      | `https://arxiv.org/abs/2301.07733 <https://arxiv.org/abs/2301.07733>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2023arXiv230107733D/exportcitation>`__                                      |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
 | AdaFactor    | *Adaptive Learning Rates with Sublinear Memory Cost*                                              | `github <https://github.com/DeadAt0m/adafactor-pytorch>`__                        | `https://arxiv.org/abs/1804.04235 <https://arxiv.org/abs/1804.04235>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2018arXiv180404235S/exportcitation>`__                                      |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
```

### Comparing `pytorch_optimizer-2.9.0/pyproject.toml` & `pytorch_optimizer-2.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pytorch_optimizer"
-version = "2.9.0"
-description = "optimizer & lr scheduler implementations in PyTorch with clean-code, strict types. Also, including useful optimization ideas."
+version = "2.9.1"
+description = "optimizer & lr scheduler collections in PyTorch"
 license = "Apache-2.0"
 authors = ["kozistr <kozistr@gmail.com>"]
 maintainers = ["kozistr <kozistr@gmail.com>"]
 readme = "README.rst"
 homepage = "https://github.com/kozistr/pytorch_optimizer"
 repository = "https://github.com/kozistr/pytorch_optimizer"
 documentation = "https://pytorch-optimizers.readthedocs.io/en/latest"
```

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/__init__.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/base/exception.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/base/exception.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/base/scheduler.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/base/scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/chebyshev.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/chebyshev.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/cosine_anealing.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/experimental/deberta_v3_lr_scheduler.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/experimental/deberta_v3_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/linear_warmup.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/linear_warmup.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/lr_scheduler/proportion.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/proportion.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/a2grad.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/a2grad.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         lips: float = 10.0,
         rho: float = 0.5,
         variant: str = 'uni',
     ):
         self.validate_learning_rate(lr)
         self.validate_non_negative(lips, 'lips')
         self.validate_non_negative(rho, 'rho')
-        self.validate_a2grad_variant(variant)
+        self.validate_options(variant, 'variant', ['uni', 'inc', 'exp'])
 
         self.variant = variant
 
         defaults: DEFAULTS = {'beta': beta, 'lips': lips}
         if variant == 'exp':
             defaults.update({'rho': rho})
```

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adabelief.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adabelief.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adabound.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adabound.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adadelta.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adadelta.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adafactor.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adafactor.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adai.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adai.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
                     state['beta1_prod'] = torch.ones_like(p)
 
                 state['step'] += 1
 
                 if self.use_gc:
-                    grad = centralize_gradient(grad, gc_conv_only=False)
+                    centralize_gradient(grad, gc_conv_only=False)
 
                 bias_correction2: float = 1.0 - beta2 ** state['step']
 
                 if not group['stable_weight_decay'] and group['weight_decay'] > 0.0:
                     self.apply_weight_decay(
                         p=p,
                         grad=grad,
```

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adamax.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adamax.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adamod.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adamod.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adamp.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adamp.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                 if len(state) == 0:
                     state['exp_avg'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
                     if group['adanorm']:
                         state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
 
                 if self.use_gc:
-                    grad = centralize_gradient(grad, gc_conv_only=False)
+                    centralize_gradient(grad, gc_conv_only=False)
 
                 s_grad = self.get_adanorm_gradient(
                     grad=grad,
                     adanorm=group['adanorm'],
                     exp_grad_norm=state.get('exp_grad_norm', None),
                     r=group.get('r', None),
                 )
```

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adams.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adams.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adan.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adan.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                     state['previous_grad'] = grad.clone().mul_(-clip_global_grad_norm)
                     if group['adanorm']:
                         state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
 
                 grad.mul_(clip_global_grad_norm)
 
                 if self.use_gc:
-                    grad = centralize_gradient(grad, gc_conv_only=False)
+                    centralize_gradient(grad, gc_conv_only=False)
 
                 grad_diff = state['previous_grad']
                 grad_diff.add_(grad)
 
                 s_grad = self.get_adanorm_gradient(
                     grad=grad,
                     adanorm=group['adanorm'],
```

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adanorm.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adanorm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adapnm.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adapnm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adashift.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adashift.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/adasmooth.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adasmooth.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/agc.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/agc.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pytorch_optimizer.optimizer.utils import unit_norm
 
 
 def agc(p: torch.Tensor, grad: torch.Tensor, agc_eps: float, agc_clip_val: float, eps: float = 1e-6) -> torch.Tensor:
     r"""Clip gradient values in excess of the unit wise norm.
 
-    :param p: Parameter. parameter.
+    :param p: torch.Tensor. parameter.
     :param grad: torch.Tensor, gradient.
     :param agc_eps: float. agc epsilon to clip the norm of parameter.
     :param agc_clip_val: float. norm clip.
     :param eps: float. simple stop from div by zero and no relation to standard optimizer eps.
     """
     p_norm = unit_norm(p).clamp_(agc_eps)
     g_norm = unit_norm(grad)
```

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/aggmo.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/aggmo.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/alig.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/alig.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/apollo.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/apollo.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,17 +33,17 @@
         weight_decay: float = 0.0,
         weight_decay_type: str = 'l2',
         warmup_steps: int = 500,
         eps: float = 1e-4,
     ):
         self.validate_learning_rate(lr)
         self.validate_range(beta, 'beta', 0.0, 1.0, range_type='[]')
-        self.validate_rebound(rebound)
+        self.validate_options(rebound, 'rebound', ['constant', 'belief'])
         self.validate_non_negative(weight_decay, 'weight_decay')
-        self.validate_weight_decay_type(weight_decay_type)
+        self.validate_options(weight_decay_type, 'weight_decay_type', ['l2', 'decoupled', 'stable'])
         self.validate_non_negative(eps, 'eps')
 
         self.lr = lr
         self.warmup_steps = warmup_steps
         self.init_lr: float = init_lr if init_lr is not None else lr / 1000.0
 
         defaults: DEFAULTS = {
```

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/avagrad.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/avagrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/dadapt.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/dadapt.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/diffgrad.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/diffgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/fp16.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/fp16.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/fromage.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/fromage.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/gravity.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/gravity.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/gsam.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/gsam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lamb.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lars.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lion.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lion.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
                 if len(state) == 0:
                     state['exp_avg'] = torch.zeros_like(p)
                     if group['adanorm']:
                         state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
 
                 if self.use_gc:
-                    grad = centralize_gradient(grad, gc_conv_only=False)
+                    centralize_gradient(grad, gc_conv_only=False)
 
                 self.apply_weight_decay(
                     p=p,
                     grad=p.grad,
                     lr=group['lr'],
                     weight_decay=group['weight_decay'],
                     weight_decouple=group['weight_decouple'],
```

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/lookahead.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lookahead.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         optimizer: OPTIMIZER,
         k: int = 5,
         alpha: float = 0.5,
         pullback_momentum: str = 'none',
     ):
         self.validate_positive(k, 'k')
         self.validate_range(alpha, 'alpha', 0.0, 1.0)
-        self.validate_pullback_momentum(pullback_momentum)
+        self.validate_options(pullback_momentum, 'pullback_momentum', ['none', 'reset', 'pullback'])
 
         self.alpha = alpha
         self.k = k
         self.pullback_momentum = pullback_momentum
 
         self.optimizer = optimizer
         self.param_groups = self.optimizer.param_groups
```

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/madgrad.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/madgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/msvag.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/msvag.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/nero.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/nero.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/novograd.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/novograd.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/pcgrad.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/pcgrad.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     r"""Gradient Surgery for Multi-Task Learning.
 
     :param optimizer: OPTIMIZER: optimizer instance.
     :param reduction: str. reduction method.
     """
 
     def __init__(self, optimizer: OPTIMIZER, reduction: str = 'mean'):
-        self.validate_reduction(reduction)
+        self.validate_options(reduction, 'reduction', ['mean', 'sum'])
 
         self.optimizer = optimizer
         self.reduction = reduction
 
     @torch.no_grad()
     def reset(self):
         self.zero_grad()
```

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/pid.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/pid.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/pnm.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/pnm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/qhadam.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/qhadam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/qhm.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/qhm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/radam.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/radam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/ranger.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/ranger.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                     state['exp_avg_sq'] = torch.zeros_like(p)
                     state['slow_buffer'] = torch.empty_like(p)
                     state['slow_buffer'].copy_(p)
                     if group['adanorm']:
                         state['exp_grad_norm'] = torch.zeros((1,), dtype=grad.dtype, device=grad.device)
 
                 if self.use_gc and grad.dim() > self.gc_gradient_threshold:
-                    grad = centralize_gradient(grad, gc_conv_only=False)
+                    centralize_gradient(grad, gc_conv_only=False)
 
                 self.apply_weight_decay(
                     p=p,
                     grad=None,
                     lr=group['lr'],
                     weight_decay=group['weight_decay'],
                     weight_decouple=group['weight_decouple'],
```

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/ranger21.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/ranger21.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,33 +92,29 @@
         self.agc_eps = agc_eps
         self.centralize_gradients = centralize_gradients
         self.normalize_gradients = normalize_gradients
         self.lookahead_merge_time = lookahead_merge_time
         self.lookahead_blending_alpha = lookahead_blending_alpha
         self.norm_loss_factor = norm_loss_factor
 
-        # lookahead
         self.lookahead_step: int = 0
-
-        # learning rate
-        self.starting_lr = lr
-        self.current_lr = lr
+        self.starting_lr: float = lr
+        self.current_lr: float = lr
 
         defaults: DEFAULTS = {
             'lr': lr,
             'betas': betas,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
             'fixed_decay': fixed_decay,
             'adam_debias': adam_debias,
             'eps': eps,
         }
         super().__init__(params, defaults)
 
-        # warmup iterations
         self.num_warm_up_iterations: int = (
             self.build_warm_up_iterations(num_iterations, betas[1])
             if num_warm_up_iterations is None
             else num_warm_up_iterations
         )
         self.num_warm_down_iterations: int = (
             self.build_warm_down_iterations(num_iterations)
@@ -136,16 +132,15 @@
         for group in self.param_groups:
             group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
                 state['grad_ma'] = torch.zeros_like(p)
                 state['variance_ma'] = torch.zeros_like(p)
-                state['lookahead_params'] = torch.empty_like(p)
-                state['lookahead_params'].copy_(p)
+                state['lookahead_params'] = p.clone()
                 state['neg_grad_ma'] = torch.zeros_like(p)
                 state['max_variance_ma'] = torch.zeros_like(p)
 
     @staticmethod
     def build_warm_up_iterations(total_iterations: int, beta2: float, warm_up_pct: float = 0.22) -> int:
         warm_up_iterations: int = math.ceil(2.0 / (1.0 - beta2))  # default un-tuned linear warmup
         beta_pct: float = warm_up_iterations / total_iterations
@@ -158,36 +153,29 @@
 
     def warm_up_dampening(self, lr: float, step: int) -> float:
         if step > self.num_warm_up_iterations:
             return lr
 
         warm_up_current_pct: float = min(1.0, (step / self.num_warm_up_iterations))
 
-        new_lr: float = lr * warm_up_current_pct
-        self.current_lr = new_lr
+        self.current_lr = lr * warm_up_current_pct
 
-        return new_lr
+        return self.current_lr
 
     def warm_down(self, lr: float, iteration: int) -> float:
         if iteration < self.start_warm_down:
             return lr
 
         # start iteration from 1, not 0
-        warm_down_iteration: int = (iteration + 1) - self.start_warm_down
-        warm_down_iteration = max(warm_down_iteration, 1)
-
-        warm_down_pct: float = warm_down_iteration / (self.num_warm_down_iterations + 1)
-        warm_down_pct = min(warm_down_pct, 1.0)
-
-        new_lr: float = self.starting_lr - self.warm_down_lr_delta * warm_down_pct
-        new_lr = max(new_lr, self.min_lr)
+        warm_down_iteration: int = max((iteration + 1) - self.start_warm_down, 1)
+        warm_down_pct: float = min(warm_down_iteration / (self.num_warm_down_iterations + 1), 1.0)
 
-        self.current_lr = new_lr
+        self.current_lr = max(self.starting_lr - self.warm_down_lr_delta * warm_down_pct, self.min_lr)
 
-        return new_lr
+        return self.current_lr
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
         loss: LOSS = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
@@ -216,60 +204,58 @@
 
                 param_size += p.numel()
 
                 state = self.state[p]
                 if len(state) == 0:
                     state['grad_ma'] = torch.zeros_like(p)
                     state['variance_ma'] = torch.zeros_like(p)
-                    state['lookahead_params'] = torch.empty_like(p)
-                    state['lookahead_params'].copy_(p)
+                    state['lookahead_params'] = p.clone()
                     state['neg_grad_ma'] = torch.zeros_like(p)
                     state['max_variance_ma'] = torch.zeros_like(p)
 
                 # Apply Adaptive Gradient Clipping (AGC)
                 grad.copy_(agc(p, grad, self.agc_eps, self.agc_clipping_value))
 
                 # Apply gradient centralization & normalization
-                grad = centralize_gradient(grad, gc_conv_only=False)
-                grad = normalize_gradient(grad)
+                centralize_gradient(grad, gc_conv_only=False)
+                normalize_gradient(grad)
 
                 # second moment estimation
                 # using positive-negative momentum and bias correction
                 variance_ma = state['variance_ma']
                 variance_ma.mul_(beta2).addcmul_(grad, grad, value=1.0 - beta2)
                 variance_ma_sum += (variance_ma / bias_correction2).sum()
 
         if param_size == 0:
             raise ZeroParameterSizeError()
 
         variance_normalized = math.sqrt(variance_ma_sum / param_size)
 
         # Phase 2 - Apply weight decay and step
         for group in self.param_groups:
-            lr: float = group['lr']
             beta1, beta2 = group['betas']
 
             bias_correction1: float = 1.0 - beta1 ** group['step']  # fmt: skip
             bias_correction2_sq: float = math.sqrt(1.0 - beta2 ** group['step'])  # fmt: skip
 
             noise_norm: float = math.sqrt((1.0 + beta2) ** 2 + beta2 ** 2)  # fmt: skip
 
             # warm up & down
-            lr = self.warm_up_dampening(lr, group['step'])
+            lr: float = self.warm_up_dampening(group['lr'], group['step'])
             lr = self.warm_down(lr, group['step'])
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 # stable weight decay
                 self.apply_weight_decay(
                     p=p,
                     grad=None,
-                    lr=group['lr'],
+                    lr=lr,
                     weight_decay=group['weight_decay'],
                     weight_decouple=group['weight_decouple'],
                     fixed_decay=group['fixed_decay'],
                     ratio=1.0 / variance_normalized,
                 )
 
                 # norm loss
@@ -283,24 +269,24 @@
                     grad_ma, neg_grad_ma = state['neg_grad_ma'], state['grad_ma']
 
                 variance_ma = state['variance_ma']
                 torch.max(state['max_variance_ma'], variance_ma, out=variance_ma)
 
                 de_nom = (variance_ma.sqrt() / bias_correction2_sq).add_(group['eps'])
 
+                if self.use_softplus:
+                    de_nom = f.softplus(de_nom, beta=self.beta_softplus)
+
                 grad = p.grad
-                grad = centralize_gradient(grad, gc_conv_only=False)
-                grad = normalize_gradient(grad)
+                centralize_gradient(grad, gc_conv_only=False)
+                normalize_gradient(grad)
 
                 grad_ma.mul_(beta1 ** 2).add_(grad, alpha=1.0 - beta1 ** 2)  # fmt: skip
 
-                step_size: float = lr if group['adam_debias'] else lr / bias_correction1
-
-                if self.use_softplus:
-                    de_nom = f.softplus(de_nom, beta=self.beta_softplus)
+                step_size: float = self.apply_adam_debias(group['adam_debias'], lr, bias_correction1)
 
                 pn_momentum = grad_ma.mul(1.0 + 1.0).add(neg_grad_ma, alpha=-1.0).mul(1.0 / noise_norm)
                 p.addcdiv_(pn_momentum, de_nom, value=-step_size)
 
         self.lookahead_process_step()
 
         return loss
```

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/rotograd.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/rotograd.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sam.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sgd.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sgd.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sgdp.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sgdp.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/shampoo.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/shampoo.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,22 +41,22 @@
         self.validate_learning_rate(lr)
         self.validate_range(momentum, 'momentum', 0.0, 1.0)
         self.validate_non_negative(weight_decay, 'weight_decay')
         self.validate_step(preconditioning_compute_steps, 'preconditioning_compute_steps')
         self.validate_non_negative(matrix_eps, 'matrix_eps')
 
         self.preconditioning_compute_steps = preconditioning_compute_steps
-        self.matrix_eps = matrix_eps
 
         defaults: DEFAULTS = {
             'lr': lr,
             'momentum': momentum,
             'weight_decay': weight_decay,
             'weight_decouple': weight_decouple,
             'fixed_decay': fixed_decay,
+            'matrix_eps': matrix_eps,
         }
         super().__init__(params, defaults)
 
     def __str__(self) -> str:
         return 'Shampoo'
 
     @torch.no_grad()
@@ -89,15 +89,15 @@
 
                 state = self.state[p]
                 if len(state) == 0:
                     if momentum > 0.0:
                         state['momentum_buffer'] = grad.clone()
 
                     for dim_id, dim in enumerate(grad.size()):
-                        state[f'pre_cond_{dim_id}'] = self.matrix_eps * torch.eye(dim, out=grad.new(dim, dim))
+                        state[f'pre_cond_{dim_id}'] = group['matrix_eps'] * torch.eye(dim, out=grad.new(dim, dim))
                         state[f'inv_pre_cond_{dim_id}'] = grad.new(dim, dim).zero_()
 
                 if momentum > 0.0:
                     grad.mul_(1.0 - momentum).add_(state['momentum_buffer'], alpha=momentum)
 
                 self.apply_weight_decay(
                     p=p,
```

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/shampoo_utils.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/shampoo_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/sm3.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sm3.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/srmm.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/srmm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/swats.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/swats.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/utils.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,30 +23,28 @@
 
 
 def to_real(x: torch.Tensor) -> torch.Tensor:
     r"""Return real value of tensor."""
     return x.real if torch.is_complex(x) else x
 
 
-def normalize_gradient(x: torch.Tensor, use_channels: bool = False, epsilon: float = 1e-8) -> torch.Tensor:
+def normalize_gradient(x: torch.Tensor, use_channels: bool = False, epsilon: float = 1e-8):
     r"""Normalize gradient with stddev.
 
     :param x: torch.Tensor. gradient.
     :param use_channels: bool. channel-wise normalization.
     :param epsilon: float. eps.
-    :return: torch.Tensor. normalized gradient.
     """
     size: int = x.dim()
     if size > 1 and use_channels:
         s = x.std(dim=tuple(range(1, size)), keepdim=True).add_(epsilon)
         x.div_(s)
     elif torch.numel(x) > 2:
         s = x.std().add_(epsilon)
         x.div_(s)
-    return x
 
 
 def flatten_grad(grads: List[torch.Tensor]) -> torch.Tensor:
     r"""Flatten the gradient."""
     return torch.cat([grad.flatten() for grad in grads])
```

### Comparing `pytorch_optimizer-2.9.0/pytorch_optimizer/optimizer/yogi.py` & `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/yogi.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.0/PKG-INFO` & `pytorch_optimizer-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pytorch-optimizer
-Version: 2.9.0
-Summary: optimizer & lr scheduler implementations in PyTorch with clean-code, strict types. Also, including useful optimization ideas.
+Version: 2.9.1
+Summary: optimizer & lr scheduler collections in PyTorch
 Home-page: https://github.com/kozistr/pytorch_optimizer
 License: Apache-2.0
 Keywords: pytorch,deep-learning,optimizer,lr scheduler,A2Grad,ASGD,AccSGD,AdaBelief,AdaBound,AdaDelta,AdaFactor,AdaMax,AdaMod,AdaNorm,AdaPNM,AdaSmooth,Adai,AdamP,AdamS,Adan,AggMo,AliG,Apollo,AvaGrad,DAdaptAdaGrad,DAdaptAdam,DAdaptAdan,DAdaptSGD,DiffGrad,Fromage,Gravity,LARS,Lamb,Lion,MADGRAD,MSVAG,Nero,NovoGrad,PID,PNM,QHAdam,QHM,RAdam,Ranger,Ranger21,SGDP,SGDW,SM3,SRMM,SWATS,ScalableShampoo,Shampoo,Yogi,SAM,GSAM,PCGrad,RotoGrad
 Author: kozistr
 Author-email: kozistr@gmail.com
 Maintainer: kozistr
 Maintainer-email: kozistr@gmail.com
@@ -168,17 +168,17 @@
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
 | Nero         | *Learning by Turning: Neural Architecture Aware Optimisation*                                     | `github <https://github.com/jxbz/nero>`__                                         | `https://arxiv.org/abs/2102.07227 <https://arxiv.org/abs/2102.07227>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2021arXiv210207227L/exportcitation>`__                                      |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
 | Adan         | *Adaptive Nesterov Momentum Algorithm for Faster Optimizing Deep Models*                          | `github <https://github.com/sail-sg/Adan>`__                                      | `https://arxiv.org/abs/2208.06677 <https://arxiv.org/abs/2208.06677>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2022arXiv220806677X/exportcitation>`__                                      |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
 | Adai         | *Disentangling the Effects of Adaptive Learning Rate and Momentum*                                | `github <https://github.com/zeke-xie/adaptive-inertia-adai>`__                    | `https://arxiv.org/abs/2006.15815 <https://arxiv.org/abs/2006.15815>`__                       | `cite <https://github.com/zeke-xie/adaptive-inertia-adai#citing>`__                                                  |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| SAM          | *Sharpness-Aware Minimization*                                                                    | `github <https://github.com/davda54/sam>`__                                       | `https://arxiv.org/abs/2010.01412 <https://arxiv.org/abs/2010.01412>`__     | `cite <https://ui.adsabs.harvard.edu/abs/2020arXiv201001412F/exportcitation>`__                                                        |
+| SAM          | *Sharpness-Aware Minimization*                                                                    | `github <https://github.com/davda54/sam>`__                                       | `https://arxiv.org/abs/2010.01412 <https://arxiv.org/abs/2010.01412>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2020arXiv201001412F/exportcitation>`__                                      |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| ASAM         | *Adaptive Sharpness-Aware Minimization*                                                           | `github <https://github.com/davda54/sam>`__                                       | `https://arxiv.org/abs/2102.11600 <https://arxiv.org/abs/2102.11600>`__     | `cite <https://ui.adsabs.harvard.edu/abs/2021arXiv210211600K/exportcitation>`__                                                        |
+| ASAM         | *Adaptive Sharpness-Aware Minimization*                                                           | `github <https://github.com/davda54/sam>`__                                       | `https://arxiv.org/abs/2102.11600 <https://arxiv.org/abs/2102.11600>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2021arXiv210211600K/exportcitation>`__                                      |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
 | GSAM         | *Surrogate Gap Guided Sharpness-Aware Minimization*                                               | `github <https://github.com/juntang-zhuang/GSAM>`__                               | `https://openreview.net/pdf?id=edONMAnhLu- <https://openreview.net/pdf?id=edONMAnhLu->`__     | `cite <https://github.com/juntang-zhuang/GSAM#citation>`__                                                           |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
 | D-Adaptation | *Learning-Rate-Free Learning by D-Adaptation*                                                     | `github <https://github.com/facebookresearch/dadaptation>`__                      | `https://arxiv.org/abs/2301.07733 <https://arxiv.org/abs/2301.07733>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2023arXiv230107733D/exportcitation>`__                                      |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
 | AdaFactor    | *Adaptive Learning Rates with Sublinear Memory Cost*                                              | `github <https://github.com/DeadAt0m/adafactor-pytorch>`__                        | `https://arxiv.org/abs/1804.04235 <https://arxiv.org/abs/1804.04235>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2018arXiv180404235S/exportcitation>`__                                      |
 +--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
```

