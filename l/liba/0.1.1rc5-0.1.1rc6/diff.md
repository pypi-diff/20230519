# Comparing `tmp/liba-0.1.1rc5.tar.gz` & `tmp/liba-0.1.1rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liba-0.1.1rc5.tar", last modified: Tue May  9 18:20:15 2023, max compression
+gzip compressed data, was "liba-0.1.1rc6.tar", last modified: Fri May 19 18:00:36 2023, max compression
```

## Comparing `liba-0.1.1rc5.tar` & `liba-0.1.1rc6.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 18:20:15.572435 liba-0.1.1rc5/
--rwxrwxrwx   0 root         (0) root         (0)       87 2023-05-06 04:29:13.000000 liba-0.1.1rc5/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     5665 2023-05-09 18:20:15.573433 liba-0.1.1rc5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3770 2023-05-06 04:29:13.000000 liba-0.1.1rc5/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 18:20:15.484013 liba-0.1.1rc5/include/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 18:20:15.519277 liba-0.1.1rc5/include/a/
--rwxrwxrwx   0 root         (0) root         (0)    40329 2023-05-07 19:41:55.000000 liba-0.1.1rc5/include/a/a.h
--rwxrwxrwx   0 root         (0) root         (0)     9641 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/avl.h
--rwxrwxrwx   0 root         (0) root         (0)    11297 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/buf.h
--rwxrwxrwx   0 root         (0) root         (0)    12712 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/complex.h
--rwxrwxrwx   0 root         (0) root         (0)     1949 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/crc.h
--rwxrwxrwx   0 root         (0) root         (0)    10250 2023-05-08 07:14:56.000000 liba-0.1.1rc5/include/a/fpid.h
--rwxrwxrwx   0 root         (0) root         (0)     1416 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/fuzzy.h
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 18:20:15.524906 liba-0.1.1rc5/include/a/host/
--rwxrwxrwx   0 root         (0) root         (0)      731 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/host/a.h
--rwxrwxrwx   0 root         (0) root         (0)    10149 2023-05-07 16:15:03.000000 liba-0.1.1rc5/include/a/host/que.h
--rwxrwxrwx   0 root         (0) root         (0)     8826 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/host/str.h
--rwxrwxrwx   0 root         (0) root         (0)    13105 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/host/vec.h
--rwxrwxrwx   0 root         (0) root         (0)    13539 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/host/vector.h
--rwxrwxrwx   0 root         (0) root         (0)    14260 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/list.h
--rwxrwxrwx   0 root         (0) root         (0)     5324 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/math.h
--rwxrwxrwx   0 root         (0) root         (0)     3350 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/mf.h
--rwxrwxrwx   0 root         (0) root         (0)   111610 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/notefreqs.h
--rwxrwxrwx   0 root         (0) root         (0)     3133 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/oop.h
--rwxrwxrwx   0 root         (0) root         (0)     2277 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/operator.h
--rwxrwxrwx   0 root         (0) root         (0)     9574 2023-05-08 06:38:14.000000 liba-0.1.1rc5/include/a/pid.h
--rwxrwxrwx   0 root         (0) root         (0)     1295 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/poly.h
--rwxrwxrwx   0 root         (0) root         (0)    16402 2023-05-08 10:18:52.000000 liba-0.1.1rc5/include/a/polytrack.h
--rwxrwxrwx   0 root         (0) root         (0)     9917 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/rbt.h
--rwxrwxrwx   0 root         (0) root         (0)     3499 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/real.h
--rwxrwxrwx   0 root         (0) root         (0)     7095 2023-05-07 15:31:27.000000 liba-0.1.1rc5/include/a/slist.h
--rwxrwxrwx   0 root         (0) root         (0)     2244 2023-05-09 10:41:29.000000 liba-0.1.1rc5/include/a/tf.h
--rwxrwxrwx   0 root         (0) root         (0)     1552 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/utf.h
--rwxrwxrwx   0 root         (0) root         (0)     7698 2023-05-06 04:29:13.000000 liba-0.1.1rc5/include/a/version.h
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 18:20:15.530475 liba-0.1.1rc5/liba.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5665 2023-05-09 18:20:15.000000 liba-0.1.1rc5/liba.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1405 2023-05-09 18:20:15.000000 liba-0.1.1rc5/liba.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-09 18:20:15.000000 liba-0.1.1rc5/liba.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-05-09 18:20:15.000000 liba-0.1.1rc5/liba.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       92 2023-05-06 04:29:13.000000 liba-0.1.1rc5/pyproject.toml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 18:20:15.486369 liba-0.1.1rc5/python/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 18:20:15.532884 liba-0.1.1rc5/python/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 18:20:15.551687 liba-0.1.1rc5/python/src/a/
--rwxrwxrwx   0 root         (0) root         (0)     1393 2023-05-06 04:29:13.000000 liba-0.1.1rc5/python/src/a/__init__.pxd
--rwxrwxrwx   0 root         (0) root         (0)       20 2023-05-06 04:29:13.000000 liba-0.1.1rc5/python/src/a/__init__.pxi
--rwxrwxrwx   0 root         (0) root         (0)     1457 2023-05-07 22:37:50.000000 liba-0.1.1rc5/python/src/a/fpid.pxd
--rwxrwxrwx   0 root         (0) root         (0)     4988 2023-05-08 10:34:17.000000 liba-0.1.1rc5/python/src/a/fpid.pxi
--rwxrwxrwx   0 root         (0) root         (0)      117 2023-05-06 04:29:13.000000 liba-0.1.1rc5/python/src/a/math.pxd
--rwxrwxrwx   0 root         (0) root         (0)      544 2023-05-06 04:29:13.000000 liba-0.1.1rc5/python/src/a/math.pxi
--rwxrwxrwx   0 root         (0) root         (0)      651 2023-05-06 04:29:13.000000 liba-0.1.1rc5/python/src/a/mf.pxd
--rwxrwxrwx   0 root         (0) root         (0)     2427 2023-05-06 04:29:13.000000 liba-0.1.1rc5/python/src/a/mf.pxi
--rwxrwxrwx   0 root         (0) root         (0)     1602 2023-05-08 06:55:51.000000 liba-0.1.1rc5/python/src/a/pid.pxd
--rwxrwxrwx   0 root         (0) root         (0)     3032 2023-05-08 10:34:25.000000 liba-0.1.1rc5/python/src/a/pid.pxi
--rwxrwxrwx   0 root         (0) root         (0)      449 2023-05-06 04:29:13.000000 liba-0.1.1rc5/python/src/a/poly.pxd
--rwxrwxrwx   0 root         (0) root         (0)      710 2023-05-06 04:29:13.000000 liba-0.1.1rc5/python/src/a/poly.pxi
--rwxrwxrwx   0 root         (0) root         (0)     2798 2023-05-06 04:29:13.000000 liba-0.1.1rc5/python/src/a/polytrack.pxd
--rwxrwxrwx   0 root         (0) root         (0)    11291 2023-05-07 16:37:07.000000 liba-0.1.1rc5/python/src/a/polytrack.pxi
--rwxrwxrwx   0 root         (0) root         (0)      504 2023-05-09 10:41:29.000000 liba-0.1.1rc5/python/src/a/tf.pxd
--rwxrwxrwx   0 root         (0) root         (0)     1297 2023-05-09 10:41:29.000000 liba-0.1.1rc5/python/src/a/tf.pxi
--rwxrwxrwx   0 root         (0) root         (0)      168 2023-05-06 04:29:13.000000 liba-0.1.1rc5/python/src/a/version.pxd
--rwxrwxrwx   0 root         (0) root         (0)      481 2023-05-06 04:29:13.000000 liba-0.1.1rc5/python/src/a/version.pxi
--rwxrwxrwx   0 root         (0) root         (0)  1287495 2023-05-09 18:20:10.000000 liba-0.1.1rc5/python/src/a.c
--rwxrwxrwx   0 root         (0) root         (0)      494 2023-05-06 04:29:13.000000 liba-0.1.1rc5/python/src/a.pyx
--rwxrwxrwx   0 root         (0) root         (0)      567 2023-05-09 18:20:15.573433 liba-0.1.1rc5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     6135 2023-05-06 04:29:13.000000 liba-0.1.1rc5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 18:20:15.567449 liba-0.1.1rc5/src/
--rwxrwxrwx   0 root         (0) root         (0)     1672 2023-05-06 10:11:24.000000 liba-0.1.1rc5/src/a.c
--rwxrwxrwx   0 root         (0) root         (0)    25528 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/avl.c
--rwxrwxrwx   0 root         (0) root         (0)     4688 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/buf.c
--rwxrwxrwx   0 root         (0) root         (0)    23728 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/complex.c
--rwxrwxrwx   0 root         (0) root         (0)      648 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/complex.h
--rwxrwxrwx   0 root         (0) root         (0)     5503 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/crc.c
--rwxrwxrwx   0 root         (0) root         (0)     7137 2023-05-09 10:41:29.000000 liba-0.1.1rc5/src/fpid.c
--rwxrwxrwx   0 root         (0) root         (0)      504 2023-05-07 19:03:08.000000 liba-0.1.1rc5/src/fpid.h
--rwxrwxrwx   0 root         (0) root         (0)      811 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/fuzzy.c
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 18:20:15.572435 liba-0.1.1rc5/src/host/
--rwxrwxrwx   0 root         (0) root         (0)      551 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/host/a.c
--rwxrwxrwx   0 root         (0) root         (0)     9439 2023-05-07 16:12:39.000000 liba-0.1.1rc5/src/host/que.c
--rwxrwxrwx   0 root         (0) root         (0)     5684 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/host/str.c
--rwxrwxrwx   0 root         (0) root         (0)     6897 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/host/vec.c
--rwxrwxrwx   0 root         (0) root         (0)     8277 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/host/vector.c
--rwxrwxrwx   0 root         (0) root         (0)     4776 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/math.c
--rwxrwxrwx   0 root         (0) root         (0)      257 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/math.h
--rwxrwxrwx   0 root         (0) root         (0)     2329 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/mf.c
--rwxrwxrwx   0 root         (0) root         (0)     5585 2023-05-08 06:53:04.000000 liba-0.1.1rc5/src/pid.c
--rwxrwxrwx   0 root         (0) root         (0)      441 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/pid.h
--rwxrwxrwx   0 root         (0) root         (0)     1407 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/poly.c
--rwxrwxrwx   0 root         (0) root         (0)    11249 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/polytrack.c
--rwxrwxrwx   0 root         (0) root         (0)    24524 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/rbt.c
--rwxrwxrwx   0 root         (0) root         (0)      877 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/real.c
--rwxrwxrwx   0 root         (0) root         (0)     1432 2023-05-09 10:41:29.000000 liba-0.1.1rc5/src/tf.c
--rwxrwxrwx   0 root         (0) root         (0)     2887 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/utf.c
--rwxrwxrwx   0 root         (0) root         (0)     1213 2023-05-06 04:29:13.000000 liba-0.1.1rc5/src/version.c
+drwxrwxrwx   0        0        0        0 2023-05-19 18:00:36.568374 liba-0.1.1rc6/
+-rw-rw-rw-   0        0        0    16727 2023-04-16 10:53:49.000000 liba-0.1.1rc6/LICENSE.txt
+-rw-rw-rw-   0        0        0       87 2023-05-06 04:29:13.000000 liba-0.1.1rc6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4517 2023-05-19 18:00:36.568374 liba-0.1.1rc6/PKG-INFO
+-rw-rw-rw-   0        0        0     3770 2023-05-06 04:29:13.000000 liba-0.1.1rc6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 18:00:36.448805 liba-0.1.1rc6/include/
+drwxrwxrwx   0        0        0        0 2023-05-19 18:00:36.487591 liba-0.1.1rc6/include/a/
+-rw-rw-rw-   0        0        0    40337 2023-05-14 06:54:59.000000 liba-0.1.1rc6/include/a/a.h
+-rw-rw-rw-   0        0        0     9641 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/avl.h
+-rw-rw-rw-   0        0        0    11297 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/buf.h
+-rw-rw-rw-   0        0        0    12712 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/complex.h
+-rw-rw-rw-   0        0        0     1949 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/crc.h
+-rw-rw-rw-   0        0        0    10381 2023-05-16 13:05:57.000000 liba-0.1.1rc6/include/a/fpid.h
+-rw-rw-rw-   0        0        0     1416 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/fuzzy.h
+drwxrwxrwx   0        0        0        0 2023-05-19 18:00:36.495254 liba-0.1.1rc6/include/a/host/
+-rw-rw-rw-   0        0        0      731 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/host/a.h
+-rw-rw-rw-   0        0        0    10149 2023-05-07 16:15:03.000000 liba-0.1.1rc6/include/a/host/que.h
+-rw-rw-rw-   0        0        0     8826 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/host/str.h
+-rw-rw-rw-   0        0        0    13105 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/host/vec.h
+-rw-rw-rw-   0        0        0    13539 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/host/vector.h
+-rw-rw-rw-   0        0        0    14260 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/list.h
+-rw-rw-rw-   0        0        0     5525 2023-05-16 10:53:09.000000 liba-0.1.1rc6/include/a/math.h
+-rw-rw-rw-   0        0        0     3350 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/mf.h
+-rw-rw-rw-   0        0        0   111610 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/notefreqs.h
+-rw-rw-rw-   0        0        0     3133 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/oop.h
+-rw-rw-rw-   0        0        0     2277 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/operator.h
+-rw-rw-rw-   0        0        0     9592 2023-05-16 11:24:27.000000 liba-0.1.1rc6/include/a/pid.h
+-rw-rw-rw-   0        0        0     1295 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/poly.h
+-rw-rw-rw-   0        0        0    12547 2023-05-19 15:24:44.000000 liba-0.1.1rc6/include/a/polytrack.h
+-rw-rw-rw-   0        0        0     9917 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/rbt.h
+-rw-rw-rw-   0        0        0     3499 2023-05-06 04:29:13.000000 liba-0.1.1rc6/include/a/real.h
+-rw-rw-rw-   0        0        0     7095 2023-05-07 15:31:27.000000 liba-0.1.1rc6/include/a/slist.h
+-rw-rw-rw-   0        0        0     2244 2023-05-09 10:41:29.000000 liba-0.1.1rc6/include/a/tf.h
+-rw-rw-rw-   0        0        0     1597 2023-05-17 19:12:49.000000 liba-0.1.1rc6/include/a/utf.h
+-rw-rw-rw-   0        0        0     7813 2023-05-18 08:36:26.000000 liba-0.1.1rc6/include/a/version.h
+drwxrwxrwx   0        0        0        0 2023-05-19 18:00:36.501576 liba-0.1.1rc6/liba.egg-info/
+-rw-rw-rw-   0        0        0     4517 2023-05-19 18:00:36.000000 liba-0.1.1rc6/liba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1432 2023-05-19 18:00:36.000000 liba-0.1.1rc6/liba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 18:00:36.000000 liba-0.1.1rc6/liba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-19 18:00:36.000000 liba-0.1.1rc6/liba.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       92 2023-05-06 04:29:13.000000 liba-0.1.1rc6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-19 18:00:36.450800 liba-0.1.1rc6/python/
+drwxrwxrwx   0        0        0        0 2023-05-19 18:00:36.505576 liba-0.1.1rc6/python/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 18:00:36.532514 liba-0.1.1rc6/python/src/a/
+-rw-rw-rw-   0        0        0     1393 2023-05-10 07:52:27.000000 liba-0.1.1rc6/python/src/a/__init__.pxd
+-rw-rw-rw-   0        0        0       20 2023-05-06 04:29:13.000000 liba-0.1.1rc6/python/src/a/__init__.pxi
+-rw-rw-rw-   0        0        0     1475 2023-05-16 11:29:18.000000 liba-0.1.1rc6/python/src/a/fpid.pxd
+-rw-rw-rw-   0        0        0     4988 2023-05-10 07:52:27.000000 liba-0.1.1rc6/python/src/a/fpid.pxi
+-rw-rw-rw-   0        0        0      117 2023-05-06 04:29:13.000000 liba-0.1.1rc6/python/src/a/math.pxd
+-rw-rw-rw-   0        0        0      544 2023-05-06 04:29:13.000000 liba-0.1.1rc6/python/src/a/math.pxi
+-rw-rw-rw-   0        0        0      651 2023-05-06 04:29:13.000000 liba-0.1.1rc6/python/src/a/mf.pxd
+-rw-rw-rw-   0        0        0     2427 2023-05-06 04:29:13.000000 liba-0.1.1rc6/python/src/a/mf.pxi
+-rw-rw-rw-   0        0        0     1620 2023-05-16 11:26:38.000000 liba-0.1.1rc6/python/src/a/pid.pxd
+-rw-rw-rw-   0        0        0     3032 2023-05-10 07:52:27.000000 liba-0.1.1rc6/python/src/a/pid.pxi
+-rw-rw-rw-   0        0        0      449 2023-05-06 04:29:13.000000 liba-0.1.1rc6/python/src/a/poly.pxd
+-rw-rw-rw-   0        0        0      710 2023-05-06 04:29:13.000000 liba-0.1.1rc6/python/src/a/poly.pxi
+-rw-rw-rw-   0        0        0     1652 2023-05-19 15:32:46.000000 liba-0.1.1rc6/python/src/a/polytrack.pxd
+-rw-rw-rw-   0        0        0     6272 2023-05-19 15:31:52.000000 liba-0.1.1rc6/python/src/a/polytrack.pxi
+-rw-rw-rw-   0        0        0      504 2023-05-09 10:41:29.000000 liba-0.1.1rc6/python/src/a/tf.pxd
+-rw-rw-rw-   0        0        0     1297 2023-05-09 10:41:29.000000 liba-0.1.1rc6/python/src/a/tf.pxi
+-rw-rw-rw-   0        0        0      168 2023-05-06 04:29:13.000000 liba-0.1.1rc6/python/src/a/version.pxd
+-rw-rw-rw-   0        0        0      481 2023-05-06 04:29:13.000000 liba-0.1.1rc6/python/src/a/version.pxi
+-rw-rw-rw-   0        0        0  1133561 2023-05-19 15:32:55.000000 liba-0.1.1rc6/python/src/a.c
+-rw-rw-rw-   0        0        0      494 2023-05-06 04:29:13.000000 liba-0.1.1rc6/python/src/a.pyx
+-rw-rw-rw-   0        0        0      590 2023-05-19 18:00:36.569397 liba-0.1.1rc6/setup.cfg
+-rw-rw-rw-   0        0        0     6135 2023-05-06 04:29:13.000000 liba-0.1.1rc6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:00:36.560396 liba-0.1.1rc6/src/
+-rw-rw-rw-   0        0        0     1672 2023-05-16 10:52:49.000000 liba-0.1.1rc6/src/a.c
+-rw-rw-rw-   0        0        0    25528 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/avl.c
+-rw-rw-rw-   0        0        0     4688 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/buf.c
+-rw-rw-rw-   0        0        0    23728 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/complex.c
+-rw-rw-rw-   0        0        0      648 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/complex.h
+-rw-rw-rw-   0        0        0     5503 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/crc.c
+-rw-rw-rw-   0        0        0     7171 2023-05-16 13:16:52.000000 liba-0.1.1rc6/src/fpid.c
+-rw-rw-rw-   0        0        0      484 2023-05-16 10:53:09.000000 liba-0.1.1rc6/src/fpid.h
+-rw-rw-rw-   0        0        0      800 2023-05-16 13:16:39.000000 liba-0.1.1rc6/src/fuzzy.c
+drwxrwxrwx   0        0        0        0 2023-05-19 18:00:36.567404 liba-0.1.1rc6/src/host/
+-rw-rw-rw-   0        0        0      551 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/host/a.c
+-rw-rw-rw-   0        0        0     9439 2023-05-07 16:12:39.000000 liba-0.1.1rc6/src/host/que.c
+-rw-rw-rw-   0        0        0     5684 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/host/str.c
+-rw-rw-rw-   0        0        0     6897 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/host/vec.c
+-rw-rw-rw-   0        0        0     8277 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/host/vector.c
+-rw-rw-rw-   0        0        0     4776 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/math.c
+-rw-rw-rw-   0        0        0      257 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/math.h
+-rw-rw-rw-   0        0        0     2329 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/mf.c
+-rw-rw-rw-   0        0        0     5335 2023-05-16 11:23:59.000000 liba-0.1.1rc6/src/pid.c
+-rw-rw-rw-   0        0        0      461 2023-05-16 10:53:09.000000 liba-0.1.1rc6/src/pid.h
+-rw-rw-rw-   0        0        0     1407 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/poly.c
+-rw-rw-rw-   0        0        0     7783 2023-05-19 15:23:08.000000 liba-0.1.1rc6/src/polytrack.c
+-rw-rw-rw-   0        0        0    24524 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/rbt.c
+-rw-rw-rw-   0        0        0      877 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/real.c
+-rw-rw-rw-   0        0        0     1432 2023-05-09 10:41:29.000000 liba-0.1.1rc6/src/tf.c
+-rw-rw-rw-   0        0        0     2890 2023-05-17 19:12:04.000000 liba-0.1.1rc6/src/utf.c
+-rw-rw-rw-   0        0        0     1213 2023-05-06 04:29:13.000000 liba-0.1.1rc6/src/version.c
```

### Comparing `liba-0.1.1rc5/README.md` & `liba-0.1.1rc6/README.md`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/a.h` & `liba-0.1.1rc6/include/a/a.h`

 * *Files 0% similar despite different names*

```diff
@@ -1051,16 +1051,16 @@
 #define a_real_p(x) a_cast_s(A_REAL_T *, x)
 #define A_REAL_P(x) a_cast_s(A_REAL_T const *, x)
 /*! compiler built-in real number type */
 #define a_real_t A_REAL_T
 
 typedef union a_real_u
 {
-    a_real_t v; //!< a real value
-    a_real_t *p; //!< real vector
+    a_real_t f; //!< as a real number
+    a_real_t *p; //!< as a real array
 } a_real_u;
 
 #if defined(__cplusplus)
 namespace a
 {
 
 typedef a_real_t real_t;
```

### Comparing `liba-0.1.1rc5/include/a/avl.h` & `liba-0.1.1rc6/include/a/avl.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/buf.h` & `liba-0.1.1rc6/include/a/buf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/complex.h` & `liba-0.1.1rc6/include/a/complex.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/crc.h` & `liba-0.1.1rc6/include/a/crc.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/fpid.h` & `liba-0.1.1rc6/include/a/fpid.h`

 * *Files 4% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 #define A_FPID_FUZZY_MASK (~((1U << A_FPID_FUZZY_BITL) - 1U) & ((1U << A_FPID_FUZZY_BITH) - 1U))
 
 /*!
  @brief instance enumeration for fuzzy PID controller operator
 */
 typedef enum a_fpid_e
 {
-    A_FPID_EQU,
+    A_FPID_EQU, //!< sqrt(l,r)*sqrt(1-(1-r)*(1-r))
     A_FPID_AND = (1 << (A_FPID_FUZZY_BITL + 2)), // 00010000 + 0100 * 0
-    A_FPID_AND_DEFAULT = A_FPID_AND + (A_FUZZY_DEFAULT << A_FPID_FUZZY_BITL),
-    A_FPID_AND_ALGEBRA = A_FPID_AND + (A_FUZZY_ALGEBRA << A_FPID_FUZZY_BITL),
-    A_FPID_AND_BOUNDED = A_FPID_AND + (A_FUZZY_BOUNDED << A_FPID_FUZZY_BITL),
+    A_FPID_AND_DEFAULT = A_FPID_AND + (A_FUZZY_DEFAULT << A_FPID_FUZZY_BITL), //!< min(l,r)
+    A_FPID_AND_ALGEBRA = A_FPID_AND + (A_FUZZY_ALGEBRA << A_FPID_FUZZY_BITL), //!< l*r
+    A_FPID_AND_BOUNDED = A_FPID_AND + (A_FUZZY_BOUNDED << A_FPID_FUZZY_BITL), //!< max(l,r)
     A_FPID_OR = (1 << (A_FPID_FUZZY_BITL + 3)), // 00100000 + 0100 * 0
-    A_FPID_OR_DEFAULT = A_FPID_OR + (A_FUZZY_DEFAULT << A_FPID_FUZZY_BITL),
-    A_FPID_OR_ALGEBRA = A_FPID_OR + (A_FUZZY_ALGEBRA << A_FPID_FUZZY_BITL),
-    A_FPID_OR_BOUNDED = A_FPID_OR + (A_FUZZY_BOUNDED << A_FPID_FUZZY_BITL)
+    A_FPID_OR_DEFAULT = A_FPID_OR + (A_FUZZY_DEFAULT << A_FPID_FUZZY_BITL), //!< max(l,r)
+    A_FPID_OR_ALGEBRA = A_FPID_OR + (A_FUZZY_ALGEBRA << A_FPID_FUZZY_BITL), //!< l+r-l*r
+    A_FPID_OR_BOUNDED = A_FPID_OR + (A_FUZZY_BOUNDED << A_FPID_FUZZY_BITL) //!< min(l,r)
 } a_fpid_e;
 
 /*!
  @brief instance structure for fuzzy PID controller
 */
 typedef struct a_fpid_s
 {
@@ -237,25 +237,25 @@
  @brief calculate function for fuzzy PID controller
  @param[in,out] ctx points to an instance of fuzzy PID controller
  @param[in] set setpoint
  @param[in] fdb feedback
  @return output value
   @retval set when fuzzy PID controller is off
 */
-A_EXTERN a_real_t a_fpid_outv(a_fpid_s *ctx, a_real_t set, a_real_t fdb);
+A_EXTERN a_real_t a_fpid_outf(a_fpid_s *ctx, a_real_t set, a_real_t fdb);
 
 /*!
  @brief calculate function for multichannel fuzzy PID controller
  @param[in,out] ctx points to an instance of fuzzy PID controller
  @param[in] set points to setpoint
  @param[in] fdb points to feedback
  @return points to output
   @retval set when fuzzy PID controller is off
 */
-A_EXTERN a_real_t *a_fpid_outp(a_fpid_s *ctx, a_real_t *set, a_real_t *fdb);
+A_EXTERN a_real_t const *a_fpid_outp(a_fpid_s *ctx, a_real_t const *set, a_real_t const *fdb);
 
 /*!
  @brief terminate function for fuzzy PID controller
  @param[in,out] ctx points to an instance of fuzzy PID controller
 */
 A_EXTERN a_fpid_s *a_fpid_exit(a_fpid_s *ctx);
```

### Comparing `liba-0.1.1rc5/include/a/fuzzy.h` & `liba-0.1.1rc6/include/a/fuzzy.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/host/a.h` & `liba-0.1.1rc6/include/a/host/a.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/host/que.h` & `liba-0.1.1rc6/include/a/host/que.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/host/str.h` & `liba-0.1.1rc6/include/a/host/str.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/host/vec.h` & `liba-0.1.1rc6/include/a/host/vec.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/host/vector.h` & `liba-0.1.1rc6/include/a/host/vector.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/list.h` & `liba-0.1.1rc6/include/a/list.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/math.h` & `liba-0.1.1rc6/include/a/math.h`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,19 @@
 #define A_ABS(x) ((x) < 0 ? -(x) : (x))
 
 /*!
  @brief signum function, \f$ \texttt{sgn}{x}=\begin{cases}+1&x>0\\0&0\\-1&x<0\end{cases} \f$
 */
 #define A_SGN(x) ((0 < (x)) - ((x) < 0))
 
+/*!
+ @brief saturation value of x, \f$ \texttt{sat}(x,min,max)=\begin{cases}min&min>x\\max&x>max\\x&else\end{cases} \f$
+*/
+#define A_SAT(x, min, max) ((min) < (x) ? (x) < (max) ? (x) : (max) : (min))
+
 #if defined(__cplusplus)
 extern "C" {
 #endif /* __cplusplus */
 
 A_EXTERN a_f32_t a_f32_hypot(a_f32_t x, a_f32_t y);
 A_EXTERN a_f64_t a_f64_hypot(a_f64_t x, a_f64_t y);
```

### Comparing `liba-0.1.1rc5/include/a/mf.h` & `liba-0.1.1rc6/include/a/mf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/notefreqs.h` & `liba-0.1.1rc6/include/a/notefreqs.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/oop.h` & `liba-0.1.1rc6/include/a/oop.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/operator.h` & `liba-0.1.1rc6/include/a/operator.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/pid.h` & `liba-0.1.1rc6/include/a/pid.h`

 * *Files 0% similar despite different names*

```diff
@@ -271,25 +271,25 @@
  @brief calculate function for PID controller
  @param[in,out] ctx points to an instance of PID controller
  @param[in] set setpoint
  @param[in] fdb feedback
  @return output value
   @retval set when PID controller is off
 */
-A_EXTERN a_real_t a_pid_outv(a_pid_s *ctx, a_real_t set, a_real_t fdb);
+A_EXTERN a_real_t a_pid_outf(a_pid_s *ctx, a_real_t set, a_real_t fdb);
 
 /*!
  @brief calculate function for multichannel PID controller
  @param[in,out] ctx points to an instance of PID controller
  @param[in] set points to setpoint
  @param[in] fdb points to feedback
  @return points to output
   @retval set when PID controller is off
 */
-A_EXTERN a_real_t *a_pid_outp(a_pid_s *ctx, a_real_t *set, a_real_t *fdb);
+A_EXTERN a_real_t const *a_pid_outp(a_pid_s *ctx, a_real_t const *set, a_real_t const *fdb);
 
 /*!
  @brief terminate function for PID controller
  @param[in,out] ctx points to an instance of PID controller
 */
 A_EXTERN a_pid_s *a_pid_exit(a_pid_s *ctx);
```

### Comparing `liba-0.1.1rc5/include/a/poly.h` & `liba-0.1.1rc6/include/a/poly.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/polytrack.h` & `liba-0.1.1rc6/include/a/polytrack.h`

 * *Files 23% similar despite different names*

```diff
@@ -17,359 +17,212 @@
 
 /*!
  @brief instance structure for cubic polynomial trajectory
 */
 typedef struct a_polytrack3_s
 {
     a_real_t k[4]; //!< quantity
-    a_real_t t[2]; //!< time unit(s)
-    a_real_t q[2]; //!< position
-    a_real_t v[2]; //!< velocity
 } a_polytrack3_s;
 
 /*!
  @brief instance structure for quintic polynomial trajectory
 */
 typedef struct a_polytrack5_s
 {
     a_real_t k[6]; //!< quantity
-    a_real_t t[2]; //!< time unit(s)
-    a_real_t q[2]; //!< position
-    a_real_t v[2]; //!< velocity
-    a_real_t a[2]; //!< acceleration
 } a_polytrack5_s;
 
 /*!
  @brief instance structure for hepta polynomial trajectory
 */
 typedef struct a_polytrack7_s
 {
     a_real_t k[8]; //!< quantity
-    a_real_t t[2]; //!< time unit(s)
-    a_real_t q[2]; //!< position
-    a_real_t v[2]; //!< velocity
-    a_real_t a[2]; //!< acceleration
-    a_real_t j[2]; //!< jerk
 } a_polytrack7_s;
 
 #if defined(__cplusplus)
 extern "C" {
 #endif /* __cplusplus */
 
 /* function for cubic polynomial trajectory */
 
 /*!
- @brief initialize function for cubic polynomial trajectory
- @param[in,out] ctx points to an instance of cubic polynomial trajectory
- @param[in] t time
-  @arg 0 source
-  @arg 1 target
- @param[in] q position
-  @arg 0 source
-  @arg 1 target
- @param[in] v velocity
-  @arg 0 source
-  @arg 1 target
-*/
-A_EXTERN a_void_t a_polytrack3_init1(a_polytrack3_s *ctx, a_real_t const t[2], a_real_t const q[2], a_real_t const v[2]);
-
-/*!
- @brief initialize function for cubic polynomial trajectory
- @param[in,out] ctx points to an instance of cubic polynomial trajectory
- @param[in] source source for trajectory
-  @arg 0 time for source
-  @arg 1 position for source
-  @arg 2 velocity for source
- @param[in] target target for trajectory
-  @arg 0 time for target
-  @arg 1 position for target
-  @arg 2 velocity for target
-*/
-A_EXTERN a_void_t a_polytrack3_init2(a_polytrack3_s *ctx, a_real_t const source[3], a_real_t const target[3]);
-
-/*!
- @brief initialize function for cubic polynomial trajectory
- @param[in,out] ctx points to an instance of cubic polynomial trajectory
- @param[in] t0 time for source
- @param[in] t1 time for target
- @param[in] q0 position for source
- @param[in] q1 position for target
- @param[in] v0 velocity for source
- @param[in] v1 velocity for target
-*/
-A_EXTERN a_void_t a_polytrack3_init(a_polytrack3_s *ctx,
-                                    a_real_t t0, a_real_t t1,
-                                    a_real_t q0, a_real_t q1,
-                                    a_real_t v0, a_real_t v1);
-
-/*!
  @brief generation function for cubic polynomial trajectory
  @f{aligned}{
   \left\{\begin{array}{l}
   t=t_{1}-t_{0}\\
   q=q_{1}-q_{0}\\
   k_{0}=q_{0}\\
   k_{1}=v_{0}\\
   k_{2}=\cfrac{\left(-2\,v_{0}-v_{1}\right)\,t+3\,q}{t^2}\\
   k_{3}=\cfrac{\left(v_{0}+v_{1}\right)\,t-2\,q}{t^3}
   \end{array}\right.
  @f}
  @param[in,out] ctx points to an instance of cubic polynomial trajectory
+ @param[in] t0 time for source
+ @param[in] t1 time for target
+ @param[in] q0 position for source
+ @param[in] q1 position for target
+ @param[in] v0 velocity for source
+ @param[in] v1 velocity for target
 */
-A_EXTERN a_void_t a_polytrack3_gen(a_polytrack3_s *ctx);
+A_EXTERN a_void_t a_polytrack3_gen(a_polytrack3_s *ctx,
+                                   a_real_t t0, a_real_t t1,
+                                   a_real_t q0, a_real_t q1,
+                                   a_real_t v0, a_real_t v1);
 
 /*!
  @brief calculate function for cubic polynomial trajectory
  @f{aligned}{
   \begin{array}{l}
   q(t)=k_{0}+k_{1}\left(t-t_{0}\right)+k_{2}\left(t-t_{0}\right)^{2}+k_{3}\left(t-t_{0}\right)^{3} \\
   \dot{q}(t)=k_{1}+2 k_{2}\left(t-t_{0}\right)+3 k_{3}\left(t-t_{0}\right)^{2} \\
   \ddot{q}(t)=2 k_{2}+6 k_{3}\left(t-t_{0}\right)
   \end{array}
  @f}
  @param[in] ctx points to an instance of cubic polynomial trajectory
- @param[in] ts current time unit(s)
+ @param[in] dt difference between current time and initial time
  @param[out] out buffer for result
   @arg 0 position output
   @arg 1 velocity output
   @arg 2 acceleration output
 */
-A_EXTERN a_void_t a_polytrack3_out(a_polytrack3_s const *ctx, a_real_t ts, a_real_t out[3]);
+A_EXTERN a_void_t a_polytrack3_out(a_polytrack3_s const *ctx, a_real_t dt, a_real_t out[3]);
 
 /*!
  @brief calculate function for cubic polynomial trajectory position
  @f{aligned}{
   \begin{array}{l}
   q(t)=k_{0}+k_{1}\left(t-t_{0}\right)+k_{2}\left(t-t_{0}\right)^{2}+k_{3}\left(t-t_{0}\right)^{3} \\
   \end{array}
  @f}
  @param[in] ctx points to an instance of cubic polynomial trajectory
- @param[in] ts current time unit(s)
+ @param[in] dt difference between current time and initial time
  @return position output
 */
-A_EXTERN a_real_t a_polytrack3_pos(a_polytrack3_s const *ctx, a_real_t ts);
+A_EXTERN a_real_t a_polytrack3_pos(a_polytrack3_s const *ctx, a_real_t dt);
 
 /*!
  @brief calculate function for cubic polynomial trajectory velocity
  @f{aligned}{
   \begin{array}{l}
   \dot{q}(t)=k_{1}+2 k_{2}\left(t-t_{0}\right)+3 k_{3}\left(t-t_{0}\right)^{2} \\
   \end{array}
  @f}
  @param[in] ctx points to an instance of cubic polynomial trajectory
- @param[in] ts current time unit(s)
+ @param[in] dt difference between current time and initial time
  @return velocity output
 */
-A_EXTERN a_real_t a_polytrack3_vec(a_polytrack3_s const *ctx, a_real_t ts);
+A_EXTERN a_real_t a_polytrack3_vec(a_polytrack3_s const *ctx, a_real_t dt);
 
 /*!
  @brief calculate function for cubic polynomial trajectory acceleration
  @f{aligned}{
   \begin{array}{l}
   \ddot{q}(t)=2 k_{2}+6 k_{3}\left(t-t_{0}\right)
   \end{array}
  @f}
  @param[in] ctx points to an instance of cubic polynomial trajectory
- @param[in] ts current time unit(s)
+ @param[in] dt difference between current time and initial time
  @return acceleration output
 */
-A_EXTERN a_real_t a_polytrack3_acc(a_polytrack3_s const *ctx, a_real_t ts);
+A_EXTERN a_real_t a_polytrack3_acc(a_polytrack3_s const *ctx, a_real_t dt);
 
 /* function for quintic polynomial trajectory */
 
 /*!
- @brief initialize function for quintic polynomial trajectory
- @param[in,out] ctx points to an instance of quintic polynomial trajectory
- @param[in] t time
-  @arg 0 source
-  @arg 1 target
- @param[in] q position
-  @arg 0 source
-  @arg 1 target
- @param[in] v velocity
-  @arg 0 source
-  @arg 1 target
- @param[in] a acceleration
-  @arg 0 source
-  @arg 1 target
-*/
-A_EXTERN a_void_t a_polytrack5_init1(a_polytrack5_s *ctx, a_real_t const t[2], a_real_t const q[2], a_real_t const v[2], a_real_t const a[2]);
-
-/*!
- @brief initialize function for quintic polynomial trajectory
- @param[in,out] ctx points to an instance of quintic polynomial trajectory
- @param[in] source source for trajectory
-  @arg 0 time for source
-  @arg 1 position for source
-  @arg 2 velocity for source
-  @arg 3 acceleration for source
- @param[in] target target for trajectory
-  @arg 0 time for target
-  @arg 1 position for target
-  @arg 2 velocity for target
-  @arg 3 acceleration for target
-*/
-A_EXTERN a_void_t a_polytrack5_init2(a_polytrack5_s *ctx, a_real_t const source[4], a_real_t const target[4]);
-
-/*!
- @brief initialize function for quintic polynomial trajectory
- @param[in,out] ctx points to an instance of quintic polynomial trajectory
- @param[in] t0 time for source
- @param[in] t1 time for target
- @param[in] q0 position for source
- @param[in] q1 position for target
- @param[in] v0 velocity for source
- @param[in] v1 velocity for target
- @param[in] a0 acceleration for source
- @param[in] a1 acceleration for target
-*/
-A_EXTERN a_void_t a_polytrack5_init(a_polytrack5_s *ctx,
-                                    a_real_t t0, a_real_t t1,
-                                    a_real_t q0, a_real_t q1,
-                                    a_real_t v0, a_real_t v1,
-                                    a_real_t a0, a_real_t a1);
-
-/*!
  @brief generation function for quintic polynomial trajectory
  @f{aligned}{
   \left\{\begin{array}{l}
   t=t_{1}-t_{0}\\
   q=q_{1}-q_{0}\\
   k_{0}=q_{0}\\
   k_{1}=v_{0}\\
   k_{2}=\cfrac{a_{0}}{2}\\
   k_{3}=\cfrac{\left(a_{1}-3\,a_{0}\right)\,t^2+\left(-12\,v_{0}-8\,v_{1}\right)\,t+20\,q}{2\,t^3}\\
   k_{4}=\cfrac{\left(3\,a_{0}-2\,a_{1}\right)\,t^2+\left(16\,v_{0}+14\,v_{1}\right)\,t-30\,q}{2\,t^4}\\
   k_{5}=\cfrac{\left(a_{1}-a_{0}\right)\,t^2+\left(-6\,v_{0}-6\,v_{1}\right)\,t+12\,q}{2\,t^5}
   \end{array}\right.
  @f}
  @param[in,out] ctx points to an instance of quintic polynomial trajectory
+ @param[in] t0 time for source
+ @param[in] t1 time for target
+ @param[in] q0 position for source
+ @param[in] q1 position for target
+ @param[in] v0 velocity for source
+ @param[in] v1 velocity for target
+ @param[in] a0 acceleration for source
+ @param[in] a1 acceleration for target
 */
-A_EXTERN a_void_t a_polytrack5_gen(a_polytrack5_s *ctx);
+A_EXTERN a_void_t a_polytrack5_gen(a_polytrack5_s *ctx,
+                                   a_real_t t0, a_real_t t1,
+                                   a_real_t q0, a_real_t q1,
+                                   a_real_t v0, a_real_t v1,
+                                   a_real_t a0, a_real_t a1);
 
 /*!
  @brief calculate function for quintic polynomial trajectory
  @f{aligned}{
   \begin{array}{l}
   q(t)=k_{0}+k_{1}\left(t-t_{0}\right)+k_{2}\left(t-t_{0}\right)^{2}+k_{3}\left(t-t_{0}\right)^{3}+k_{4}\left(t-t_{0}\right)^{4}+k_{5}\left(t-t_{0}\right)^{5}\\
   \dot{q}(t)=k_{1}+2 k_{2}\left(t-t_{0}\right)+3 k_{3}\left(t-t_{0}\right)^{2}+4 k_{4}\left(t-t_{0}\right)^{3}+5 k_{5}\left(t-t_{0}\right)^{4}\\
   \ddot{q}(t)=2 k_{2}+6 k_{3}\left(t-t_{0}\right)+12 k_{4}\left(t-t_{0}\right)^{2}+20 k_{5}\left(t-t_{0}\right)^{3}
   \end{array}
  @f}
  @param[in] ctx points to an instance of quintic polynomial trajectory
- @param[in] ts current time unit(s)
+ @param[in] dt difference between current time and initial time
  @param[out] out buffer for result
   @arg 0 position output
   @arg 1 velocity output
   @arg 2 acceleration output
 */
-A_EXTERN a_void_t a_polytrack5_out(a_polytrack5_s const *ctx, a_real_t ts, a_real_t out[3]);
+A_EXTERN a_void_t a_polytrack5_out(a_polytrack5_s const *ctx, a_real_t dt, a_real_t out[3]);
 
 /*!
  @brief calculate function for quintic polynomial trajectory position
  @f{aligned}{
   \begin{array}{l}
   q(t)=k_{0}+k_{1}\left(t-t_{0}\right)+k_{2}\left(t-t_{0}\right)^{2}+k_{3}\left(t-t_{0}\right)^{3}+k_{4}\left(t-t_{0}\right)^{4}+k_{5}\left(t-t_{0}\right)^{5}\\
   \end{array}
  @f}
  @param[in] ctx points to an instance of quintic polynomial trajectory
- @param[in] ts current time unit(s)
+ @param[in] dt difference between current time and initial time
  @return position output
 */
-A_EXTERN a_real_t a_polytrack5_pos(a_polytrack5_s const *ctx, a_real_t ts);
+A_EXTERN a_real_t a_polytrack5_pos(a_polytrack5_s const *ctx, a_real_t dt);
 
 /*!
  @brief calculate function for quintic polynomial trajectory velocity
  @f{aligned}{
   \begin{array}{l}
   \dot{q}(t)=k_{1}+2 k_{2}\left(t-t_{0}\right)+3 k_{3}\left(t-t_{0}\right)^{2}+4 k_{4}\left(t-t_{0}\right)^{3}+5 k_{5}\left(t-t_{0}\right)^{4}\\
   \end{array}
  @f}
  @param[in] ctx points to an instance of quintic polynomial trajectory
- @param[in] ts current time unit(s)
+ @param[in] dt difference between current time and initial time
  @return velocity output
 */
-A_EXTERN a_real_t a_polytrack5_vec(a_polytrack5_s const *ctx, a_real_t ts);
+A_EXTERN a_real_t a_polytrack5_vec(a_polytrack5_s const *ctx, a_real_t dt);
 
 /*!
  @brief calculate function for quintic polynomial trajectory acceleration
  @f{aligned}{
   \begin{array}{l}
   \ddot{q}(t)=2 k_{2}+6 k_{3}\left(t-t_{0}\right)+12 k_{4}\left(t-t_{0}\right)^{2}+20 k_{5}\left(t-t_{0}\right)^{3}
   \end{array}
  @f}
  @param[in] ctx points to an instance of quintic polynomial trajectory
- @param[in] ts current time unit(s)
+ @param[in] dt difference between current time and initial time
  @return acceleration output
 */
-A_EXTERN a_real_t a_polytrack5_acc(a_polytrack5_s const *ctx, a_real_t ts);
+A_EXTERN a_real_t a_polytrack5_acc(a_polytrack5_s const *ctx, a_real_t dt);
 
 /* function for hepta polynomial trajectory */
 
 /*!
- @brief initialize function for hepta polynomial trajectory
- @param[in,out] ctx points to an instance of hepta polynomial trajectory
- @param[in] t time
-  @arg 0 source
-  @arg 1 target
- @param[in] q position
-  @arg 0 source
-  @arg 1 target
- @param[in] v velocity
-  @arg 0 source
-  @arg 1 target
- @param[in] a acceleration
-  @arg 0 source
-  @arg 1 target
- @param[in] j jerk
-  @arg 0 source
-  @arg 1 target
-*/
-A_EXTERN a_void_t a_polytrack7_init1(a_polytrack7_s *ctx, a_real_t const t[2], a_real_t const q[2], a_real_t const v[2], a_real_t const a[2], a_real_t const j[2]);
-
-/*!
- @brief initialize function for hepta polynomial trajectory
- @param[in,out] ctx points to an instance of hepta polynomial trajectory
- @param[in] source source for trajectory
-  @arg 0 time for source
-  @arg 1 position for source
-  @arg 2 velocity for source
-  @arg 3 acceleration for source
-  @arg 4 jerk for source
- @param[in] target target for trajectory
-  @arg 0 time for target
-  @arg 1 position for target
-  @arg 2 velocity for target
-  @arg 3 acceleration for target
-  @arg 4 jerk for target
-*/
-A_EXTERN a_void_t a_polytrack7_init2(a_polytrack7_s *ctx, a_real_t const source[5], a_real_t const target[5]);
-
-/*!
- @brief initialize function for hepta polynomial trajectory
- @param[in,out] ctx points to an instance of hepta polynomial trajectory
- @param[in] t0 time for source
- @param[in] t1 time for target
- @param[in] q0 position for source
- @param[in] q1 position for target
- @param[in] v0 velocity for source
- @param[in] v1 velocity for target
- @param[in] a0 acceleration for source
- @param[in] a1 acceleration for target
- @param[in] j0 jerk for source
- @param[in] j1 jerk for target
-*/
-A_EXTERN a_void_t a_polytrack7_init(a_polytrack7_s *ctx,
-                                    a_real_t t0, a_real_t t1,
-                                    a_real_t q0, a_real_t q1,
-                                    a_real_t v0, a_real_t v1,
-                                    a_real_t a0, a_real_t a1,
-                                    a_real_t j0, a_real_t j1);
-
-/*!
  @brief generation function for hepta polynomial trajectory
  @f{aligned}{
   \left\{\begin{array}{l}
   t=t_{1}-t_{0}\\
   q=q_{1}-q_{0}\\
   k_{0}=q_{0}\\
   k_{1}=v_{0}\\
@@ -378,88 +231,103 @@
   k_{4}=\cfrac{\left(-4\,j_{0}-j_{1}\right)\,t^3+\left(15\,a_{1}-30\,a_{0}\right)\,t^2+\left(-120\,v_{0}-90\,v_{1}\right)\,t+210\,q}{6\,t^4}\\
   k_{5}=\cfrac{\left(2\,j_{0}+j_{1}\right)\,t^3+\left(20\,a_{0}-14\,a_{1}\right)\,t^2+\left(90\,v_{0}+78\,v_{1}\right)\,t-168\,q}{2\,t^5}\\
   k_{6}=\cfrac{\left(-4\,j_{0}-3\,j_{1}\right)\,t^3+\left(39\,a_{1}-45\,a_{0}\right)\,t^2+\left(-216\,v_{0}-204\,v_{1}\right)\,t+420\,q}{6\,t^6}\\
   k_{7}=\cfrac{\left(j_{0}+j_{1}\right)\,t^3+\left(12\,a_{0}-12\,a_{1}\right)\,t^2+\left(60\,v_{0}+60\,v_{1}\right)\,t-120\,q}{6\,t^7}
   \end{array}\right.
  @f}
  @param[in,out] ctx points to an instance of hepta polynomial trajectory
+ @param[in] t0 time for source
+ @param[in] t1 time for target
+ @param[in] q0 position for source
+ @param[in] q1 position for target
+ @param[in] v0 velocity for source
+ @param[in] v1 velocity for target
+ @param[in] a0 acceleration for source
+ @param[in] a1 acceleration for target
+ @param[in] j0 jerk for source
+ @param[in] j1 jerk for target
 */
-A_EXTERN a_void_t a_polytrack7_gen(a_polytrack7_s *ctx);
+A_EXTERN a_void_t a_polytrack7_gen(a_polytrack7_s *ctx,
+                                   a_real_t t0, a_real_t t1,
+                                   a_real_t q0, a_real_t q1,
+                                   a_real_t v0, a_real_t v1,
+                                   a_real_t a0, a_real_t a1,
+                                   a_real_t j0, a_real_t j1);
 
 /*!
  @brief calculate function for hepta polynomial trajectory
  @f{aligned}{
   \begin{array}{l}
   q(t)=k_{0}+k_{1}\left(t-t_{0}\right)+k_{2}\left(t-t_{0}\right)^{2}+k_{3}\left(t-t_{0}\right)^{3}+k_{4}\left(t-t_{0}\right)^{4}+k_{5}\left(t-t_{0}\right)^{5}+k_{6}\left(t-t_{0}\right)^{6}+k_{7}\left(t-t_{0}\right)^{7}\\
   \dot{q}(t)=k_{1}+2 k_{2}\left(t-t_{0}\right)+3 k_{3}\left(t-t_{0}\right)^{2}+4 k_{4}\left(t-t_{0}\right)^{3}+5 k_{5}\left(t-t_{0}\right)^{4}+6 k_{6}\left(t-t_{0}\right)^{5}+7 k_{7}\left(t-t_{0}\right)^{6}\\
   \ddot{q}(t)=2 k_{2}+6 k_{3}\left(t-t_{0}\right)+12 k_{4}\left(t-t_{0}\right)^{2}+20 k_{5}\left(t-t_{0}\right)^{3}+30 k_{6}\left(t-t_{0}\right)^{4}+42 k_{7}\left(t-t_{0}\right)^{5}\\
   q^{(3)}(t)=6 k_{3}+24 k_{4}\left(t-t_{0}\right)+60 k_{5}\left(t-t_{0}\right)^{2}+120 k_{6}\left(t-t_{0}\right)^{3}+210 k_{7}\left(t-t_{0}\right)^{4}
   \end{array}
  @f}
  @param[in] ctx points to an instance of hepta polynomial trajectory
- @param[in] ts current time unit(s)
+ @param[in] dt difference between current time and initial time
  @param[out] out buffer for result
   @arg 0 position output
   @arg 1 velocity output
   @arg 2 acceleration output
   @arg 3 jerk output
 */
-A_EXTERN a_void_t a_polytrack7_out(a_polytrack7_s const *ctx, a_real_t ts, a_real_t out[4]);
+A_EXTERN a_void_t a_polytrack7_out(a_polytrack7_s const *ctx, a_real_t dt, a_real_t out[4]);
 
 /*!
  @brief calculate function for hepta polynomial trajectory position
  @f{aligned}{
   \begin{array}{l}
   q(t)=k_{0}+k_{1}\left(t-t_{0}\right)+k_{2}\left(t-t_{0}\right)^{2}+k_{3}\left(t-t_{0}\right)^{3}+k_{4}\left(t-t_{0}\right)^{4}+k_{5}\left(t-t_{0}\right)^{5}+k_{6}\left(t-t_{0}\right)^{6}+k_{7}\left(t-t_{0}\right)^{7}\\
   \end{array}
  @f}
  @param[in] ctx points to an instance of hepta polynomial trajectory
- @param[in] ts current time unit(s)
+ @param[in] dt difference between current time and initial time
  @return position output
 */
-A_EXTERN a_real_t a_polytrack7_pos(a_polytrack7_s const *ctx, a_real_t ts);
+A_EXTERN a_real_t a_polytrack7_pos(a_polytrack7_s const *ctx, a_real_t dt);
 
 /*!
  @brief calculate function for hepta polynomial trajectory velocity
  @f{aligned}{
   \begin{array}{l}
   \dot{q}(t)=k_{1}+2 k_{2}\left(t-t_{0}\right)+3 k_{3}\left(t-t_{0}\right)^{2}+4 k_{4}\left(t-t_{0}\right)^{3}+5 k_{5}\left(t-t_{0}\right)^{4}+6 k_{6}\left(t-t_{0}\right)^{5}+7 k_{7}\left(t-t_{0}\right)^{6}\\
   \end{array}
  @f}
  @param[in] ctx points to an instance of hepta polynomial trajectory
- @param[in] ts current time unit(s)
+ @param[in] dt difference between current time and initial time
  @return velocity output
 */
-A_EXTERN a_real_t a_polytrack7_vec(a_polytrack7_s const *ctx, a_real_t ts);
+A_EXTERN a_real_t a_polytrack7_vec(a_polytrack7_s const *ctx, a_real_t dt);
 
 /*!
  @brief calculate function for hepta polynomial trajectory acceleration
  @f{aligned}{
   \begin{array}{l}
   \ddot{q}(t)=2 k_{2}+6 k_{3}\left(t-t_{0}\right)+12 k_{4}\left(t-t_{0}\right)^{2}+20 k_{5}\left(t-t_{0}\right)^{3}+30 k_{6}\left(t-t_{0}\right)^{4}+42 k_{7}\left(t-t_{0}\right)^{5}\\
   \end{array}
  @f}
  @param[in] ctx points to an instance of hepta polynomial trajectory
- @param[in] ts current time unit(s)
+ @param[in] dt difference between current time and initial time
  @return acceleration output
 */
-A_EXTERN a_real_t a_polytrack7_acc(a_polytrack7_s const *ctx, a_real_t ts);
+A_EXTERN a_real_t a_polytrack7_acc(a_polytrack7_s const *ctx, a_real_t dt);
 
 /*!
  @brief calculate function for hepta polynomial trajectory jerk
  @f{aligned}{
   \begin{array}{l}
   q^{(3)}(t)=6 k_{3}+24 k_{4}\left(t-t_{0}\right)+60 k_{5}\left(t-t_{0}\right)^{2}+120 k_{6}\left(t-t_{0}\right)^{3}+210 k_{7}\left(t-t_{0}\right)^{4}
   \end{array}
  @f}
  @param[in] ctx points to an instance of hepta polynomial trajectory
- @param[in] ts current time unit(s)
+ @param[in] dt difference between current time and initial time
  @return jerk output
 */
-A_EXTERN a_real_t a_polytrack7_jer(a_polytrack7_s const *ctx, a_real_t ts);
+A_EXTERN a_real_t a_polytrack7_jer(a_polytrack7_s const *ctx, a_real_t dt);
 
 #if defined(__cplusplus)
 } /* extern "C" */
 #endif /* __cplusplus */
 
 /*! @} A_POLYTRACK */
```

### Comparing `liba-0.1.1rc5/include/a/rbt.h` & `liba-0.1.1rc6/include/a/rbt.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/real.h` & `liba-0.1.1rc6/include/a/real.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/slist.h` & `liba-0.1.1rc6/include/a/slist.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/tf.h` & `liba-0.1.1rc6/include/a/tf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/include/a/utf.h` & `liba-0.1.1rc6/include/a/utf.h`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,18 @@
 A_EXTERN a_uint_t a_utf_decode(a_cptr_t str, a_u32_t *val);
 
 /*!
  @brief length of a UTF-8 string terminated with a null character
  @param[in] str string terminated with a null character
  @return length of the UTF-8 string
 */
-A_EXTERN a_size_t a_utf_len(a_cptr_t str);
+A_EXTERN a_size_t a_utf_length(a_cptr_t str);
 
 #if defined(__cplusplus)
 } /* extern "C" */
 #endif /* __cplusplus */
 
+#define a_utf_len(str) a_utf_length(str)
+
 /*! @} A_UTF */
 
 #endif /* utf.h */
```

### Comparing `liba-0.1.1rc5/include/a/version.h` & `liba-0.1.1rc6/include/a/version.h`

 * *Files 6% similar despite different names*

```diff
@@ -19,85 +19,104 @@
 #define A_VERSION "0.0.0"
 #endif /* A_VERSION */
 
 /*! algorithm library version major */
 #ifndef A_VERSION_MAJOR
 #define A_VERSION_MAJOR 0
 #endif /* A_VERSION_MAJOR */
+#undef major
 
 /*! algorithm library version minor */
 #ifndef A_VERSION_MINOR
 #define A_VERSION_MINOR 0
 #endif /* A_VERSION_MINOR */
+#undef minor
 
 /*! algorithm library version patch */
 #ifndef A_VERSION_PATCH
 #define A_VERSION_PATCH 0
 #endif /* A_VERSION_PATCH */
+#undef patch
 
 /*! algorithm library version tweak */
 #ifndef A_VERSION_TWEAK
 #define A_VERSION_TWEAK A_U64_C(0)
 #endif /* A_VERSION_TWEAK */
 
 #if defined(__cplusplus)
-#define A_VERSION_C(maj, min, pat) a_version_s(maj, min, pat)
+#define A_VERSION_C(maj, min, pat) a::version(maj, min, pat)
 #else /* !__cplusplus */
 // clang-format off
 #define A_VERSION_C(maj, min, pat) {maj, min, pat}
 // clang-format on
 #endif /* __cplusplus */
 
-/*!
- @brief instance structure for version
-*/
-typedef struct a_version_s
-{
-#undef major
-#undef minor
-#undef patch
-#if defined(__cplusplus)
-    A_PUBLIC a_bool_t operator<(a_version_s const &ver) const;
-    A_PUBLIC a_bool_t operator>(a_version_s const &ver) const;
-    A_PUBLIC a_bool_t operator<=(a_version_s const &ver) const;
-    A_PUBLIC a_bool_t operator>=(a_version_s const &ver) const;
-    A_PUBLIC a_bool_t operator==(a_version_s const &ver) const;
-    A_PUBLIC a_bool_t operator!=(a_version_s const &ver) const;
-    A_PUBLIC a_version_s(a_uint_t const maj = 0,
-                         a_uint_t const min = 0,
-                         a_uint_t const pat = 0)
-        : major(maj)
-        , minor(min)
-        , patch(pat)
-    {
-    }
-#endif /* __cplusplus */
-    a_uint_t major;
-    a_uint_t minor;
-    a_uint_t patch;
-} a_version_s;
-
 #if defined(__cplusplus)
 namespace a
 {
-
 /*! algorithm library version string */
 cstr_t const VERSION = A_VERSION;
 /*! algorithm library version major */
 uint_t const VERSION_MAJOR = A_VERSION_MAJOR;
 /*! algorithm library version minor */
 uint_t const VERSION_MINOR = A_VERSION_MINOR;
 /*! algorithm library version patch */
 uint_t const VERSION_PATCH = A_VERSION_PATCH;
 /*! algorithm library version tweak */
 u64_t const VERSION_TWEAK = A_VERSION_TWEAK;
-/* instance structure for version */
-typedef a_version_s version;
+#endif /* __cplusplus */
+
+/*!
+ @brief instance structure for version
+*/
+#if defined(__cplusplus)
+struct version
+{
+    A_PUBLIC a_bool_t operator<(version const &ver) const;
+    A_PUBLIC a_bool_t operator>(version const &ver) const;
+    A_PUBLIC a_bool_t operator<=(version const &ver) const;
+    A_PUBLIC a_bool_t operator>=(version const &ver) const;
+    A_PUBLIC a_bool_t operator==(version const &ver) const;
+    A_PUBLIC a_bool_t operator!=(version const &ver) const;
+    A_PUBLIC version(a_uint_t const maj = 0,
+                     a_uint_t const min = 0,
+                     a_uint_t const pat = 0)
+        : major(maj)
+        , minor(min)
+        , patch(pat)
+    {
+    }
+#else /* !__cplusplus */
+typedef struct a_version_s
+{
+#endif /* __cplusplus */
+    a_uint_t major; //!< major number
+    a_uint_t minor; //!< minor number
+    a_uint_t patch; //!< patch number
+#if defined(__cplusplus)
+};
+#else /* !__cplusplus */
+} a_version_s;
+#endif /* __cplusplus */
 
+#if defined(__cplusplus)
+/*!
+ @brief algorithm library version major
+*/
+A_EXTERN uint_t version_major(void);
+/*!
+ @brief algorithm library version minor
+*/
+A_EXTERN uint_t version_minor(void);
+/*!
+ @brief algorithm library version patch
+*/
+A_EXTERN uint_t version_patch(void);
 } /* namespace a */
+typedef a::version a_version_s;
 extern "C" {
 #endif /* __cplusplus */
 
 /*!
  @brief algorithm library version string
 */
 A_EXTERN a_cstr_t a_version(void);
@@ -206,14 +225,15 @@
 #endif /* A_HAVE_INLINE */
 #if defined(A_HAVE_INLINE) || defined(LIBA_VERSION_C)
 A_INTERN a_bool_t a_version_le(a_version_s const *const lhs, a_version_s const *const rhs)
 {
     return !a_version_lt(rhs, lhs);
 }
 #endif /* A_HAVE_INLINE */
+
 /*!
  @brief version lhs greater than or equal version rhs
  @param[in] lhs operand on the left
  @param[in] rhs operand on the right
  @return result of comparison
 */
 #if !defined A_HAVE_INLINE || defined(LIBA_VERSION_C)
@@ -261,31 +281,12 @@
 #if defined(LIBA_VERSION_C)
 #undef A_INTERN
 #define A_INTERN static A_INLINE
 #endif /* LIBA_VERSION_C */
 
 #if defined(__cplusplus)
 } /* extern "C" */
-namespace a
-{
-
-/*!
- @brief algorithm library version major
-*/
-A_EXTERN uint_t version_major(void);
-
-/*!
- @brief algorithm library version minor
-*/
-A_EXTERN uint_t version_minor(void);
-
-/*!
- @brief algorithm library version patch
-*/
-A_EXTERN uint_t version_patch(void);
-
-} /* namespace a */
 #endif /* __cplusplus */
 
 /*! @} A_VERSION */
 
 #endif /* version.h */
```

### Comparing `liba-0.1.1rc5/liba.egg-info/SOURCES.txt` & `liba-0.1.1rc6/liba.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 include/a/a.h
 include/a/avl.h
@@ -31,14 +32,15 @@
 include/a/host/vec.h
 include/a/host/vector.h
 liba.egg-info/PKG-INFO
 liba.egg-info/SOURCES.txt
 liba.egg-info/dependency_links.txt
 liba.egg-info/top_level.txt
 python/src/a.c
+python/src/a.c
 python/src/a.pyx
 python/src/a/__init__.pxd
 python/src/a/__init__.pxi
 python/src/a/fpid.pxd
 python/src/a/fpid.pxi
 python/src/a/math.pxd
 python/src/a/math.pxi
```

### Comparing `liba-0.1.1rc5/python/src/a/__init__.pxd` & `liba-0.1.1rc6/python/src/a/__init__.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -45,9 +45,9 @@
     ctypedef  float a_f32_t
     ctypedef double a_f64_t
     IF A_SIZE_REAL == 8:
         ctypedef double a_real_t
     IF A_SIZE_REAL == 4:
         ctypedef float a_real_t
     ctypedef union a_real_u:
-        a_real_t v
+        a_real_t f
         a_real_t *p
```

### Comparing `liba-0.1.1rc5/python/src/a/fpid.pxd` & `liba-0.1.1rc6/python/src/a/fpid.pxd`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,14 @@
     a_fpid_s *a_fpid_kpid(a_fpid_s *ctx, a_real_t kp, a_real_t ki, a_real_t kd)
     a_fpid_s *a_fpid_buff(a_fpid_s *ctx, a_uint_t *idx, a_real_t *mms, a_real_t *mat)
     a_fpid_s *a_fpid_setv(a_fpid_s *ctx, a_real_t *out, a_real_t *fdb, a_real_t *sum, a_real_t *ec, a_real_t *e)
     a_fpid_s *a_fpid_base(a_fpid_s *ctx, a_uint_t col, const a_real_t *mec, const a_real_t *mec,
                           const a_real_t *mkp, const a_real_t *mki, const a_real_t *mkd)
     a_fpid_s *a_fpid_init(a_fpid_s *ctx, a_real_t dt, a_uint_t col, const a_real_t *mec, const a_real_t *mec,
                           const a_real_t *mkp, const a_real_t *mki, const a_real_t *mkd, a_real_t min, a_real_t max)
-    a_real_t *a_fpid_outp(a_fpid_s *ctx, a_real_t *set, a_real_t *fdb)
-    a_real_t a_fpid_outv(a_fpid_s *ctx, a_real_t set, a_real_t fdb)
+    a_real_t a_fpid_outf(a_fpid_s *ctx, a_real_t set, a_real_t fdb)
+    const a_real_t *a_fpid_outp(a_fpid_s *ctx, const a_real_t *set, const a_real_t *fdb)
     a_fpid_s *a_fpid_exit(a_fpid_s *ctx)
     a_fpid_s *a_fpid_zero(a_fpid_s *ctx)
     a_uint_t a_fpid_bufnum(const a_fpid_s *ctx)
     a_vptr_t a_fpid_bufptr(const a_fpid_s *ctx)
     a_uint_t a_fpid_col(const a_fpid_s *ctx)
```

### Comparing `liba-0.1.1rc5/python/src/a/fpid.pxi` & `liba-0.1.1rc6/python/src/a/fpid.pxi`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         if sum:
             a_fpid_pos(&self.ctx, sum)
         else:
             a_fpid_inc(&self.ctx)
         self.buf = num
     def __call__(self, set: a_real_t, fdb: a_real_t) -> a_real_t:
         '''calculate function for fuzzy PID controller'''
-        return a_fpid_outv(&self.ctx, set, fdb)
+        return a_fpid_outf(&self.ctx, set, fdb)
     def __dealloc__(self):
         '''terminate function for fuzzy PID controller'''
         a_fpid_exit(&self.ctx)
         PyMem_Free(self.ptr)
     def zero(self):
         '''zero function for fuzzy PID controller'''
         a_fpid_zero(&self.ctx)
@@ -136,17 +136,17 @@
         a_fpid_buf1(&self.ctx, self.ptr, max)
 
     @property
     def col(self) -> a_uint_t:
         return a_fpid_col(&self.ctx)
     @property
     def out(self) -> a_real_t:
-        return self.ctx.pid.out.v
+        return self.ctx.pid.out.f
     @property
     def fdb(self) -> a_real_t:
-        return self.ctx.pid.fdb.v
+        return self.ctx.pid.fdb.f
     @property
     def ec(self) -> a_real_t:
-        return self.ctx.pid.ec.v
+        return self.ctx.pid.ec.f
     @property
     def e(self) -> a_real_t:
-        return self.ctx.pid.e.v
+        return self.ctx.pid.e.f
```

### Comparing `liba-0.1.1rc5/python/src/a/math.pxi` & `liba-0.1.1rc6/python/src/a/math.pxi`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/python/src/a/mf.pxd` & `liba-0.1.1rc6/python/src/a/mf.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/python/src/a/mf.pxi` & `liba-0.1.1rc6/python/src/a/mf.pxi`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/python/src/a/pid.pxd` & `liba-0.1.1rc6/python/src/a/pid.pxd`

 * *Files 11% similar despite different names*

```diff
@@ -15,25 +15,25 @@
         a_real_u e
     a_pid_s *a_pid_off(a_pid_s *ctx)
     a_pid_s *a_pid_inc(a_pid_s *ctx)
     a_pid_s *a_pid_pos(a_pid_s *ctx, a_real_t max)
     a_pid_s *a_pid_kpid(a_pid_s *ctx, a_real_t kp, a_real_t ki, a_real_t kd)
     a_pid_s *a_pid_chan(a_pid_s *ctx, a_uint_t num, a_real_t *out, a_real_t *fdb, a_real_t *sum, a_real_t *ec, a_real_t *e)
     a_pid_s *a_pid_init(a_pid_s *ctx, a_real_t dt, a_real_t min, a_real_t max)
-    a_real_t *a_pid_outp(a_pid_s *ctx, a_real_t *set, a_real_t *fdb)
-    a_real_t a_pid_outv(a_pid_s *ctx, a_real_t set, a_real_t fdb)
+    a_real_t a_pid_outf(a_pid_s *ctx, a_real_t set, a_real_t fdb)
+    const a_real_t *a_pid_outp(a_pid_s *ctx, const a_real_t *set, const a_real_t *fdb)
     a_pid_s *a_pid_exit(a_pid_s *ctx)
     a_pid_s *a_pid_zero(a_pid_s *ctx)
-    a_void_t a_pid_set_dt(a_pid_s *ctx, a_real_t dt)
     a_real_t a_pid_dt(const a_pid_s *ctx)
-    a_void_t a_pid_set_kp(a_pid_s *ctx, a_real_t kp)
+    a_void_t a_pid_set_dt(a_pid_s *ctx, a_real_t dt)
     a_real_t a_pid_kp(const a_pid_s *ctx)
-    a_void_t a_pid_set_ki(a_pid_s *ctx, a_real_t ki)
+    a_void_t a_pid_set_kp(a_pid_s *ctx, a_real_t kp)
     a_real_t a_pid_ki(const a_pid_s *ctx)
-    a_void_t a_pid_set_kd(a_pid_s *ctx, a_real_t kd)
+    a_void_t a_pid_set_ki(a_pid_s *ctx, a_real_t ki)
     a_real_t a_pid_kd(const a_pid_s *ctx)
-    a_void_t a_pid_set_num(a_pid_s *ctx, a_uint_t num)
+    a_void_t a_pid_set_kd(a_pid_s *ctx, a_real_t kd)
     a_uint_t a_pid_num(const a_pid_s *ctx)
-    a_void_t a_pid_set_reg(a_pid_s *ctx, a_uint_t reg)
+    a_void_t a_pid_set_num(a_pid_s *ctx, a_uint_t num)
     a_uint_t a_pid_reg(const a_pid_s *ctx)
-    a_void_t a_pid_set_mode(a_pid_s *ctx, a_uint_t mode)
+    a_void_t a_pid_set_reg(a_pid_s *ctx, a_uint_t reg)
     a_uint_t a_pid_mode(const a_pid_s *ctx)
+    a_void_t a_pid_set_mode(a_pid_s *ctx, a_uint_t mode)
```

### Comparing `liba-0.1.1rc5/python/src/a/pid.pxi` & `liba-0.1.1rc6/python/src/a/pid.pxi`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         a_pid_init(&self.ctx, dt, min, max)
         if sum:
             a_pid_pos(&self.ctx, sum)
         else:
             a_pid_inc(&self.ctx)
     def __call__(self, set: a_real_t, fdb: a_real_t) -> a_real_t:
         '''calculate function for PID controller'''
-        return a_pid_outv(&self.ctx, set, fdb)
+        return a_pid_outf(&self.ctx, set, fdb)
     def __dealloc__(self):
         '''terminate function for PID controller'''
         a_pid_exit(&self.ctx)
     def zero(self):
         '''zero function for PID controller'''
         a_pid_zero(&self.ctx)
         return self
@@ -95,17 +95,17 @@
         return a_pid_kd(&self.ctx)
     @kd.setter
     def kd(self, kd: a_real_t):
         a_pid_set_kd(&self.ctx, kd)
 
     @property
     def out(self) -> a_real_t:
-        return self.ctx.out.v
+        return self.ctx.out.f
     @property
     def fdb(self) -> a_real_t:
-        return self.ctx.fdb.v
+        return self.ctx.fdb.f
     @property
     def ec(self) -> a_real_t:
-        return self.ctx.ec.v
+        return self.ctx.ec.f
     @property
     def e(self) -> a_real_t:
-        return self.ctx.e.v
+        return self.ctx.e.f
```

### Comparing `liba-0.1.1rc5/python/src/a/poly.pxi` & `liba-0.1.1rc6/python/src/a/poly.pxi`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/python/src/a/tf.pxi` & `liba-0.1.1rc6/python/src/a/tf.pxi`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/python/src/a.c` & `liba-0.1.1rc6/python/src/a.c`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.33 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "A_HAVE_H",
-                "\"../build/a.setup.h\""
+                "\"..\\build\\a.setup.h\""
             ],
             [
                 "A_EXPORTS",
                 null
             ],
             [
                 "A_SIZE_REAL",
@@ -21,36 +21,36 @@
         "include_dirs": [
             "include"
         ],
         "language": "c",
         "name": "liba",
         "sources": [
             "python/src/a.pyx",
-            "src/a.c",
-            "src/avl.c",
-            "src/buf.c",
-            "src/complex.c",
-            "src/crc.c",
-            "src/fpid.c",
-            "src/fuzzy.c",
-            "src/math.c",
-            "src/mf.c",
-            "src/pid.c",
-            "src/poly.c",
-            "src/polytrack.c",
-            "src/rbt.c",
-            "src/real.c",
-            "src/tf.c",
-            "src/utf.c",
-            "src/version.c",
-            "src/host/a.c",
-            "src/host/que.c",
-            "src/host/str.c",
-            "src/host/vec.c",
-            "src/host/vector.c"
+            "src\\a.c",
+            "src\\avl.c",
+            "src\\buf.c",
+            "src\\complex.c",
+            "src\\crc.c",
+            "src\\fpid.c",
+            "src\\fuzzy.c",
+            "src\\math.c",
+            "src\\mf.c",
+            "src\\pid.c",
+            "src\\poly.c",
+            "src\\polytrack.c",
+            "src\\rbt.c",
+            "src\\real.c",
+            "src\\tf.c",
+            "src\\utf.c",
+            "src\\version.c",
+            "src\\host\\a.c",
+            "src\\host\\que.c",
+            "src\\host\\str.c",
+            "src\\host\\vec.c",
+            "src\\host\\vector.c"
         ]
     },
     "module_name": "liba"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -58,16 +58,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_33"
+#define CYTHON_HEX_VERSION 0x001D21F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -136,15 +136,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -601,35 +601,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1013,24 +1013,24 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "python/src/a/mf.pxi",
-  "python/src/a/math.pxi",
+  "python\\src\\a/mf.pxi",
+  "python\\src\\a/math.pxi",
   "stringsource",
-  "python/src/a.pyx",
-  "python/src/a/version.pxi",
-  "python/src/a/tf.pxi",
-  "python/src/a/pid.pxi",
-  "python/src/a/fpid.pxi",
-  "python/src/a/poly.pxi",
-  "python/src/a/polytrack.pxi",
+  "python\\src\\a.pyx",
+  "python\\src\\a/version.pxi",
+  "python\\src\\a/tf.pxi",
+  "python\\src\\a/pid.pxi",
+  "python\\src\\a/fpid.pxi",
+  "python\\src\\a/poly.pxi",
+  "python\\src\\a/polytrack.pxi",
   "array.pxd",
   "type.pxd",
   "bool.pxd",
   "complex.pxd",
 };
 
 /*--- Type declarations ---*/
@@ -1141,28 +1141,28 @@
  */
 struct __pyx_obj_4liba_polytrack3 {
   PyObject_HEAD
   a_polytrack3_s ctx;
 };
 
 
-/* "python/src/a/polytrack.pxi":125
+/* "python/src/a/polytrack.pxi":59
  * @cython.wraparound(False)
  * @cython.boundscheck(False)
  * cdef class polytrack5:             # <<<<<<<<<<<<<<
  *     '''quintic polynomial trajectory'''
  *     cdef a_polytrack5_s ctx
  */
 struct __pyx_obj_4liba_polytrack5 {
   PyObject_HEAD
   a_polytrack5_s ctx;
 };
 
 
-/* "python/src/a/polytrack.pxi":267
+/* "python/src/a/polytrack.pxi":113
  * @cython.wraparound(False)
  * @cython.boundscheck(False)
  * cdef class polytrack7:             # <<<<<<<<<<<<<<
  *     '''hepta polynomial trajectory'''
  *     cdef a_polytrack7_s ctx
  */
 struct __pyx_obj_4liba_polytrack7 {
@@ -1613,26 +1613,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1693,14 +1693,32 @@
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseClosureNameError(const char *varname);
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
+/* Import.proto */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
+
+/* ImportFrom.proto */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
+
+/* PyObjectCall2Args.proto */
+static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+
+/* HasAttr.proto */
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
+
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -1715,32 +1733,14 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
-/* PySequenceContains.proto */
-static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
-    int result = PySequence_Contains(seq, item);
-    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
-}
-
-/* Import.proto */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
-
-/* ImportFrom.proto */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
-
-/* PyObjectCall2Args.proto */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
-
-/* HasAttr.proto */
-static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
-
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
@@ -2247,15 +2247,14 @@
 static const char __pyx_k_me[] = "me";
 static const char __pyx_k_mf[] = "mf";
 static const char __pyx_k_q0[] = "q0";
 static const char __pyx_k_q1[] = "q1";
 static const char __pyx_k_t0[] = "t0";
 static const char __pyx_k_t1[] = "t1";
 static const char __pyx_k_tf[] = "tf";
-static const char __pyx_k_ts[] = "ts";
 static const char __pyx_k_v0[] = "v0";
 static const char __pyx_k_v1[] = "v1";
 static const char __pyx_k_INC[] = "INC";
 static const char __pyx_k_NUL[] = "NUL";
 static const char __pyx_k_OFF[] = "OFF";
 static const char __pyx_k_POS[] = "POS";
 static const char __pyx_k_SIG[] = "SIG";
@@ -2326,19 +2325,19 @@
 static const char __pyx_k_version_minor[] = "version_minor";
 static const char __pyx_k_version_patch[] = "version_patch";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_pyx_unpickle_mf[] = "__pyx_unpickle_mf";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_base_locals_genexpr[] = "base.<locals>.genexpr";
-static const char __pyx_k_python_src_a_mf_pxi[] = "python/src/a/mf.pxi";
-static const char __pyx_k_python_src_a_math_pxi[] = "python/src/a/math.pxi";
-static const char __pyx_k_python_src_a_poly_pxi[] = "python/src/a/poly.pxi";
+static const char __pyx_k_python_src_a_mf_pxi[] = "python\\src\\a/mf.pxi";
+static const char __pyx_k_python_src_a_math_pxi[] = "python\\src\\a/math.pxi";
+static const char __pyx_k_python_src_a_poly_pxi[] = "python\\src\\a/poly.pxi";
 static const char __pyx_k_cinit___locals_genexpr[] = "__cinit__.<locals>.genexpr";
-static const char __pyx_k_python_src_a_version_pxi[] = "python/src/a/version.pxi";
+static const char __pyx_k_python_src_a_version_pxi[] = "python\\src\\a/version.pxi";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static PyObject *__pyx_n_s_GAUSS;
 static PyObject *__pyx_n_s_GBELL;
 static PyObject *__pyx_n_s_INC;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_MemoryError;
@@ -2437,15 +2436,14 @@
 static PyObject *__pyx_n_s_t0;
 static PyObject *__pyx_n_s_t1;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_tf;
 static PyObject *__pyx_n_s_throw;
 static PyObject *__pyx_n_s_trap;
 static PyObject *__pyx_n_s_tri;
-static PyObject *__pyx_n_s_ts;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_v;
 static PyObject *__pyx_n_s_v0;
 static PyObject *__pyx_n_s_v1;
 static PyObject *__pyx_n_s_version;
 static PyObject *__pyx_n_s_version_major;
 static PyObject *__pyx_n_s_version_minor;
@@ -2551,111 +2549,39 @@
 static PyObject *__pyx_pf_4liba_4fpid_2ec___get__(struct __pyx_obj_4liba_fpid *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_4liba_4fpid_1e___get__(struct __pyx_obj_4liba_fpid *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_4liba_4fpid_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_4liba_fpid *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_4liba_4fpid_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_4liba_fpid *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_4liba_12poly_eval(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_x, PyObject *__pyx_v_a); /* proto */
 static PyObject *__pyx_pf_4liba_14poly_evar(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_x, PyObject *__pyx_v_a); /* proto */
 static int __pyx_pf_4liba_10polytrack3___cinit__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_t0, a_real_t __pyx_v_t1, a_real_t __pyx_v_q0, a_real_t __pyx_v_q1, a_real_t __pyx_v_v0, a_real_t __pyx_v_v1); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack3_2__call__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_ts); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack3_4pos(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_ts); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack3_6vec(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_ts); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack3_8acc(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_ts); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack3_10gen(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack3_2gen(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_t0, a_real_t __pyx_v_t1, a_real_t __pyx_v_q0, a_real_t __pyx_v_q1, a_real_t __pyx_v_v0, a_real_t __pyx_v_v1); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack3_4__call__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_dt); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack3_6pos(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_dt); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack3_8vec(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_dt); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack3_10acc(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_dt); /* proto */
 static PyObject *__pyx_pf_4liba_10polytrack3_1k___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack3_1t___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack3_1t_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack3_1q___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack3_1q_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack3_1v___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack3_1v_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack3_2t0___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack3_2t0_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack3_2q0___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack3_2q0_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack3_2v0___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack3_2v0_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack3_2t1___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack3_2t1_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack3_2q1___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack3_2q1_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack3_2v1___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack3_2v1_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
 static PyObject *__pyx_pf_4liba_10polytrack3_12__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_4liba_polytrack3 *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_4liba_10polytrack3_14__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_4liba_10polytrack5___cinit__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_t0, a_real_t __pyx_v_t1, a_real_t __pyx_v_q0, a_real_t __pyx_v_q1, a_real_t __pyx_v_v0, a_real_t __pyx_v_v1, a_real_t __pyx_v_a0, a_real_t __pyx_v_a1); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_2__call__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_ts); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_4pos(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_ts); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_6vec(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_ts); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_8acc(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_ts); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_10gen(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack5_2gen(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_t0, a_real_t __pyx_v_t1, a_real_t __pyx_v_q0, a_real_t __pyx_v_q1, a_real_t __pyx_v_v0, a_real_t __pyx_v_v1, a_real_t __pyx_v_a0, a_real_t __pyx_v_a1); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack5_4__call__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_dt); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack5_6pos(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_dt); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack5_8vec(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_dt); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack5_10acc(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_dt); /* proto */
 static PyObject *__pyx_pf_4liba_10polytrack5_1k___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_1t___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack5_1t_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_1q___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack5_1q_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_1v___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack5_1v_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_1a___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack5_1a_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_2t0___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack5_2t0_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_2q0___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack5_2q0_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_2v0___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack5_2v0_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_2a0___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack5_2a0_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_2t1___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack5_2t1_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_2q1___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack5_2q1_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_2v1___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack5_2v1_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack5_2a1___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack5_2a1_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
 static PyObject *__pyx_pf_4liba_10polytrack5_12__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_4liba_polytrack5 *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_4liba_10polytrack5_14__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_4liba_10polytrack7___cinit__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_t0, a_real_t __pyx_v_t1, a_real_t __pyx_v_q0, a_real_t __pyx_v_q1, a_real_t __pyx_v_v0, a_real_t __pyx_v_v1, a_real_t __pyx_v_a0, a_real_t __pyx_v_a1, a_real_t __pyx_v_j0, a_real_t __pyx_v_j1); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_2__call__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_ts); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_4pos(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_ts); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_6vec(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_ts); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_8acc(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_ts); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_10jer(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_ts); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_12gen(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack7_2gen(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_t0, a_real_t __pyx_v_t1, a_real_t __pyx_v_q0, a_real_t __pyx_v_q1, a_real_t __pyx_v_v0, a_real_t __pyx_v_v1, a_real_t __pyx_v_a0, a_real_t __pyx_v_a1, a_real_t __pyx_v_j0, a_real_t __pyx_v_j1); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack7_4__call__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_dt); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack7_6pos(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_dt); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack7_8vec(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_dt); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack7_10acc(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_dt); /* proto */
+static PyObject *__pyx_pf_4liba_10polytrack7_12jer(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_dt); /* proto */
 static PyObject *__pyx_pf_4liba_10polytrack7_1k___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_1t___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_1t_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_1q___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_1q_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_1v___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_1v_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_1a___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_1a_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_1j___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_1j_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_2t0___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_2t0_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_2q0___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_2q0_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_2v0___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_2v0_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_2a0___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_2a0_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_2j0___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_2j0_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_2t1___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_2t1_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_2q1___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_2q1_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_2v1___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_2v1_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_2a1___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_2a1_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
-static PyObject *__pyx_pf_4liba_10polytrack7_2j1___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
-static int __pyx_pf_4liba_10polytrack7_2j1_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val); /* proto */
 static PyObject *__pyx_pf_4liba_10polytrack7_14__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_4liba_polytrack7 *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_4liba_10polytrack7_16__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_4liba_16__pyx_unpickle_mf(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_7cpython_5array_5array___getbuffer__(arrayobject *__pyx_v_self, Py_buffer *__pyx_v_info, CYTHON_UNUSED int __pyx_v_flags); /* proto */
 static void __pyx_pf_7cpython_5array_5array_2__releasebuffer__(CYTHON_UNUSED arrayobject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
 static PyObject *__pyx_tp_new_4liba_mf(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_4liba_tf(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
@@ -5754,15 +5680,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_mf, (type(self), 0xd41d8cd, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_mf__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_4liba___pyx_unpickle_mf__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_mf, (type(self), 0xd41d8cd, state)
@@ -6714,15 +6640,15 @@
 }
 
 /* "python/src/a/pid.pxi":17
  *         else:
  *             a_pid_inc(&self.ctx)
  *     def __call__(self, set: a_real_t, fdb: a_real_t) -> a_real_t:             # <<<<<<<<<<<<<<
  *         '''calculate function for PID controller'''
- *         return a_pid_outv(&self.ctx, set, fdb)
+ *         return a_pid_outf(&self.ctx, set, fdb)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4liba_3pid_3__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_4liba_3pid_2__call__[] = "calculate function for PID controller";
 #if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_4liba_3pid_2__call__;
@@ -6797,31 +6723,31 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
   /* "python/src/a/pid.pxi":19
  *     def __call__(self, set: a_real_t, fdb: a_real_t) -> a_real_t:
  *         '''calculate function for PID controller'''
- *         return a_pid_outv(&self.ctx, set, fdb)             # <<<<<<<<<<<<<<
+ *         return a_pid_outf(&self.ctx, set, fdb)             # <<<<<<<<<<<<<<
  *     def __dealloc__(self):
  *         '''terminate function for PID controller'''
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(a_pid_outv((&__pyx_v_self->ctx), __pyx_v_set, __pyx_v_fdb)); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 19, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(a_pid_outf((&__pyx_v_self->ctx), __pyx_v_set, __pyx_v_fdb)); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "python/src/a/pid.pxi":17
  *         else:
  *             a_pid_inc(&self.ctx)
  *     def __call__(self, set: a_real_t, fdb: a_real_t) -> a_real_t:             # <<<<<<<<<<<<<<
  *         '''calculate function for PID controller'''
- *         return a_pid_outv(&self.ctx, set, fdb)
+ *         return a_pid_outf(&self.ctx, set, fdb)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("liba.pid.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
@@ -6829,15 +6755,15 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "python/src/a/pid.pxi":20
  *         '''calculate function for PID controller'''
- *         return a_pid_outv(&self.ctx, set, fdb)
+ *         return a_pid_outf(&self.ctx, set, fdb)
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         '''terminate function for PID controller'''
  *         a_pid_exit(&self.ctx)
  */
 
 /* Python wrapper */
 static void __pyx_pw_4liba_3pid_5__dealloc__(PyObject *__pyx_v_self); /*proto*/
@@ -6861,15 +6787,15 @@
  *     def zero(self):
  *         '''zero function for PID controller'''
  */
   (void)(a_pid_exit((&__pyx_v_self->ctx)));
 
   /* "python/src/a/pid.pxi":20
  *         '''calculate function for PID controller'''
- *         return a_pid_outv(&self.ctx, set, fdb)
+ *         return a_pid_outf(&self.ctx, set, fdb)
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         '''terminate function for PID controller'''
  *         a_pid_exit(&self.ctx)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -8265,15 +8191,15 @@
   return __pyx_r;
 }
 
 /* "python/src/a/pid.pxi":101
  * 
  *     @property
  *     def out(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.out.v
+ *         return self.ctx.out.f
  *     @property
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4liba_3pid_3out_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_4liba_3pid_3out_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
@@ -8294,30 +8220,30 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "python/src/a/pid.pxi":102
  *     @property
  *     def out(self) -> a_real_t:
- *         return self.ctx.out.v             # <<<<<<<<<<<<<<
+ *         return self.ctx.out.f             # <<<<<<<<<<<<<<
  *     @property
  *     def fdb(self) -> a_real_t:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.out.v); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 102, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.out.f); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "python/src/a/pid.pxi":101
  * 
  *     @property
  *     def out(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.out.v
+ *         return self.ctx.out.f
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("liba.pid.out.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -8325,18 +8251,18 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "python/src/a/pid.pxi":104
- *         return self.ctx.out.v
+ *         return self.ctx.out.f
  *     @property
  *     def fdb(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.fdb.v
+ *         return self.ctx.fdb.f
  *     @property
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4liba_3pid_3fdb_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_4liba_3pid_3fdb_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
@@ -8357,30 +8283,30 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "python/src/a/pid.pxi":105
  *     @property
  *     def fdb(self) -> a_real_t:
- *         return self.ctx.fdb.v             # <<<<<<<<<<<<<<
+ *         return self.ctx.fdb.f             # <<<<<<<<<<<<<<
  *     @property
  *     def ec(self) -> a_real_t:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.fdb.v); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 105, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.fdb.f); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "python/src/a/pid.pxi":104
- *         return self.ctx.out.v
+ *         return self.ctx.out.f
  *     @property
  *     def fdb(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.fdb.v
+ *         return self.ctx.fdb.f
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("liba.pid.fdb.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -8388,18 +8314,18 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "python/src/a/pid.pxi":107
- *         return self.ctx.fdb.v
+ *         return self.ctx.fdb.f
  *     @property
  *     def ec(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.ec.v
+ *         return self.ctx.ec.f
  *     @property
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4liba_3pid_2ec_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_4liba_3pid_2ec_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
@@ -8420,30 +8346,30 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "python/src/a/pid.pxi":108
  *     @property
  *     def ec(self) -> a_real_t:
- *         return self.ctx.ec.v             # <<<<<<<<<<<<<<
+ *         return self.ctx.ec.f             # <<<<<<<<<<<<<<
  *     @property
  *     def e(self) -> a_real_t:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.ec.v); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 108, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.ec.f); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "python/src/a/pid.pxi":107
- *         return self.ctx.fdb.v
+ *         return self.ctx.fdb.f
  *     @property
  *     def ec(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.ec.v
+ *         return self.ctx.ec.f
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("liba.pid.ec.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -8451,18 +8377,18 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "python/src/a/pid.pxi":110
- *         return self.ctx.ec.v
+ *         return self.ctx.ec.f
  *     @property
  *     def e(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.e.v
+ *         return self.ctx.e.f
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4liba_3pid_1e_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_4liba_3pid_1e_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -8482,28 +8408,28 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "python/src/a/pid.pxi":111
  *     @property
  *     def e(self) -> a_real_t:
- *         return self.ctx.e.v             # <<<<<<<<<<<<<<
+ *         return self.ctx.e.f             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.e.v); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 111, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.e.f); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "python/src/a/pid.pxi":110
- *         return self.ctx.ec.v
+ *         return self.ctx.ec.f
  *     @property
  *     def e(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.e.v
+ *         return self.ctx.e.f
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("liba.pid.e.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
@@ -10137,15 +10063,15 @@
 }
 
 /* "python/src/a/fpid.pxi":32
  *             a_fpid_inc(&self.ctx)
  *         self.buf = num
  *     def __call__(self, set: a_real_t, fdb: a_real_t) -> a_real_t:             # <<<<<<<<<<<<<<
  *         '''calculate function for fuzzy PID controller'''
- *         return a_fpid_outv(&self.ctx, set, fdb)
+ *         return a_fpid_outf(&self.ctx, set, fdb)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4liba_4fpid_3__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_4liba_4fpid_2__call__[] = "calculate function for fuzzy PID controller";
 #if CYTHON_UPDATE_DESCRIPTOR_DOC
 struct wrapperbase __pyx_wrapperbase_4liba_4fpid_2__call__;
@@ -10220,31 +10146,31 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
   /* "python/src/a/fpid.pxi":34
  *     def __call__(self, set: a_real_t, fdb: a_real_t) -> a_real_t:
  *         '''calculate function for fuzzy PID controller'''
- *         return a_fpid_outv(&self.ctx, set, fdb)             # <<<<<<<<<<<<<<
+ *         return a_fpid_outf(&self.ctx, set, fdb)             # <<<<<<<<<<<<<<
  *     def __dealloc__(self):
  *         '''terminate function for fuzzy PID controller'''
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(a_fpid_outv((&__pyx_v_self->ctx), __pyx_v_set, __pyx_v_fdb)); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 34, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(a_fpid_outf((&__pyx_v_self->ctx), __pyx_v_set, __pyx_v_fdb)); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "python/src/a/fpid.pxi":32
  *             a_fpid_inc(&self.ctx)
  *         self.buf = num
  *     def __call__(self, set: a_real_t, fdb: a_real_t) -> a_real_t:             # <<<<<<<<<<<<<<
  *         '''calculate function for fuzzy PID controller'''
- *         return a_fpid_outv(&self.ctx, set, fdb)
+ *         return a_fpid_outf(&self.ctx, set, fdb)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("liba.fpid.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
@@ -10252,15 +10178,15 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "python/src/a/fpid.pxi":35
  *         '''calculate function for fuzzy PID controller'''
- *         return a_fpid_outv(&self.ctx, set, fdb)
+ *         return a_fpid_outf(&self.ctx, set, fdb)
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         '''terminate function for fuzzy PID controller'''
  *         a_fpid_exit(&self.ctx)
  */
 
 /* Python wrapper */
 static void __pyx_pw_4liba_4fpid_5__dealloc__(PyObject *__pyx_v_self); /*proto*/
@@ -10293,15 +10219,15 @@
  *     def zero(self):
  *         '''zero function for fuzzy PID controller'''
  */
   PyMem_Free(__pyx_v_self->ptr);
 
   /* "python/src/a/fpid.pxi":35
  *         '''calculate function for fuzzy PID controller'''
- *         return a_fpid_outv(&self.ctx, set, fdb)
+ *         return a_fpid_outf(&self.ctx, set, fdb)
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         '''terminate function for fuzzy PID controller'''
  *         a_fpid_exit(&self.ctx)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -13300,15 +13226,15 @@
   return __pyx_r;
 }
 
 /* "python/src/a/fpid.pxi":142
  *         return a_fpid_col(&self.ctx)
  *     @property
  *     def out(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.pid.out.v
+ *         return self.ctx.pid.out.f
  *     @property
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4liba_4fpid_3out_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_4liba_4fpid_3out_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
@@ -13329,30 +13255,30 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "python/src/a/fpid.pxi":143
  *     @property
  *     def out(self) -> a_real_t:
- *         return self.ctx.pid.out.v             # <<<<<<<<<<<<<<
+ *         return self.ctx.pid.out.f             # <<<<<<<<<<<<<<
  *     @property
  *     def fdb(self) -> a_real_t:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.pid.out.v); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 143, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.pid.out.f); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "python/src/a/fpid.pxi":142
  *         return a_fpid_col(&self.ctx)
  *     @property
  *     def out(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.pid.out.v
+ *         return self.ctx.pid.out.f
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("liba.fpid.out.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -13360,18 +13286,18 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "python/src/a/fpid.pxi":145
- *         return self.ctx.pid.out.v
+ *         return self.ctx.pid.out.f
  *     @property
  *     def fdb(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.pid.fdb.v
+ *         return self.ctx.pid.fdb.f
  *     @property
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4liba_4fpid_3fdb_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_4liba_4fpid_3fdb_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
@@ -13392,30 +13318,30 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "python/src/a/fpid.pxi":146
  *     @property
  *     def fdb(self) -> a_real_t:
- *         return self.ctx.pid.fdb.v             # <<<<<<<<<<<<<<
+ *         return self.ctx.pid.fdb.f             # <<<<<<<<<<<<<<
  *     @property
  *     def ec(self) -> a_real_t:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.pid.fdb.v); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 146, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.pid.fdb.f); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "python/src/a/fpid.pxi":145
- *         return self.ctx.pid.out.v
+ *         return self.ctx.pid.out.f
  *     @property
  *     def fdb(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.pid.fdb.v
+ *         return self.ctx.pid.fdb.f
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("liba.fpid.fdb.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -13423,18 +13349,18 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "python/src/a/fpid.pxi":148
- *         return self.ctx.pid.fdb.v
+ *         return self.ctx.pid.fdb.f
  *     @property
  *     def ec(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.pid.ec.v
+ *         return self.ctx.pid.ec.f
  *     @property
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4liba_4fpid_2ec_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_4liba_4fpid_2ec_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
@@ -13455,30 +13381,30 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "python/src/a/fpid.pxi":149
  *     @property
  *     def ec(self) -> a_real_t:
- *         return self.ctx.pid.ec.v             # <<<<<<<<<<<<<<
+ *         return self.ctx.pid.ec.f             # <<<<<<<<<<<<<<
  *     @property
  *     def e(self) -> a_real_t:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.pid.ec.v); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 149, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.pid.ec.f); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "python/src/a/fpid.pxi":148
- *         return self.ctx.pid.fdb.v
+ *         return self.ctx.pid.fdb.f
  *     @property
  *     def ec(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.pid.ec.v
+ *         return self.ctx.pid.ec.f
  *     @property
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("liba.fpid.ec.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -13486,18 +13412,18 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "python/src/a/fpid.pxi":151
- *         return self.ctx.pid.ec.v
+ *         return self.ctx.pid.ec.f
  *     @property
  *     def e(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.pid.e.v
+ *         return self.ctx.pid.e.f
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4liba_4fpid_1e_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_4liba_4fpid_1e_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -13517,28 +13443,28 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "python/src/a/fpid.pxi":152
  *     @property
  *     def e(self) -> a_real_t:
- *         return self.ctx.pid.e.v             # <<<<<<<<<<<<<<
+ *         return self.ctx.pid.e.f             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.pid.e.v); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 152, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->ctx.pid.e.f); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "python/src/a/fpid.pxi":151
- *         return self.ctx.pid.ec.v
+ *         return self.ctx.pid.ec.f
  *     @property
  *     def e(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.pid.e.v
+ *         return self.ctx.pid.e.f
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("liba.fpid.e.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
@@ -14076,16 +14002,16 @@
   return __pyx_r;
 }
 
 /* "python/src/a/polytrack.pxi":8
  *     '''cubic polynomial trajectory'''
  *     cdef a_polytrack3_s ctx
  *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0):             # <<<<<<<<<<<<<<
- *         a_polytrack3_init(&self.ctx, t0, t1, q0, q1, v0, v1)
- *     def __call__(self, ts):
+ *         a_polytrack3_gen(&self.ctx, t0, t1, q0, q1, v0, v1)
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0):
  */
 
 /* Python wrapper */
 static int __pyx_pw_4liba_10polytrack3_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_4liba_10polytrack3_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   a_real_t __pyx_v_t0;
   a_real_t __pyx_v_t1;
@@ -14208,100 +14134,258 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
   /* "python/src/a/polytrack.pxi":9
  *     cdef a_polytrack3_s ctx
  *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0):
- *         a_polytrack3_init(&self.ctx, t0, t1, q0, q1, v0, v1)             # <<<<<<<<<<<<<<
- *     def __call__(self, ts):
- *         '''calculate all'''
+ *         a_polytrack3_gen(&self.ctx, t0, t1, q0, q1, v0, v1)             # <<<<<<<<<<<<<<
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0):
+ *         '''generation function'''
  */
-  a_polytrack3_init((&__pyx_v_self->ctx), __pyx_v_t0, __pyx_v_t1, __pyx_v_q0, __pyx_v_q1, __pyx_v_v0, __pyx_v_v1);
+  a_polytrack3_gen((&__pyx_v_self->ctx), __pyx_v_t0, __pyx_v_t1, __pyx_v_q0, __pyx_v_q1, __pyx_v_v0, __pyx_v_v1);
 
   /* "python/src/a/polytrack.pxi":8
  *     '''cubic polynomial trajectory'''
  *     cdef a_polytrack3_s ctx
  *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0):             # <<<<<<<<<<<<<<
- *         a_polytrack3_init(&self.ctx, t0, t1, q0, q1, v0, v1)
- *     def __call__(self, ts):
+ *         a_polytrack3_gen(&self.ctx, t0, t1, q0, q1, v0, v1)
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "python/src/a/polytrack.pxi":10
  *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0):
- *         a_polytrack3_init(&self.ctx, t0, t1, q0, q1, v0, v1)
- *     def __call__(self, ts):             # <<<<<<<<<<<<<<
+ *         a_polytrack3_gen(&self.ctx, t0, t1, q0, q1, v0, v1)
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0):             # <<<<<<<<<<<<<<
+ *         '''generation function'''
+ *         a_polytrack3_gen(&self.ctx, t0, t1, q0, q1, v0, v1)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_4liba_10polytrack3_3gen(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_4liba_10polytrack3_2gen[] = "generation function";
+static PyObject *__pyx_pw_4liba_10polytrack3_3gen(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  a_real_t __pyx_v_t0;
+  a_real_t __pyx_v_t1;
+  a_real_t __pyx_v_q0;
+  a_real_t __pyx_v_q1;
+  a_real_t __pyx_v_v0;
+  a_real_t __pyx_v_v1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("gen (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_t0,&__pyx_n_s_t1,&__pyx_n_s_q0,&__pyx_n_s_q1,&__pyx_n_s_v0,&__pyx_n_s_v1,0};
+    PyObject* values[6] = {0,0,0,0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_t0)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_t1)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("gen", 0, 4, 6, 1); __PYX_ERR(9, 10, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_q0)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("gen", 0, 4, 6, 2); __PYX_ERR(9, 10, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_q1)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("gen", 0, 4, 6, 3); __PYX_ERR(9, 10, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  4:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v0);
+          if (value) { values[4] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v1);
+          if (value) { values[5] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gen") < 0)) __PYX_ERR(9, 10, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_t0 = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_t0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 10, __pyx_L3_error)
+    __pyx_v_t1 = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_t1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 10, __pyx_L3_error)
+    __pyx_v_q0 = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_q0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 10, __pyx_L3_error)
+    __pyx_v_q1 = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_q1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 10, __pyx_L3_error)
+    if (values[4]) {
+      __pyx_v_v0 = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_v0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 10, __pyx_L3_error)
+    } else {
+      __pyx_v_v0 = ((a_real_t)0.0);
+    }
+    if (values[5]) {
+      __pyx_v_v1 = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_v1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 10, __pyx_L3_error)
+    } else {
+      __pyx_v_v1 = ((a_real_t)0.0);
+    }
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("gen", 0, 4, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(9, 10, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("liba.polytrack3.gen", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_4liba_10polytrack3_2gen(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), __pyx_v_t0, __pyx_v_t1, __pyx_v_q0, __pyx_v_q1, __pyx_v_v0, __pyx_v_v1);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_4liba_10polytrack3_2gen(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_t0, a_real_t __pyx_v_t1, a_real_t __pyx_v_q0, a_real_t __pyx_v_q1, a_real_t __pyx_v_v0, a_real_t __pyx_v_v1) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("gen", 0);
+
+  /* "python/src/a/polytrack.pxi":12
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0):
+ *         '''generation function'''
+ *         a_polytrack3_gen(&self.ctx, t0, t1, q0, q1, v0, v1)             # <<<<<<<<<<<<<<
+ *     def __call__(self, dt):
+ *         '''calculate all'''
+ */
+  a_polytrack3_gen((&__pyx_v_self->ctx), __pyx_v_t0, __pyx_v_t1, __pyx_v_q0, __pyx_v_q1, __pyx_v_v0, __pyx_v_v1);
+
+  /* "python/src/a/polytrack.pxi":10
+ *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0):
+ *         a_polytrack3_gen(&self.ctx, t0, t1, q0, q1, v0, v1)
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0):             # <<<<<<<<<<<<<<
+ *         '''generation function'''
+ *         a_polytrack3_gen(&self.ctx, t0, t1, q0, q1, v0, v1)
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "python/src/a/polytrack.pxi":13
+ *         '''generation function'''
+ *         a_polytrack3_gen(&self.ctx, t0, t1, q0, q1, v0, v1)
+ *     def __call__(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate all'''
  *         cdef a_real_t out[3]
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack3_3__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_4liba_10polytrack3_2__call__[] = "calculate all";
+static PyObject *__pyx_pw_4liba_10polytrack3_5__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_4liba_10polytrack3_4__call__[] = "calculate all";
 #if CYTHON_UPDATE_DESCRIPTOR_DOC
-struct wrapperbase __pyx_wrapperbase_4liba_10polytrack3_2__call__;
+struct wrapperbase __pyx_wrapperbase_4liba_10polytrack3_4__call__;
 #endif
-static PyObject *__pyx_pw_4liba_10polytrack3_3__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_ts = 0;
+static PyObject *__pyx_pw_4liba_10polytrack3_5__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_dt = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__call__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_ts,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_dt,0};
     PyObject* values[1] = {0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ts)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dt)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(9, 10, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(9, 13, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
-    __pyx_v_ts = values[0];
+    __pyx_v_dt = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(9, 10, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(9, 13, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("liba.polytrack3.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack3_2__call__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), __pyx_v_ts);
+  __pyx_r = __pyx_pf_4liba_10polytrack3_4__call__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), __pyx_v_dt);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4liba_10polytrack3_2__call__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pf_4liba_10polytrack3_4__call__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_dt) {
   a_real_t __pyx_v_out[3];
   arrayobject *__pyx_v_p = NULL;
   arrayobject *__pyx_v_v = NULL;
   arrayobject *__pyx_v_a = NULL;
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_v_it = NULL;
   PyObject *__pyx_r = NULL;
@@ -14316,256 +14400,256 @@
   a_real_t __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "python/src/a/polytrack.pxi":13
+  /* "python/src/a/polytrack.pxi":16
  *         '''calculate all'''
  *         cdef a_real_t out[3]
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             p = reals(ts)
- *             v = reals(ts)
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             p = reals(dt)
+ *             v = reals(dt)
  */
-  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_ts) != 0);
+  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_dt) != 0);
   if (__pyx_t_1) {
 
-    /* "python/src/a/polytrack.pxi":14
+    /* "python/src/a/polytrack.pxi":17
  *         cdef a_real_t out[3]
- *         if iterable(ts):
- *             p = reals(ts)             # <<<<<<<<<<<<<<
- *             v = reals(ts)
- *             a = reals(ts)
+ *         if iterable(dt):
+ *             p = reals(dt)             # <<<<<<<<<<<<<<
+ *             v = reals(dt)
+ *             a = reals(dt)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 14, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 17, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_p = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":15
- *         if iterable(ts):
- *             p = reals(ts)
- *             v = reals(ts)             # <<<<<<<<<<<<<<
- *             a = reals(ts)
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":18
+ *         if iterable(dt):
+ *             p = reals(dt)
+ *             v = reals(dt)             # <<<<<<<<<<<<<<
+ *             a = reals(dt)
+ *             for i, it in enumerate(dt):
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 15, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 18, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_v = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":16
- *             p = reals(ts)
- *             v = reals(ts)
- *             a = reals(ts)             # <<<<<<<<<<<<<<
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":19
+ *             p = reals(dt)
+ *             v = reals(dt)
+ *             a = reals(dt)             # <<<<<<<<<<<<<<
+ *             for i, it in enumerate(dt):
  *                 a_polytrack3_out(&self.ctx, it, out)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 16, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 19, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_a = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":17
- *             v = reals(ts)
- *             a = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+    /* "python/src/a/polytrack.pxi":20
+ *             v = reals(dt)
+ *             a = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 a_polytrack3_out(&self.ctx, it, out)
  *                 p[i] = out[0]
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
-    if (likely(PyList_CheckExact(__pyx_v_ts)) || PyTuple_CheckExact(__pyx_v_ts)) {
-      __pyx_t_4 = __pyx_v_ts; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+    if (likely(PyList_CheckExact(__pyx_v_dt)) || PyTuple_CheckExact(__pyx_v_dt)) {
+      __pyx_t_4 = __pyx_v_dt; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ts); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 17, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_dt); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 20, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 17, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 20, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 17, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 20, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 17, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 20, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 17, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 20, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 17, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 20, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(9, 17, __pyx_L1_error)
+            else __PYX_ERR(9, 20, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 17, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 20, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":18
- *             a = reals(ts)
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":21
+ *             a = reals(dt)
+ *             for i, it in enumerate(dt):
  *                 a_polytrack3_out(&self.ctx, it, out)             # <<<<<<<<<<<<<<
  *                 p[i] = out[0]
  *                 v[i] = out[1]
  */
-      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 18, __pyx_L1_error)
+      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 21, __pyx_L1_error)
       a_polytrack3_out((&__pyx_v_self->ctx), __pyx_t_8, __pyx_v_out);
 
-      /* "python/src/a/polytrack.pxi":19
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":22
+ *             for i, it in enumerate(dt):
  *                 a_polytrack3_out(&self.ctx, it, out)
  *                 p[i] = out[0]             # <<<<<<<<<<<<<<
  *                 v[i] = out[1]
  *                 a[i] = out[2]
  */
-      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[0])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 19, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[0])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 22, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_p), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 19, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_p), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 22, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":20
+      /* "python/src/a/polytrack.pxi":23
  *                 a_polytrack3_out(&self.ctx, it, out)
  *                 p[i] = out[0]
  *                 v[i] = out[1]             # <<<<<<<<<<<<<<
  *                 a[i] = out[2]
  *             return p, v, a
  */
-      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[1])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 20, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[1])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 23, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_v), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 20, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_v), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 23, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":21
+      /* "python/src/a/polytrack.pxi":24
  *                 p[i] = out[0]
  *                 v[i] = out[1]
  *                 a[i] = out[2]             # <<<<<<<<<<<<<<
  *             return p, v, a
- *         a_polytrack3_out(&self.ctx, ts, out)
+ *         a_polytrack3_out(&self.ctx, dt, out)
  */
-      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[2])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 21, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[2])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 24, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_a), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 21, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_a), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 24, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":17
- *             v = reals(ts)
- *             a = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+      /* "python/src/a/polytrack.pxi":20
+ *             v = reals(dt)
+ *             a = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 a_polytrack3_out(&self.ctx, it, out)
  *                 p[i] = out[0]
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":22
+    /* "python/src/a/polytrack.pxi":25
  *                 v[i] = out[1]
  *                 a[i] = out[2]
  *             return p, v, a             # <<<<<<<<<<<<<<
- *         a_polytrack3_out(&self.ctx, ts, out)
+ *         a_polytrack3_out(&self.ctx, dt, out)
  *         return out[0], out[1], out[2]
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 22, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 25, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(((PyObject *)__pyx_v_p));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_p));
     PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_v_p));
     __Pyx_INCREF(((PyObject *)__pyx_v_v));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_v));
     PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)__pyx_v_v));
     __Pyx_INCREF(((PyObject *)__pyx_v_a));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_a));
     PyTuple_SET_ITEM(__pyx_t_2, 2, ((PyObject *)__pyx_v_a));
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "python/src/a/polytrack.pxi":13
+    /* "python/src/a/polytrack.pxi":16
  *         '''calculate all'''
  *         cdef a_real_t out[3]
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             p = reals(ts)
- *             v = reals(ts)
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             p = reals(dt)
+ *             v = reals(dt)
  */
   }
 
-  /* "python/src/a/polytrack.pxi":23
+  /* "python/src/a/polytrack.pxi":26
  *                 a[i] = out[2]
  *             return p, v, a
- *         a_polytrack3_out(&self.ctx, ts, out)             # <<<<<<<<<<<<<<
+ *         a_polytrack3_out(&self.ctx, dt, out)             # <<<<<<<<<<<<<<
  *         return out[0], out[1], out[2]
- *     def pos(self, ts):
+ *     def pos(self, dt):
  */
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_ts); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 23, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 26, __pyx_L1_error)
   a_polytrack3_out((&__pyx_v_self->ctx), __pyx_t_8, __pyx_v_out);
 
-  /* "python/src/a/polytrack.pxi":24
+  /* "python/src/a/polytrack.pxi":27
  *             return p, v, a
- *         a_polytrack3_out(&self.ctx, ts, out)
+ *         a_polytrack3_out(&self.ctx, dt, out)
  *         return out[0], out[1], out[2]             # <<<<<<<<<<<<<<
- *     def pos(self, ts):
+ *     def pos(self, dt):
  *         '''calculate position'''
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_out[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 24, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_out[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_out[1])); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 24, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_out[1])); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[2])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 24, __pyx_L1_error)
+  __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[2])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(9, 24, __pyx_L1_error)
+  __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(9, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_t_7);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
   __pyx_t_7 = 0;
   __pyx_r = __pyx_t_9;
   __pyx_t_9 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":10
- *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0):
- *         a_polytrack3_init(&self.ctx, t0, t1, q0, q1, v0, v1)
- *     def __call__(self, ts):             # <<<<<<<<<<<<<<
+  /* "python/src/a/polytrack.pxi":13
+ *         '''generation function'''
+ *         a_polytrack3_gen(&self.ctx, t0, t1, q0, q1, v0, v1)
+ *     def __call__(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate all'''
  *         cdef a_real_t out[3]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -14581,37 +14665,37 @@
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_it);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":25
- *         a_polytrack3_out(&self.ctx, ts, out)
+/* "python/src/a/polytrack.pxi":28
+ *         a_polytrack3_out(&self.ctx, dt, out)
  *         return out[0], out[1], out[2]
- *     def pos(self, ts):             # <<<<<<<<<<<<<<
+ *     def pos(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate position'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack3_5pos(PyObject *__pyx_v_self, PyObject *__pyx_v_ts); /*proto*/
-static char __pyx_doc_4liba_10polytrack3_4pos[] = "calculate position";
-static PyObject *__pyx_pw_4liba_10polytrack3_5pos(PyObject *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pw_4liba_10polytrack3_7pos(PyObject *__pyx_v_self, PyObject *__pyx_v_dt); /*proto*/
+static char __pyx_doc_4liba_10polytrack3_6pos[] = "calculate position";
+static PyObject *__pyx_pw_4liba_10polytrack3_7pos(PyObject *__pyx_v_self, PyObject *__pyx_v_dt) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("pos (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_4pos(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((PyObject *)__pyx_v_ts));
+  __pyx_r = __pyx_pf_4liba_10polytrack3_6pos(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((PyObject *)__pyx_v_dt));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4liba_10polytrack3_4pos(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pf_4liba_10polytrack3_6pos(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_dt) {
   arrayobject *__pyx_v_out = NULL;
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_v_it = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -14622,162 +14706,162 @@
   PyObject *__pyx_t_7 = NULL;
   a_real_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pos", 0);
 
-  /* "python/src/a/polytrack.pxi":27
- *     def pos(self, ts):
+  /* "python/src/a/polytrack.pxi":30
+ *     def pos(self, dt):
  *         '''calculate position'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
-  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_ts) != 0);
+  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_dt) != 0);
   if (__pyx_t_1) {
 
-    /* "python/src/a/polytrack.pxi":28
+    /* "python/src/a/polytrack.pxi":31
  *         '''calculate position'''
- *         if iterable(ts):
- *             out = reals(ts)             # <<<<<<<<<<<<<<
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):
+ *             out = reals(dt)             # <<<<<<<<<<<<<<
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack3_pos(&self.ctx, it)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 28, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 31, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_out = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":29
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+    /* "python/src/a/polytrack.pxi":32
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack3_pos(&self.ctx, it)
  *             return out
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
-    if (likely(PyList_CheckExact(__pyx_v_ts)) || PyTuple_CheckExact(__pyx_v_ts)) {
-      __pyx_t_4 = __pyx_v_ts; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+    if (likely(PyList_CheckExact(__pyx_v_dt)) || PyTuple_CheckExact(__pyx_v_dt)) {
+      __pyx_t_4 = __pyx_v_dt; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ts); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 29, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_dt); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 32, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 29, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 32, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 29, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 32, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 29, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 32, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 29, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 32, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 29, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 32, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(9, 29, __pyx_L1_error)
+            else __PYX_ERR(9, 32, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 29, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 32, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":30
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":33
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack3_pos(&self.ctx, it)             # <<<<<<<<<<<<<<
  *             return out
- *         return a_polytrack3_pos(&self.ctx, ts)
+ *         return a_polytrack3_pos(&self.ctx, dt)
  */
-      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 30, __pyx_L1_error)
-      __pyx_t_7 = PyFloat_FromDouble(a_polytrack3_pos((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 30, __pyx_L1_error)
+      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 33, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble(a_polytrack3_pos((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 33, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 30, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 33, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":29
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+      /* "python/src/a/polytrack.pxi":32
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack3_pos(&self.ctx, it)
  *             return out
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":31
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":34
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack3_pos(&self.ctx, it)
  *             return out             # <<<<<<<<<<<<<<
- *         return a_polytrack3_pos(&self.ctx, ts)
- *     def vec(self, ts):
+ *         return a_polytrack3_pos(&self.ctx, dt)
+ *     def vec(self, dt):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_out));
     __pyx_r = ((PyObject *)__pyx_v_out);
     goto __pyx_L0;
 
-    /* "python/src/a/polytrack.pxi":27
- *     def pos(self, ts):
+    /* "python/src/a/polytrack.pxi":30
+ *     def pos(self, dt):
  *         '''calculate position'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
   }
 
-  /* "python/src/a/polytrack.pxi":32
+  /* "python/src/a/polytrack.pxi":35
  *                 out[i] = a_polytrack3_pos(&self.ctx, it)
  *             return out
- *         return a_polytrack3_pos(&self.ctx, ts)             # <<<<<<<<<<<<<<
- *     def vec(self, ts):
+ *         return a_polytrack3_pos(&self.ctx, dt)             # <<<<<<<<<<<<<<
+ *     def vec(self, dt):
  *         '''calculate velocity'''
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_ts); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 32, __pyx_L1_error)
-  __pyx_t_2 = PyFloat_FromDouble(a_polytrack3_pos((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 32, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 35, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(a_polytrack3_pos((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":25
- *         a_polytrack3_out(&self.ctx, ts, out)
+  /* "python/src/a/polytrack.pxi":28
+ *         a_polytrack3_out(&self.ctx, dt, out)
  *         return out[0], out[1], out[2]
- *     def pos(self, ts):             # <<<<<<<<<<<<<<
+ *     def pos(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate position'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
@@ -14788,37 +14872,37 @@
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_it);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":33
+/* "python/src/a/polytrack.pxi":36
  *             return out
- *         return a_polytrack3_pos(&self.ctx, ts)
- *     def vec(self, ts):             # <<<<<<<<<<<<<<
+ *         return a_polytrack3_pos(&self.ctx, dt)
+ *     def vec(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate velocity'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack3_7vec(PyObject *__pyx_v_self, PyObject *__pyx_v_ts); /*proto*/
-static char __pyx_doc_4liba_10polytrack3_6vec[] = "calculate velocity";
-static PyObject *__pyx_pw_4liba_10polytrack3_7vec(PyObject *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pw_4liba_10polytrack3_9vec(PyObject *__pyx_v_self, PyObject *__pyx_v_dt); /*proto*/
+static char __pyx_doc_4liba_10polytrack3_8vec[] = "calculate velocity";
+static PyObject *__pyx_pw_4liba_10polytrack3_9vec(PyObject *__pyx_v_self, PyObject *__pyx_v_dt) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("vec (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_6vec(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((PyObject *)__pyx_v_ts));
+  __pyx_r = __pyx_pf_4liba_10polytrack3_8vec(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((PyObject *)__pyx_v_dt));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4liba_10polytrack3_6vec(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pf_4liba_10polytrack3_8vec(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_dt) {
   arrayobject *__pyx_v_out = NULL;
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_v_it = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -14829,162 +14913,162 @@
   PyObject *__pyx_t_7 = NULL;
   a_real_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("vec", 0);
 
-  /* "python/src/a/polytrack.pxi":35
- *     def vec(self, ts):
+  /* "python/src/a/polytrack.pxi":38
+ *     def vec(self, dt):
  *         '''calculate velocity'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
-  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_ts) != 0);
+  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_dt) != 0);
   if (__pyx_t_1) {
 
-    /* "python/src/a/polytrack.pxi":36
+    /* "python/src/a/polytrack.pxi":39
  *         '''calculate velocity'''
- *         if iterable(ts):
- *             out = reals(ts)             # <<<<<<<<<<<<<<
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):
+ *             out = reals(dt)             # <<<<<<<<<<<<<<
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack3_vec(&self.ctx, it)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 36, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_out = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":37
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+    /* "python/src/a/polytrack.pxi":40
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack3_vec(&self.ctx, it)
  *             return out
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
-    if (likely(PyList_CheckExact(__pyx_v_ts)) || PyTuple_CheckExact(__pyx_v_ts)) {
-      __pyx_t_4 = __pyx_v_ts; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+    if (likely(PyList_CheckExact(__pyx_v_dt)) || PyTuple_CheckExact(__pyx_v_dt)) {
+      __pyx_t_4 = __pyx_v_dt; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ts); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 37, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_dt); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 40, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 37, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 40, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 37, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 40, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 37, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 40, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 37, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 40, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 37, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 40, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(9, 37, __pyx_L1_error)
+            else __PYX_ERR(9, 40, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 37, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 40, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":38
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":41
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack3_vec(&self.ctx, it)             # <<<<<<<<<<<<<<
  *             return out
- *         return a_polytrack3_vec(&self.ctx, ts)
+ *         return a_polytrack3_vec(&self.ctx, dt)
  */
-      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 38, __pyx_L1_error)
-      __pyx_t_7 = PyFloat_FromDouble(a_polytrack3_vec((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 38, __pyx_L1_error)
+      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 41, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble(a_polytrack3_vec((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 41, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 38, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 41, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":37
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+      /* "python/src/a/polytrack.pxi":40
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack3_vec(&self.ctx, it)
  *             return out
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":39
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":42
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack3_vec(&self.ctx, it)
  *             return out             # <<<<<<<<<<<<<<
- *         return a_polytrack3_vec(&self.ctx, ts)
- *     def acc(self, ts):
+ *         return a_polytrack3_vec(&self.ctx, dt)
+ *     def acc(self, dt):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_out));
     __pyx_r = ((PyObject *)__pyx_v_out);
     goto __pyx_L0;
 
-    /* "python/src/a/polytrack.pxi":35
- *     def vec(self, ts):
+    /* "python/src/a/polytrack.pxi":38
+ *     def vec(self, dt):
  *         '''calculate velocity'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
   }
 
-  /* "python/src/a/polytrack.pxi":40
+  /* "python/src/a/polytrack.pxi":43
  *                 out[i] = a_polytrack3_vec(&self.ctx, it)
  *             return out
- *         return a_polytrack3_vec(&self.ctx, ts)             # <<<<<<<<<<<<<<
- *     def acc(self, ts):
+ *         return a_polytrack3_vec(&self.ctx, dt)             # <<<<<<<<<<<<<<
+ *     def acc(self, dt):
  *         '''calculate acceleration'''
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_ts); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 40, __pyx_L1_error)
-  __pyx_t_2 = PyFloat_FromDouble(a_polytrack3_vec((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 40, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 43, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(a_polytrack3_vec((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":33
+  /* "python/src/a/polytrack.pxi":36
  *             return out
- *         return a_polytrack3_pos(&self.ctx, ts)
- *     def vec(self, ts):             # <<<<<<<<<<<<<<
+ *         return a_polytrack3_pos(&self.ctx, dt)
+ *     def vec(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate velocity'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
@@ -14995,37 +15079,37 @@
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_it);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":41
+/* "python/src/a/polytrack.pxi":44
  *             return out
- *         return a_polytrack3_vec(&self.ctx, ts)
- *     def acc(self, ts):             # <<<<<<<<<<<<<<
+ *         return a_polytrack3_vec(&self.ctx, dt)
+ *     def acc(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate acceleration'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack3_9acc(PyObject *__pyx_v_self, PyObject *__pyx_v_ts); /*proto*/
-static char __pyx_doc_4liba_10polytrack3_8acc[] = "calculate acceleration";
-static PyObject *__pyx_pw_4liba_10polytrack3_9acc(PyObject *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pw_4liba_10polytrack3_11acc(PyObject *__pyx_v_self, PyObject *__pyx_v_dt); /*proto*/
+static char __pyx_doc_4liba_10polytrack3_10acc[] = "calculate acceleration";
+static PyObject *__pyx_pw_4liba_10polytrack3_11acc(PyObject *__pyx_v_self, PyObject *__pyx_v_dt) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("acc (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_8acc(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((PyObject *)__pyx_v_ts));
+  __pyx_r = __pyx_pf_4liba_10polytrack3_10acc(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((PyObject *)__pyx_v_dt));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4liba_10polytrack3_8acc(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pf_4liba_10polytrack3_10acc(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_dt) {
   arrayobject *__pyx_v_out = NULL;
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_v_it = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -15036,162 +15120,162 @@
   PyObject *__pyx_t_7 = NULL;
   a_real_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("acc", 0);
 
-  /* "python/src/a/polytrack.pxi":43
- *     def acc(self, ts):
+  /* "python/src/a/polytrack.pxi":46
+ *     def acc(self, dt):
  *         '''calculate acceleration'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
-  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_ts) != 0);
+  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_dt) != 0);
   if (__pyx_t_1) {
 
-    /* "python/src/a/polytrack.pxi":44
+    /* "python/src/a/polytrack.pxi":47
  *         '''calculate acceleration'''
- *         if iterable(ts):
- *             out = reals(ts)             # <<<<<<<<<<<<<<
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):
+ *             out = reals(dt)             # <<<<<<<<<<<<<<
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack3_acc(&self.ctx, it)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 44, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 47, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_out = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":45
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+    /* "python/src/a/polytrack.pxi":48
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack3_acc(&self.ctx, it)
  *             return out
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
-    if (likely(PyList_CheckExact(__pyx_v_ts)) || PyTuple_CheckExact(__pyx_v_ts)) {
-      __pyx_t_4 = __pyx_v_ts; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+    if (likely(PyList_CheckExact(__pyx_v_dt)) || PyTuple_CheckExact(__pyx_v_dt)) {
+      __pyx_t_4 = __pyx_v_dt; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ts); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 45, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_dt); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 48, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 45, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 48, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 45, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 48, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 45, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 48, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 45, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 48, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 45, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 48, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(9, 45, __pyx_L1_error)
+            else __PYX_ERR(9, 48, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 45, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 48, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":46
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":49
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack3_acc(&self.ctx, it)             # <<<<<<<<<<<<<<
  *             return out
- *         return a_polytrack3_acc(&self.ctx, ts)
+ *         return a_polytrack3_acc(&self.ctx, dt)
  */
-      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 46, __pyx_L1_error)
-      __pyx_t_7 = PyFloat_FromDouble(a_polytrack3_acc((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 46, __pyx_L1_error)
+      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 49, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble(a_polytrack3_acc((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 49, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 46, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 49, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":45
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+      /* "python/src/a/polytrack.pxi":48
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack3_acc(&self.ctx, it)
  *             return out
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":47
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":50
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack3_acc(&self.ctx, it)
  *             return out             # <<<<<<<<<<<<<<
- *         return a_polytrack3_acc(&self.ctx, ts)
- *     def gen(self):
+ *         return a_polytrack3_acc(&self.ctx, dt)
+ * 
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_out));
     __pyx_r = ((PyObject *)__pyx_v_out);
     goto __pyx_L0;
 
-    /* "python/src/a/polytrack.pxi":43
- *     def acc(self, ts):
+    /* "python/src/a/polytrack.pxi":46
+ *     def acc(self, dt):
  *         '''calculate acceleration'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
   }
 
-  /* "python/src/a/polytrack.pxi":48
+  /* "python/src/a/polytrack.pxi":51
  *                 out[i] = a_polytrack3_acc(&self.ctx, it)
  *             return out
- *         return a_polytrack3_acc(&self.ctx, ts)             # <<<<<<<<<<<<<<
- *     def gen(self):
- *         '''generation function'''
+ *         return a_polytrack3_acc(&self.ctx, dt)             # <<<<<<<<<<<<<<
+ * 
+ *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_ts); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 48, __pyx_L1_error)
-  __pyx_t_2 = PyFloat_FromDouble(a_polytrack3_acc((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 48, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 51, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(a_polytrack3_acc((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":41
+  /* "python/src/a/polytrack.pxi":44
  *             return out
- *         return a_polytrack3_vec(&self.ctx, ts)
- *     def acc(self, ts):             # <<<<<<<<<<<<<<
+ *         return a_polytrack3_vec(&self.ctx, dt)
+ *     def acc(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate acceleration'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
@@ -15202,65 +15286,14 @@
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_it);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":49
- *             return out
- *         return a_polytrack3_acc(&self.ctx, ts)
- *     def gen(self):             # <<<<<<<<<<<<<<
- *         '''generation function'''
- *         a_polytrack3_gen(&self.ctx)
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack3_11gen(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_4liba_10polytrack3_10gen[] = "generation function";
-static PyObject *__pyx_pw_4liba_10polytrack3_11gen(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("gen (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_10gen(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack3_10gen(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("gen", 0);
-
-  /* "python/src/a/polytrack.pxi":51
- *     def gen(self):
- *         '''generation function'''
- *         a_polytrack3_gen(&self.ctx)             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  a_polytrack3_gen((&__pyx_v_self->ctx));
-
-  /* "python/src/a/polytrack.pxi":49
- *             return out
- *         return a_polytrack3_acc(&self.ctx, ts)
- *     def gen(self):             # <<<<<<<<<<<<<<
- *         '''generation function'''
- *         a_polytrack3_gen(&self.ctx)
- */
-
-  /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 /* "python/src/a/polytrack.pxi":54
  * 
  *     @property
  *     def k(self):             # <<<<<<<<<<<<<<
  *         return self.ctx.k
  * 
  */
@@ -15288,15 +15321,15 @@
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "python/src/a/polytrack.pxi":55
  *     @property
  *     def k(self):
  *         return self.ctx.k             # <<<<<<<<<<<<<<
  * 
- *     @property
+ * @cython.wraparound(False)
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.k, 4); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -15316,1184 +15349,14 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":58
- * 
- *     @property
- *     def t(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.t
- *     @t.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack3_1t_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack3_1t_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_1t___get__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack3_1t___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":59
- *     @property
- *     def t(self):
- *         return self.ctx.t             # <<<<<<<<<<<<<<
- *     @t.setter
- *     def t(self, val):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.t, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 59, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":58
- * 
- *     @property
- *     def t(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.t
- *     @t.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack3.t.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":61
- *         return self.ctx.t
- *     @t.setter
- *     def t(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.t[0] = val[0]
- *         self.ctx.t[1] = val[1]
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack3_1t_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack3_1t_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_1t_2__set__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((PyObject *)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack3_1t_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  a_real_t __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":62
- *     @t.setter
- *     def t(self, val):
- *         self.ctx.t[0] = val[0]             # <<<<<<<<<<<<<<
- *         self.ctx.t[1] = val[1]
- * 
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 62, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 62, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.t[0]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":63
- *     def t(self, val):
- *         self.ctx.t[0] = val[0]
- *         self.ctx.t[1] = val[1]             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 63, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 63, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.t[1]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":61
- *         return self.ctx.t
- *     @t.setter
- *     def t(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.t[0] = val[0]
- *         self.ctx.t[1] = val[1]
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack3.t.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":66
- * 
- *     @property
- *     def q(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.q
- *     @q.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack3_1q_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack3_1q_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_1q___get__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack3_1q___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":67
- *     @property
- *     def q(self):
- *         return self.ctx.q             # <<<<<<<<<<<<<<
- *     @q.setter
- *     def q(self, val):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.q, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 67, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":66
- * 
- *     @property
- *     def q(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.q
- *     @q.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack3.q.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":69
- *         return self.ctx.q
- *     @q.setter
- *     def q(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.q[0] = val[0]
- *         self.ctx.q[1] = val[1]
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack3_1q_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack3_1q_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_1q_2__set__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((PyObject *)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack3_1q_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  a_real_t __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":70
- *     @q.setter
- *     def q(self, val):
- *         self.ctx.q[0] = val[0]             # <<<<<<<<<<<<<<
- *         self.ctx.q[1] = val[1]
- * 
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 70, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 70, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.q[0]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":71
- *     def q(self, val):
- *         self.ctx.q[0] = val[0]
- *         self.ctx.q[1] = val[1]             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 71, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 71, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.q[1]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":69
- *         return self.ctx.q
- *     @q.setter
- *     def q(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.q[0] = val[0]
- *         self.ctx.q[1] = val[1]
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack3.q.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":74
- * 
- *     @property
- *     def v(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.v
- *     @v.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack3_1v_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack3_1v_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_1v___get__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack3_1v___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":75
- *     @property
- *     def v(self):
- *         return self.ctx.v             # <<<<<<<<<<<<<<
- *     @v.setter
- *     def v(self, val):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.v, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 75, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":74
- * 
- *     @property
- *     def v(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.v
- *     @v.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack3.v.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":77
- *         return self.ctx.v
- *     @v.setter
- *     def v(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.v[0] = val[0]
- *         self.ctx.v[1] = val[1]
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack3_1v_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack3_1v_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_1v_2__set__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((PyObject *)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack3_1v_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  a_real_t __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":78
- *     @v.setter
- *     def v(self, val):
- *         self.ctx.v[0] = val[0]             # <<<<<<<<<<<<<<
- *         self.ctx.v[1] = val[1]
- * 
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 78, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 78, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.v[0]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":79
- *     def v(self, val):
- *         self.ctx.v[0] = val[0]
- *         self.ctx.v[1] = val[1]             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 79, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 79, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.v[1]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":77
- *         return self.ctx.v
- *     @v.setter
- *     def v(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.v[0] = val[0]
- *         self.ctx.v[1] = val[1]
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack3.v.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":82
- * 
- *     @property
- *     def t0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.t[0]
- *     @t0.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack3_2t0_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack3_2t0_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_2t0___get__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack3_2t0___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":83
- *     @property
- *     def t0(self) -> a_real_t:
- *         return self.ctx.t[0]             # <<<<<<<<<<<<<<
- *     @t0.setter
- *     def t0(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.t[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 83, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":82
- * 
- *     @property
- *     def t0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.t[0]
- *     @t0.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack3.t0.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":85
- *         return self.ctx.t[0]
- *     @t0.setter
- *     def t0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.t[0] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack3_2t0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack3_2t0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 85, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack3.t0.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack3_2t0_2__set__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack3_2t0_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":86
- *     @t0.setter
- *     def t0(self, val: a_real_t):
- *         self.ctx.t[0] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.t[0]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":85
- *         return self.ctx.t[0]
- *     @t0.setter
- *     def t0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.t[0] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":89
- * 
- *     @property
- *     def q0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.q[0]
- *     @q0.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack3_2q0_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack3_2q0_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_2q0___get__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack3_2q0___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":90
- *     @property
- *     def q0(self) -> a_real_t:
- *         return self.ctx.q[0]             # <<<<<<<<<<<<<<
- *     @q0.setter
- *     def q0(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.q[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":89
- * 
- *     @property
- *     def q0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.q[0]
- *     @q0.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack3.q0.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":92
- *         return self.ctx.q[0]
- *     @q0.setter
- *     def q0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.q[0] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack3_2q0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack3_2q0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 92, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack3.q0.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack3_2q0_2__set__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack3_2q0_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":93
- *     @q0.setter
- *     def q0(self, val: a_real_t):
- *         self.ctx.q[0] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.q[0]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":92
- *         return self.ctx.q[0]
- *     @q0.setter
- *     def q0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.q[0] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":96
- * 
- *     @property
- *     def v0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.v[0]
- *     @v0.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack3_2v0_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack3_2v0_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_2v0___get__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack3_2v0___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":97
- *     @property
- *     def v0(self) -> a_real_t:
- *         return self.ctx.v[0]             # <<<<<<<<<<<<<<
- *     @v0.setter
- *     def v0(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.v[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 97, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":96
- * 
- *     @property
- *     def v0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.v[0]
- *     @v0.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack3.v0.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":99
- *         return self.ctx.v[0]
- *     @v0.setter
- *     def v0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.v[0] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack3_2v0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack3_2v0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 99, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack3.v0.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack3_2v0_2__set__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack3_2v0_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":100
- *     @v0.setter
- *     def v0(self, val: a_real_t):
- *         self.ctx.v[0] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.v[0]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":99
- *         return self.ctx.v[0]
- *     @v0.setter
- *     def v0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.v[0] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":103
- * 
- *     @property
- *     def t1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.t[1]
- *     @t1.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack3_2t1_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack3_2t1_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_2t1___get__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack3_2t1___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":104
- *     @property
- *     def t1(self) -> a_real_t:
- *         return self.ctx.t[1]             # <<<<<<<<<<<<<<
- *     @t1.setter
- *     def t1(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.t[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 104, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":103
- * 
- *     @property
- *     def t1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.t[1]
- *     @t1.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack3.t1.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":106
- *         return self.ctx.t[1]
- *     @t1.setter
- *     def t1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.t[1] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack3_2t1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack3_2t1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 106, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack3.t1.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack3_2t1_2__set__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack3_2t1_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":107
- *     @t1.setter
- *     def t1(self, val: a_real_t):
- *         self.ctx.t[1] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.t[1]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":106
- *         return self.ctx.t[1]
- *     @t1.setter
- *     def t1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.t[1] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":110
- * 
- *     @property
- *     def q1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.q[1]
- *     @q1.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack3_2q1_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack3_2q1_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_2q1___get__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack3_2q1___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":111
- *     @property
- *     def q1(self) -> a_real_t:
- *         return self.ctx.q[1]             # <<<<<<<<<<<<<<
- *     @q1.setter
- *     def q1(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.q[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 111, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":110
- * 
- *     @property
- *     def q1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.q[1]
- *     @q1.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack3.q1.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":113
- *         return self.ctx.q[1]
- *     @q1.setter
- *     def q1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.q[1] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack3_2q1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack3_2q1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 113, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack3.q1.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack3_2q1_2__set__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack3_2q1_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":114
- *     @q1.setter
- *     def q1(self, val: a_real_t):
- *         self.ctx.q[1] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.q[1]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":113
- *         return self.ctx.q[1]
- *     @q1.setter
- *     def q1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.q[1] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":117
- * 
- *     @property
- *     def v1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.v[1]
- *     @v1.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack3_2v1_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack3_2v1_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack3_2v1___get__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack3_2v1___get__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":118
- *     @property
- *     def v1(self) -> a_real_t:
- *         return self.ctx.v[1]             # <<<<<<<<<<<<<<
- *     @v1.setter
- *     def v1(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.v[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 118, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":117
- * 
- *     @property
- *     def v1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.v[1]
- *     @v1.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack3.v1.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":120
- *         return self.ctx.v[1]
- *     @v1.setter
- *     def v1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.v[1] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack3_2v1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack3_2v1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 120, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack3.v1.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack3_2v1_2__set__(((struct __pyx_obj_4liba_polytrack3 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack3_2v1_2__set__(struct __pyx_obj_4liba_polytrack3 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":121
- *     @v1.setter
- *     def v1(self, val: a_real_t):
- *         self.ctx.v[1] = val             # <<<<<<<<<<<<<<
- * 
- * @cython.wraparound(False)
- */
-  (__pyx_v_self->ctx.v[1]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":120
- *         return self.ctx.v[1]
- *     @v1.setter
- *     def v1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.v[1] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
@@ -16599,20 +15462,20 @@
   __Pyx_AddTraceback("liba.polytrack3.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":128
+/* "python/src/a/polytrack.pxi":62
  *     '''quintic polynomial trajectory'''
  *     cdef a_polytrack5_s ctx
  *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0):             # <<<<<<<<<<<<<<
- *         a_polytrack5_init(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)
- *     def __call__(self, ts):
+ *         a_polytrack5_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0):
  */
 
 /* Python wrapper */
 static int __pyx_pw_4liba_10polytrack5_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_4liba_10polytrack5_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   a_real_t __pyx_v_t0;
   a_real_t __pyx_v_t1;
@@ -16659,27 +15522,27 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_t0)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_t1)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 8, 1); __PYX_ERR(9, 128, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 8, 1); __PYX_ERR(9, 62, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_q0)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 8, 2); __PYX_ERR(9, 128, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 8, 2); __PYX_ERR(9, 62, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_q1)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 8, 3); __PYX_ERR(9, 128, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 8, 3); __PYX_ERR(9, 62, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v0);
           if (value) { values[4] = value; kw_args--; }
         }
@@ -16699,15 +15562,15 @@
         case  7:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a1);
           if (value) { values[7] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(9, 128, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(9, 62, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
@@ -16719,42 +15582,42 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_t0 = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_t0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 128, __pyx_L3_error)
-    __pyx_v_t1 = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_t1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 128, __pyx_L3_error)
-    __pyx_v_q0 = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_q0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 128, __pyx_L3_error)
-    __pyx_v_q1 = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_q1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 128, __pyx_L3_error)
+    __pyx_v_t0 = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_t0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 62, __pyx_L3_error)
+    __pyx_v_t1 = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_t1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 62, __pyx_L3_error)
+    __pyx_v_q0 = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_q0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 62, __pyx_L3_error)
+    __pyx_v_q1 = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_q1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 62, __pyx_L3_error)
     if (values[4]) {
-      __pyx_v_v0 = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_v0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 128, __pyx_L3_error)
+      __pyx_v_v0 = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_v0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 62, __pyx_L3_error)
     } else {
       __pyx_v_v0 = ((a_real_t)0.0);
     }
     if (values[5]) {
-      __pyx_v_v1 = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_v1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 128, __pyx_L3_error)
+      __pyx_v_v1 = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_v1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 62, __pyx_L3_error)
     } else {
       __pyx_v_v1 = ((a_real_t)0.0);
     }
     if (values[6]) {
-      __pyx_v_a0 = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_a0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 128, __pyx_L3_error)
+      __pyx_v_a0 = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_a0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 62, __pyx_L3_error)
     } else {
       __pyx_v_a0 = ((a_real_t)0.0);
     }
     if (values[7]) {
-      __pyx_v_a1 = __pyx_PyFloat_AsDouble(values[7]); if (unlikely((__pyx_v_a1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 128, __pyx_L3_error)
+      __pyx_v_a1 = __pyx_PyFloat_AsDouble(values[7]); if (unlikely((__pyx_v_a1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 62, __pyx_L3_error)
     } else {
       __pyx_v_a1 = ((a_real_t)0.0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 8, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(9, 128, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 8, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(9, 62, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("liba.polytrack5.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_4liba_10polytrack5___cinit__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), __pyx_v_t0, __pyx_v_t1, __pyx_v_q0, __pyx_v_q1, __pyx_v_v0, __pyx_v_v1, __pyx_v_a0, __pyx_v_a1);
 
@@ -16764,103 +15627,293 @@
 }
 
 static int __pyx_pf_4liba_10polytrack5___cinit__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_t0, a_real_t __pyx_v_t1, a_real_t __pyx_v_q0, a_real_t __pyx_v_q1, a_real_t __pyx_v_v0, a_real_t __pyx_v_v1, a_real_t __pyx_v_a0, a_real_t __pyx_v_a1) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "python/src/a/polytrack.pxi":129
+  /* "python/src/a/polytrack.pxi":63
  *     cdef a_polytrack5_s ctx
  *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0):
- *         a_polytrack5_init(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)             # <<<<<<<<<<<<<<
- *     def __call__(self, ts):
- *         '''calculate all'''
+ *         a_polytrack5_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)             # <<<<<<<<<<<<<<
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0):
+ *         '''generation function'''
  */
-  a_polytrack5_init((&__pyx_v_self->ctx), __pyx_v_t0, __pyx_v_t1, __pyx_v_q0, __pyx_v_q1, __pyx_v_v0, __pyx_v_v1, __pyx_v_a0, __pyx_v_a1);
+  a_polytrack5_gen((&__pyx_v_self->ctx), __pyx_v_t0, __pyx_v_t1, __pyx_v_q0, __pyx_v_q1, __pyx_v_v0, __pyx_v_v1, __pyx_v_a0, __pyx_v_a1);
 
-  /* "python/src/a/polytrack.pxi":128
+  /* "python/src/a/polytrack.pxi":62
  *     '''quintic polynomial trajectory'''
  *     cdef a_polytrack5_s ctx
  *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0):             # <<<<<<<<<<<<<<
- *         a_polytrack5_init(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)
- *     def __call__(self, ts):
+ *         a_polytrack5_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":130
+/* "python/src/a/polytrack.pxi":64
  *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0):
- *         a_polytrack5_init(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)
- *     def __call__(self, ts):             # <<<<<<<<<<<<<<
+ *         a_polytrack5_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0):             # <<<<<<<<<<<<<<
+ *         '''generation function'''
+ *         a_polytrack5_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_4liba_10polytrack5_3gen(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_4liba_10polytrack5_2gen[] = "generation function";
+static PyObject *__pyx_pw_4liba_10polytrack5_3gen(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  a_real_t __pyx_v_t0;
+  a_real_t __pyx_v_t1;
+  a_real_t __pyx_v_q0;
+  a_real_t __pyx_v_q1;
+  a_real_t __pyx_v_v0;
+  a_real_t __pyx_v_v1;
+  a_real_t __pyx_v_a0;
+  a_real_t __pyx_v_a1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("gen (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_t0,&__pyx_n_s_t1,&__pyx_n_s_q0,&__pyx_n_s_q1,&__pyx_n_s_v0,&__pyx_n_s_v1,&__pyx_n_s_a0,&__pyx_n_s_a1,0};
+    PyObject* values[8] = {0,0,0,0,0,0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
+        case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_t0)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_t1)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("gen", 0, 4, 8, 1); __PYX_ERR(9, 64, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_q0)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("gen", 0, 4, 8, 2); __PYX_ERR(9, 64, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_q1)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("gen", 0, 4, 8, 3); __PYX_ERR(9, 64, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  4:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v0);
+          if (value) { values[4] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v1);
+          if (value) { values[5] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  6:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a0);
+          if (value) { values[6] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  7:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a1);
+          if (value) { values[7] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gen") < 0)) __PYX_ERR(9, 64, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
+        case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_t0 = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_t0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 64, __pyx_L3_error)
+    __pyx_v_t1 = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_t1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 64, __pyx_L3_error)
+    __pyx_v_q0 = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_q0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 64, __pyx_L3_error)
+    __pyx_v_q1 = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_q1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 64, __pyx_L3_error)
+    if (values[4]) {
+      __pyx_v_v0 = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_v0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 64, __pyx_L3_error)
+    } else {
+      __pyx_v_v0 = ((a_real_t)0.0);
+    }
+    if (values[5]) {
+      __pyx_v_v1 = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_v1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 64, __pyx_L3_error)
+    } else {
+      __pyx_v_v1 = ((a_real_t)0.0);
+    }
+    if (values[6]) {
+      __pyx_v_a0 = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_a0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 64, __pyx_L3_error)
+    } else {
+      __pyx_v_a0 = ((a_real_t)0.0);
+    }
+    if (values[7]) {
+      __pyx_v_a1 = __pyx_PyFloat_AsDouble(values[7]); if (unlikely((__pyx_v_a1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 64, __pyx_L3_error)
+    } else {
+      __pyx_v_a1 = ((a_real_t)0.0);
+    }
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("gen", 0, 4, 8, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(9, 64, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("liba.polytrack5.gen", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_4liba_10polytrack5_2gen(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), __pyx_v_t0, __pyx_v_t1, __pyx_v_q0, __pyx_v_q1, __pyx_v_v0, __pyx_v_v1, __pyx_v_a0, __pyx_v_a1);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_4liba_10polytrack5_2gen(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_t0, a_real_t __pyx_v_t1, a_real_t __pyx_v_q0, a_real_t __pyx_v_q1, a_real_t __pyx_v_v0, a_real_t __pyx_v_v1, a_real_t __pyx_v_a0, a_real_t __pyx_v_a1) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("gen", 0);
+
+  /* "python/src/a/polytrack.pxi":66
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0):
+ *         '''generation function'''
+ *         a_polytrack5_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)             # <<<<<<<<<<<<<<
+ *     def __call__(self, dt):
+ *         '''calculate all'''
+ */
+  a_polytrack5_gen((&__pyx_v_self->ctx), __pyx_v_t0, __pyx_v_t1, __pyx_v_q0, __pyx_v_q1, __pyx_v_v0, __pyx_v_v1, __pyx_v_a0, __pyx_v_a1);
+
+  /* "python/src/a/polytrack.pxi":64
+ *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0):
+ *         a_polytrack5_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0):             # <<<<<<<<<<<<<<
+ *         '''generation function'''
+ *         a_polytrack5_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "python/src/a/polytrack.pxi":67
+ *         '''generation function'''
+ *         a_polytrack5_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)
+ *     def __call__(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate all'''
  *         cdef a_real_t out[3]
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_3__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_4liba_10polytrack5_2__call__[] = "calculate all";
+static PyObject *__pyx_pw_4liba_10polytrack5_5__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_4liba_10polytrack5_4__call__[] = "calculate all";
 #if CYTHON_UPDATE_DESCRIPTOR_DOC
-struct wrapperbase __pyx_wrapperbase_4liba_10polytrack5_2__call__;
+struct wrapperbase __pyx_wrapperbase_4liba_10polytrack5_4__call__;
 #endif
-static PyObject *__pyx_pw_4liba_10polytrack5_3__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_ts = 0;
+static PyObject *__pyx_pw_4liba_10polytrack5_5__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_dt = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__call__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_ts,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_dt,0};
     PyObject* values[1] = {0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ts)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dt)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(9, 130, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(9, 67, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
-    __pyx_v_ts = values[0];
+    __pyx_v_dt = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(9, 130, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(9, 67, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("liba.polytrack5.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2__call__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), __pyx_v_ts);
+  __pyx_r = __pyx_pf_4liba_10polytrack5_4__call__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), __pyx_v_dt);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4liba_10polytrack5_2__call__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pf_4liba_10polytrack5_4__call__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_dt) {
   a_real_t __pyx_v_out[3];
   arrayobject *__pyx_v_p = NULL;
   arrayobject *__pyx_v_v = NULL;
   arrayobject *__pyx_v_a = NULL;
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_v_it = NULL;
   PyObject *__pyx_r = NULL;
@@ -16875,256 +15928,256 @@
   a_real_t __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "python/src/a/polytrack.pxi":133
+  /* "python/src/a/polytrack.pxi":70
  *         '''calculate all'''
  *         cdef a_real_t out[3]
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             p = reals(ts)
- *             v = reals(ts)
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             p = reals(dt)
+ *             v = reals(dt)
  */
-  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_ts) != 0);
+  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_dt) != 0);
   if (__pyx_t_1) {
 
-    /* "python/src/a/polytrack.pxi":134
+    /* "python/src/a/polytrack.pxi":71
  *         cdef a_real_t out[3]
- *         if iterable(ts):
- *             p = reals(ts)             # <<<<<<<<<<<<<<
- *             v = reals(ts)
- *             a = reals(ts)
+ *         if iterable(dt):
+ *             p = reals(dt)             # <<<<<<<<<<<<<<
+ *             v = reals(dt)
+ *             a = reals(dt)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 134, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_p = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":135
- *         if iterable(ts):
- *             p = reals(ts)
- *             v = reals(ts)             # <<<<<<<<<<<<<<
- *             a = reals(ts)
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":72
+ *         if iterable(dt):
+ *             p = reals(dt)
+ *             v = reals(dt)             # <<<<<<<<<<<<<<
+ *             a = reals(dt)
+ *             for i, it in enumerate(dt):
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 135, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_v = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":136
- *             p = reals(ts)
- *             v = reals(ts)
- *             a = reals(ts)             # <<<<<<<<<<<<<<
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":73
+ *             p = reals(dt)
+ *             v = reals(dt)
+ *             a = reals(dt)             # <<<<<<<<<<<<<<
+ *             for i, it in enumerate(dt):
  *                 a_polytrack5_out(&self.ctx, it, out)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 136, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_a = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":137
- *             v = reals(ts)
- *             a = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+    /* "python/src/a/polytrack.pxi":74
+ *             v = reals(dt)
+ *             a = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 a_polytrack5_out(&self.ctx, it, out)
  *                 p[i] = out[0]
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
-    if (likely(PyList_CheckExact(__pyx_v_ts)) || PyTuple_CheckExact(__pyx_v_ts)) {
-      __pyx_t_4 = __pyx_v_ts; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+    if (likely(PyList_CheckExact(__pyx_v_dt)) || PyTuple_CheckExact(__pyx_v_dt)) {
+      __pyx_t_4 = __pyx_v_dt; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ts); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 137, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_dt); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 74, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 137, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 74, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 137, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 74, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 137, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 74, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 137, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 74, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 137, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 74, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(9, 137, __pyx_L1_error)
+            else __PYX_ERR(9, 74, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 137, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 74, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":138
- *             a = reals(ts)
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":75
+ *             a = reals(dt)
+ *             for i, it in enumerate(dt):
  *                 a_polytrack5_out(&self.ctx, it, out)             # <<<<<<<<<<<<<<
  *                 p[i] = out[0]
  *                 v[i] = out[1]
  */
-      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 138, __pyx_L1_error)
+      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 75, __pyx_L1_error)
       a_polytrack5_out((&__pyx_v_self->ctx), __pyx_t_8, __pyx_v_out);
 
-      /* "python/src/a/polytrack.pxi":139
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":76
+ *             for i, it in enumerate(dt):
  *                 a_polytrack5_out(&self.ctx, it, out)
  *                 p[i] = out[0]             # <<<<<<<<<<<<<<
  *                 v[i] = out[1]
  *                 a[i] = out[2]
  */
-      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[0])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 139, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[0])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 76, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_p), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 139, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_p), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 76, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":140
+      /* "python/src/a/polytrack.pxi":77
  *                 a_polytrack5_out(&self.ctx, it, out)
  *                 p[i] = out[0]
  *                 v[i] = out[1]             # <<<<<<<<<<<<<<
  *                 a[i] = out[2]
  *             return p, v, a
  */
-      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[1])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 140, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[1])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 77, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_v), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 140, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_v), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 77, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":141
+      /* "python/src/a/polytrack.pxi":78
  *                 p[i] = out[0]
  *                 v[i] = out[1]
  *                 a[i] = out[2]             # <<<<<<<<<<<<<<
  *             return p, v, a
- *         a_polytrack5_out(&self.ctx, ts, out)
+ *         a_polytrack5_out(&self.ctx, dt, out)
  */
-      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[2])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 141, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[2])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 78, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_a), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 141, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_a), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 78, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":137
- *             v = reals(ts)
- *             a = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+      /* "python/src/a/polytrack.pxi":74
+ *             v = reals(dt)
+ *             a = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 a_polytrack5_out(&self.ctx, it, out)
  *                 p[i] = out[0]
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":142
+    /* "python/src/a/polytrack.pxi":79
  *                 v[i] = out[1]
  *                 a[i] = out[2]
  *             return p, v, a             # <<<<<<<<<<<<<<
- *         a_polytrack5_out(&self.ctx, ts, out)
+ *         a_polytrack5_out(&self.ctx, dt, out)
  *         return out[0], out[1], out[2]
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 142, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 79, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(((PyObject *)__pyx_v_p));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_p));
     PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_v_p));
     __Pyx_INCREF(((PyObject *)__pyx_v_v));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_v));
     PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)__pyx_v_v));
     __Pyx_INCREF(((PyObject *)__pyx_v_a));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_a));
     PyTuple_SET_ITEM(__pyx_t_2, 2, ((PyObject *)__pyx_v_a));
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "python/src/a/polytrack.pxi":133
+    /* "python/src/a/polytrack.pxi":70
  *         '''calculate all'''
  *         cdef a_real_t out[3]
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             p = reals(ts)
- *             v = reals(ts)
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             p = reals(dt)
+ *             v = reals(dt)
  */
   }
 
-  /* "python/src/a/polytrack.pxi":143
+  /* "python/src/a/polytrack.pxi":80
  *                 a[i] = out[2]
  *             return p, v, a
- *         a_polytrack5_out(&self.ctx, ts, out)             # <<<<<<<<<<<<<<
+ *         a_polytrack5_out(&self.ctx, dt, out)             # <<<<<<<<<<<<<<
  *         return out[0], out[1], out[2]
- *     def pos(self, ts):
+ *     def pos(self, dt):
  */
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_ts); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 143, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 80, __pyx_L1_error)
   a_polytrack5_out((&__pyx_v_self->ctx), __pyx_t_8, __pyx_v_out);
 
-  /* "python/src/a/polytrack.pxi":144
+  /* "python/src/a/polytrack.pxi":81
  *             return p, v, a
- *         a_polytrack5_out(&self.ctx, ts, out)
+ *         a_polytrack5_out(&self.ctx, dt, out)
  *         return out[0], out[1], out[2]             # <<<<<<<<<<<<<<
- *     def pos(self, ts):
+ *     def pos(self, dt):
  *         '''calculate position'''
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_out[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 144, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_out[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_out[1])); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 144, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_out[1])); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[2])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 144, __pyx_L1_error)
+  __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[2])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(9, 144, __pyx_L1_error)
+  __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(9, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_t_7);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
   __pyx_t_7 = 0;
   __pyx_r = __pyx_t_9;
   __pyx_t_9 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":130
- *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0):
- *         a_polytrack5_init(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)
- *     def __call__(self, ts):             # <<<<<<<<<<<<<<
+  /* "python/src/a/polytrack.pxi":67
+ *         '''generation function'''
+ *         a_polytrack5_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1)
+ *     def __call__(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate all'''
  *         cdef a_real_t out[3]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -17140,37 +16193,37 @@
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_it);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":145
- *         a_polytrack5_out(&self.ctx, ts, out)
+/* "python/src/a/polytrack.pxi":82
+ *         a_polytrack5_out(&self.ctx, dt, out)
  *         return out[0], out[1], out[2]
- *     def pos(self, ts):             # <<<<<<<<<<<<<<
+ *     def pos(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate position'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_5pos(PyObject *__pyx_v_self, PyObject *__pyx_v_ts); /*proto*/
-static char __pyx_doc_4liba_10polytrack5_4pos[] = "calculate position";
-static PyObject *__pyx_pw_4liba_10polytrack5_5pos(PyObject *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pw_4liba_10polytrack5_7pos(PyObject *__pyx_v_self, PyObject *__pyx_v_dt); /*proto*/
+static char __pyx_doc_4liba_10polytrack5_6pos[] = "calculate position";
+static PyObject *__pyx_pw_4liba_10polytrack5_7pos(PyObject *__pyx_v_self, PyObject *__pyx_v_dt) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("pos (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_4pos(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((PyObject *)__pyx_v_ts));
+  __pyx_r = __pyx_pf_4liba_10polytrack5_6pos(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((PyObject *)__pyx_v_dt));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4liba_10polytrack5_4pos(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pf_4liba_10polytrack5_6pos(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_dt) {
   arrayobject *__pyx_v_out = NULL;
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_v_it = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -17181,162 +16234,162 @@
   PyObject *__pyx_t_7 = NULL;
   a_real_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pos", 0);
 
-  /* "python/src/a/polytrack.pxi":147
- *     def pos(self, ts):
+  /* "python/src/a/polytrack.pxi":84
+ *     def pos(self, dt):
  *         '''calculate position'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
-  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_ts) != 0);
+  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_dt) != 0);
   if (__pyx_t_1) {
 
-    /* "python/src/a/polytrack.pxi":148
+    /* "python/src/a/polytrack.pxi":85
  *         '''calculate position'''
- *         if iterable(ts):
- *             out = reals(ts)             # <<<<<<<<<<<<<<
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):
+ *             out = reals(dt)             # <<<<<<<<<<<<<<
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack5_pos(&self.ctx, it)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 148, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 85, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_out = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":149
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+    /* "python/src/a/polytrack.pxi":86
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack5_pos(&self.ctx, it)
  *             return out
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
-    if (likely(PyList_CheckExact(__pyx_v_ts)) || PyTuple_CheckExact(__pyx_v_ts)) {
-      __pyx_t_4 = __pyx_v_ts; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+    if (likely(PyList_CheckExact(__pyx_v_dt)) || PyTuple_CheckExact(__pyx_v_dt)) {
+      __pyx_t_4 = __pyx_v_dt; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ts); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 149, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_dt); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 86, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 149, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 86, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 149, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 86, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 149, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 86, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 149, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 86, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 149, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 86, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(9, 149, __pyx_L1_error)
+            else __PYX_ERR(9, 86, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 149, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 86, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":150
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":87
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack5_pos(&self.ctx, it)             # <<<<<<<<<<<<<<
  *             return out
- *         return a_polytrack5_pos(&self.ctx, ts)
+ *         return a_polytrack5_pos(&self.ctx, dt)
  */
-      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 150, __pyx_L1_error)
-      __pyx_t_7 = PyFloat_FromDouble(a_polytrack5_pos((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 150, __pyx_L1_error)
+      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 87, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble(a_polytrack5_pos((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 87, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 150, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 87, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":149
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+      /* "python/src/a/polytrack.pxi":86
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack5_pos(&self.ctx, it)
  *             return out
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":151
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":88
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack5_pos(&self.ctx, it)
  *             return out             # <<<<<<<<<<<<<<
- *         return a_polytrack5_pos(&self.ctx, ts)
- *     def vec(self, ts):
+ *         return a_polytrack5_pos(&self.ctx, dt)
+ *     def vec(self, dt):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_out));
     __pyx_r = ((PyObject *)__pyx_v_out);
     goto __pyx_L0;
 
-    /* "python/src/a/polytrack.pxi":147
- *     def pos(self, ts):
+    /* "python/src/a/polytrack.pxi":84
+ *     def pos(self, dt):
  *         '''calculate position'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
   }
 
-  /* "python/src/a/polytrack.pxi":152
+  /* "python/src/a/polytrack.pxi":89
  *                 out[i] = a_polytrack5_pos(&self.ctx, it)
  *             return out
- *         return a_polytrack5_pos(&self.ctx, ts)             # <<<<<<<<<<<<<<
- *     def vec(self, ts):
+ *         return a_polytrack5_pos(&self.ctx, dt)             # <<<<<<<<<<<<<<
+ *     def vec(self, dt):
  *         '''calculate velocity'''
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_ts); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 152, __pyx_L1_error)
-  __pyx_t_2 = PyFloat_FromDouble(a_polytrack5_pos((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 152, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 89, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(a_polytrack5_pos((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":145
- *         a_polytrack5_out(&self.ctx, ts, out)
+  /* "python/src/a/polytrack.pxi":82
+ *         a_polytrack5_out(&self.ctx, dt, out)
  *         return out[0], out[1], out[2]
- *     def pos(self, ts):             # <<<<<<<<<<<<<<
+ *     def pos(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate position'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
@@ -17347,37 +16400,37 @@
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_it);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":153
+/* "python/src/a/polytrack.pxi":90
  *             return out
- *         return a_polytrack5_pos(&self.ctx, ts)
- *     def vec(self, ts):             # <<<<<<<<<<<<<<
+ *         return a_polytrack5_pos(&self.ctx, dt)
+ *     def vec(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate velocity'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_7vec(PyObject *__pyx_v_self, PyObject *__pyx_v_ts); /*proto*/
-static char __pyx_doc_4liba_10polytrack5_6vec[] = "calculate velocity";
-static PyObject *__pyx_pw_4liba_10polytrack5_7vec(PyObject *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pw_4liba_10polytrack5_9vec(PyObject *__pyx_v_self, PyObject *__pyx_v_dt); /*proto*/
+static char __pyx_doc_4liba_10polytrack5_8vec[] = "calculate velocity";
+static PyObject *__pyx_pw_4liba_10polytrack5_9vec(PyObject *__pyx_v_self, PyObject *__pyx_v_dt) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("vec (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_6vec(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((PyObject *)__pyx_v_ts));
+  __pyx_r = __pyx_pf_4liba_10polytrack5_8vec(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((PyObject *)__pyx_v_dt));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4liba_10polytrack5_6vec(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pf_4liba_10polytrack5_8vec(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_dt) {
   arrayobject *__pyx_v_out = NULL;
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_v_it = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -17388,162 +16441,162 @@
   PyObject *__pyx_t_7 = NULL;
   a_real_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("vec", 0);
 
-  /* "python/src/a/polytrack.pxi":155
- *     def vec(self, ts):
+  /* "python/src/a/polytrack.pxi":92
+ *     def vec(self, dt):
  *         '''calculate velocity'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
-  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_ts) != 0);
+  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_dt) != 0);
   if (__pyx_t_1) {
 
-    /* "python/src/a/polytrack.pxi":156
+    /* "python/src/a/polytrack.pxi":93
  *         '''calculate velocity'''
- *         if iterable(ts):
- *             out = reals(ts)             # <<<<<<<<<<<<<<
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):
+ *             out = reals(dt)             # <<<<<<<<<<<<<<
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack5_vec(&self.ctx, it)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 156, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_out = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":157
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+    /* "python/src/a/polytrack.pxi":94
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack5_vec(&self.ctx, it)
  *             return out
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
-    if (likely(PyList_CheckExact(__pyx_v_ts)) || PyTuple_CheckExact(__pyx_v_ts)) {
-      __pyx_t_4 = __pyx_v_ts; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+    if (likely(PyList_CheckExact(__pyx_v_dt)) || PyTuple_CheckExact(__pyx_v_dt)) {
+      __pyx_t_4 = __pyx_v_dt; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ts); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 157, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_dt); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 157, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 94, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 157, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 94, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 157, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 94, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 157, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 94, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 157, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 94, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(9, 157, __pyx_L1_error)
+            else __PYX_ERR(9, 94, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 157, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 94, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":158
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":95
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack5_vec(&self.ctx, it)             # <<<<<<<<<<<<<<
  *             return out
- *         return a_polytrack5_vec(&self.ctx, ts)
+ *         return a_polytrack5_vec(&self.ctx, dt)
  */
-      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 158, __pyx_L1_error)
-      __pyx_t_7 = PyFloat_FromDouble(a_polytrack5_vec((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 158, __pyx_L1_error)
+      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 95, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble(a_polytrack5_vec((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 95, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 158, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 95, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":157
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+      /* "python/src/a/polytrack.pxi":94
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack5_vec(&self.ctx, it)
  *             return out
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":159
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":96
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack5_vec(&self.ctx, it)
  *             return out             # <<<<<<<<<<<<<<
- *         return a_polytrack5_vec(&self.ctx, ts)
- *     def acc(self, ts):
+ *         return a_polytrack5_vec(&self.ctx, dt)
+ *     def acc(self, dt):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_out));
     __pyx_r = ((PyObject *)__pyx_v_out);
     goto __pyx_L0;
 
-    /* "python/src/a/polytrack.pxi":155
- *     def vec(self, ts):
+    /* "python/src/a/polytrack.pxi":92
+ *     def vec(self, dt):
  *         '''calculate velocity'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
   }
 
-  /* "python/src/a/polytrack.pxi":160
+  /* "python/src/a/polytrack.pxi":97
  *                 out[i] = a_polytrack5_vec(&self.ctx, it)
  *             return out
- *         return a_polytrack5_vec(&self.ctx, ts)             # <<<<<<<<<<<<<<
- *     def acc(self, ts):
+ *         return a_polytrack5_vec(&self.ctx, dt)             # <<<<<<<<<<<<<<
+ *     def acc(self, dt):
  *         '''calculate acceleration'''
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_ts); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 160, __pyx_L1_error)
-  __pyx_t_2 = PyFloat_FromDouble(a_polytrack5_vec((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 160, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 97, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(a_polytrack5_vec((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":153
+  /* "python/src/a/polytrack.pxi":90
  *             return out
- *         return a_polytrack5_pos(&self.ctx, ts)
- *     def vec(self, ts):             # <<<<<<<<<<<<<<
+ *         return a_polytrack5_pos(&self.ctx, dt)
+ *     def vec(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate velocity'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
@@ -17554,37 +16607,37 @@
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_it);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":161
+/* "python/src/a/polytrack.pxi":98
  *             return out
- *         return a_polytrack5_vec(&self.ctx, ts)
- *     def acc(self, ts):             # <<<<<<<<<<<<<<
+ *         return a_polytrack5_vec(&self.ctx, dt)
+ *     def acc(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate acceleration'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_9acc(PyObject *__pyx_v_self, PyObject *__pyx_v_ts); /*proto*/
-static char __pyx_doc_4liba_10polytrack5_8acc[] = "calculate acceleration";
-static PyObject *__pyx_pw_4liba_10polytrack5_9acc(PyObject *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pw_4liba_10polytrack5_11acc(PyObject *__pyx_v_self, PyObject *__pyx_v_dt); /*proto*/
+static char __pyx_doc_4liba_10polytrack5_10acc[] = "calculate acceleration";
+static PyObject *__pyx_pw_4liba_10polytrack5_11acc(PyObject *__pyx_v_self, PyObject *__pyx_v_dt) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("acc (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_8acc(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((PyObject *)__pyx_v_ts));
+  __pyx_r = __pyx_pf_4liba_10polytrack5_10acc(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((PyObject *)__pyx_v_dt));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4liba_10polytrack5_8acc(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pf_4liba_10polytrack5_10acc(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_dt) {
   arrayobject *__pyx_v_out = NULL;
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_v_it = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -17595,162 +16648,162 @@
   PyObject *__pyx_t_7 = NULL;
   a_real_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("acc", 0);
 
-  /* "python/src/a/polytrack.pxi":163
- *     def acc(self, ts):
+  /* "python/src/a/polytrack.pxi":100
+ *     def acc(self, dt):
  *         '''calculate acceleration'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
-  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_ts) != 0);
+  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_dt) != 0);
   if (__pyx_t_1) {
 
-    /* "python/src/a/polytrack.pxi":164
+    /* "python/src/a/polytrack.pxi":101
  *         '''calculate acceleration'''
- *         if iterable(ts):
- *             out = reals(ts)             # <<<<<<<<<<<<<<
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):
+ *             out = reals(dt)             # <<<<<<<<<<<<<<
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack5_acc(&self.ctx, it)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 164, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 101, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_out = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":165
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+    /* "python/src/a/polytrack.pxi":102
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack5_acc(&self.ctx, it)
  *             return out
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
-    if (likely(PyList_CheckExact(__pyx_v_ts)) || PyTuple_CheckExact(__pyx_v_ts)) {
-      __pyx_t_4 = __pyx_v_ts; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+    if (likely(PyList_CheckExact(__pyx_v_dt)) || PyTuple_CheckExact(__pyx_v_dt)) {
+      __pyx_t_4 = __pyx_v_dt; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ts); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 165, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_dt); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 102, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 165, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 102, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 165, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 102, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 165, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 102, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 165, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 102, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 165, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 102, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(9, 165, __pyx_L1_error)
+            else __PYX_ERR(9, 102, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 165, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 102, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":166
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":103
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack5_acc(&self.ctx, it)             # <<<<<<<<<<<<<<
  *             return out
- *         return a_polytrack5_acc(&self.ctx, ts)
+ *         return a_polytrack5_acc(&self.ctx, dt)
  */
-      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 166, __pyx_L1_error)
-      __pyx_t_7 = PyFloat_FromDouble(a_polytrack5_acc((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 166, __pyx_L1_error)
+      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 103, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble(a_polytrack5_acc((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 103, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 166, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 103, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":165
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+      /* "python/src/a/polytrack.pxi":102
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack5_acc(&self.ctx, it)
  *             return out
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":167
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":104
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack5_acc(&self.ctx, it)
  *             return out             # <<<<<<<<<<<<<<
- *         return a_polytrack5_acc(&self.ctx, ts)
- *     def gen(self):
+ *         return a_polytrack5_acc(&self.ctx, dt)
+ * 
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_out));
     __pyx_r = ((PyObject *)__pyx_v_out);
     goto __pyx_L0;
 
-    /* "python/src/a/polytrack.pxi":163
- *     def acc(self, ts):
+    /* "python/src/a/polytrack.pxi":100
+ *     def acc(self, dt):
  *         '''calculate acceleration'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
   }
 
-  /* "python/src/a/polytrack.pxi":168
+  /* "python/src/a/polytrack.pxi":105
  *                 out[i] = a_polytrack5_acc(&self.ctx, it)
  *             return out
- *         return a_polytrack5_acc(&self.ctx, ts)             # <<<<<<<<<<<<<<
- *     def gen(self):
- *         '''generation function'''
+ *         return a_polytrack5_acc(&self.ctx, dt)             # <<<<<<<<<<<<<<
+ * 
+ *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_ts); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 168, __pyx_L1_error)
-  __pyx_t_2 = PyFloat_FromDouble(a_polytrack5_acc((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 168, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 105, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(a_polytrack5_acc((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":161
+  /* "python/src/a/polytrack.pxi":98
  *             return out
- *         return a_polytrack5_vec(&self.ctx, ts)
- *     def acc(self, ts):             # <<<<<<<<<<<<<<
+ *         return a_polytrack5_vec(&self.ctx, dt)
+ *     def acc(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate acceleration'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
@@ -17761,66 +16814,15 @@
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_it);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":169
- *             return out
- *         return a_polytrack5_acc(&self.ctx, ts)
- *     def gen(self):             # <<<<<<<<<<<<<<
- *         '''generation function'''
- *         a_polytrack5_gen(&self.ctx)
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_11gen(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_4liba_10polytrack5_10gen[] = "generation function";
-static PyObject *__pyx_pw_4liba_10polytrack5_11gen(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("gen (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_10gen(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack5_10gen(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("gen", 0);
-
-  /* "python/src/a/polytrack.pxi":171
- *     def gen(self):
- *         '''generation function'''
- *         a_polytrack5_gen(&self.ctx)             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  a_polytrack5_gen((&__pyx_v_self->ctx));
-
-  /* "python/src/a/polytrack.pxi":169
- *             return out
- *         return a_polytrack5_acc(&self.ctx, ts)
- *     def gen(self):             # <<<<<<<<<<<<<<
- *         '''generation function'''
- *         a_polytrack5_gen(&self.ctx)
- */
-
-  /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":174
+/* "python/src/a/polytrack.pxi":108
  * 
  *     @property
  *     def k(self):             # <<<<<<<<<<<<<<
  *         return self.ctx.k
  * 
  */
 
@@ -17842,29 +16844,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "python/src/a/polytrack.pxi":175
+  /* "python/src/a/polytrack.pxi":109
  *     @property
  *     def k(self):
  *         return self.ctx.k             # <<<<<<<<<<<<<<
  * 
- *     @property
+ * @cython.wraparound(False)
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.k, 6); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 175, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.k, 6); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":174
+  /* "python/src/a/polytrack.pxi":108
  * 
  *     @property
  *     def k(self):             # <<<<<<<<<<<<<<
  *         return self.ctx.k
  * 
  */
 
@@ -17875,1574 +16877,14 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":178
- * 
- *     @property
- *     def t(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.t
- *     @t.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_1t_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack5_1t_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_1t___get__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack5_1t___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":179
- *     @property
- *     def t(self):
- *         return self.ctx.t             # <<<<<<<<<<<<<<
- *     @t.setter
- *     def t(self, val):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.t, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 179, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":178
- * 
- *     @property
- *     def t(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.t
- *     @t.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.t.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":181
- *         return self.ctx.t
- *     @t.setter
- *     def t(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.t[0] = val[0]
- *         self.ctx.t[1] = val[1]
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack5_1t_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack5_1t_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_1t_2__set__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((PyObject *)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack5_1t_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  a_real_t __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":182
- *     @t.setter
- *     def t(self, val):
- *         self.ctx.t[0] = val[0]             # <<<<<<<<<<<<<<
- *         self.ctx.t[1] = val[1]
- * 
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 182, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 182, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.t[0]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":183
- *     def t(self, val):
- *         self.ctx.t[0] = val[0]
- *         self.ctx.t[1] = val[1]             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 183, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 183, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.t[1]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":181
- *         return self.ctx.t
- *     @t.setter
- *     def t(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.t[0] = val[0]
- *         self.ctx.t[1] = val[1]
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.t.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":186
- * 
- *     @property
- *     def q(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.q
- *     @q.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_1q_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack5_1q_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_1q___get__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack5_1q___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":187
- *     @property
- *     def q(self):
- *         return self.ctx.q             # <<<<<<<<<<<<<<
- *     @q.setter
- *     def q(self, val):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.q, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 187, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":186
- * 
- *     @property
- *     def q(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.q
- *     @q.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.q.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":189
- *         return self.ctx.q
- *     @q.setter
- *     def q(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.q[0] = val[0]
- *         self.ctx.q[1] = val[1]
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack5_1q_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack5_1q_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_1q_2__set__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((PyObject *)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack5_1q_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  a_real_t __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":190
- *     @q.setter
- *     def q(self, val):
- *         self.ctx.q[0] = val[0]             # <<<<<<<<<<<<<<
- *         self.ctx.q[1] = val[1]
- * 
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 190, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 190, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.q[0]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":191
- *     def q(self, val):
- *         self.ctx.q[0] = val[0]
- *         self.ctx.q[1] = val[1]             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 191, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 191, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.q[1]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":189
- *         return self.ctx.q
- *     @q.setter
- *     def q(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.q[0] = val[0]
- *         self.ctx.q[1] = val[1]
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.q.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":194
- * 
- *     @property
- *     def v(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.v
- *     @v.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_1v_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack5_1v_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_1v___get__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack5_1v___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":195
- *     @property
- *     def v(self):
- *         return self.ctx.v             # <<<<<<<<<<<<<<
- *     @v.setter
- *     def v(self, val):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.v, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 195, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":194
- * 
- *     @property
- *     def v(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.v
- *     @v.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.v.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":197
- *         return self.ctx.v
- *     @v.setter
- *     def v(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.v[0] = val[0]
- *         self.ctx.v[1] = val[1]
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack5_1v_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack5_1v_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_1v_2__set__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((PyObject *)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack5_1v_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  a_real_t __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":198
- *     @v.setter
- *     def v(self, val):
- *         self.ctx.v[0] = val[0]             # <<<<<<<<<<<<<<
- *         self.ctx.v[1] = val[1]
- * 
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 198, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 198, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.v[0]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":199
- *     def v(self, val):
- *         self.ctx.v[0] = val[0]
- *         self.ctx.v[1] = val[1]             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 199, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 199, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.v[1]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":197
- *         return self.ctx.v
- *     @v.setter
- *     def v(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.v[0] = val[0]
- *         self.ctx.v[1] = val[1]
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.v.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":202
- * 
- *     @property
- *     def a(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.a
- *     @a.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_1a_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack5_1a_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_1a___get__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack5_1a___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":203
- *     @property
- *     def a(self):
- *         return self.ctx.a             # <<<<<<<<<<<<<<
- *     @a.setter
- *     def a(self, val):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.a, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 203, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":202
- * 
- *     @property
- *     def a(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.a
- *     @a.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.a.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":205
- *         return self.ctx.a
- *     @a.setter
- *     def a(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.a[0] = val[0]
- *         self.ctx.a[1] = val[1]
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack5_1a_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack5_1a_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_1a_2__set__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((PyObject *)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack5_1a_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  a_real_t __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":206
- *     @a.setter
- *     def a(self, val):
- *         self.ctx.a[0] = val[0]             # <<<<<<<<<<<<<<
- *         self.ctx.a[1] = val[1]
- * 
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 206, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 206, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.a[0]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":207
- *     def a(self, val):
- *         self.ctx.a[0] = val[0]
- *         self.ctx.a[1] = val[1]             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 207, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 207, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.a[1]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":205
- *         return self.ctx.a
- *     @a.setter
- *     def a(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.a[0] = val[0]
- *         self.ctx.a[1] = val[1]
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.a.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":210
- * 
- *     @property
- *     def t0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.t[0]
- *     @t0.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_2t0_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack5_2t0_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2t0___get__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack5_2t0___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":211
- *     @property
- *     def t0(self) -> a_real_t:
- *         return self.ctx.t[0]             # <<<<<<<<<<<<<<
- *     @t0.setter
- *     def t0(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.t[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 211, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":210
- * 
- *     @property
- *     def t0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.t[0]
- *     @t0.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.t0.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":213
- *         return self.ctx.t[0]
- *     @t0.setter
- *     def t0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.t[0] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack5_2t0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack5_2t0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 213, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack5.t0.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2t0_2__set__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack5_2t0_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":214
- *     @t0.setter
- *     def t0(self, val: a_real_t):
- *         self.ctx.t[0] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.t[0]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":213
- *         return self.ctx.t[0]
- *     @t0.setter
- *     def t0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.t[0] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":217
- * 
- *     @property
- *     def q0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.q[0]
- *     @q0.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_2q0_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack5_2q0_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2q0___get__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack5_2q0___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":218
- *     @property
- *     def q0(self) -> a_real_t:
- *         return self.ctx.q[0]             # <<<<<<<<<<<<<<
- *     @q0.setter
- *     def q0(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.q[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 218, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":217
- * 
- *     @property
- *     def q0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.q[0]
- *     @q0.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.q0.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":220
- *         return self.ctx.q[0]
- *     @q0.setter
- *     def q0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.q[0] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack5_2q0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack5_2q0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 220, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack5.q0.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2q0_2__set__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack5_2q0_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":221
- *     @q0.setter
- *     def q0(self, val: a_real_t):
- *         self.ctx.q[0] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.q[0]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":220
- *         return self.ctx.q[0]
- *     @q0.setter
- *     def q0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.q[0] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":224
- * 
- *     @property
- *     def v0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.v[0]
- *     @v0.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_2v0_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack5_2v0_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2v0___get__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack5_2v0___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":225
- *     @property
- *     def v0(self) -> a_real_t:
- *         return self.ctx.v[0]             # <<<<<<<<<<<<<<
- *     @v0.setter
- *     def v0(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.v[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 225, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":224
- * 
- *     @property
- *     def v0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.v[0]
- *     @v0.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.v0.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":227
- *         return self.ctx.v[0]
- *     @v0.setter
- *     def v0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.v[0] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack5_2v0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack5_2v0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 227, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack5.v0.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2v0_2__set__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack5_2v0_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":228
- *     @v0.setter
- *     def v0(self, val: a_real_t):
- *         self.ctx.v[0] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.v[0]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":227
- *         return self.ctx.v[0]
- *     @v0.setter
- *     def v0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.v[0] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":231
- * 
- *     @property
- *     def a0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.a[0]
- *     @a0.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_2a0_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack5_2a0_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2a0___get__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack5_2a0___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":232
- *     @property
- *     def a0(self) -> a_real_t:
- *         return self.ctx.a[0]             # <<<<<<<<<<<<<<
- *     @a0.setter
- *     def a0(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.a[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 232, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":231
- * 
- *     @property
- *     def a0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.a[0]
- *     @a0.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.a0.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":234
- *         return self.ctx.a[0]
- *     @a0.setter
- *     def a0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.a[0] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack5_2a0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack5_2a0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 234, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack5.a0.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2a0_2__set__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack5_2a0_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":235
- *     @a0.setter
- *     def a0(self, val: a_real_t):
- *         self.ctx.a[0] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.a[0]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":234
- *         return self.ctx.a[0]
- *     @a0.setter
- *     def a0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.a[0] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":238
- * 
- *     @property
- *     def t1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.t[1]
- *     @t1.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_2t1_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack5_2t1_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2t1___get__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack5_2t1___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":239
- *     @property
- *     def t1(self) -> a_real_t:
- *         return self.ctx.t[1]             # <<<<<<<<<<<<<<
- *     @t1.setter
- *     def t1(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.t[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 239, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":238
- * 
- *     @property
- *     def t1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.t[1]
- *     @t1.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.t1.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":241
- *         return self.ctx.t[1]
- *     @t1.setter
- *     def t1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.t[1] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack5_2t1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack5_2t1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 241, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack5.t1.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2t1_2__set__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack5_2t1_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":242
- *     @t1.setter
- *     def t1(self, val: a_real_t):
- *         self.ctx.t[1] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.t[1]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":241
- *         return self.ctx.t[1]
- *     @t1.setter
- *     def t1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.t[1] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":245
- * 
- *     @property
- *     def q1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.q[1]
- *     @q1.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_2q1_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack5_2q1_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2q1___get__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack5_2q1___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":246
- *     @property
- *     def q1(self) -> a_real_t:
- *         return self.ctx.q[1]             # <<<<<<<<<<<<<<
- *     @q1.setter
- *     def q1(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.q[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 246, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":245
- * 
- *     @property
- *     def q1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.q[1]
- *     @q1.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.q1.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":248
- *         return self.ctx.q[1]
- *     @q1.setter
- *     def q1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.q[1] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack5_2q1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack5_2q1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 248, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack5.q1.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2q1_2__set__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack5_2q1_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":249
- *     @q1.setter
- *     def q1(self, val: a_real_t):
- *         self.ctx.q[1] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.q[1]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":248
- *         return self.ctx.q[1]
- *     @q1.setter
- *     def q1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.q[1] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":252
- * 
- *     @property
- *     def v1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.v[1]
- *     @v1.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_2v1_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack5_2v1_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2v1___get__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack5_2v1___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":253
- *     @property
- *     def v1(self) -> a_real_t:
- *         return self.ctx.v[1]             # <<<<<<<<<<<<<<
- *     @v1.setter
- *     def v1(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.v[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 253, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":252
- * 
- *     @property
- *     def v1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.v[1]
- *     @v1.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.v1.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":255
- *         return self.ctx.v[1]
- *     @v1.setter
- *     def v1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.v[1] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack5_2v1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack5_2v1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 255, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack5.v1.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2v1_2__set__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack5_2v1_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":256
- *     @v1.setter
- *     def v1(self, val: a_real_t):
- *         self.ctx.v[1] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.v[1]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":255
- *         return self.ctx.v[1]
- *     @v1.setter
- *     def v1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.v[1] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":259
- * 
- *     @property
- *     def a1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.a[1]
- *     @a1.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack5_2a1_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack5_2a1_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2a1___get__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack5_2a1___get__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":260
- *     @property
- *     def a1(self) -> a_real_t:
- *         return self.ctx.a[1]             # <<<<<<<<<<<<<<
- *     @a1.setter
- *     def a1(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.a[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 260, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":259
- * 
- *     @property
- *     def a1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.a[1]
- *     @a1.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack5.a1.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":262
- *         return self.ctx.a[1]
- *     @a1.setter
- *     def a1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.a[1] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack5_2a1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack5_2a1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 262, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack5.a1.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack5_2a1_2__set__(((struct __pyx_obj_4liba_polytrack5 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack5_2a1_2__set__(struct __pyx_obj_4liba_polytrack5 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":263
- *     @a1.setter
- *     def a1(self, val: a_real_t):
- *         self.ctx.a[1] = val             # <<<<<<<<<<<<<<
- * 
- * @cython.wraparound(False)
- */
-  (__pyx_v_self->ctx.a[1]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":262
- *         return self.ctx.a[1]
- *     @a1.setter
- *     def a1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.a[1] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
@@ -19548,20 +16990,20 @@
   __Pyx_AddTraceback("liba.polytrack5.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":270
+/* "python/src/a/polytrack.pxi":116
  *     '''hepta polynomial trajectory'''
  *     cdef a_polytrack7_s ctx
  *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0, a_real_t j0 = 0, a_real_t j1 = 0):             # <<<<<<<<<<<<<<
- *         a_polytrack7_init(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)
- *     def __call__(self, ts):
+ *         a_polytrack7_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0, a_real_t j0 = 0, a_real_t j1 = 0):
  */
 
 /* Python wrapper */
 static int __pyx_pw_4liba_10polytrack7_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_4liba_10polytrack7_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   a_real_t __pyx_v_t0;
   a_real_t __pyx_v_t1;
@@ -19614,27 +17056,27 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_t0)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_t1)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 10, 1); __PYX_ERR(9, 270, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 10, 1); __PYX_ERR(9, 116, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_q0)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 10, 2); __PYX_ERR(9, 270, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 10, 2); __PYX_ERR(9, 116, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_q1)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 10, 3); __PYX_ERR(9, 270, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 10, 3); __PYX_ERR(9, 116, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v0);
           if (value) { values[4] = value; kw_args--; }
         }
@@ -19666,15 +17108,15 @@
         case  9:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_j1);
           if (value) { values[9] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(9, 270, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(9, 116, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case 10: values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
         CYTHON_FALLTHROUGH;
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
@@ -19690,52 +17132,52 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_t0 = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_t0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 270, __pyx_L3_error)
-    __pyx_v_t1 = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_t1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 270, __pyx_L3_error)
-    __pyx_v_q0 = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_q0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 270, __pyx_L3_error)
-    __pyx_v_q1 = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_q1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 270, __pyx_L3_error)
+    __pyx_v_t0 = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_t0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 116, __pyx_L3_error)
+    __pyx_v_t1 = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_t1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 116, __pyx_L3_error)
+    __pyx_v_q0 = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_q0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 116, __pyx_L3_error)
+    __pyx_v_q1 = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_q1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 116, __pyx_L3_error)
     if (values[4]) {
-      __pyx_v_v0 = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_v0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 270, __pyx_L3_error)
+      __pyx_v_v0 = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_v0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 116, __pyx_L3_error)
     } else {
       __pyx_v_v0 = ((a_real_t)0.0);
     }
     if (values[5]) {
-      __pyx_v_v1 = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_v1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 270, __pyx_L3_error)
+      __pyx_v_v1 = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_v1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 116, __pyx_L3_error)
     } else {
       __pyx_v_v1 = ((a_real_t)0.0);
     }
     if (values[6]) {
-      __pyx_v_a0 = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_a0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 270, __pyx_L3_error)
+      __pyx_v_a0 = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_a0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 116, __pyx_L3_error)
     } else {
       __pyx_v_a0 = ((a_real_t)0.0);
     }
     if (values[7]) {
-      __pyx_v_a1 = __pyx_PyFloat_AsDouble(values[7]); if (unlikely((__pyx_v_a1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 270, __pyx_L3_error)
+      __pyx_v_a1 = __pyx_PyFloat_AsDouble(values[7]); if (unlikely((__pyx_v_a1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 116, __pyx_L3_error)
     } else {
       __pyx_v_a1 = ((a_real_t)0.0);
     }
     if (values[8]) {
-      __pyx_v_j0 = __pyx_PyFloat_AsDouble(values[8]); if (unlikely((__pyx_v_j0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 270, __pyx_L3_error)
+      __pyx_v_j0 = __pyx_PyFloat_AsDouble(values[8]); if (unlikely((__pyx_v_j0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 116, __pyx_L3_error)
     } else {
       __pyx_v_j0 = ((a_real_t)0.0);
     }
     if (values[9]) {
-      __pyx_v_j1 = __pyx_PyFloat_AsDouble(values[9]); if (unlikely((__pyx_v_j1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 270, __pyx_L3_error)
+      __pyx_v_j1 = __pyx_PyFloat_AsDouble(values[9]); if (unlikely((__pyx_v_j1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 116, __pyx_L3_error)
     } else {
       __pyx_v_j1 = ((a_real_t)0.0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 10, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(9, 270, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 10, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(9, 116, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("liba.polytrack7.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_4liba_10polytrack7___cinit__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), __pyx_v_t0, __pyx_v_t1, __pyx_v_q0, __pyx_v_q1, __pyx_v_v0, __pyx_v_v1, __pyx_v_a0, __pyx_v_a1, __pyx_v_j0, __pyx_v_j1);
 
@@ -19745,103 +17187,325 @@
 }
 
 static int __pyx_pf_4liba_10polytrack7___cinit__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_t0, a_real_t __pyx_v_t1, a_real_t __pyx_v_q0, a_real_t __pyx_v_q1, a_real_t __pyx_v_v0, a_real_t __pyx_v_v1, a_real_t __pyx_v_a0, a_real_t __pyx_v_a1, a_real_t __pyx_v_j0, a_real_t __pyx_v_j1) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "python/src/a/polytrack.pxi":271
+  /* "python/src/a/polytrack.pxi":117
  *     cdef a_polytrack7_s ctx
  *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0, a_real_t j0 = 0, a_real_t j1 = 0):
- *         a_polytrack7_init(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)             # <<<<<<<<<<<<<<
- *     def __call__(self, ts):
- *         '''calculate all'''
+ *         a_polytrack7_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)             # <<<<<<<<<<<<<<
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0, a_real_t j0 = 0, a_real_t j1 = 0):
+ *         '''generation function'''
  */
-  a_polytrack7_init((&__pyx_v_self->ctx), __pyx_v_t0, __pyx_v_t1, __pyx_v_q0, __pyx_v_q1, __pyx_v_v0, __pyx_v_v1, __pyx_v_a0, __pyx_v_a1, __pyx_v_j0, __pyx_v_j1);
+  a_polytrack7_gen((&__pyx_v_self->ctx), __pyx_v_t0, __pyx_v_t1, __pyx_v_q0, __pyx_v_q1, __pyx_v_v0, __pyx_v_v1, __pyx_v_a0, __pyx_v_a1, __pyx_v_j0, __pyx_v_j1);
 
-  /* "python/src/a/polytrack.pxi":270
+  /* "python/src/a/polytrack.pxi":116
  *     '''hepta polynomial trajectory'''
  *     cdef a_polytrack7_s ctx
  *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0, a_real_t j0 = 0, a_real_t j1 = 0):             # <<<<<<<<<<<<<<
- *         a_polytrack7_init(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)
- *     def __call__(self, ts):
+ *         a_polytrack7_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0, a_real_t j0 = 0, a_real_t j1 = 0):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":272
+/* "python/src/a/polytrack.pxi":118
+ *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0, a_real_t j0 = 0, a_real_t j1 = 0):
+ *         a_polytrack7_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0, a_real_t j0 = 0, a_real_t j1 = 0):             # <<<<<<<<<<<<<<
+ *         '''generation function'''
+ *         a_polytrack7_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_4liba_10polytrack7_3gen(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_4liba_10polytrack7_2gen[] = "generation function";
+static PyObject *__pyx_pw_4liba_10polytrack7_3gen(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  a_real_t __pyx_v_t0;
+  a_real_t __pyx_v_t1;
+  a_real_t __pyx_v_q0;
+  a_real_t __pyx_v_q1;
+  a_real_t __pyx_v_v0;
+  a_real_t __pyx_v_v1;
+  a_real_t __pyx_v_a0;
+  a_real_t __pyx_v_a1;
+  a_real_t __pyx_v_j0;
+  a_real_t __pyx_v_j1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("gen (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_t0,&__pyx_n_s_t1,&__pyx_n_s_q0,&__pyx_n_s_q1,&__pyx_n_s_v0,&__pyx_n_s_v1,&__pyx_n_s_a0,&__pyx_n_s_a1,&__pyx_n_s_j0,&__pyx_n_s_j1,0};
+    PyObject* values[10] = {0,0,0,0,0,0,0,0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case 10: values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
+        CYTHON_FALLTHROUGH;
+        case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
+        case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
+        case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_t0)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_t1)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("gen", 0, 4, 10, 1); __PYX_ERR(9, 118, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_q0)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("gen", 0, 4, 10, 2); __PYX_ERR(9, 118, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_q1)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("gen", 0, 4, 10, 3); __PYX_ERR(9, 118, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  4:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v0);
+          if (value) { values[4] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_v1);
+          if (value) { values[5] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  6:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a0);
+          if (value) { values[6] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  7:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a1);
+          if (value) { values[7] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  8:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_j0);
+          if (value) { values[8] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  9:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_j1);
+          if (value) { values[9] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gen") < 0)) __PYX_ERR(9, 118, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case 10: values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
+        CYTHON_FALLTHROUGH;
+        case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
+        case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
+        case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_t0 = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_t0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 118, __pyx_L3_error)
+    __pyx_v_t1 = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_t1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 118, __pyx_L3_error)
+    __pyx_v_q0 = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_q0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 118, __pyx_L3_error)
+    __pyx_v_q1 = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_q1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 118, __pyx_L3_error)
+    if (values[4]) {
+      __pyx_v_v0 = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_v0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 118, __pyx_L3_error)
+    } else {
+      __pyx_v_v0 = ((a_real_t)0.0);
+    }
+    if (values[5]) {
+      __pyx_v_v1 = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_v1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 118, __pyx_L3_error)
+    } else {
+      __pyx_v_v1 = ((a_real_t)0.0);
+    }
+    if (values[6]) {
+      __pyx_v_a0 = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_a0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 118, __pyx_L3_error)
+    } else {
+      __pyx_v_a0 = ((a_real_t)0.0);
+    }
+    if (values[7]) {
+      __pyx_v_a1 = __pyx_PyFloat_AsDouble(values[7]); if (unlikely((__pyx_v_a1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 118, __pyx_L3_error)
+    } else {
+      __pyx_v_a1 = ((a_real_t)0.0);
+    }
+    if (values[8]) {
+      __pyx_v_j0 = __pyx_PyFloat_AsDouble(values[8]); if (unlikely((__pyx_v_j0 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 118, __pyx_L3_error)
+    } else {
+      __pyx_v_j0 = ((a_real_t)0.0);
+    }
+    if (values[9]) {
+      __pyx_v_j1 = __pyx_PyFloat_AsDouble(values[9]); if (unlikely((__pyx_v_j1 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 118, __pyx_L3_error)
+    } else {
+      __pyx_v_j1 = ((a_real_t)0.0);
+    }
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("gen", 0, 4, 10, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(9, 118, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("liba.polytrack7.gen", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_4liba_10polytrack7_2gen(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), __pyx_v_t0, __pyx_v_t1, __pyx_v_q0, __pyx_v_q1, __pyx_v_v0, __pyx_v_v1, __pyx_v_a0, __pyx_v_a1, __pyx_v_j0, __pyx_v_j1);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_4liba_10polytrack7_2gen(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_t0, a_real_t __pyx_v_t1, a_real_t __pyx_v_q0, a_real_t __pyx_v_q1, a_real_t __pyx_v_v0, a_real_t __pyx_v_v1, a_real_t __pyx_v_a0, a_real_t __pyx_v_a1, a_real_t __pyx_v_j0, a_real_t __pyx_v_j1) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("gen", 0);
+
+  /* "python/src/a/polytrack.pxi":120
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0, a_real_t j0 = 0, a_real_t j1 = 0):
+ *         '''generation function'''
+ *         a_polytrack7_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)             # <<<<<<<<<<<<<<
+ *     def __call__(self, dt):
+ *         '''calculate all'''
+ */
+  a_polytrack7_gen((&__pyx_v_self->ctx), __pyx_v_t0, __pyx_v_t1, __pyx_v_q0, __pyx_v_q1, __pyx_v_v0, __pyx_v_v1, __pyx_v_a0, __pyx_v_a1, __pyx_v_j0, __pyx_v_j1);
+
+  /* "python/src/a/polytrack.pxi":118
  *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0, a_real_t j0 = 0, a_real_t j1 = 0):
- *         a_polytrack7_init(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)
- *     def __call__(self, ts):             # <<<<<<<<<<<<<<
+ *         a_polytrack7_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)
+ *     def gen(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0, a_real_t j0 = 0, a_real_t j1 = 0):             # <<<<<<<<<<<<<<
+ *         '''generation function'''
+ *         a_polytrack7_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "python/src/a/polytrack.pxi":121
+ *         '''generation function'''
+ *         a_polytrack7_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)
+ *     def __call__(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate all'''
  *         cdef a_real_t out[4]
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_3__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_4liba_10polytrack7_2__call__[] = "calculate all";
+static PyObject *__pyx_pw_4liba_10polytrack7_5__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_4liba_10polytrack7_4__call__[] = "calculate all";
 #if CYTHON_UPDATE_DESCRIPTOR_DOC
-struct wrapperbase __pyx_wrapperbase_4liba_10polytrack7_2__call__;
+struct wrapperbase __pyx_wrapperbase_4liba_10polytrack7_4__call__;
 #endif
-static PyObject *__pyx_pw_4liba_10polytrack7_3__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyObject *__pyx_v_ts = 0;
+static PyObject *__pyx_pw_4liba_10polytrack7_5__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_dt = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__call__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_ts,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_dt,0};
     PyObject* values[1] = {0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ts)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dt)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(9, 272, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__call__") < 0)) __PYX_ERR(9, 121, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
-    __pyx_v_ts = values[0];
+    __pyx_v_dt = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(9, 272, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(9, 121, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("liba.polytrack7.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2__call__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), __pyx_v_ts);
+  __pyx_r = __pyx_pf_4liba_10polytrack7_4__call__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), __pyx_v_dt);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4liba_10polytrack7_2__call__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pf_4liba_10polytrack7_4__call__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_dt) {
   a_real_t __pyx_v_out[4];
   arrayobject *__pyx_v_p = NULL;
   arrayobject *__pyx_v_v = NULL;
   arrayobject *__pyx_v_a = NULL;
   arrayobject *__pyx_v_j = NULL;
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_v_it = NULL;
@@ -19858,216 +17522,216 @@
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
 
-  /* "python/src/a/polytrack.pxi":275
+  /* "python/src/a/polytrack.pxi":124
  *         '''calculate all'''
  *         cdef a_real_t out[4]
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             p = reals(ts)
- *             v = reals(ts)
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             p = reals(dt)
+ *             v = reals(dt)
  */
-  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_ts) != 0);
+  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_dt) != 0);
   if (__pyx_t_1) {
 
-    /* "python/src/a/polytrack.pxi":276
+    /* "python/src/a/polytrack.pxi":125
  *         cdef a_real_t out[4]
- *         if iterable(ts):
- *             p = reals(ts)             # <<<<<<<<<<<<<<
- *             v = reals(ts)
- *             a = reals(ts)
+ *         if iterable(dt):
+ *             p = reals(dt)             # <<<<<<<<<<<<<<
+ *             v = reals(dt)
+ *             a = reals(dt)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 276, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 125, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_p = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":277
- *         if iterable(ts):
- *             p = reals(ts)
- *             v = reals(ts)             # <<<<<<<<<<<<<<
- *             a = reals(ts)
- *             j = reals(ts)
+    /* "python/src/a/polytrack.pxi":126
+ *         if iterable(dt):
+ *             p = reals(dt)
+ *             v = reals(dt)             # <<<<<<<<<<<<<<
+ *             a = reals(dt)
+ *             j = reals(dt)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 277, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_v = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":278
- *             p = reals(ts)
- *             v = reals(ts)
- *             a = reals(ts)             # <<<<<<<<<<<<<<
- *             j = reals(ts)
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":127
+ *             p = reals(dt)
+ *             v = reals(dt)
+ *             a = reals(dt)             # <<<<<<<<<<<<<<
+ *             j = reals(dt)
+ *             for i, it in enumerate(dt):
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 278, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 127, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_a = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":279
- *             v = reals(ts)
- *             a = reals(ts)
- *             j = reals(ts)             # <<<<<<<<<<<<<<
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":128
+ *             v = reals(dt)
+ *             a = reals(dt)
+ *             j = reals(dt)             # <<<<<<<<<<<<<<
+ *             for i, it in enumerate(dt):
  *                 a_polytrack7_out(&self.ctx, it, out)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 279, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 128, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_j = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":280
- *             a = reals(ts)
- *             j = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+    /* "python/src/a/polytrack.pxi":129
+ *             a = reals(dt)
+ *             j = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 a_polytrack7_out(&self.ctx, it, out)
  *                 p[i] = out[0]
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
-    if (likely(PyList_CheckExact(__pyx_v_ts)) || PyTuple_CheckExact(__pyx_v_ts)) {
-      __pyx_t_4 = __pyx_v_ts; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+    if (likely(PyList_CheckExact(__pyx_v_dt)) || PyTuple_CheckExact(__pyx_v_dt)) {
+      __pyx_t_4 = __pyx_v_dt; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ts); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 280, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_dt); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 129, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 280, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 129, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 280, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 129, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 280, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 129, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 280, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 129, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 280, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 129, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(9, 280, __pyx_L1_error)
+            else __PYX_ERR(9, 129, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 280, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 129, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":281
- *             j = reals(ts)
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":130
+ *             j = reals(dt)
+ *             for i, it in enumerate(dt):
  *                 a_polytrack7_out(&self.ctx, it, out)             # <<<<<<<<<<<<<<
  *                 p[i] = out[0]
  *                 v[i] = out[1]
  */
-      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 281, __pyx_L1_error)
+      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 130, __pyx_L1_error)
       a_polytrack7_out((&__pyx_v_self->ctx), __pyx_t_8, __pyx_v_out);
 
-      /* "python/src/a/polytrack.pxi":282
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":131
+ *             for i, it in enumerate(dt):
  *                 a_polytrack7_out(&self.ctx, it, out)
  *                 p[i] = out[0]             # <<<<<<<<<<<<<<
  *                 v[i] = out[1]
  *                 a[i] = out[2]
  */
-      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[0])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 282, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[0])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 131, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_p), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 282, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_p), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 131, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":283
+      /* "python/src/a/polytrack.pxi":132
  *                 a_polytrack7_out(&self.ctx, it, out)
  *                 p[i] = out[0]
  *                 v[i] = out[1]             # <<<<<<<<<<<<<<
  *                 a[i] = out[2]
  *                 j[i] = out[3]
  */
-      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[1])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 283, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[1])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 132, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_v), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 283, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_v), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 132, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":284
+      /* "python/src/a/polytrack.pxi":133
  *                 p[i] = out[0]
  *                 v[i] = out[1]
  *                 a[i] = out[2]             # <<<<<<<<<<<<<<
  *                 j[i] = out[3]
  *             return p, v, a, j
  */
-      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[2])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 284, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[2])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 133, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_a), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 284, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_a), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 133, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":285
+      /* "python/src/a/polytrack.pxi":134
  *                 v[i] = out[1]
  *                 a[i] = out[2]
  *                 j[i] = out[3]             # <<<<<<<<<<<<<<
  *             return p, v, a, j
- *         a_polytrack7_out(&self.ctx, ts, out)
+ *         a_polytrack7_out(&self.ctx, dt, out)
  */
-      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[3])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 285, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[3])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 134, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_j), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 285, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_j), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 134, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":280
- *             a = reals(ts)
- *             j = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+      /* "python/src/a/polytrack.pxi":129
+ *             a = reals(dt)
+ *             j = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 a_polytrack7_out(&self.ctx, it, out)
  *                 p[i] = out[0]
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":286
+    /* "python/src/a/polytrack.pxi":135
  *                 a[i] = out[2]
  *                 j[i] = out[3]
  *             return p, v, a, j             # <<<<<<<<<<<<<<
- *         a_polytrack7_out(&self.ctx, ts, out)
+ *         a_polytrack7_out(&self.ctx, dt, out)
  *         return out[0], out[1], out[2], out[3]
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 286, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 135, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(((PyObject *)__pyx_v_p));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_p));
     PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_v_p));
     __Pyx_INCREF(((PyObject *)__pyx_v_v));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_v));
     PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)__pyx_v_v));
@@ -20077,50 +17741,50 @@
     __Pyx_INCREF(((PyObject *)__pyx_v_j));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_j));
     PyTuple_SET_ITEM(__pyx_t_2, 3, ((PyObject *)__pyx_v_j));
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "python/src/a/polytrack.pxi":275
+    /* "python/src/a/polytrack.pxi":124
  *         '''calculate all'''
  *         cdef a_real_t out[4]
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             p = reals(ts)
- *             v = reals(ts)
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             p = reals(dt)
+ *             v = reals(dt)
  */
   }
 
-  /* "python/src/a/polytrack.pxi":287
+  /* "python/src/a/polytrack.pxi":136
  *                 j[i] = out[3]
  *             return p, v, a, j
- *         a_polytrack7_out(&self.ctx, ts, out)             # <<<<<<<<<<<<<<
+ *         a_polytrack7_out(&self.ctx, dt, out)             # <<<<<<<<<<<<<<
  *         return out[0], out[1], out[2], out[3]
- *     def pos(self, ts):
+ *     def pos(self, dt):
  */
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_ts); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 287, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 136, __pyx_L1_error)
   a_polytrack7_out((&__pyx_v_self->ctx), __pyx_t_8, __pyx_v_out);
 
-  /* "python/src/a/polytrack.pxi":288
+  /* "python/src/a/polytrack.pxi":137
  *             return p, v, a, j
- *         a_polytrack7_out(&self.ctx, ts, out)
+ *         a_polytrack7_out(&self.ctx, dt, out)
  *         return out[0], out[1], out[2], out[3]             # <<<<<<<<<<<<<<
- *     def pos(self, ts):
+ *     def pos(self, dt):
  *         '''calculate position'''
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_out[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 288, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble((__pyx_v_out[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_out[1])); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 288, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_out[1])); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[2])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 288, __pyx_L1_error)
+  __pyx_t_7 = PyFloat_FromDouble((__pyx_v_out[2])); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_9 = PyFloat_FromDouble((__pyx_v_out[3])); if (unlikely(!__pyx_t_9)) __PYX_ERR(9, 288, __pyx_L1_error)
+  __pyx_t_9 = PyFloat_FromDouble((__pyx_v_out[3])); if (unlikely(!__pyx_t_9)) __PYX_ERR(9, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_10 = PyTuple_New(4); if (unlikely(!__pyx_t_10)) __PYX_ERR(9, 288, __pyx_L1_error)
+  __pyx_t_10 = PyTuple_New(4); if (unlikely(!__pyx_t_10)) __PYX_ERR(9, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_10, 2, __pyx_t_7);
@@ -20130,18 +17794,18 @@
   __pyx_t_4 = 0;
   __pyx_t_7 = 0;
   __pyx_t_9 = 0;
   __pyx_r = __pyx_t_10;
   __pyx_t_10 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":272
- *     def __cinit__(self, a_real_t t0, a_real_t t1, a_real_t q0, a_real_t q1, a_real_t v0 = 0, a_real_t v1 = 0, a_real_t a0 = 0, a_real_t a1 = 0, a_real_t j0 = 0, a_real_t j1 = 0):
- *         a_polytrack7_init(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)
- *     def __call__(self, ts):             # <<<<<<<<<<<<<<
+  /* "python/src/a/polytrack.pxi":121
+ *         '''generation function'''
+ *         a_polytrack7_gen(&self.ctx, t0, t1, q0, q1, v0, v1, a0, a1, j0, j1)
+ *     def __call__(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate all'''
  *         cdef a_real_t out[4]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -20159,37 +17823,37 @@
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_it);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":289
- *         a_polytrack7_out(&self.ctx, ts, out)
+/* "python/src/a/polytrack.pxi":138
+ *         a_polytrack7_out(&self.ctx, dt, out)
  *         return out[0], out[1], out[2], out[3]
- *     def pos(self, ts):             # <<<<<<<<<<<<<<
+ *     def pos(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate position'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_5pos(PyObject *__pyx_v_self, PyObject *__pyx_v_ts); /*proto*/
-static char __pyx_doc_4liba_10polytrack7_4pos[] = "calculate position";
-static PyObject *__pyx_pw_4liba_10polytrack7_5pos(PyObject *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pw_4liba_10polytrack7_7pos(PyObject *__pyx_v_self, PyObject *__pyx_v_dt); /*proto*/
+static char __pyx_doc_4liba_10polytrack7_6pos[] = "calculate position";
+static PyObject *__pyx_pw_4liba_10polytrack7_7pos(PyObject *__pyx_v_self, PyObject *__pyx_v_dt) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("pos (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_4pos(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((PyObject *)__pyx_v_ts));
+  __pyx_r = __pyx_pf_4liba_10polytrack7_6pos(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((PyObject *)__pyx_v_dt));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4liba_10polytrack7_4pos(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pf_4liba_10polytrack7_6pos(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_dt) {
   arrayobject *__pyx_v_out = NULL;
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_v_it = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -20200,162 +17864,162 @@
   PyObject *__pyx_t_7 = NULL;
   a_real_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pos", 0);
 
-  /* "python/src/a/polytrack.pxi":291
- *     def pos(self, ts):
+  /* "python/src/a/polytrack.pxi":140
+ *     def pos(self, dt):
  *         '''calculate position'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
-  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_ts) != 0);
+  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_dt) != 0);
   if (__pyx_t_1) {
 
-    /* "python/src/a/polytrack.pxi":292
+    /* "python/src/a/polytrack.pxi":141
  *         '''calculate position'''
- *         if iterable(ts):
- *             out = reals(ts)             # <<<<<<<<<<<<<<
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):
+ *             out = reals(dt)             # <<<<<<<<<<<<<<
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack7_pos(&self.ctx, it)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 292, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 141, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_out = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":293
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+    /* "python/src/a/polytrack.pxi":142
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack7_pos(&self.ctx, it)
  *             return out
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
-    if (likely(PyList_CheckExact(__pyx_v_ts)) || PyTuple_CheckExact(__pyx_v_ts)) {
-      __pyx_t_4 = __pyx_v_ts; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+    if (likely(PyList_CheckExact(__pyx_v_dt)) || PyTuple_CheckExact(__pyx_v_dt)) {
+      __pyx_t_4 = __pyx_v_dt; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ts); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 293, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_dt); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 142, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 293, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 142, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 293, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 142, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 293, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 142, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 293, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 142, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 293, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 142, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(9, 293, __pyx_L1_error)
+            else __PYX_ERR(9, 142, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 293, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 142, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":294
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":143
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack7_pos(&self.ctx, it)             # <<<<<<<<<<<<<<
  *             return out
- *         return a_polytrack7_pos(&self.ctx, ts)
+ *         return a_polytrack7_pos(&self.ctx, dt)
  */
-      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 294, __pyx_L1_error)
-      __pyx_t_7 = PyFloat_FromDouble(a_polytrack7_pos((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 294, __pyx_L1_error)
+      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 143, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble(a_polytrack7_pos((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 143, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 294, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 143, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":293
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+      /* "python/src/a/polytrack.pxi":142
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack7_pos(&self.ctx, it)
  *             return out
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":295
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":144
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack7_pos(&self.ctx, it)
  *             return out             # <<<<<<<<<<<<<<
- *         return a_polytrack7_pos(&self.ctx, ts)
- *     def vec(self, ts):
+ *         return a_polytrack7_pos(&self.ctx, dt)
+ *     def vec(self, dt):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_out));
     __pyx_r = ((PyObject *)__pyx_v_out);
     goto __pyx_L0;
 
-    /* "python/src/a/polytrack.pxi":291
- *     def pos(self, ts):
+    /* "python/src/a/polytrack.pxi":140
+ *     def pos(self, dt):
  *         '''calculate position'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
   }
 
-  /* "python/src/a/polytrack.pxi":296
+  /* "python/src/a/polytrack.pxi":145
  *                 out[i] = a_polytrack7_pos(&self.ctx, it)
  *             return out
- *         return a_polytrack7_pos(&self.ctx, ts)             # <<<<<<<<<<<<<<
- *     def vec(self, ts):
+ *         return a_polytrack7_pos(&self.ctx, dt)             # <<<<<<<<<<<<<<
+ *     def vec(self, dt):
  *         '''calculate velocity'''
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_ts); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 296, __pyx_L1_error)
-  __pyx_t_2 = PyFloat_FromDouble(a_polytrack7_pos((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 296, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 145, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(a_polytrack7_pos((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":289
- *         a_polytrack7_out(&self.ctx, ts, out)
+  /* "python/src/a/polytrack.pxi":138
+ *         a_polytrack7_out(&self.ctx, dt, out)
  *         return out[0], out[1], out[2], out[3]
- *     def pos(self, ts):             # <<<<<<<<<<<<<<
+ *     def pos(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate position'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
@@ -20366,37 +18030,37 @@
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_it);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":297
+/* "python/src/a/polytrack.pxi":146
  *             return out
- *         return a_polytrack7_pos(&self.ctx, ts)
- *     def vec(self, ts):             # <<<<<<<<<<<<<<
+ *         return a_polytrack7_pos(&self.ctx, dt)
+ *     def vec(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate velocity'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_7vec(PyObject *__pyx_v_self, PyObject *__pyx_v_ts); /*proto*/
-static char __pyx_doc_4liba_10polytrack7_6vec[] = "calculate velocity";
-static PyObject *__pyx_pw_4liba_10polytrack7_7vec(PyObject *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pw_4liba_10polytrack7_9vec(PyObject *__pyx_v_self, PyObject *__pyx_v_dt); /*proto*/
+static char __pyx_doc_4liba_10polytrack7_8vec[] = "calculate velocity";
+static PyObject *__pyx_pw_4liba_10polytrack7_9vec(PyObject *__pyx_v_self, PyObject *__pyx_v_dt) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("vec (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_6vec(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((PyObject *)__pyx_v_ts));
+  __pyx_r = __pyx_pf_4liba_10polytrack7_8vec(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((PyObject *)__pyx_v_dt));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4liba_10polytrack7_6vec(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pf_4liba_10polytrack7_8vec(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_dt) {
   arrayobject *__pyx_v_out = NULL;
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_v_it = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -20407,162 +18071,162 @@
   PyObject *__pyx_t_7 = NULL;
   a_real_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("vec", 0);
 
-  /* "python/src/a/polytrack.pxi":299
- *     def vec(self, ts):
+  /* "python/src/a/polytrack.pxi":148
+ *     def vec(self, dt):
  *         '''calculate velocity'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
-  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_ts) != 0);
+  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_dt) != 0);
   if (__pyx_t_1) {
 
-    /* "python/src/a/polytrack.pxi":300
+    /* "python/src/a/polytrack.pxi":149
  *         '''calculate velocity'''
- *         if iterable(ts):
- *             out = reals(ts)             # <<<<<<<<<<<<<<
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):
+ *             out = reals(dt)             # <<<<<<<<<<<<<<
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack7_vec(&self.ctx, it)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 300, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_out = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":301
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+    /* "python/src/a/polytrack.pxi":150
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack7_vec(&self.ctx, it)
  *             return out
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
-    if (likely(PyList_CheckExact(__pyx_v_ts)) || PyTuple_CheckExact(__pyx_v_ts)) {
-      __pyx_t_4 = __pyx_v_ts; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+    if (likely(PyList_CheckExact(__pyx_v_dt)) || PyTuple_CheckExact(__pyx_v_dt)) {
+      __pyx_t_4 = __pyx_v_dt; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ts); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 301, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_dt); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 150, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 301, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 150, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 301, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 150, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 301, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 150, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 301, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 150, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 301, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 150, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(9, 301, __pyx_L1_error)
+            else __PYX_ERR(9, 150, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 301, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 150, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":302
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":151
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack7_vec(&self.ctx, it)             # <<<<<<<<<<<<<<
  *             return out
- *         return a_polytrack7_vec(&self.ctx, ts)
+ *         return a_polytrack7_vec(&self.ctx, dt)
  */
-      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 302, __pyx_L1_error)
-      __pyx_t_7 = PyFloat_FromDouble(a_polytrack7_vec((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 302, __pyx_L1_error)
+      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 151, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble(a_polytrack7_vec((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 151, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 302, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 151, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":301
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+      /* "python/src/a/polytrack.pxi":150
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack7_vec(&self.ctx, it)
  *             return out
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":303
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":152
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack7_vec(&self.ctx, it)
  *             return out             # <<<<<<<<<<<<<<
- *         return a_polytrack7_vec(&self.ctx, ts)
- *     def acc(self, ts):
+ *         return a_polytrack7_vec(&self.ctx, dt)
+ *     def acc(self, dt):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_out));
     __pyx_r = ((PyObject *)__pyx_v_out);
     goto __pyx_L0;
 
-    /* "python/src/a/polytrack.pxi":299
- *     def vec(self, ts):
+    /* "python/src/a/polytrack.pxi":148
+ *     def vec(self, dt):
  *         '''calculate velocity'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
   }
 
-  /* "python/src/a/polytrack.pxi":304
+  /* "python/src/a/polytrack.pxi":153
  *                 out[i] = a_polytrack7_vec(&self.ctx, it)
  *             return out
- *         return a_polytrack7_vec(&self.ctx, ts)             # <<<<<<<<<<<<<<
- *     def acc(self, ts):
+ *         return a_polytrack7_vec(&self.ctx, dt)             # <<<<<<<<<<<<<<
+ *     def acc(self, dt):
  *         '''calculate acceleration'''
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_ts); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 304, __pyx_L1_error)
-  __pyx_t_2 = PyFloat_FromDouble(a_polytrack7_vec((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 304, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 153, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(a_polytrack7_vec((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":297
+  /* "python/src/a/polytrack.pxi":146
  *             return out
- *         return a_polytrack7_pos(&self.ctx, ts)
- *     def vec(self, ts):             # <<<<<<<<<<<<<<
+ *         return a_polytrack7_pos(&self.ctx, dt)
+ *     def vec(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate velocity'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
@@ -20573,37 +18237,37 @@
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_it);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":305
+/* "python/src/a/polytrack.pxi":154
  *             return out
- *         return a_polytrack7_vec(&self.ctx, ts)
- *     def acc(self, ts):             # <<<<<<<<<<<<<<
+ *         return a_polytrack7_vec(&self.ctx, dt)
+ *     def acc(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate acceleration'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_9acc(PyObject *__pyx_v_self, PyObject *__pyx_v_ts); /*proto*/
-static char __pyx_doc_4liba_10polytrack7_8acc[] = "calculate acceleration";
-static PyObject *__pyx_pw_4liba_10polytrack7_9acc(PyObject *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pw_4liba_10polytrack7_11acc(PyObject *__pyx_v_self, PyObject *__pyx_v_dt); /*proto*/
+static char __pyx_doc_4liba_10polytrack7_10acc[] = "calculate acceleration";
+static PyObject *__pyx_pw_4liba_10polytrack7_11acc(PyObject *__pyx_v_self, PyObject *__pyx_v_dt) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("acc (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_8acc(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((PyObject *)__pyx_v_ts));
+  __pyx_r = __pyx_pf_4liba_10polytrack7_10acc(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((PyObject *)__pyx_v_dt));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4liba_10polytrack7_8acc(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pf_4liba_10polytrack7_10acc(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_dt) {
   arrayobject *__pyx_v_out = NULL;
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_v_it = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -20614,162 +18278,162 @@
   PyObject *__pyx_t_7 = NULL;
   a_real_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("acc", 0);
 
-  /* "python/src/a/polytrack.pxi":307
- *     def acc(self, ts):
+  /* "python/src/a/polytrack.pxi":156
+ *     def acc(self, dt):
  *         '''calculate acceleration'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
-  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_ts) != 0);
+  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_dt) != 0);
   if (__pyx_t_1) {
 
-    /* "python/src/a/polytrack.pxi":308
+    /* "python/src/a/polytrack.pxi":157
  *         '''calculate acceleration'''
- *         if iterable(ts):
- *             out = reals(ts)             # <<<<<<<<<<<<<<
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):
+ *             out = reals(dt)             # <<<<<<<<<<<<<<
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack7_acc(&self.ctx, it)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 308, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 157, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_out = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":309
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+    /* "python/src/a/polytrack.pxi":158
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack7_acc(&self.ctx, it)
  *             return out
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
-    if (likely(PyList_CheckExact(__pyx_v_ts)) || PyTuple_CheckExact(__pyx_v_ts)) {
-      __pyx_t_4 = __pyx_v_ts; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+    if (likely(PyList_CheckExact(__pyx_v_dt)) || PyTuple_CheckExact(__pyx_v_dt)) {
+      __pyx_t_4 = __pyx_v_dt; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ts); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 309, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_dt); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 158, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 309, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 158, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 309, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 158, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 309, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 158, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 309, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 158, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 309, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 158, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(9, 309, __pyx_L1_error)
+            else __PYX_ERR(9, 158, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 309, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 158, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":310
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":159
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack7_acc(&self.ctx, it)             # <<<<<<<<<<<<<<
  *             return out
- *         return a_polytrack7_acc(&self.ctx, ts)
+ *         return a_polytrack7_acc(&self.ctx, dt)
  */
-      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 310, __pyx_L1_error)
-      __pyx_t_7 = PyFloat_FromDouble(a_polytrack7_acc((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 310, __pyx_L1_error)
+      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 159, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble(a_polytrack7_acc((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 159, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 310, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 159, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":309
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+      /* "python/src/a/polytrack.pxi":158
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack7_acc(&self.ctx, it)
  *             return out
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":311
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":160
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack7_acc(&self.ctx, it)
  *             return out             # <<<<<<<<<<<<<<
- *         return a_polytrack7_acc(&self.ctx, ts)
- *     def jer(self, ts):
+ *         return a_polytrack7_acc(&self.ctx, dt)
+ *     def jer(self, dt):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_out));
     __pyx_r = ((PyObject *)__pyx_v_out);
     goto __pyx_L0;
 
-    /* "python/src/a/polytrack.pxi":307
- *     def acc(self, ts):
+    /* "python/src/a/polytrack.pxi":156
+ *     def acc(self, dt):
  *         '''calculate acceleration'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
   }
 
-  /* "python/src/a/polytrack.pxi":312
+  /* "python/src/a/polytrack.pxi":161
  *                 out[i] = a_polytrack7_acc(&self.ctx, it)
  *             return out
- *         return a_polytrack7_acc(&self.ctx, ts)             # <<<<<<<<<<<<<<
- *     def jer(self, ts):
+ *         return a_polytrack7_acc(&self.ctx, dt)             # <<<<<<<<<<<<<<
+ *     def jer(self, dt):
  *         '''calculate jerk'''
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_ts); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 312, __pyx_L1_error)
-  __pyx_t_2 = PyFloat_FromDouble(a_polytrack7_acc((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 312, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 161, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(a_polytrack7_acc((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":305
+  /* "python/src/a/polytrack.pxi":154
  *             return out
- *         return a_polytrack7_vec(&self.ctx, ts)
- *     def acc(self, ts):             # <<<<<<<<<<<<<<
+ *         return a_polytrack7_vec(&self.ctx, dt)
+ *     def acc(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate acceleration'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
@@ -20780,37 +18444,37 @@
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_it);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":313
+/* "python/src/a/polytrack.pxi":162
  *             return out
- *         return a_polytrack7_acc(&self.ctx, ts)
- *     def jer(self, ts):             # <<<<<<<<<<<<<<
+ *         return a_polytrack7_acc(&self.ctx, dt)
+ *     def jer(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate jerk'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_11jer(PyObject *__pyx_v_self, PyObject *__pyx_v_ts); /*proto*/
-static char __pyx_doc_4liba_10polytrack7_10jer[] = "calculate jerk";
-static PyObject *__pyx_pw_4liba_10polytrack7_11jer(PyObject *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pw_4liba_10polytrack7_13jer(PyObject *__pyx_v_self, PyObject *__pyx_v_dt); /*proto*/
+static char __pyx_doc_4liba_10polytrack7_12jer[] = "calculate jerk";
+static PyObject *__pyx_pw_4liba_10polytrack7_13jer(PyObject *__pyx_v_self, PyObject *__pyx_v_dt) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("jer (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_10jer(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((PyObject *)__pyx_v_ts));
+  __pyx_r = __pyx_pf_4liba_10polytrack7_12jer(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((PyObject *)__pyx_v_dt));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4liba_10polytrack7_10jer(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_ts) {
+static PyObject *__pyx_pf_4liba_10polytrack7_12jer(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_dt) {
   arrayobject *__pyx_v_out = NULL;
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_v_it = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -20821,162 +18485,162 @@
   PyObject *__pyx_t_7 = NULL;
   a_real_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("jer", 0);
 
-  /* "python/src/a/polytrack.pxi":315
- *     def jer(self, ts):
+  /* "python/src/a/polytrack.pxi":164
+ *     def jer(self, dt):
  *         '''calculate jerk'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
-  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_ts) != 0);
+  __pyx_t_1 = (__pyx_f_4liba_iterable(__pyx_v_dt) != 0);
   if (__pyx_t_1) {
 
-    /* "python/src/a/polytrack.pxi":316
+    /* "python/src/a/polytrack.pxi":165
  *         '''calculate jerk'''
- *         if iterable(ts):
- *             out = reals(ts)             # <<<<<<<<<<<<<<
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):
+ *             out = reals(dt)             # <<<<<<<<<<<<<<
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack7_jer(&self.ctx, it)
  */
     __pyx_t_3.__pyx_n = 1;
-    __pyx_t_3.o = __pyx_v_ts;
-    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 316, __pyx_L1_error)
+    __pyx_t_3.o = __pyx_v_dt;
+    __pyx_t_2 = ((PyObject *)__pyx_f_4liba_reals(&__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_out = ((arrayobject *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":317
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+    /* "python/src/a/polytrack.pxi":166
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack7_jer(&self.ctx, it)
  *             return out
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
-    if (likely(PyList_CheckExact(__pyx_v_ts)) || PyTuple_CheckExact(__pyx_v_ts)) {
-      __pyx_t_4 = __pyx_v_ts; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
+    if (likely(PyList_CheckExact(__pyx_v_dt)) || PyTuple_CheckExact(__pyx_v_dt)) {
+      __pyx_t_4 = __pyx_v_dt; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_ts); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 317, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_dt); if (unlikely(!__pyx_t_4)) __PYX_ERR(9, 166, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 317, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(9, 166, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 317, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 166, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 317, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 166, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 317, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(9, 166, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 317, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 166, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(9, 317, __pyx_L1_error)
+            else __PYX_ERR(9, 166, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_2);
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 317, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 166, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":318
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+      /* "python/src/a/polytrack.pxi":167
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack7_jer(&self.ctx, it)             # <<<<<<<<<<<<<<
  *             return out
- *         return a_polytrack7_jer(&self.ctx, ts)
+ *         return a_polytrack7_jer(&self.ctx, dt)
  */
-      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 318, __pyx_L1_error)
-      __pyx_t_7 = PyFloat_FromDouble(a_polytrack7_jer((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 318, __pyx_L1_error)
+      __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_it); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 167, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble(a_polytrack7_jer((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_7)) __PYX_ERR(9, 167, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 318, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_out), __pyx_v_i, __pyx_t_7) < 0)) __PYX_ERR(9, 167, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "python/src/a/polytrack.pxi":317
- *         if iterable(ts):
- *             out = reals(ts)
- *             for i, it in enumerate(ts):             # <<<<<<<<<<<<<<
+      /* "python/src/a/polytrack.pxi":166
+ *         if iterable(dt):
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):             # <<<<<<<<<<<<<<
  *                 out[i] = a_polytrack7_jer(&self.ctx, it)
  *             return out
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "python/src/a/polytrack.pxi":319
- *             for i, it in enumerate(ts):
+    /* "python/src/a/polytrack.pxi":168
+ *             for i, it in enumerate(dt):
  *                 out[i] = a_polytrack7_jer(&self.ctx, it)
  *             return out             # <<<<<<<<<<<<<<
- *         return a_polytrack7_jer(&self.ctx, ts)
- *     def gen(self):
+ *         return a_polytrack7_jer(&self.ctx, dt)
+ * 
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_out));
     __pyx_r = ((PyObject *)__pyx_v_out);
     goto __pyx_L0;
 
-    /* "python/src/a/polytrack.pxi":315
- *     def jer(self, ts):
+    /* "python/src/a/polytrack.pxi":164
+ *     def jer(self, dt):
  *         '''calculate jerk'''
- *         if iterable(ts):             # <<<<<<<<<<<<<<
- *             out = reals(ts)
- *             for i, it in enumerate(ts):
+ *         if iterable(dt):             # <<<<<<<<<<<<<<
+ *             out = reals(dt)
+ *             for i, it in enumerate(dt):
  */
   }
 
-  /* "python/src/a/polytrack.pxi":320
+  /* "python/src/a/polytrack.pxi":169
  *                 out[i] = a_polytrack7_jer(&self.ctx, it)
  *             return out
- *         return a_polytrack7_jer(&self.ctx, ts)             # <<<<<<<<<<<<<<
- *     def gen(self):
- *         '''generation function'''
+ *         return a_polytrack7_jer(&self.ctx, dt)             # <<<<<<<<<<<<<<
+ * 
+ *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_ts); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 320, __pyx_L1_error)
-  __pyx_t_2 = PyFloat_FromDouble(a_polytrack7_jer((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 320, __pyx_L1_error)
+  __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_dt); if (unlikely((__pyx_t_8 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 169, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(a_polytrack7_jer((&__pyx_v_self->ctx), __pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(9, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":313
+  /* "python/src/a/polytrack.pxi":162
  *             return out
- *         return a_polytrack7_acc(&self.ctx, ts)
- *     def jer(self, ts):             # <<<<<<<<<<<<<<
+ *         return a_polytrack7_acc(&self.ctx, dt)
+ *     def jer(self, dt):             # <<<<<<<<<<<<<<
  *         '''calculate jerk'''
- *         if iterable(ts):
+ *         if iterable(dt):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
@@ -20987,71 +18651,19 @@
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_it);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":321
- *             return out
- *         return a_polytrack7_jer(&self.ctx, ts)
- *     def gen(self):             # <<<<<<<<<<<<<<
- *         '''generation function'''
- *         a_polytrack7_gen(&self.ctx)
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_13gen(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_4liba_10polytrack7_12gen[] = "generation function";
-static PyObject *__pyx_pw_4liba_10polytrack7_13gen(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("gen (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_12gen(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_12gen(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("gen", 0);
-
-  /* "python/src/a/polytrack.pxi":323
- *     def gen(self):
- *         '''generation function'''
- *         a_polytrack7_gen(&self.ctx)             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  a_polytrack7_gen((&__pyx_v_self->ctx));
-
-  /* "python/src/a/polytrack.pxi":321
- *             return out
- *         return a_polytrack7_jer(&self.ctx, ts)
- *     def gen(self):             # <<<<<<<<<<<<<<
- *         '''generation function'''
- *         a_polytrack7_gen(&self.ctx)
- */
-
-  /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":326
+/* "python/src/a/polytrack.pxi":172
  * 
  *     @property
  *     def k(self):             # <<<<<<<<<<<<<<
  *         return self.ctx.k
- * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4liba_10polytrack7_1k_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_4liba_10polytrack7_1k_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -21068,1993 +18680,44 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "python/src/a/polytrack.pxi":327
+  /* "python/src/a/polytrack.pxi":173
  *     @property
  *     def k(self):
  *         return self.ctx.k             # <<<<<<<<<<<<<<
- * 
- *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.k, 8); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 327, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.k, 8); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "python/src/a/polytrack.pxi":326
+  /* "python/src/a/polytrack.pxi":172
  * 
  *     @property
  *     def k(self):             # <<<<<<<<<<<<<<
  *         return self.ctx.k
- * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("liba.polytrack7.k.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "python/src/a/polytrack.pxi":330
- * 
- *     @property
- *     def t(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.t
- *     @t.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_1t_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_1t_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_1t___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_1t___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":331
- *     @property
- *     def t(self):
- *         return self.ctx.t             # <<<<<<<<<<<<<<
- *     @t.setter
- *     def t(self, val):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.t, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 331, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":330
- * 
- *     @property
- *     def t(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.t
- *     @t.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.t.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":333
- *         return self.ctx.t
- *     @t.setter
- *     def t(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.t[0] = val[0]
- *         self.ctx.t[1] = val[1]
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_1t_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_1t_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_1t_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((PyObject *)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_1t_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  a_real_t __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":334
- *     @t.setter
- *     def t(self, val):
- *         self.ctx.t[0] = val[0]             # <<<<<<<<<<<<<<
- *         self.ctx.t[1] = val[1]
- * 
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 334, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 334, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.t[0]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":335
- *     def t(self, val):
- *         self.ctx.t[0] = val[0]
- *         self.ctx.t[1] = val[1]             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 335, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 335, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.t[1]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":333
- *         return self.ctx.t
- *     @t.setter
- *     def t(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.t[0] = val[0]
- *         self.ctx.t[1] = val[1]
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.t.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":338
- * 
- *     @property
- *     def q(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.q
- *     @q.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_1q_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_1q_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_1q___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_1q___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":339
- *     @property
- *     def q(self):
- *         return self.ctx.q             # <<<<<<<<<<<<<<
- *     @q.setter
- *     def q(self, val):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.q, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 339, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":338
- * 
- *     @property
- *     def q(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.q
- *     @q.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.q.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":341
- *         return self.ctx.q
- *     @q.setter
- *     def q(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.q[0] = val[0]
- *         self.ctx.q[1] = val[1]
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_1q_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_1q_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_1q_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((PyObject *)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_1q_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  a_real_t __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":342
- *     @q.setter
- *     def q(self, val):
- *         self.ctx.q[0] = val[0]             # <<<<<<<<<<<<<<
- *         self.ctx.q[1] = val[1]
- * 
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 342, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 342, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.q[0]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":343
- *     def q(self, val):
- *         self.ctx.q[0] = val[0]
- *         self.ctx.q[1] = val[1]             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 343, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 343, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.q[1]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":341
- *         return self.ctx.q
- *     @q.setter
- *     def q(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.q[0] = val[0]
- *         self.ctx.q[1] = val[1]
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.q.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":346
- * 
- *     @property
- *     def v(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.v
- *     @v.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_1v_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_1v_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_1v___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_1v___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":347
- *     @property
- *     def v(self):
- *         return self.ctx.v             # <<<<<<<<<<<<<<
- *     @v.setter
- *     def v(self, val):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.v, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 347, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":346
- * 
- *     @property
- *     def v(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.v
- *     @v.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.v.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":349
- *         return self.ctx.v
- *     @v.setter
- *     def v(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.v[0] = val[0]
- *         self.ctx.v[1] = val[1]
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_1v_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_1v_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_1v_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((PyObject *)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_1v_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  a_real_t __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":350
- *     @v.setter
- *     def v(self, val):
- *         self.ctx.v[0] = val[0]             # <<<<<<<<<<<<<<
- *         self.ctx.v[1] = val[1]
- * 
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 350, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 350, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.v[0]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":351
- *     def v(self, val):
- *         self.ctx.v[0] = val[0]
- *         self.ctx.v[1] = val[1]             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 351, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 351, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.v[1]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":349
- *         return self.ctx.v
- *     @v.setter
- *     def v(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.v[0] = val[0]
- *         self.ctx.v[1] = val[1]
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.v.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":354
- * 
- *     @property
- *     def a(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.a
- *     @a.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_1a_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_1a_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_1a___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_1a___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":355
- *     @property
- *     def a(self):
- *         return self.ctx.a             # <<<<<<<<<<<<<<
- *     @a.setter
- *     def a(self, val):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.a, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 355, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":354
- * 
- *     @property
- *     def a(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.a
- *     @a.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.a.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":357
- *         return self.ctx.a
- *     @a.setter
- *     def a(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.a[0] = val[0]
- *         self.ctx.a[1] = val[1]
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_1a_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_1a_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_1a_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((PyObject *)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_1a_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  a_real_t __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":358
- *     @a.setter
- *     def a(self, val):
- *         self.ctx.a[0] = val[0]             # <<<<<<<<<<<<<<
- *         self.ctx.a[1] = val[1]
- * 
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 358, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 358, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.a[0]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":359
- *     def a(self, val):
- *         self.ctx.a[0] = val[0]
- *         self.ctx.a[1] = val[1]             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 359, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 359, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.a[1]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":357
- *         return self.ctx.a
- *     @a.setter
- *     def a(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.a[0] = val[0]
- *         self.ctx.a[1] = val[1]
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.a.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":362
- * 
- *     @property
- *     def j(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.j
- *     @j.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_1j_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_1j_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_1j___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_1j___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":363
- *     @property
- *     def j(self):
- *         return self.ctx.j             # <<<<<<<<<<<<<<
- *     @j.setter
- *     def j(self, val):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_carray_to_py_a_real_t(__pyx_v_self->ctx.j, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 363, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":362
- * 
- *     @property
- *     def j(self):             # <<<<<<<<<<<<<<
- *         return self.ctx.j
- *     @j.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.j.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":365
- *         return self.ctx.j
- *     @j.setter
- *     def j(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.j[0] = val[0]
- *         self.ctx.j[1] = val[1]
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_1j_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_1j_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_1j_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((PyObject *)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_1j_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, PyObject *__pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  a_real_t __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":366
- *     @j.setter
- *     def j(self, val):
- *         self.ctx.j[0] = val[0]             # <<<<<<<<<<<<<<
- *         self.ctx.j[1] = val[1]
- * 
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 366, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 366, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.j[0]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":367
- *     def j(self, val):
- *         self.ctx.j[0] = val[0]
- *         self.ctx.j[1] = val[1]             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_val, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 367, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_2 == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 367, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  (__pyx_v_self->ctx.j[1]) = __pyx_t_2;
-
-  /* "python/src/a/polytrack.pxi":365
- *         return self.ctx.j
- *     @j.setter
- *     def j(self, val):             # <<<<<<<<<<<<<<
- *         self.ctx.j[0] = val[0]
- *         self.ctx.j[1] = val[1]
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.j.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":370
- * 
- *     @property
- *     def t0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.t[0]
- *     @t0.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_2t0_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_2t0_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2t0___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_2t0___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":371
- *     @property
- *     def t0(self) -> a_real_t:
- *         return self.ctx.t[0]             # <<<<<<<<<<<<<<
- *     @t0.setter
- *     def t0(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.t[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 371, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":370
- * 
- *     @property
- *     def t0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.t[0]
- *     @t0.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.t0.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":373
- *         return self.ctx.t[0]
- *     @t0.setter
- *     def t0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.t[0] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_2t0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_2t0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 373, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack7.t0.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2t0_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_2t0_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":374
- *     @t0.setter
- *     def t0(self, val: a_real_t):
- *         self.ctx.t[0] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.t[0]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":373
- *         return self.ctx.t[0]
- *     @t0.setter
- *     def t0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.t[0] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":377
- * 
- *     @property
- *     def q0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.q[0]
- *     @q0.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_2q0_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_2q0_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2q0___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_2q0___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":378
- *     @property
- *     def q0(self) -> a_real_t:
- *         return self.ctx.q[0]             # <<<<<<<<<<<<<<
- *     @q0.setter
- *     def q0(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.q[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 378, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":377
- * 
- *     @property
- *     def q0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.q[0]
- *     @q0.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.q0.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":380
- *         return self.ctx.q[0]
- *     @q0.setter
- *     def q0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.q[0] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_2q0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_2q0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 380, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack7.q0.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2q0_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_2q0_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":381
- *     @q0.setter
- *     def q0(self, val: a_real_t):
- *         self.ctx.q[0] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.q[0]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":380
- *         return self.ctx.q[0]
- *     @q0.setter
- *     def q0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.q[0] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":384
- * 
- *     @property
- *     def v0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.v[0]
- *     @v0.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_2v0_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_2v0_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2v0___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_2v0___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":385
- *     @property
- *     def v0(self) -> a_real_t:
- *         return self.ctx.v[0]             # <<<<<<<<<<<<<<
- *     @v0.setter
- *     def v0(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.v[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 385, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":384
- * 
- *     @property
- *     def v0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.v[0]
- *     @v0.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.v0.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":387
- *         return self.ctx.v[0]
- *     @v0.setter
- *     def v0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.v[0] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_2v0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_2v0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 387, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack7.v0.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2v0_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_2v0_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":388
- *     @v0.setter
- *     def v0(self, val: a_real_t):
- *         self.ctx.v[0] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.v[0]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":387
- *         return self.ctx.v[0]
- *     @v0.setter
- *     def v0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.v[0] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":391
- * 
- *     @property
- *     def a0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.a[0]
- *     @a0.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_2a0_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_2a0_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2a0___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_2a0___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":392
- *     @property
- *     def a0(self) -> a_real_t:
- *         return self.ctx.a[0]             # <<<<<<<<<<<<<<
- *     @a0.setter
- *     def a0(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.a[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 392, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":391
- * 
- *     @property
- *     def a0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.a[0]
- *     @a0.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.a0.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":394
- *         return self.ctx.a[0]
- *     @a0.setter
- *     def a0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.a[0] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_2a0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_2a0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 394, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack7.a0.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2a0_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_2a0_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":395
- *     @a0.setter
- *     def a0(self, val: a_real_t):
- *         self.ctx.a[0] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.a[0]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":394
- *         return self.ctx.a[0]
- *     @a0.setter
- *     def a0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.a[0] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":398
- * 
- *     @property
- *     def j0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.j[0]
- *     @j0.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_2j0_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_2j0_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2j0___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_2j0___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":399
- *     @property
- *     def j0(self) -> a_real_t:
- *         return self.ctx.j[0]             # <<<<<<<<<<<<<<
- *     @j0.setter
- *     def j0(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.j[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 399, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":398
- * 
- *     @property
- *     def j0(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.j[0]
- *     @j0.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.j0.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":401
- *         return self.ctx.j[0]
- *     @j0.setter
- *     def j0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.j[0] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_2j0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_2j0_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 401, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack7.j0.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2j0_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_2j0_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":402
- *     @j0.setter
- *     def j0(self, val: a_real_t):
- *         self.ctx.j[0] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.j[0]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":401
- *         return self.ctx.j[0]
- *     @j0.setter
- *     def j0(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.j[0] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":405
- * 
- *     @property
- *     def t1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.t[1]
- *     @t1.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_2t1_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_2t1_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2t1___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_2t1___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":406
- *     @property
- *     def t1(self) -> a_real_t:
- *         return self.ctx.t[1]             # <<<<<<<<<<<<<<
- *     @t1.setter
- *     def t1(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.t[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 406, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":405
- * 
- *     @property
- *     def t1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.t[1]
- *     @t1.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.t1.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":408
- *         return self.ctx.t[1]
- *     @t1.setter
- *     def t1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.t[1] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_2t1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_2t1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 408, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack7.t1.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2t1_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_2t1_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":409
- *     @t1.setter
- *     def t1(self, val: a_real_t):
- *         self.ctx.t[1] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.t[1]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":408
- *         return self.ctx.t[1]
- *     @t1.setter
- *     def t1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.t[1] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":412
- * 
- *     @property
- *     def q1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.q[1]
- *     @q1.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_2q1_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_2q1_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2q1___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_2q1___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":413
- *     @property
- *     def q1(self) -> a_real_t:
- *         return self.ctx.q[1]             # <<<<<<<<<<<<<<
- *     @q1.setter
- *     def q1(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.q[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 413, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":412
- * 
- *     @property
- *     def q1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.q[1]
- *     @q1.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.q1.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":415
- *         return self.ctx.q[1]
- *     @q1.setter
- *     def q1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.q[1] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_2q1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_2q1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 415, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack7.q1.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2q1_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_2q1_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":416
- *     @q1.setter
- *     def q1(self, val: a_real_t):
- *         self.ctx.q[1] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.q[1]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":415
- *         return self.ctx.q[1]
- *     @q1.setter
- *     def q1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.q[1] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":419
- * 
- *     @property
- *     def v1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.v[1]
- *     @v1.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_2v1_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_2v1_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2v1___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_2v1___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":420
- *     @property
- *     def v1(self) -> a_real_t:
- *         return self.ctx.v[1]             # <<<<<<<<<<<<<<
- *     @v1.setter
- *     def v1(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.v[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 420, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":419
- * 
- *     @property
- *     def v1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.v[1]
- *     @v1.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.v1.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":422
- *         return self.ctx.v[1]
- *     @v1.setter
- *     def v1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.v[1] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_2v1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_2v1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 422, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack7.v1.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2v1_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_2v1_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":423
- *     @v1.setter
- *     def v1(self, val: a_real_t):
- *         self.ctx.v[1] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.v[1]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":422
- *         return self.ctx.v[1]
- *     @v1.setter
- *     def v1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.v[1] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":426
- * 
- *     @property
- *     def a1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.a[1]
- *     @a1.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_2a1_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_2a1_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2a1___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_2a1___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":427
- *     @property
- *     def a1(self) -> a_real_t:
- *         return self.ctx.a[1]             # <<<<<<<<<<<<<<
- *     @a1.setter
- *     def a1(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.a[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 427, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":426
- * 
- *     @property
- *     def a1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.a[1]
- *     @a1.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.a1.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":429
- *         return self.ctx.a[1]
- *     @a1.setter
- *     def a1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.a[1] = val
- * 
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_2a1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_2a1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 429, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack7.a1.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2a1_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_2a1_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":430
- *     @a1.setter
- *     def a1(self, val: a_real_t):
- *         self.ctx.a[1] = val             # <<<<<<<<<<<<<<
- * 
- *     @property
- */
-  (__pyx_v_self->ctx.a[1]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":429
- *         return self.ctx.a[1]
- *     @a1.setter
- *     def a1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.a[1] = val
- * 
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":433
- * 
- *     @property
- *     def j1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.j[1]
- *     @j1.setter
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_4liba_10polytrack7_2j1_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_4liba_10polytrack7_2j1_1__get__(PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2j1___get__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_4liba_10polytrack7_2j1___get__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
-
-  /* "python/src/a/polytrack.pxi":434
- *     @property
- *     def j1(self) -> a_real_t:
- *         return self.ctx.j[1]             # <<<<<<<<<<<<<<
- *     @j1.setter
- *     def j1(self, val: a_real_t):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_self->ctx.j[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 434, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "python/src/a/polytrack.pxi":433
- * 
- *     @property
- *     def j1(self) -> a_real_t:             # <<<<<<<<<<<<<<
- *         return self.ctx.j[1]
- *     @j1.setter
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("liba.polytrack7.j1.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "python/src/a/polytrack.pxi":436
- *         return self.ctx.j[1]
- *     @j1.setter
- *     def j1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.j[1] = val
- */
-
-/* Python wrapper */
-static int __pyx_pw_4liba_10polytrack7_2j1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val); /*proto*/
-static int __pyx_pw_4liba_10polytrack7_2j1_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_arg_val) {
-  a_real_t __pyx_v_val;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  assert(__pyx_arg_val); {
-    __pyx_v_val = __pyx_PyFloat_AsDouble(__pyx_arg_val); if (unlikely((__pyx_v_val == ((a_real_t)-1)) && PyErr_Occurred())) __PYX_ERR(9, 436, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("liba.polytrack7.j1.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return -1;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4liba_10polytrack7_2j1_2__set__(((struct __pyx_obj_4liba_polytrack7 *)__pyx_v_self), ((a_real_t)__pyx_v_val));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static int __pyx_pf_4liba_10polytrack7_2j1_2__set__(struct __pyx_obj_4liba_polytrack7 *__pyx_v_self, a_real_t __pyx_v_val) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__set__", 0);
-
-  /* "python/src/a/polytrack.pxi":437
- *     @j1.setter
- *     def j1(self, val: a_real_t):
- *         self.ctx.j[1] = val             # <<<<<<<<<<<<<<
- */
-  (__pyx_v_self->ctx.j[1]) = __pyx_v_val;
-
-  /* "python/src/a/polytrack.pxi":436
- *         return self.ctx.j[1]
- *     @j1.setter
- *     def j1(self, val: a_real_t):             # <<<<<<<<<<<<<<
- *         self.ctx.j[1] = val
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
@@ -23381,15 +19044,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = mf.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_mf__set_state(<mf> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_mf__set_state(mf __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_f_4liba___pyx_unpickle_mf__set_state(((struct __pyx_obj_4liba_mf *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = mf.__new__(__pyx_type)
@@ -25333,161 +20996,26 @@
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyObject *__pyx_getprop_4liba_10polytrack3_k(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_4liba_10polytrack3_1k_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_4liba_10polytrack3_t(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack3_1t_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack3_t(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack3_1t_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack3_q(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack3_1q_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack3_q(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack3_1q_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack3_v(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack3_1v_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack3_v(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack3_1v_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack3_t0(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack3_2t0_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack3_t0(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack3_2t0_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack3_q0(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack3_2q0_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack3_q0(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack3_2q0_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack3_v0(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack3_2v0_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack3_v0(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack3_2v0_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack3_t1(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack3_2t1_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack3_t1(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack3_2t1_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack3_q1(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack3_2q1_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack3_q1(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack3_2q1_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack3_v1(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack3_2v1_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack3_v1(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack3_2v1_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
 static PyMethodDef __pyx_methods_4liba_polytrack3[] = {
-  {"pos", (PyCFunction)__pyx_pw_4liba_10polytrack3_5pos, METH_O, __pyx_doc_4liba_10polytrack3_4pos},
-  {"vec", (PyCFunction)__pyx_pw_4liba_10polytrack3_7vec, METH_O, __pyx_doc_4liba_10polytrack3_6vec},
-  {"acc", (PyCFunction)__pyx_pw_4liba_10polytrack3_9acc, METH_O, __pyx_doc_4liba_10polytrack3_8acc},
-  {"gen", (PyCFunction)__pyx_pw_4liba_10polytrack3_11gen, METH_NOARGS, __pyx_doc_4liba_10polytrack3_10gen},
+  {"gen", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4liba_10polytrack3_3gen, METH_VARARGS|METH_KEYWORDS, __pyx_doc_4liba_10polytrack3_2gen},
+  {"pos", (PyCFunction)__pyx_pw_4liba_10polytrack3_7pos, METH_O, __pyx_doc_4liba_10polytrack3_6pos},
+  {"vec", (PyCFunction)__pyx_pw_4liba_10polytrack3_9vec, METH_O, __pyx_doc_4liba_10polytrack3_8vec},
+  {"acc", (PyCFunction)__pyx_pw_4liba_10polytrack3_11acc, METH_O, __pyx_doc_4liba_10polytrack3_10acc},
   {"__reduce_cython__", (PyCFunction)__pyx_pw_4liba_10polytrack3_13__reduce_cython__, METH_NOARGS, 0},
   {"__setstate_cython__", (PyCFunction)__pyx_pw_4liba_10polytrack3_15__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_4liba_polytrack3[] = {
   {(char *)"k", __pyx_getprop_4liba_10polytrack3_k, 0, (char *)0, 0},
-  {(char *)"t", __pyx_getprop_4liba_10polytrack3_t, __pyx_setprop_4liba_10polytrack3_t, (char *)0, 0},
-  {(char *)"q", __pyx_getprop_4liba_10polytrack3_q, __pyx_setprop_4liba_10polytrack3_q, (char *)0, 0},
-  {(char *)"v", __pyx_getprop_4liba_10polytrack3_v, __pyx_setprop_4liba_10polytrack3_v, (char *)0, 0},
-  {(char *)"t0", __pyx_getprop_4liba_10polytrack3_t0, __pyx_setprop_4liba_10polytrack3_t0, (char *)0, 0},
-  {(char *)"q0", __pyx_getprop_4liba_10polytrack3_q0, __pyx_setprop_4liba_10polytrack3_q0, (char *)0, 0},
-  {(char *)"v0", __pyx_getprop_4liba_10polytrack3_v0, __pyx_setprop_4liba_10polytrack3_v0, (char *)0, 0},
-  {(char *)"t1", __pyx_getprop_4liba_10polytrack3_t1, __pyx_setprop_4liba_10polytrack3_t1, (char *)0, 0},
-  {(char *)"q1", __pyx_getprop_4liba_10polytrack3_q1, __pyx_setprop_4liba_10polytrack3_q1, (char *)0, 0},
-  {(char *)"v1", __pyx_getprop_4liba_10polytrack3_v1, __pyx_setprop_4liba_10polytrack3_v1, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type_4liba_polytrack3 = {
   PyVarObject_HEAD_INIT(0, 0)
   "liba.polytrack3", /*tp_name*/
   sizeof(struct __pyx_obj_4liba_polytrack3), /*tp_basicsize*/
@@ -25508,15 +21036,15 @@
   0, /*tp_as_async*/
   #endif
   0, /*tp_repr*/
   0, /*tp_as_number*/
   0, /*tp_as_sequence*/
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
-  __pyx_pw_4liba_10polytrack3_3__call__, /*tp_call*/
+  __pyx_pw_4liba_10polytrack3_5__call__, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE, /*tp_flags*/
   "cubic polynomial trajectory", /*tp_doc*/
   0, /*tp_traverse*/
@@ -25583,206 +21111,26 @@
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyObject *__pyx_getprop_4liba_10polytrack5_k(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_4liba_10polytrack5_1k_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_4liba_10polytrack5_t(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack5_1t_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack5_t(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack5_1t_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack5_q(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack5_1q_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack5_q(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack5_1q_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack5_v(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack5_1v_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack5_v(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack5_1v_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack5_a(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack5_1a_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack5_a(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack5_1a_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack5_t0(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack5_2t0_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack5_t0(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack5_2t0_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack5_q0(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack5_2q0_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack5_q0(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack5_2q0_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack5_v0(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack5_2v0_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack5_v0(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack5_2v0_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack5_a0(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack5_2a0_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack5_a0(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack5_2a0_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack5_t1(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack5_2t1_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack5_t1(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack5_2t1_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack5_q1(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack5_2q1_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack5_q1(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack5_2q1_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack5_v1(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack5_2v1_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack5_v1(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack5_2v1_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack5_a1(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack5_2a1_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack5_a1(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack5_2a1_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
 static PyMethodDef __pyx_methods_4liba_polytrack5[] = {
-  {"pos", (PyCFunction)__pyx_pw_4liba_10polytrack5_5pos, METH_O, __pyx_doc_4liba_10polytrack5_4pos},
-  {"vec", (PyCFunction)__pyx_pw_4liba_10polytrack5_7vec, METH_O, __pyx_doc_4liba_10polytrack5_6vec},
-  {"acc", (PyCFunction)__pyx_pw_4liba_10polytrack5_9acc, METH_O, __pyx_doc_4liba_10polytrack5_8acc},
-  {"gen", (PyCFunction)__pyx_pw_4liba_10polytrack5_11gen, METH_NOARGS, __pyx_doc_4liba_10polytrack5_10gen},
+  {"gen", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4liba_10polytrack5_3gen, METH_VARARGS|METH_KEYWORDS, __pyx_doc_4liba_10polytrack5_2gen},
+  {"pos", (PyCFunction)__pyx_pw_4liba_10polytrack5_7pos, METH_O, __pyx_doc_4liba_10polytrack5_6pos},
+  {"vec", (PyCFunction)__pyx_pw_4liba_10polytrack5_9vec, METH_O, __pyx_doc_4liba_10polytrack5_8vec},
+  {"acc", (PyCFunction)__pyx_pw_4liba_10polytrack5_11acc, METH_O, __pyx_doc_4liba_10polytrack5_10acc},
   {"__reduce_cython__", (PyCFunction)__pyx_pw_4liba_10polytrack5_13__reduce_cython__, METH_NOARGS, 0},
   {"__setstate_cython__", (PyCFunction)__pyx_pw_4liba_10polytrack5_15__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_4liba_polytrack5[] = {
   {(char *)"k", __pyx_getprop_4liba_10polytrack5_k, 0, (char *)0, 0},
-  {(char *)"t", __pyx_getprop_4liba_10polytrack5_t, __pyx_setprop_4liba_10polytrack5_t, (char *)0, 0},
-  {(char *)"q", __pyx_getprop_4liba_10polytrack5_q, __pyx_setprop_4liba_10polytrack5_q, (char *)0, 0},
-  {(char *)"v", __pyx_getprop_4liba_10polytrack5_v, __pyx_setprop_4liba_10polytrack5_v, (char *)0, 0},
-  {(char *)"a", __pyx_getprop_4liba_10polytrack5_a, __pyx_setprop_4liba_10polytrack5_a, (char *)0, 0},
-  {(char *)"t0", __pyx_getprop_4liba_10polytrack5_t0, __pyx_setprop_4liba_10polytrack5_t0, (char *)0, 0},
-  {(char *)"q0", __pyx_getprop_4liba_10polytrack5_q0, __pyx_setprop_4liba_10polytrack5_q0, (char *)0, 0},
-  {(char *)"v0", __pyx_getprop_4liba_10polytrack5_v0, __pyx_setprop_4liba_10polytrack5_v0, (char *)0, 0},
-  {(char *)"a0", __pyx_getprop_4liba_10polytrack5_a0, __pyx_setprop_4liba_10polytrack5_a0, (char *)0, 0},
-  {(char *)"t1", __pyx_getprop_4liba_10polytrack5_t1, __pyx_setprop_4liba_10polytrack5_t1, (char *)0, 0},
-  {(char *)"q1", __pyx_getprop_4liba_10polytrack5_q1, __pyx_setprop_4liba_10polytrack5_q1, (char *)0, 0},
-  {(char *)"v1", __pyx_getprop_4liba_10polytrack5_v1, __pyx_setprop_4liba_10polytrack5_v1, (char *)0, 0},
-  {(char *)"a1", __pyx_getprop_4liba_10polytrack5_a1, __pyx_setprop_4liba_10polytrack5_a1, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type_4liba_polytrack5 = {
   PyVarObject_HEAD_INIT(0, 0)
   "liba.polytrack5", /*tp_name*/
   sizeof(struct __pyx_obj_4liba_polytrack5), /*tp_basicsize*/
@@ -25803,15 +21151,15 @@
   0, /*tp_as_async*/
   #endif
   0, /*tp_repr*/
   0, /*tp_as_number*/
   0, /*tp_as_sequence*/
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
-  __pyx_pw_4liba_10polytrack5_3__call__, /*tp_call*/
+  __pyx_pw_4liba_10polytrack5_5__call__, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE, /*tp_flags*/
   "quintic polynomial trajectory", /*tp_doc*/
   0, /*tp_traverse*/
@@ -25878,252 +21226,27 @@
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyObject *__pyx_getprop_4liba_10polytrack7_k(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_4liba_10polytrack7_1k_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_4liba_10polytrack7_t(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_1t_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_t(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_1t_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack7_q(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_1q_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_q(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_1q_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack7_v(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_1v_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_v(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_1v_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack7_a(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_1a_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_a(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_1a_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack7_j(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_1j_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_j(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_1j_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack7_t0(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_2t0_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_t0(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_2t0_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack7_q0(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_2q0_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_q0(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_2q0_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack7_v0(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_2v0_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_v0(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_2v0_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack7_a0(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_2a0_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_a0(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_2a0_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack7_j0(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_2j0_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_j0(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_2j0_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack7_t1(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_2t1_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_t1(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_2t1_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack7_q1(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_2q1_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_q1(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_2q1_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack7_v1(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_2v1_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_v1(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_2v1_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack7_a1(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_2a1_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_a1(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_2a1_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
-static PyObject *__pyx_getprop_4liba_10polytrack7_j1(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_4liba_10polytrack7_2j1_1__get__(o);
-}
-
-static int __pyx_setprop_4liba_10polytrack7_j1(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
-  if (v) {
-    return __pyx_pw_4liba_10polytrack7_2j1_3__set__(o, v);
-  }
-  else {
-    PyErr_SetString(PyExc_NotImplementedError, "__del__");
-    return -1;
-  }
-}
-
 static PyMethodDef __pyx_methods_4liba_polytrack7[] = {
-  {"pos", (PyCFunction)__pyx_pw_4liba_10polytrack7_5pos, METH_O, __pyx_doc_4liba_10polytrack7_4pos},
-  {"vec", (PyCFunction)__pyx_pw_4liba_10polytrack7_7vec, METH_O, __pyx_doc_4liba_10polytrack7_6vec},
-  {"acc", (PyCFunction)__pyx_pw_4liba_10polytrack7_9acc, METH_O, __pyx_doc_4liba_10polytrack7_8acc},
-  {"jer", (PyCFunction)__pyx_pw_4liba_10polytrack7_11jer, METH_O, __pyx_doc_4liba_10polytrack7_10jer},
-  {"gen", (PyCFunction)__pyx_pw_4liba_10polytrack7_13gen, METH_NOARGS, __pyx_doc_4liba_10polytrack7_12gen},
+  {"gen", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4liba_10polytrack7_3gen, METH_VARARGS|METH_KEYWORDS, __pyx_doc_4liba_10polytrack7_2gen},
+  {"pos", (PyCFunction)__pyx_pw_4liba_10polytrack7_7pos, METH_O, __pyx_doc_4liba_10polytrack7_6pos},
+  {"vec", (PyCFunction)__pyx_pw_4liba_10polytrack7_9vec, METH_O, __pyx_doc_4liba_10polytrack7_8vec},
+  {"acc", (PyCFunction)__pyx_pw_4liba_10polytrack7_11acc, METH_O, __pyx_doc_4liba_10polytrack7_10acc},
+  {"jer", (PyCFunction)__pyx_pw_4liba_10polytrack7_13jer, METH_O, __pyx_doc_4liba_10polytrack7_12jer},
   {"__reduce_cython__", (PyCFunction)__pyx_pw_4liba_10polytrack7_15__reduce_cython__, METH_NOARGS, 0},
   {"__setstate_cython__", (PyCFunction)__pyx_pw_4liba_10polytrack7_17__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_4liba_polytrack7[] = {
   {(char *)"k", __pyx_getprop_4liba_10polytrack7_k, 0, (char *)0, 0},
-  {(char *)"t", __pyx_getprop_4liba_10polytrack7_t, __pyx_setprop_4liba_10polytrack7_t, (char *)0, 0},
-  {(char *)"q", __pyx_getprop_4liba_10polytrack7_q, __pyx_setprop_4liba_10polytrack7_q, (char *)0, 0},
-  {(char *)"v", __pyx_getprop_4liba_10polytrack7_v, __pyx_setprop_4liba_10polytrack7_v, (char *)0, 0},
-  {(char *)"a", __pyx_getprop_4liba_10polytrack7_a, __pyx_setprop_4liba_10polytrack7_a, (char *)0, 0},
-  {(char *)"j", __pyx_getprop_4liba_10polytrack7_j, __pyx_setprop_4liba_10polytrack7_j, (char *)0, 0},
-  {(char *)"t0", __pyx_getprop_4liba_10polytrack7_t0, __pyx_setprop_4liba_10polytrack7_t0, (char *)0, 0},
-  {(char *)"q0", __pyx_getprop_4liba_10polytrack7_q0, __pyx_setprop_4liba_10polytrack7_q0, (char *)0, 0},
-  {(char *)"v0", __pyx_getprop_4liba_10polytrack7_v0, __pyx_setprop_4liba_10polytrack7_v0, (char *)0, 0},
-  {(char *)"a0", __pyx_getprop_4liba_10polytrack7_a0, __pyx_setprop_4liba_10polytrack7_a0, (char *)0, 0},
-  {(char *)"j0", __pyx_getprop_4liba_10polytrack7_j0, __pyx_setprop_4liba_10polytrack7_j0, (char *)0, 0},
-  {(char *)"t1", __pyx_getprop_4liba_10polytrack7_t1, __pyx_setprop_4liba_10polytrack7_t1, (char *)0, 0},
-  {(char *)"q1", __pyx_getprop_4liba_10polytrack7_q1, __pyx_setprop_4liba_10polytrack7_q1, (char *)0, 0},
-  {(char *)"v1", __pyx_getprop_4liba_10polytrack7_v1, __pyx_setprop_4liba_10polytrack7_v1, (char *)0, 0},
-  {(char *)"a1", __pyx_getprop_4liba_10polytrack7_a1, __pyx_setprop_4liba_10polytrack7_a1, (char *)0, 0},
-  {(char *)"j1", __pyx_getprop_4liba_10polytrack7_j1, __pyx_setprop_4liba_10polytrack7_j1, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type_4liba_polytrack7 = {
   PyVarObject_HEAD_INIT(0, 0)
   "liba.polytrack7", /*tp_name*/
   sizeof(struct __pyx_obj_4liba_polytrack7), /*tp_basicsize*/
@@ -26144,15 +21267,15 @@
   0, /*tp_as_async*/
   #endif
   0, /*tp_repr*/
   0, /*tp_as_number*/
   0, /*tp_as_sequence*/
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
-  __pyx_pw_4liba_10polytrack7_3__call__, /*tp_call*/
+  __pyx_pw_4liba_10polytrack7_5__call__, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE, /*tp_flags*/
   "hepta polynomial trajectory", /*tp_doc*/
   0, /*tp_traverse*/
@@ -27883,15 +23006,14 @@
   {&__pyx_n_s_t0, __pyx_k_t0, sizeof(__pyx_k_t0), 0, 0, 1, 1},
   {&__pyx_n_s_t1, __pyx_k_t1, sizeof(__pyx_k_t1), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_tf, __pyx_k_tf, sizeof(__pyx_k_tf), 0, 0, 1, 1},
   {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
   {&__pyx_n_s_trap, __pyx_k_trap, sizeof(__pyx_k_trap), 0, 0, 1, 1},
   {&__pyx_n_s_tri, __pyx_k_tri, sizeof(__pyx_k_tri), 0, 0, 1, 1},
-  {&__pyx_n_s_ts, __pyx_k_ts, sizeof(__pyx_k_ts), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
   {&__pyx_n_s_v0, __pyx_k_v0, sizeof(__pyx_k_v0), 0, 0, 1, 1},
   {&__pyx_n_s_v1, __pyx_k_v1, sizeof(__pyx_k_v1), 0, 0, 1, 1},
   {&__pyx_n_s_version, __pyx_k_version, sizeof(__pyx_k_version), 0, 0, 1, 1},
   {&__pyx_n_s_version_major, __pyx_k_version_major, sizeof(__pyx_k_version_major), 0, 0, 1, 1},
   {&__pyx_n_s_version_minor, __pyx_k_version_minor, sizeof(__pyx_k_version_minor), 0, 0, 1, 1},
@@ -28214,15 +23336,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(3, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(3, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(3, 1, __pyx_L1_error)
   __pyx_int_222419149 = PyInt_FromLong(222419149L); if (unlikely(!__pyx_int_222419149)) __PYX_ERR(3, 1, __pyx_L1_error)
   __pyx_int_228825662 = PyInt_FromLong(228825662L); if (unlikely(!__pyx_int_228825662)) __PYX_ERR(3, 1, __pyx_L1_error)
   __pyx_int_238750788 = PyInt_FromLong(238750788L); if (unlikely(!__pyx_int_238750788)) __PYX_ERR(3, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
@@ -28345,62 +23467,62 @@
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_4liba_polytrack3.tp_dictoffset && __pyx_type_4liba_polytrack3.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_4liba_polytrack3.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
     PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_4liba_polytrack3, "__call__"); if (unlikely(!wrapper)) __PYX_ERR(9, 5, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
-      __pyx_wrapperbase_4liba_10polytrack3_2__call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
-      __pyx_wrapperbase_4liba_10polytrack3_2__call__.doc = __pyx_doc_4liba_10polytrack3_2__call__;
-      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_4liba_10polytrack3_2__call__;
+      __pyx_wrapperbase_4liba_10polytrack3_4__call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
+      __pyx_wrapperbase_4liba_10polytrack3_4__call__.doc = __pyx_doc_4liba_10polytrack3_4__call__;
+      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_4liba_10polytrack3_4__call__;
     }
   }
   #endif
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_polytrack3, (PyObject *)&__pyx_type_4liba_polytrack3) < 0) __PYX_ERR(9, 5, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_4liba_polytrack3) < 0) __PYX_ERR(9, 5, __pyx_L1_error)
   __pyx_ptype_4liba_polytrack3 = &__pyx_type_4liba_polytrack3;
-  if (PyType_Ready(&__pyx_type_4liba_polytrack5) < 0) __PYX_ERR(9, 125, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_4liba_polytrack5) < 0) __PYX_ERR(9, 59, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_4liba_polytrack5.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_4liba_polytrack5.tp_dictoffset && __pyx_type_4liba_polytrack5.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_4liba_polytrack5.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
-    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_4liba_polytrack5, "__call__"); if (unlikely(!wrapper)) __PYX_ERR(9, 125, __pyx_L1_error)
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_4liba_polytrack5, "__call__"); if (unlikely(!wrapper)) __PYX_ERR(9, 59, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
-      __pyx_wrapperbase_4liba_10polytrack5_2__call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
-      __pyx_wrapperbase_4liba_10polytrack5_2__call__.doc = __pyx_doc_4liba_10polytrack5_2__call__;
-      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_4liba_10polytrack5_2__call__;
+      __pyx_wrapperbase_4liba_10polytrack5_4__call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
+      __pyx_wrapperbase_4liba_10polytrack5_4__call__.doc = __pyx_doc_4liba_10polytrack5_4__call__;
+      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_4liba_10polytrack5_4__call__;
     }
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_polytrack5, (PyObject *)&__pyx_type_4liba_polytrack5) < 0) __PYX_ERR(9, 125, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_4liba_polytrack5) < 0) __PYX_ERR(9, 125, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_polytrack5, (PyObject *)&__pyx_type_4liba_polytrack5) < 0) __PYX_ERR(9, 59, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_4liba_polytrack5) < 0) __PYX_ERR(9, 59, __pyx_L1_error)
   __pyx_ptype_4liba_polytrack5 = &__pyx_type_4liba_polytrack5;
-  if (PyType_Ready(&__pyx_type_4liba_polytrack7) < 0) __PYX_ERR(9, 267, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_4liba_polytrack7) < 0) __PYX_ERR(9, 113, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_4liba_polytrack7.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_4liba_polytrack7.tp_dictoffset && __pyx_type_4liba_polytrack7.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_4liba_polytrack7.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
-    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_4liba_polytrack7, "__call__"); if (unlikely(!wrapper)) __PYX_ERR(9, 267, __pyx_L1_error)
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_4liba_polytrack7, "__call__"); if (unlikely(!wrapper)) __PYX_ERR(9, 113, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
-      __pyx_wrapperbase_4liba_10polytrack7_2__call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
-      __pyx_wrapperbase_4liba_10polytrack7_2__call__.doc = __pyx_doc_4liba_10polytrack7_2__call__;
-      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_4liba_10polytrack7_2__call__;
+      __pyx_wrapperbase_4liba_10polytrack7_4__call__ = *((PyWrapperDescrObject *)wrapper)->d_base;
+      __pyx_wrapperbase_4liba_10polytrack7_4__call__.doc = __pyx_doc_4liba_10polytrack7_4__call__;
+      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_4liba_10polytrack7_4__call__;
     }
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_polytrack7, (PyObject *)&__pyx_type_4liba_polytrack7) < 0) __PYX_ERR(9, 267, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_4liba_polytrack7) < 0) __PYX_ERR(9, 267, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_polytrack7, (PyObject *)&__pyx_type_4liba_polytrack7) < 0) __PYX_ERR(9, 113, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_4liba_polytrack7) < 0) __PYX_ERR(9, 113, __pyx_L1_error)
   __pyx_ptype_4liba_polytrack7 = &__pyx_type_4liba_polytrack7;
   if (PyType_Ready(&__pyx_type_4liba___pyx_scope_struct____cinit__) < 0) __PYX_ERR(7, 15, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_4liba___pyx_scope_struct____cinit__.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_4liba___pyx_scope_struct____cinit__.tp_dictoffset && __pyx_type_4liba___pyx_scope_struct____cinit__.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_4liba___pyx_scope_struct____cinit__.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
@@ -28722,15 +23844,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(3, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(3, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(3, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(3, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(3, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_liba) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(3, 1, __pyx_L1_error)
@@ -30121,101 +25243,14 @@
 #endif
 
 /* None */
 static CYTHON_INLINE void __Pyx_RaiseClosureNameError(const char *varname) {
     PyErr_Format(PyExc_NameError, "free variable '%s' referenced before assignment in enclosing scope", varname);
 }
 
-/* GetItemInt */
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
-    PyObject *r;
-    if (!j) return NULL;
-    r = PyObject_GetItem(o, j);
-    Py_DECREF(j);
-    return r;
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyList_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
-        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyTuple_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
-        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
-                                                     CYTHON_NCP_UNUSED int wraparound,
-                                                     CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
-        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
-            PyObject *r = PyList_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    }
-    else if (PyTuple_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
-            PyObject *r = PyTuple_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return NULL;
-                    PyErr_Clear();
-                }
-            }
-            return m->sq_item(o, i);
-        }
-    }
-#else
-    if (is_list || PySequence_Check(o)) {
-        return PySequence_GetItem(o, i);
-    }
-#endif
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-}
-
 /* Import */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
     PyObject *empty_list = 0;
     PyObject *module = 0;
     PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
     PyObject *list;
@@ -30334,14 +25369,101 @@
         return 0;
     } else {
         Py_DECREF(r);
         return 1;
     }
 }
 
+/* GetItemInt */
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+    PyObject *r;
+    if (!j) return NULL;
+    r = PyObject_GetItem(o, j);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyList_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
+        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyTuple_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
+        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
+                                                     CYTHON_NCP_UNUSED int wraparound,
+                                                     CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
+        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
+            PyObject *r = PyList_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    }
+    else if (PyTuple_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
+            PyObject *r = PyTuple_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    } else {
+        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
+        if (likely(m && m->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
+                Py_ssize_t l = m->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return NULL;
+                    PyErr_Clear();
+                }
+            }
+            return m->sq_item(o, i);
+        }
+    }
+#else
+    if (is_list || PySequence_Check(o)) {
+        return PySequence_GetItem(o, i);
+    }
+#endif
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+}
+
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
                  "'%.50s' object has no attribute '%U'",
                  tp->tp_name, attr_name);
@@ -30593,15 +25715,15 @@
         result = __Pyx_GetGlobalNameAfterAttributeLookup(name);
     }
     return result;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `liba-0.1.1rc5/setup.cfg` & `liba-0.1.1rc6/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6c69 6261 0a76 6572 7369 6f6e 203d  = liba.version =
-00000020: 2030 2e31 2e31 2d72 6335 0a75 726c 203d   0.1.1-rc5.url =
-00000030: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000040: 636f 6d2f 7471 6678 2f6c 6962 612e 6769  com/tqfx/liba.gi
-00000050: 740a 6175 7468 6f72 203d 2074 7166 780a  t.author = tqfx.
-00000060: 6175 7468 6f72 5f65 6d61 696c 203d 2074  author_email = t
-00000070: 7166 7840 666f 786d 6169 6c2e 636f 6d0a  qfx@foxmail.com.
-00000080: 636c 6173 7369 6669 6572 7320 3d20 0a09  classifiers = ..
-00000090: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000000a0: 7561 6765 203a 3a20 430a 0950 726f 6772  uage :: C..Progr
-000000b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000000c0: 3a3a 2043 2b2b 0a09 5072 6f67 7261 6d6d  :: C++..Programm
-000000d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000000e0: 4379 7468 6f6e 0a09 5072 6f67 7261 6d6d  Cython..Programm
-000000f0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000100: 5079 7468 6f6e 0a09 4c69 6365 6e73 6520  Python..License 
-00000110: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000120: 3a3a 204d 6f7a 696c 6c61 2050 7562 6c69  :: Mozilla Publi
-00000130: 6320 4c69 6365 6e73 6520 322e 3020 284d  c License 2.0 (M
-00000140: 504c 2032 2e30 290a 6c69 6365 6e73 6520  PL 2.0).license 
-00000150: 3d20 4d50 4c2d 322e 300a 6465 7363 7269  = MPL-2.0.descri
-00000160: 7074 696f 6e20 3d20 416e 2061 6c67 6f72  ption = An algor
-00000170: 6974 686d 206c 6962 7261 7279 2062 6173  ithm library bas
-00000180: 6564 206f 6e20 432f 432b 2b20 6c61 6e67  ed on C/C++ lang
-00000190: 7561 6765 0a6c 6f6e 675f 6465 7363 7269  uage.long_descri
-000001a0: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
-000001b0: 4144 4d45 2e6d 640a 6c6f 6e67 5f64 6573  ADME.md.long_des
-000001c0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-000001d0: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
-000001e0: 6b64 6f77 6e0a 6b65 7977 6f72 6473 203d  kdown.keywords =
-000001f0: 2061 6c67 6f72 6974 686d 730a 706c 6174   algorithms.plat
-00000200: 666f 726d 7320 3d20 4350 7974 686f 6e0a  forms = CPython.
-00000210: 0a5b 6567 675f 696e 666f 5d0a 7461 675f  .[egg_info].tag_
-00000220: 6275 696c 6420 3d20 0a74 6167 5f64 6174  build = .tag_dat
-00000230: 6520 3d20 300a 0a                        e = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 206c 6962 610d 0a76 6572 7369 6f6e   = liba..version
+00000020: 203d 2030 2e31 2e31 2d72 6336 0d0a 7572   = 0.1.1-rc6..ur
+00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
+00000040: 7562 2e63 6f6d 2f74 7166 782f 6c69 6261  ub.com/tqfx/liba
+00000050: 2e67 6974 0d0a 6175 7468 6f72 203d 2074  .git..author = t
+00000060: 7166 780d 0a61 7574 686f 725f 656d 6169  qfx..author_emai
+00000070: 6c20 3d20 7471 6678 4066 6f78 6d61 696c  l = tqfx@foxmail
+00000080: 2e63 6f6d 0d0a 636c 6173 7369 6669 6572  .com..classifier
+00000090: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
+000000a0: 6e67 204c 616e 6775 6167 6520 3a3a 2043  ng Language :: C
+000000b0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+000000c0: 616e 6775 6167 6520 3a3a 2043 2b2b 0d0a  anguage :: C++..
+000000d0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000000e0: 6775 6167 6520 3a3a 2043 7974 686f 6e0d  guage :: Cython.
+000000f0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000100: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000110: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
+00000120: 4920 4170 7072 6f76 6564 203a 3a20 4d6f  I Approved :: Mo
+00000130: 7a69 6c6c 6120 5075 626c 6963 204c 6963  zilla Public Lic
+00000140: 656e 7365 2032 2e30 2028 4d50 4c20 322e  ense 2.0 (MPL 2.
+00000150: 3029 0d0a 6c69 6365 6e73 6520 3d20 4d50  0)..license = MP
+00000160: 4c2d 322e 300d 0a64 6573 6372 6970 7469  L-2.0..descripti
+00000170: 6f6e 203d 2041 6e20 616c 676f 7269 7468  on = An algorith
+00000180: 6d20 6c69 6272 6172 7920 6261 7365 6420  m library based 
+00000190: 6f6e 2043 2f43 2b2b 206c 616e 6775 6167  on C/C++ languag
+000001a0: 650d 0a6c 6f6e 675f 6465 7363 7269 7074  e..long_descript
+000001b0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+000001c0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
+000001d0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+000001e0: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+000001f0: 646f 776e 0d0a 6b65 7977 6f72 6473 203d  down..keywords =
+00000200: 2061 6c67 6f72 6974 686d 730d 0a70 6c61   algorithms..pla
+00000210: 7466 6f72 6d73 203d 2043 5079 7468 6f6e  tforms = CPython
+00000220: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000230: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000240: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `liba-0.1.1rc5/setup.py` & `liba-0.1.1rc6/setup.py`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/a.c` & `liba-0.1.1rc6/src/a.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/avl.c` & `liba-0.1.1rc6/src/avl.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/buf.c` & `liba-0.1.1rc6/src/buf.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/complex.c` & `liba-0.1.1rc6/src/complex.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/complex.h` & `liba-0.1.1rc6/src/complex.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/crc.c` & `liba-0.1.1rc6/src/crc.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/fpid.c` & `liba-0.1.1rc6/src/fpid.c`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,22 @@
     ctx->pid.reg |= op;
     switch (op)
     {
     case A_FPID_OR_ALGEBRA:
         ctx->op = a_fpid_op_or;
         break;
     case A_FPID_OR_BOUNDED:
-    case A_FPID_AND:
+    case A_FPID_AND_DEFAULT:
         ctx->op = a_real_min;
         break;
     case A_FPID_AND_ALGEBRA:
         ctx->op = a_fpid_op_and;
         break;
     case A_FPID_AND_BOUNDED:
-    case A_FPID_OR:
+    case A_FPID_OR_DEFAULT:
         ctx->op = a_real_max;
         break;
     case A_FPID_EQU:
     default:
         ctx->op = a_fpid_op_equ;
     }
 }
@@ -232,23 +232,23 @@
             }
         }
         qv[2] *= inv;
     }
     a_pid_kpid(&ctx->pid, ctx->kp + qv[0], ctx->ki + qv[1], ctx->kd + qv[2]);
 }
 
-a_real_t a_fpid_outv(a_fpid_s *const ctx, a_real_t const set, a_real_t const fdb)
+a_real_t a_fpid_outf(a_fpid_s *const ctx, a_real_t const set, a_real_t const fdb)
 {
     a_real_t const e = set - fdb;
-    a_real_t const ec = e - ctx->pid.e.v;
+    a_real_t const ec = e - ctx->pid.e.f;
     a_fpid_iter_(ctx, a_fpid_col(ctx), ec, e);
-    return a_pid_outv_(&ctx->pid, a_pid_mode(&ctx->pid), set, fdb, ec, e);
+    return a_pid_outf_(&ctx->pid, a_pid_mode(&ctx->pid), set, fdb, ec, e);
 }
 
-a_real_t *a_fpid_outp(a_fpid_s *const ctx, a_real_t *const set, a_real_t *const fdb)
+a_real_t const *a_fpid_outp(a_fpid_s *const ctx, a_real_t const *const set, a_real_t const *const fdb)
 {
     a_uint_t const col = a_fpid_col(ctx);
     a_uint_t const num = a_pid_num(&ctx->pid);
     a_uint_t const mode = a_pid_mode(&ctx->pid);
     for (a_uint_t i = 0; i != num; ++i)
     {
         a_real_t const e = set[i] - fdb[i];
```

### Comparing `liba-0.1.1rc5/src/fuzzy.c` & `liba-0.1.1rc6/src/fuzzy.c`

 * *Files 2% similar despite different names*

```diff
@@ -27,10 +27,9 @@
     default:
         return a_real_min(l, r);
     }
 }
 
 a_real_t a_fuzzy_equ(a_real_t const gamma, a_real_t const l, a_real_t const r)
 {
-    return a_real_pow(l * r, 1 - gamma) *
-           a_real_pow(1 - (1 - l) * (1 - r), gamma);
+    return a_real_pow(l * r, 1 - gamma) * a_real_pow(1 - (1 - l) * (1 - r), gamma);
 }
```

### Comparing `liba-0.1.1rc5/src/host/a.c` & `liba-0.1.1rc6/src/host/a.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/host/que.c` & `liba-0.1.1rc6/src/host/que.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/host/str.c` & `liba-0.1.1rc6/src/host/str.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/host/vec.c` & `liba-0.1.1rc6/src/host/vec.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/host/vector.c` & `liba-0.1.1rc6/src/host/vector.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/math.c` & `liba-0.1.1rc6/src/math.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/mf.c` & `liba-0.1.1rc6/src/mf.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/pid.c` & `liba-0.1.1rc6/src/pid.c`

 * *Files 10% similar despite different names*

```diff
@@ -86,125 +86,109 @@
             ctx->fdb.p[i] = 0;
             ctx->ec.p[i] = 0;
             ctx->e.p[i] = 0;
         }
     }
     else
     {
-        ctx->out.v = 0;
-        ctx->sum.v = 0;
-        ctx->fdb.v = 0;
-        ctx->ec.v = 0;
-        ctx->e.v = 0;
+        ctx->out.f = 0;
+        ctx->sum.f = 0;
+        ctx->fdb.f = 0;
+        ctx->ec.f = 0;
+        ctx->e.f = 0;
     }
     return ctx;
 }
 
-a_real_t a_pid_outv_(a_pid_s *const ctx, a_uint_t const mode, a_real_t const set, a_real_t const fdb, a_real_t const ec, a_real_t const e)
+a_real_t a_pid_outf_(a_pid_s *const ctx, a_uint_t const mode, a_real_t const set, a_real_t const fdb, a_real_t const ec, a_real_t const e)
 {
     /* calculation */
     switch (mode)
     {
     case A_PID_INC:
     {
-        /* K_p[e(k)-e(k-1)]+K_i e(k)+K_d[ec(k)-ec(k-1)] */
-        ctx->sum.v += ctx->kp * ec + ctx->ki * e + ctx->kd * (ec - ctx->ec.v);
-        ctx->out.v = ctx->sum.v;
+        /* K_p[e(k)-e(k-1)]+K_i[e(k)]+K_d[ec(k)-ec(k-1)] */
+        ctx->sum.f += ctx->kp * ec + ctx->ki * e + ctx->kd * (ec - ctx->ec.f);
+        ctx->out.f = ctx->sum.f;
         break;
     }
     case A_PID_POS:
     {
         a_real_t const sum = ctx->ki * e;
         /* when the limit of integration is exceeded or */
         /* the direction of integration is the same, the integration stops. */
-        if ((-ctx->summax < ctx->sum.v && ctx->sum.v < ctx->summax) || ctx->sum.v * sum < 0)
+        if ((-ctx->summax < ctx->sum.f && ctx->sum.f < ctx->summax) || ctx->sum.f * sum < 0)
         {
-            /* sum = K_i \sum^k_{i=0} e(i) */
-            ctx->sum.v += sum;
+            /* sum = K_i[\sum^k_{i=0}e(i)] */
+            ctx->sum.f += sum;
         }
         /* avoid derivative kick, fdb[k-1]-fdb[k] */
-        /* out = K_p e(k) + sum + K_d [fdb(k-1)-fdb(k)] */
-        ctx->out.v = ctx->kp * e + ctx->sum.v + ctx->kd * (ctx->fdb.v - fdb);
+        /* out = K_p[e(k)]+sum+K_d[fdb(k-1)-fdb(k)] */
+        ctx->out.f = ctx->kp * e + ctx->sum.f + ctx->kd * (ctx->fdb.f - fdb);
         break;
     }
     case A_PID_OFF:
     default:
-        ctx->out.v = ctx->sum.v = set;
-    }
-    /* output limiter */
-    if (ctx->outmax < ctx->out.v)
-    {
-        ctx->out.v = ctx->outmax;
-    }
-    else if (ctx->out.v < ctx->outmin)
-    {
-        ctx->out.v = ctx->outmin;
+        ctx->out.f = ctx->sum.f = set;
     }
+    ctx->out.f = A_SAT(ctx->out.f, ctx->outmin, ctx->outmax);
     /* cache data */
-    ctx->fdb.v = fdb;
-    ctx->ec.v = ec;
-    ctx->e.v = e;
-    return ctx->out.v;
+    ctx->fdb.f = fdb;
+    ctx->ec.f = ec;
+    ctx->e.f = e;
+    return ctx->out.f;
 }
 
 a_real_t a_pid_outp_(a_pid_s *const ctx, a_uint_t const mode, a_real_t const set, a_real_t const fdb, a_real_t const ec, a_real_t const e, a_uint_t const i)
 {
     /* calculation */
     switch (mode)
     {
     case A_PID_INC:
     {
-        /* K_p[e(k)-e(k-1)]+K_i e(k)+K_d[ec(k)-ec(k-1)] */
+        /* K_p[e(k)-e(k-1)]+K_i[e(k)]+K_d[ec(k)-ec(k-1)] */
         ctx->sum.p[i] += ctx->kp * ec + ctx->ki * e + ctx->kd * (ec - ctx->ec.p[i]);
         ctx->out.p[i] = ctx->sum.p[i];
         break;
     }
     case A_PID_POS:
     {
         a_real_t const sum = ctx->ki * e;
         /* when the limit of integration is exceeded or */
         /* the direction of integration is the same, the integration stops. */
         if ((-ctx->summax < ctx->sum.p[i] && ctx->sum.p[i] < ctx->summax) || ctx->sum.p[i] * sum < 0)
         {
-            /* sum = K_i \sum^k_{i=0} e(i) */
+            /* sum = K_i[\sum^k_{i=0}e(i)] */
             ctx->sum.p[i] += sum;
         }
         /* avoid derivative kick, fdb[k-1]-fdb[k] */
-        /* out = K_p e(k) + sum + K_d [fdb(k-1)-fdb(k)] */
+        /* out = K_p[e(k)]+sum+K_d[fdb(k-1)-fdb(k)] */
         ctx->out.p[i] = ctx->kp * e + ctx->sum.p[i] + ctx->kd * (ctx->fdb.p[i] - fdb);
         break;
     }
     case A_PID_OFF:
     default:
         ctx->out.p[i] = ctx->sum.p[i] = set;
     }
-    /* output limiter */
-    if (ctx->outmax < ctx->out.p[i])
-    {
-        ctx->out.p[i] = ctx->outmax;
-    }
-    else if (ctx->out.p[i] < ctx->outmin)
-    {
-        ctx->out.p[i] = ctx->outmin;
-    }
+    ctx->out.p[i] = A_SAT(ctx->out.p[i], ctx->outmin, ctx->outmax);
     /* cache data */
     ctx->fdb.p[i] = fdb;
     ctx->ec.p[i] = ec;
     ctx->e.p[i] = e;
     return ctx->out.p[i];
 }
 
-a_real_t a_pid_outv(a_pid_s *const ctx, a_real_t const set, a_real_t const fdb)
+a_real_t a_pid_outf(a_pid_s *const ctx, a_real_t const set, a_real_t const fdb)
 {
     a_real_t const e = set - fdb;
-    a_real_t const ec = e - ctx->e.v;
-    return a_pid_outv_(ctx, a_pid_mode(ctx), set, fdb, ec, e);
+    a_real_t const ec = e - ctx->e.f;
+    return a_pid_outf_(ctx, a_pid_mode(ctx), set, fdb, ec, e);
 }
 
-a_real_t *a_pid_outp(a_pid_s *const ctx, a_real_t *const set, a_real_t *const fdb)
+a_real_t const *a_pid_outp(a_pid_s *const ctx, a_real_t const *const set, a_real_t const *const fdb)
 {
     a_uint_t const num = a_pid_num(ctx);
     a_uint_t const mode = a_pid_mode(ctx);
     for (a_uint_t i = 0; i != num; ++i)
     {
         a_real_t const e = set[i] - fdb[i];
         a_real_t const ec = e - ctx->e.p[i];
```

### Comparing `liba-0.1.1rc5/src/poly.c` & `liba-0.1.1rc6/src/poly.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/rbt.c` & `liba-0.1.1rc6/src/rbt.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/real.c` & `liba-0.1.1rc6/src/real.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/tf.c` & `liba-0.1.1rc6/src/tf.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.1rc5/src/utf.c` & `liba-0.1.1rc6/src/utf.c`

 * *Files 4% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     if (val)
     {
         *val = res;
     }
     return offset + 1;
 }
 
-a_size_t a_utf_len(a_cptr_t const _str)
+a_size_t a_utf_length(a_cptr_t const _str)
 {
     a_size_t length = 0;
     a_cstr_t str = a_cstr_c(_str);
     for (a_uint_t offset; (void)(offset = a_utf_decode(str, A_NULL)), offset; str += offset)
     {
         ++length;
     }
```

### Comparing `liba-0.1.1rc5/src/version.c` & `liba-0.1.1rc6/src/version.c`

 * *Files identical despite different names*

