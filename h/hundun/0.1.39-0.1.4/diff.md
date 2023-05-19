# Comparing `tmp/hundun-0.1.39.tar.gz` & `tmp/hundun-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hundun-0.1.39.tar", last modified: Fri May 19 10:00:19 2023, max compression
+gzip compressed data, was "hundun-0.1.4.tar", last modified: Wed Jan 19 06:12:20 2022, max compression
```

## Comparing `hundun-0.1.39.tar` & `hundun-0.1.4.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:00:19.137154 hundun-0.1.39/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 10:00:05.000000 hundun-0.1.39/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 10:00:05.000000 hundun-0.1.39/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-19 10:00:19.137154 hundun-0.1.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-19 10:00:05.000000 hundun-0.1.39/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:00:19.133154 hundun-0.1.39/hundun/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:00:19.133154 hundun-0.1.39/hundun/equations/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/equations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/equations/henon.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/equations/logistic.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/equations/lorenz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:00:19.137154 hundun-0.1.39/hundun/exploration/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/exploration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/exploration/_afn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/exploration/_autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/exploration/_box3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/exploration/_fnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/exploration/_gp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/exploration/_mutualinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/exploration/_recurrenceplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/exploration/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/exploration/_wayland.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:00:19.137154 hundun-0.1.39/hundun/lyapunov/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/lyapunov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/lyapunov/_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/lyapunov/_les_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/lyapunov/_les_differential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:00:19.137154 hundun-0.1.39/hundun/systems/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/systems/_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/systems/_differential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/systems/_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/systems/_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/systems/_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/systems/_tu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:00:19.137154 hundun-0.1.39/hundun/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-19 10:00:05.000000 hundun-0.1.39/hundun/utils/_draw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:00:19.133154 hundun-0.1.39/hundun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-19 10:00:19.000000 hundun-0.1.39/hundun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-19 10:00:19.000000 hundun-0.1.39/hundun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:00:19.000000 hundun-0.1.39/hundun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-19 10:00:19.000000 hundun-0.1.39/hundun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 10:00:19.000000 hundun-0.1.39/hundun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-19 10:00:05.000000 hundun-0.1.39/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 10:00:19.137154 hundun-0.1.39/setup.cfg
+drwxr-xr-x   0 kosh       (501) staff       (20)        0 2022-01-19 06:12:20.178965 hundun-0.1.4/
+-rw-r--r--   0 kosh       (501) staff       (20)     1068 2021-12-31 14:56:00.000000 hundun-0.1.4/LICENSE.txt
+-rw-r--r--   0 kosh       (501) staff       (20)       23 2021-12-24 07:32:27.000000 hundun-0.1.4/MANIFEST.in
+-rw-r--r--   0 kosh       (501) staff       (20)    23045 2022-01-19 06:12:20.178803 hundun-0.1.4/PKG-INFO
+-rw-r--r--   0 kosh       (501) staff       (20)    22664 2022-01-19 06:11:47.000000 hundun-0.1.4/README.md
+drwxr-xr-x   0 kosh       (501) staff       (20)        0 2022-01-19 06:12:20.173743 hundun-0.1.4/hundun/
+-rw-r--r--   0 kosh       (501) staff       (20)      273 2022-01-17 02:27:18.000000 hundun-0.1.4/hundun/__init__.py
+-rw-r--r--   0 kosh       (501) staff       (20)       72 2022-01-18 09:37:01.000000 hundun-0.1.4/hundun/__version__.py
+drwxr-xr-x   0 kosh       (501) staff       (20)        0 2022-01-19 06:12:20.175408 hundun-0.1.4/hundun/equations/
+-rw-r--r--   0 kosh       (501) staff       (20)      112 2022-01-12 06:34:04.000000 hundun-0.1.4/hundun/equations/__init__.py
+-rw-r--r--   0 kosh       (501) staff       (20)      448 2022-01-15 08:17:16.000000 hundun-0.1.4/hundun/equations/henon.py
+-rw-r--r--   0 kosh       (501) staff       (20)      304 2022-01-12 03:46:13.000000 hundun-0.1.4/hundun/equations/logistic.py
+-rw-r--r--   0 kosh       (501) staff       (20)      604 2022-01-11 08:22:11.000000 hundun-0.1.4/hundun/equations/lorenz.py
+drwxr-xr-x   0 kosh       (501) staff       (20)        0 2022-01-19 06:12:20.176609 hundun-0.1.4/hundun/exploration/
+-rw-r--r--   0 kosh       (501) staff       (20)      340 2022-01-17 06:54:43.000000 hundun-0.1.4/hundun/exploration/__init__.py
+-rw-r--r--   0 kosh       (501) staff       (20)     1237 2022-01-15 08:33:26.000000 hundun-0.1.4/hundun/exploration/_afn.py
+-rw-r--r--   0 kosh       (501) staff       (20)      699 2022-01-17 06:53:23.000000 hundun-0.1.4/hundun/exploration/_autocorrelation.py
+-rw-r--r--   0 kosh       (501) staff       (20)     1145 2022-01-15 08:41:35.000000 hundun-0.1.4/hundun/exploration/_fnn.py
+-rw-r--r--   0 kosh       (501) staff       (20)     1618 2022-01-15 08:16:06.000000 hundun-0.1.4/hundun/exploration/_gp.py
+-rw-r--r--   0 kosh       (501) staff       (20)      954 2022-01-16 08:38:24.000000 hundun-0.1.4/hundun/exploration/_mutualinfo.py
+-rw-r--r--   0 kosh       (501) staff       (20)      897 2022-01-17 03:43:58.000000 hundun-0.1.4/hundun/exploration/_recurrenceplot.py
+-rw-r--r--   0 kosh       (501) staff       (20)     1703 2022-01-17 06:55:15.000000 hundun-0.1.4/hundun/exploration/_utils.py
+-rw-r--r--   0 kosh       (501) staff       (20)     1351 2022-01-01 13:30:29.000000 hundun-0.1.4/hundun/exploration/_wayland.py
+drwxr-xr-x   0 kosh       (501) staff       (20)        0 2022-01-19 06:12:20.177212 hundun-0.1.4/hundun/lyapunov/
+-rw-r--r--   0 kosh       (501) staff       (20)      948 2022-01-17 02:26:41.000000 hundun-0.1.4/hundun/lyapunov/__init__.py
+-rw-r--r--   0 kosh       (501) staff       (20)      535 2022-01-17 02:25:41.000000 hundun-0.1.4/hundun/lyapunov/_func.py
+-rw-r--r--   0 kosh       (501) staff       (20)     1591 2022-01-17 08:06:13.000000 hundun-0.1.4/hundun/lyapunov/_les_difference.py
+-rw-r--r--   0 kosh       (501) staff       (20)     4899 2022-01-18 09:03:00.000000 hundun-0.1.4/hundun/lyapunov/_les_differential.py
+drwxr-xr-x   0 kosh       (501) staff       (20)        0 2022-01-19 06:12:20.178357 hundun-0.1.4/hundun/systems/
+-rw-r--r--   0 kosh       (501) staff       (20)      148 2022-01-18 07:15:50.000000 hundun-0.1.4/hundun/systems/__init__.py
+-rw-r--r--   0 kosh       (501) staff       (20)      268 2021-12-24 07:32:27.000000 hundun-0.1.4/hundun/systems/_difference.py
+-rw-r--r--   0 kosh       (501) staff       (20)      399 2021-12-24 07:32:27.000000 hundun-0.1.4/hundun/systems/_differential.py
+-rw-r--r--   0 kosh       (501) staff       (20)     1516 2021-12-24 07:32:27.000000 hundun-0.1.4/hundun/systems/_solver.py
+-rw-------   0 kosh       (501) staff       (20)     1966 2022-01-18 07:18:24.000000 hundun-0.1.4/hundun/systems/_sync.py
+-rw-r--r--   0 kosh       (501) staff       (20)     2873 2022-01-11 08:22:22.000000 hundun-0.1.4/hundun/systems/_systems.py
+-rw-r--r--   0 kosh       (501) staff       (20)      123 2021-12-24 07:32:27.000000 hundun-0.1.4/hundun/systems/_tu.py
+drwxr-xr-x   0 kosh       (501) staff       (20)        0 2022-01-19 06:12:20.178572 hundun-0.1.4/hundun/utils/
+-rw-r--r--   0 kosh       (501) staff       (20)       27 2021-12-24 07:32:27.000000 hundun-0.1.4/hundun/utils/__init__.py
+-rw-r--r--   0 kosh       (501) staff       (20)     3926 2022-01-18 06:01:46.000000 hundun-0.1.4/hundun/utils/_draw.py
+drwxr-xr-x   0 kosh       (501) staff       (20)        0 2022-01-19 06:12:20.174675 hundun-0.1.4/hundun.egg-info/
+-rw-r--r--   0 kosh       (501) staff       (20)    23045 2022-01-19 06:12:20.000000 hundun-0.1.4/hundun.egg-info/PKG-INFO
+-rw-r--r--   0 kosh       (501) staff       (20)     1014 2022-01-19 06:12:20.000000 hundun-0.1.4/hundun.egg-info/SOURCES.txt
+-rw-r--r--   0 kosh       (501) staff       (20)        1 2022-01-19 06:12:20.000000 hundun-0.1.4/hundun.egg-info/dependency_links.txt
+-rw-r--r--   0 kosh       (501) staff       (20)        1 2022-01-16 09:14:06.000000 hundun-0.1.4/hundun.egg-info/not-zip-safe
+-rw-r--r--   0 kosh       (501) staff       (20)       23 2022-01-19 06:12:20.000000 hundun-0.1.4/hundun.egg-info/requires.txt
+-rw-r--r--   0 kosh       (501) staff       (20)        7 2022-01-19 06:12:20.000000 hundun-0.1.4/hundun.egg-info/top_level.txt
+-rw-r--r--   0 kosh       (501) staff       (20)       38 2022-01-19 06:12:20.179010 hundun-0.1.4/setup.cfg
+-rw-r--r--   0 kosh       (501) staff       (20)     1060 2021-12-24 07:32:27.000000 hundun-0.1.4/setup.py
```

### Comparing `hundun-0.1.39/LICENSE.txt` & `hundun-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hundun-0.1.39/hundun/equations/lorenz.py` & `hundun-0.1.4/hundun/equations/lorenz.py`

 * *Files identical despite different names*

### Comparing `hundun-0.1.39/hundun/exploration/_gp.py` & `hundun-0.1.4/hundun/exploration/_gp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Grassberger-Procaccia Algorithm (グラスバーガー - プロカッチャ アルゴリズム)
 
 from itertools import combinations as _combinations
-import warnings as _warnings
 
 import numpy as _np
 
 
 def _dist(a, b):
     return _np.linalg.norm(a - b)
 
@@ -27,27 +26,23 @@
 def calc_correlation_dimention_w_gp(e_seq,
                                     base=8, h_r=0.05, loop=200, batch_ave=10,
                                     normalize=True):
     """
     bは相関係数を計算するためのバッチサイズです。
     プロットの直線部分が相関係数0.999以上の場合の最大の勾配をD_2としている。
     """
-    msg = 'It will not be available after version 0.2. ' \
-          'Use `calc_dimension_correlation` instead.'
-    _warnings.warn(msg)
-
     if normalize:
         v_max = e_seq.max(axis=0, keepdims=True)
         v_min = e_seq.min(axis=0, keepdims=True)
         e_seq = (e_seq-v_min)/(v_max-v_min)
 
     rs, crs = _calc_cr(e_seq, base, h_r, loop)
 
     correlation_max, slope = 0, None
     for i in range(len(crs)-batch_ave):
         log_cr, log_r = _np.log(crs[i:i+batch_ave]), _np.log(rs[i:i+batch_ave])
-        correlation = _np.corrcoef(log_cr, log_r)[0, 1]
+        correlation = _np.corrcoef(log_cr, log_r)[0,1]
         if (correlation >= 0.999) and (correlation > correlation_max):
-            slope, _ = _np.polyfit(log_r, log_cr, 1)
+            slope, _ = _np.polyfit(log_r, log_cr ,1)
             correlation_max = correlation
 
     return slope, rs, crs
```

### Comparing `hundun-0.1.39/hundun/exploration/_recurrenceplot.py` & `hundun-0.1.4/hundun/exploration/_recurrenceplot.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,43 +3,35 @@
 
 import numpy as _np
 
 from ..utils._draw import Drawing as _Drawing
 
 
 def simple_threshold(ds, theta=0.5):
-    if (d_max := _np.max(ds)) != 0:
-        pv = (ds/d_max > theta)*255
+    if (d_max:=_np.max(ds))!=0:
+        pv = (ds/d_max>theta)*255
         return pv
     return ds
 
 
-def calc_recurrence_plot(u_seq, rule=simple_threshold, *params, **kargs):
+def calc_recurrence_plot(u_seq, rule=simple_threshold, *params, **kwargs):
     size = len(u_seq)
-    rp = _np.zeros((size, size))
+    rp = _np.zeros((size,size))
 
-    ds = _np.array([_dist(u1, u2) for u1, u2 in _combinations(u_seq, 2)])
+    ds =  _np.array([_dist(u1, u2) for u1, u2 in _combinations(u_seq, 2)])
 
-    pv = rule(ds, *params, **kargs)
+    pv = rule(ds, *params, **kwargs)
 
-    rp[_np.triu(_np.ones((size, size), dtype=bool), k=1)] = pv
+    rp[_np.triu(_np.ones((size,size), dtype=bool), k=1)] = pv
 
     return rp+rp.T
 
 
-def show_recurrence_plot(u_seq, rule=simple_threshold, cmap=False,
-                         path_save_plot=None,
-                         *params, **kargs):
-    rp = calc_recurrence_plot(u_seq, rule, *params, **kargs)
+def show_recurrence_plot(u_seq, rule=simple_threshold, cmap=False, *params, **kwargs):
+    rp = calc_recurrence_plot(u_seq, rule, *params, **kwargs)
 
     d = _Drawing()
-    im = d[0, 0].imshow(rp, origin='lower')
+    im = d[0,0].imshow(rp, origin='lower')
     if cmap:
         d.fig.colorbar(im)
-
-    if path_save_plot is not None:
-        d.save(path_save_plot)
-
     d.show()
     d.close()
-
-    return rp
```

### Comparing `hundun-0.1.39/hundun/exploration/_utils.py` & `hundun-0.1.4/hundun/exploration/_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,65 @@
 from itertools import accumulate as _accumulate
 from operator import add as _add
 
 import numpy as _np
 from scipy import signal as _signal
-from scipy.stats import norm as _norm
 
 
 def reshape(u_seq):
-    if (ndim := u_seq.ndim) == 1:
+    if (ndim:=u_seq.ndim) == 1:
         u_seq = u_seq.reshape(len(u_seq), 1)
     elif ndim >= 3:
         raise NotImplementedError(f'{ndim} ndim is not supported')
     return u_seq
 
 
 def embedding_seq(u_seq, T, D):
-    idx = _np.arange(0, D, 1)*T
-    return _np.array([u_seq[idx+i, :] for i in range(len(u_seq)-(D-1)*T)])
+    idx = _np.arange(0,D,1)*T
+    return _np.array([u_seq[idx+i,:] for i in range(len(u_seq)-(D-1)*T)])
 
 
 def embedding_seq_1dim(u_seq, T, D):
-    idx = _np.arange(0, D, 1)*T
-    e_seq = _np.array([u_seq[idx+i, :] for i in range(len(u_seq)-(D-1)*T)])
+    idx = _np.arange(0,D,1)*T
+    e_seq = _np.array([u_seq[idx+i,:] for i in range(len(u_seq)-(D-1)*T)])
     return e_seq.reshape(len(e_seq), D)
 
 
 def embedding(u_seq, T, D):
     dim, length = u_seq.ndim, len(u_seq)
-    if len(u_seq.shape) == 1:
+    if len(u_seq.shape)==1:
         u_seq = u_seq.reshape(length, dim)
 
-    idx = _np.arange(0, D, 1)*T
-    e_seq = _np.array([u_seq[idx+i, :] for i in range(length-(D-1)*T)])
+    idx = _np.arange(0,D,1)*T
+    e_seq = _np.array([u_seq[idx+i,:] for i in range(length-(D-1)*T)])
 
     if u_seq.shape[1] == 1:
         e_seq = e_seq.reshape(len(e_seq), D)
     return e_seq
 
 
 def get_bottom(seq, threshold=float('inf')):
     _, dim = seq.shape
 
     lags = []
     for i in range(dim):
         us = seq[:, i]
         min_idx = _signal.argrelmin(us, order=1)[0]
-        candidate = min_idx[us[min_idx] <= threshold]
+        candidate = min_idx[us[min_idx]<=threshold]
         if len(candidate):
             lags.append(candidate[0])
         else:
             lags.append(None)
     return tuple(lags)
 
 
-def bartlett(seq, alpha=0.95):
-    _, dim = seq.shape
+def bartlett(seq):
+    N, dim = seq.shape
     N = len(seq)
     var = [_np.ones(dim)/N,
-           *[(1+2*rho)/N for rho in _accumulate(seq[1:, ]**2, _add)]]
-    z = _norm.ppf(alpha)
-    return z*_np.array(var)**(1/2)
+           *[(1+2*rho)/N for rho in _accumulate(seq[1:,]**2, _add)]]
+    return _np.array(var)**(1/2)
 
 
 def get_minidx_below_seq(rho_seq, var_seq):
     _, dim = rho_seq.shape
-    return [(rho_seq[:, i] < var_seq[:, i]).argmax() for i in range(dim)]
+    return [(rho_seq[:, i]<var_seq[:, i]).argmax() for i in range(dim)]
```

### Comparing `hundun-0.1.39/hundun/lyapunov/__init__.py` & `hundun-0.1.4/hundun/lyapunov/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 from ._les_differential import (calc_les_differential,
                                 calc_les_differential_w_qr,
                                 calc_max_le_differential,
                                 calc_les_differential_w_orth)
 from ._les_difference import calc_les_difference
 
 
-__all__ = ['calc_lyapunov_dimension', 'calc_les_differential_w_qr',
-           'calc_max_le_differential', 'calc_les_differential_w_orth']
-
 # def
 
 import numpy as _np
 
 from ..systems._systems import DynamicalSystems as _DynamicalSystems
 from ..systems._differential import Differential as _Differential
 from ..systems._difference import Difference as _Difference
@@ -25,8 +22,8 @@
 
     elif issubclass(system, _Difference):
         return calc_les_difference(system, **options)
 
     if not issubclass(system, _DynamicalSystems):
         raise TypeError(f"{system} must be a DynamicalSystems")
 
-    return _np.zeros((3, 3)), (0, 0, 0)
+    return _np.zeros((3, 3)), (None, None, None)
```

### Comparing `hundun-0.1.39/hundun/lyapunov/_func.py` & `hundun-0.1.4/hundun/lyapunov/_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from operator import add as _add
 
 import numpy as _np
 
 
 def _calc_lyapunov_dimension(les):
     sum_le = _np.array(list(_accumulate(les, _add)))
-    ok = les[sum_le > 0]
+    ok = les[sum_le>0]
     d = len(ok)
 
     return d + sum(ok)/_np.abs(les[d])
 
 
 def calc_lyapunov_dimension(les):
     if not isinstance(les, _np.ndarray):
```

### Comparing `hundun-0.1.39/hundun/lyapunov/_les_difference.py` & `hundun-0.1.4/hundun/lyapunov/_les_difference.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def calc_les_difference_dim_geq_2(difference, N, n_average=100):
     if difference.inf:
         raise ValueError('Initial value is outside basin of attraction')
 
     Q, R = _np.linalg.qr(difference.j())
 
-    R_list = [_np.diag(R)]
+    R_list= [_np.diag(R)]
     les = [_np.log(_np.abs(_np.diag(R)))]
     for _ in range(N):
         difference.solve(*difference.internal_state)
         J = difference.j()
         Q, R = _np.linalg.qr(J@Q)
         R_list.append(_np.diag(R))
         les.append(_np.log(_np.abs(_np.diag(R))))
@@ -35,18 +35,17 @@
 
 def calc_les_difference_dim_1(difference, N, n_average=100):
     le_list = []
     for _ in range(N):
         difference.solve(*difference.internal_state)
         le_list.append(_np.log(_np.abs(difference.j())))
     le_list = _np.array(
-        [le/i for i, le in enumerate(_accumulate(le_list, _add), 1)])
+        [le/i for i, le in enumerate(_accumulate(le_list, _add), 1) ])
     return le_list, _np.array([_np.average(le_list[-n_average:])])
 
-
 def _make_model(difference, u0=None, **options):
     if u0 is None:
         model = difference.on_attractor(u0=u0, **options)
     else:
         model = difference(**options)
         model.u, model.t = u0, 0
     return model
```

### Comparing `hundun-0.1.39/hundun/lyapunov/_les_differential.py` & `hundun-0.1.4/hundun/lyapunov/_les_differential.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 from itertools import accumulate as _accumulate
 from operator import add as _add
 
 import numpy as _np
 
 
-def sorting(_les_seq, _les, dim):
-    l = [(_les[i], _les_seq[:, i]) for i in range(dim)]  # noqa:
-    return _np.array([s[1] for s in l]).T, _np.array([s[0] for s in l])
-
-
 def calc_les_differential(differential, **options):
 
     if differential().jacobian() is None:
         return calc_les_differential_w_orth(differential, **options)
 
     else:
         return calc_les_differential_w_qr(differential, **options)
 
 
 def calc_les_differential_w_qr(differential,
-                               h=0.001, N=100000, u0=None, n_average=100,
-                               dynamic_para=None,
-                               error_func=False,
-                               dynamic_func=False,
-                               **options):
+                h=0.001, N=100000, u0=None, n_average=100,
+                dynamic_para=None,
+                error_func=False,
+                **options):
 
     model = _make_model(differential, h=h, u0=u0, **options)
 
-    if error_func or dynamic_func:
+    if error_func:
         jacobian = model.dynamic_jacobian
         func_solve = lambda t, u, **option : \
-            model.solve(t, u, f=model.dynamic_eq, **option)  # noqa:
+            model.solve(t, u, f=model.dynamic_eq, **option)
     else:
         jacobian = model.j
         func_solve = model.solve
 
     # main
     dim = model.dim
 
@@ -48,30 +42,28 @@
 
         les.append(_np.log(_np.abs(R.diagonal())))
 
         func_solve(model.t, model.u, h=h, **p)
 
     les_list = [l/(i*h) for i, l in enumerate(_accumulate(les, _add), 1)]
     les_average = _np.average(les_list[-n_average:], axis=0)
-    return sorting(_np.array(les_list), les_average, dim)
+    return _np.array(les_list), sorted(les_average, reverse=True)
 
 
 def calc_max_le_differential(differential,
-                             h=0.01, N=10000, u0=None, n_average=100,
-                             n_split=10,
-                             dynamic_para=None,
-                             error_func=False,
-                             dynamic_func=False,
-                             **options):
+                     h=0.01, N=10000, u0=None, n_average=100, n_split=10,
+                     dynamic_para=None,
+                     error_func=False,
+                     **options):
 
     model = _make_model(differential, u0=u0, h=h, **options)
 
-    if error_func or dynamic_func:
-        func_solve = lambda t, u, **option: \
-            model.solve(t, u, f=model.dynamic_eq, **option)  # noqa:
+    if error_func:
+        func_solve = lambda t, u, **option : \
+            model.solve(t, u, f=model.dynamic_eq, **option)
     else:
         func_solve = model.solve
 
     # main
     w_s = _np.random.random(model.dim)*(10**(-3))
     z_0 = _np.linalg.norm(w_s)
 
@@ -95,35 +87,34 @@
         for j in range(n_split):
             d = dp[i*n_split+j]
             _, u = func_solve(i*n_split*h+j*h, u, h=h, **d)
 
         w_e = u - u_tilde
         v += _np.log(_np.linalg.norm(w_e)*(1/z_0))
 
-        T = (1/n_split)*(i+2)
+        T=(1/n_split)*(i+2)
         les_list.append(v/T)
 
         w_s = z_0/_np.linalg.norm(w_e)*w_e
         u = u_tilde+w_s
 
     return les_list, _np.average(les_list[-n_average:])
 
 
 def calc_les_differential_w_orth(differential,
-                                 h=0.01, N=10000, u0=None, n_average=100,
-                                 dynamic_para=None,
-                                 error_func=False,
-                                 dynamic_func=False,
-                                 **options):
+                  h=0.01, N=10000, u0=None, n_average=100,
+                  dynamic_para=None,
+                  error_func=False,
+                  **options):
 
     model = _make_model(differential, u0=u0, h=h, **options)
 
-    if error_func or dynamic_func:
-        func_solve = lambda t, u, **option: \
-            model.solve(t, u, f=model.dynamic_eq, **option)  # noqa:
+    if error_func:
+        func_solve = lambda t, u, **option : \
+            model.solve(t, u, f=model.dynamic_eq, **option)
     else:
         func_solve = model.solve
 
     dim = model.dim
 
     # main
     d_0 = _np.array([_np.random.rand(dim) for _ in range(dim)])
@@ -146,37 +137,37 @@
             d_tau.append(u_hat[i] - u_tilde)
         d_tau = _np.array(d_tau)
 
         d_tau_bot = _np.linalg.qr(d_tau.T)[0].T
 
         for i in range(dim):
             on = _np.linalg.norm(d_0[i])
-            d_0[i] = on * d_tau_bot[i]
+            d_0[i] =  on * d_tau_bot[i]
             u_hat[i] = u_tilde + d_0[i]
 
         d_ups, d_downs = _np.ones(3), _np.ones(3)
         for i in range(dim):
             d_ups = _np.linalg.norm(_np.outer(d_ups, d_tau[i]))
             d_downs = _np.linalg.norm(_np.outer(d_downs, d_0[i]))
 
             lm[i].append(_np.log(d_ups / d_downs))
 
-    calc_l = lambda l: [sum(l[:i])/(i*h) for i in range(1, len(l)+1)]  # noqa:
-    les_plus_list = [_np.array(calc_l(l)) for l in lm]  # noqa:
+    calc_l = lambda l : [sum(l[:i])/(i*h) for i in range(1, len(l)+1)]
+    les_plus_list = [_np.array(calc_l(l)) for l in lm]
 
     les_list = []
     les_list.append(les_plus_list[0])
     for i in range(1, dim):
         les_list.append(les_plus_list[i] - les_plus_list[i-1])
-    les_average = [_np.average(les[-n_average:]) for les in les_list]
+    les_average = [_np.average(l[-n_average:]) for l in les_list]
 
-    les_average = sorted(les_average, reverse=True)
-    return sorting(_np.array(les_list).T, les_average, dim)
+    les_average=sorted(les_average, reverse=True)
+    return _np.array(les_list).T, les_average
 
 
 def _make_model(differential, u0=None, h=0.01, **options):
     if u0 is None:
-        model = differential.on_attractor(h=h, **options)
+        model = differential.on_attractor(**options)
     else:
         model = differential(**options)
         model.u, model.t = u0, 0
     return model
```

### Comparing `hundun-0.1.39/hundun/systems/_solver.py` & `hundun-0.1.4/hundun/systems/_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 
 
 def solve_simple(f, t0, u0, n_loop, *, h=0.01, solver=RK4):
     sol = solver(f, h=h)
     u = _np.array(u0)
     t_seq = [t0 + i*h for i in range(n_loop)]
 
-    u_seq = _np.array([u0, *[u := sol(t, u) for t in t_seq]])  # noqa:
+    u_seq = _np.array([u0, *[u := sol(t, u) for t in t_seq]])
     t_seq = _np.array([*t_seq, t0 + n_loop*h])
     return t_seq, u_seq
```

### Comparing `hundun-0.1.39/hundun/systems/_sync.py` & `hundun-0.1.4/hundun/systems/_sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     @_abstractmethod
     def supporting(self):
         '''supporting model'''
 
     def set_model(self, shift=0):
         dq = _deque([self.leading, self.supporting])
         dq.rotate(shift)
-        self._cyc = _cycle(dq)
+        self._cyc =_cycle(dq)
         return self._cyc
 
     def _sync(self):
         return next(self._cyc)
 
     def get_signal(self):
         if self._signal_seq is None:
@@ -49,33 +49,33 @@
             return next(self._cyc)
         except AttributeError:
             raise AttributeError(f'need {self.__class__.__name__}.set_model()')
 
 
 def _make_parameter(func, params):
     signals = _getfullargspec(func).args
-    params = {s: p for s, p in zip(signals[3:], params)}
+    params = {s:p for s, p in zip(signals[3:], params)}
     params['f'] = func
     return params
 
 
 def _check_oscillator(oscillators):
     for o in oscillators:
         if not isinstance(o, Synchronization):
             raise TypeError(
                 f'{o.__class__.__name__} need to have Synchronization')
 
 
-def coupling_oneway(o1, o2, N, **params):
+def coupling_oneway(o1, o2, N):
     _check_oscillator([o1, o2])
 
     for _ in range(N):
         signal1 = o1.get_signal()
         signal2 = o2.get_signal()
 
         params1 = _make_parameter(o1.leading, [signal2])
         params2 = _make_parameter(o2.supporting, [signal1])
 
-        o1.solve(*o1.internal_state, **dict(params1, **params))
-        o2.solve(*o2.internal_state, **dict(params2, **params))
+        o1.solve(*o1.internal_state, **params1)
+        o2.solve(*o2.internal_state, **params2)
 
     return o1, o2
```

### Comparing `hundun-0.1.39/hundun/systems/_systems.py` & `hundun-0.1.4/hundun/systems/_systems.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,31 +5,29 @@
 import numpy as _np
 
 from ._tu import TU as _TU
 
 
 class DynamicalSystems(_ABC):
 
-    def __init__(self, t=None, u=None, **params):
+    def __init__(self, t=None, u=None):
         self.dim = 0
         self.parameter()
 
         if self.dim == 0:
             class_name = self.__class__.__name__
             msg = (f"need to set {class_name}'s dimension "
                    f"({class_name}.dim=? in parameter())")
             raise NotImplementedError(msg)
 
         self.t = t or 0
         self.u = u if u is not None else _np.zeros(self.dim)
 
         self._t_seq, self._u_seq = [], []
 
-        self.parameter(**params)
-
     @property
     def inf(self):
         return any(_np.isinf(self.u))
 
     @property
     def internal_state(self):
         return _TU(self.t, self.u)
@@ -45,20 +43,14 @@
     @classmethod
     def on_attractor(cls, t0=None, u0=None, h=0.01, *, T_0=5000, **params):
         c = cls(t0, u0)
         c.parameter(**params)
         c.settle_on_attractor(t0, u0, h=h, T_0=T_0)
         return c
 
-    @classmethod
-    def get_u_seq(cls, n, *args, **kwargs):
-        c = cls.on_attractor(*args, **kwargs)
-        c.solve_n_times(n)
-        return c.u_seq
-
     @_abstractmethod
     def equation(self, t, u):
         """equation"""
 
     def j(self, **params):
         return _np.array(self.jacobian(**params))
```

### Comparing `hundun-0.1.39/hundun.egg-info/SOURCES.txt` & `hundun-0.1.4/hundun.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 LICENSE.txt
 MANIFEST.in
 README.md
-pyproject.toml
+setup.py
 hundun/__init__.py
+hundun/__version__.py
 hundun.egg-info/PKG-INFO
 hundun.egg-info/SOURCES.txt
 hundun.egg-info/dependency_links.txt
+hundun.egg-info/not-zip-safe
 hundun.egg-info/requires.txt
 hundun.egg-info/top_level.txt
 hundun/equations/__init__.py
 hundun/equations/henon.py
 hundun/equations/logistic.py
 hundun/equations/lorenz.py
 hundun/exploration/__init__.py
 hundun/exploration/_afn.py
 hundun/exploration/_autocorrelation.py
-hundun/exploration/_box3.py
 hundun/exploration/_fnn.py
 hundun/exploration/_gp.py
 hundun/exploration/_mutualinfo.py
 hundun/exploration/_recurrenceplot.py
 hundun/exploration/_utils.py
 hundun/exploration/_wayland.py
 hundun/lyapunov/__init__.py
```

