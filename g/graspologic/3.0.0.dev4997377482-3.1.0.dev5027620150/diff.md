# Comparing `tmp/graspologic-3.0.0.dev4997377482.tar.gz` & `tmp/graspologic-3.1.0.dev5027620150.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graspologic-3.0.0.dev4997377482.tar", last modified: Tue May 16 23:08:01 2023, max compression
+gzip compressed data, was "graspologic-3.1.0.dev5027620150.tar", last modified: Fri May 19 19:47:44 2023, max compression
```

## Comparing `graspologic-3.0.0.dev4997377482.tar` & `graspologic-3.1.0.dev5027620150.tar`

### file list

```diff
@@ -1,217 +1,217 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.613437 graspologic-3.0.0.dev4997377482/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-16 23:08:01.613437 graspologic-3.0.0.dev4997377482/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.565435 graspologic-3.0.0.dev4997377482/graspologic/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.565435 graspologic-3.0.0.dev4997377482/graspologic/align/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/align/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/align/orthogonal_procrustes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/align/seedless_procrustes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/align/sign_flips.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.569435 graspologic-3.0.0.dev4997377482/graspologic/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29918 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/cluster/autogmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/cluster/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/cluster/divisive_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/cluster/gclust.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/cluster/kclust.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.569435 graspologic-3.0.0.dev4997377482/graspologic/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.569435 graspologic-3.0.0.dev4997377482/graspologic/datasets/drosophila/
--rw-r--r--   0 runner    (1001) docker     (123)    87769 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/drosophila/left_adjacency.csv
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/drosophila/left_cell_labels.csv
--rw-r--r--   0 runner    (1001) docker     (123)    91164 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/drosophila/right_adjacency.csv
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/drosophila/right_cell_labels.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.569435 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/
--rw-r--r--   0 runner    (1001) docker     (123)    19847 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/atlas.csv
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/blocks.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.593436 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/
--rw-r--r--   0 runner    (1001) docker     (123)   465335 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   417268 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   481030 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   513067 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   486685 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   502512 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   501644 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   490182 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   423952 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   410522 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   418663 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   426113 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   459110 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   456778 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   500977 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   429240 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   412281 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   486497 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   466098 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   469626 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   431457 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   408031 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   450727 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   343162 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   451278 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   496115 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   493788 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   481678 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   479782 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   416610 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   363031 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist
--rw-r--r--   0 runner    (1001) docker     (123)   474339 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.601436 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/
--rwxr-xr-x   0 runner    (1001) docker     (123)    33536 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54776.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33530 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54777.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33537 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54779.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33535 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54781.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33544 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54790.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54793.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33549 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54794.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33555 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54797.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33519 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54811.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33525 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54813.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33530 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54815.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33528 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54817.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33501 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54821.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33510 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54823.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33536 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54829.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33538 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54831.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33530 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54833.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33535 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54835.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33505 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54842.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33508 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54847.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33520 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54849.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33520 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54851.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33525 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54853.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33527 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54855.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54864.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54866.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54868.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33552 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54870.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33508 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54883.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33514 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54885.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33509 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54887.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    33496 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54890.csv
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/participants.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.601436 graspologic-3.0.0.dev4997377482/graspologic/embed/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/embed/ase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/embed/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/embed/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/embed/lse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/embed/mase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/embed/mds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/embed/mug2vec.py
--rw-r--r--   0 runner    (1001) docker     (123)    19443 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/embed/n2v.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/embed/omni.py
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/embed/svd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.605437 graspologic-3.0.0.dev4997377482/graspologic/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/inference/binomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/inference/density_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/inference/group_connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/inference/latent_distribution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/inference/latent_position_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/inference/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.605437 graspologic-3.0.0.dev4997377482/graspologic/layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/layouts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/layouts/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/layouts/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/layouts/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.605437 graspologic-3.0.0.dev4997377482/graspologic/layouts/include/
--rw-r--r--   0 runner    (1001) docker     (123)    28486 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/layouts/include/colors-100.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.605437 graspologic-3.0.0.dev4997377482/graspologic/layouts/nooverlap/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/layouts/nooverlap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/layouts/nooverlap/_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/layouts/nooverlap/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    42453 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/layouts/nooverlap/_quad_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/layouts/nooverlap/_quad_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/layouts/nooverlap/nooverlap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/layouts/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.605437 graspologic-3.0.0.dev4997377482/graspologic/match/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/match/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/match/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/match/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/match/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.609437 graspologic-3.0.0.dev4997377482/graspologic/models/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/models/edge_swaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/models/er.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/models/rdpg.py
--rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/models/sbm_estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.609437 graspologic-3.0.0.dev4997377482/graspologic/nominate/
--rw-r--r--   0 runner    (1001) docker     (123)    16972 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/nominate/VNviaSGM.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/nominate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/nominate/spectralVN.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.609437 graspologic-3.0.0.dev4997377482/graspologic/partition/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/partition/leiden.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/partition/modularity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.609437 graspologic-3.0.0.dev4997377482/graspologic/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.609437 graspologic-3.0.0.dev4997377482/graspologic/pipeline/embed/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/pipeline/embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/pipeline/embed/_elbow.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/pipeline/embed/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/pipeline/embed/adjacency_spectral_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/pipeline/embed/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/pipeline/embed/laplacian_spectral_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/pipeline/embed/omnibus_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/pipeline/graph_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.609437 graspologic-3.0.0.dev4997377482/graspologic/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63595 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    34796 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/plot/plot_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/preconditions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.609437 graspologic-3.0.0.dev4997377482/graspologic/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/preprocessing/graph_cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.609437 graspologic-3.0.0.dev4997377482/graspologic/simulations/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/simulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/simulations/rdpg_corr.py
--rw-r--r--   0 runner    (1001) docker     (123)    38533 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/simulations/simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/simulations/simulations_corr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.609437 graspologic-3.0.0.dev4997377482/graspologic/subgraph/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/subgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/subgraph/sg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.613437 graspologic-3.0.0.dev4997377482/graspologic/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/utils/ptr.py
--rw-r--r--   0 runner    (1001) docker     (123)    40473 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/graspologic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.565435 graspologic-3.0.0.dev4997377482/graspologic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-16 23:08:01.000000 graspologic-3.0.0.dev4997377482/graspologic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-05-16 23:08:01.000000 graspologic-3.0.0.dev4997377482/graspologic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 23:08:01.000000 graspologic-3.0.0.dev4997377482/graspologic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-16 23:08:01.000000 graspologic-3.0.0.dev4997377482/graspologic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 23:08:01.000000 graspologic-3.0.0.dev4997377482/graspologic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-16 23:08:01.613437 graspologic-3.0.0.dev4997377482/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.561434 graspologic-3.0.0.dev4997377482/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.613437 graspologic-3.0.0.dev4997377482/tests/embed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/tests/embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/tests/embed/test_n2v.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/tests/embed/test_omni.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.613437 graspologic-3.0.0.dev4997377482/tests/layouts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/tests/layouts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.613437 graspologic-3.0.0.dev4997377482/tests/layouts/nooverlap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/tests/layouts/nooverlap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/tests/layouts/nooverlap/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/tests/layouts/nooverlap/test_grid_cell_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/tests/layouts/nooverlap/test_nooverlap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/tests/layouts/nooverlap/test_overlap_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/tests/layouts/test_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.613437 graspologic-3.0.0.dev4997377482/tests/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/tests/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/tests/pipeline/test_graph_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:08:01.613437 graspologic-3.0.0.dev4997377482/tests/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/tests/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-16 23:06:52.000000 graspologic-3.0.0.dev4997377482/tests/preprocessing/graph_cuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.134748 graspologic-3.1.0.dev5027620150/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-19 19:47:44.134748 graspologic-3.1.0.dev5027620150/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.070748 graspologic-3.1.0.dev5027620150/graspologic/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.070748 graspologic-3.1.0.dev5027620150/graspologic/align/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/align/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/align/orthogonal_procrustes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/align/seedless_procrustes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/align/sign_flips.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.074748 graspologic-3.1.0.dev5027620150/graspologic/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29918 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/cluster/autogmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/cluster/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/cluster/divisive_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/cluster/gclust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/cluster/kclust.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.074748 graspologic-3.1.0.dev5027620150/graspologic/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.074748 graspologic-3.1.0.dev5027620150/graspologic/datasets/drosophila/
+-rw-r--r--   0 runner    (1001) docker     (123)    87769 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/drosophila/left_adjacency.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/drosophila/left_cell_labels.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    91164 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/drosophila/right_adjacency.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/drosophila/right_cell_labels.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.074748 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/
+-rw-r--r--   0 runner    (1001) docker     (123)    19847 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/atlas.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/blocks.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.098748 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/
+-rw-r--r--   0 runner    (1001) docker     (123)   465335 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   417268 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   481030 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   513067 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   486685 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   502512 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   501644 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   490182 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   423952 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   410522 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   418663 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   426113 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   459110 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   456778 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   500977 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   429240 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   412281 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   486497 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   466098 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   469626 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   431457 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   408031 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   450727 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   343162 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   451278 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   496115 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   493788 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   481678 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   479782 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   416610 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   363031 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist
+-rw-r--r--   0 runner    (1001) docker     (123)   474339 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.110748 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33536 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54776.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33530 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54777.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33537 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54779.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33535 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54781.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33544 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54790.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54793.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33549 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54794.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33555 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54797.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33519 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54811.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33525 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54813.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33530 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54815.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33528 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54817.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33501 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54821.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33510 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54823.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33536 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54829.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33538 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54831.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33530 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54833.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33535 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54835.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33505 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54842.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33508 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54847.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33520 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54849.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33520 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54851.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33525 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54853.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33527 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54855.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54864.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54866.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33551 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54868.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33552 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54870.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33508 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54883.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33514 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54885.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33509 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54887.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33496 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54890.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/participants.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.114748 graspologic-3.1.0.dev5027620150/graspologic/embed/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/embed/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/embed/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/embed/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/embed/lse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/embed/mase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/embed/mds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/embed/mug2vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19443 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/embed/n2v.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/embed/omni.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/embed/svd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.114748 graspologic-3.1.0.dev5027620150/graspologic/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/inference/binomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/inference/density_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/inference/group_connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/inference/latent_distribution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/inference/latent_position_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/inference/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.118748 graspologic-3.1.0.dev5027620150/graspologic/layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/layouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/layouts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/layouts/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/layouts/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/layouts/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.118748 graspologic-3.1.0.dev5027620150/graspologic/layouts/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    28486 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/layouts/include/colors-100.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.118748 graspologic-3.1.0.dev5027620150/graspologic/layouts/nooverlap/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/layouts/nooverlap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/layouts/nooverlap/_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/layouts/nooverlap/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42453 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/layouts/nooverlap/_quad_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/layouts/nooverlap/_quad_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/layouts/nooverlap/nooverlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/layouts/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.122748 graspologic-3.1.0.dev5027620150/graspologic/match/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/match/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/match/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/match/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/match/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.122748 graspologic-3.1.0.dev5027620150/graspologic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/models/edge_swaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/models/er.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/models/rdpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/models/sbm_estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.126748 graspologic-3.1.0.dev5027620150/graspologic/nominate/
+-rw-r--r--   0 runner    (1001) docker     (123)    16972 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/nominate/VNviaSGM.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/nominate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/nominate/spectralVN.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.126748 graspologic-3.1.0.dev5027620150/graspologic/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/partition/leiden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/partition/modularity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.126748 graspologic-3.1.0.dev5027620150/graspologic/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.126748 graspologic-3.1.0.dev5027620150/graspologic/pipeline/embed/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/pipeline/embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/pipeline/embed/_elbow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/pipeline/embed/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/pipeline/embed/adjacency_spectral_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/pipeline/embed/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/pipeline/embed/laplacian_spectral_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/pipeline/embed/omnibus_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/pipeline/graph_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.130748 graspologic-3.1.0.dev5027620150/graspologic/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63595 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34796 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/plot/plot_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/preconditions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.130748 graspologic-3.1.0.dev5027620150/graspologic/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/preprocessing/graph_cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.130748 graspologic-3.1.0.dev5027620150/graspologic/simulations/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/simulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/simulations/rdpg_corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38533 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/simulations/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/simulations/simulations_corr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.130748 graspologic-3.1.0.dev5027620150/graspologic/subgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/subgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/subgraph/sg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.130748 graspologic-3.1.0.dev5027620150/graspologic/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/utils/ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40473 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/graspologic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.070748 graspologic-3.1.0.dev5027620150/graspologic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-19 19:47:43.000000 graspologic-3.1.0.dev5027620150/graspologic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-05-19 19:47:44.000000 graspologic-3.1.0.dev5027620150/graspologic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:47:43.000000 graspologic-3.1.0.dev5027620150/graspologic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-19 19:47:43.000000 graspologic-3.1.0.dev5027620150/graspologic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-19 19:47:43.000000 graspologic-3.1.0.dev5027620150/graspologic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-19 19:47:44.138748 graspologic-3.1.0.dev5027620150/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.066748 graspologic-3.1.0.dev5027620150/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.134748 graspologic-3.1.0.dev5027620150/tests/embed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/tests/embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/tests/embed/test_n2v.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/tests/embed/test_omni.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.134748 graspologic-3.1.0.dev5027620150/tests/layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/tests/layouts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.134748 graspologic-3.1.0.dev5027620150/tests/layouts/nooverlap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/tests/layouts/nooverlap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/tests/layouts/nooverlap/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/tests/layouts/nooverlap/test_grid_cell_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/tests/layouts/nooverlap/test_nooverlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/tests/layouts/nooverlap/test_overlap_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/tests/layouts/test_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.134748 graspologic-3.1.0.dev5027620150/tests/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/tests/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/tests/pipeline/test_graph_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:47:44.134748 graspologic-3.1.0.dev5027620150/tests/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/tests/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-19 19:46:23.000000 graspologic-3.1.0.dev5027620150/tests/preprocessing/graph_cuts.py
```

### Comparing `graspologic-3.0.0.dev4997377482/LICENSE.txt` & `graspologic-3.1.0.dev5027620150/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/PKG-INFO` & `graspologic-3.1.0.dev5027620150/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graspologic
-Version: 3.0.0.dev4997377482
+Version: 3.1.0.dev5027620150
 Summary: A set of python modules for graph statistics
 Home-page: https://github.com/microsoft/graspologic
 Author: Eric Bridgeford, Jaewon Chung, Benjamin Pedigo, Bijan Varjavand
 Author-email: j1c@jhu.edu
 Maintainer: Dax Pryce
 Maintainer-email: daxpryce@microsoft.com
 License: MIT
```

### Comparing `graspologic-3.0.0.dev4997377482/README.md` & `graspologic-3.1.0.dev5027620150/README.md`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/__init__.py` & `graspologic-3.1.0.dev5027620150/graspologic/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/align/base.py` & `graspologic-3.1.0.dev5027620150/graspologic/align/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/align/orthogonal_procrustes.py` & `graspologic-3.1.0.dev5027620150/graspologic/align/orthogonal_procrustes.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/align/seedless_procrustes.py` & `graspologic-3.1.0.dev5027620150/graspologic/align/seedless_procrustes.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/align/sign_flips.py` & `graspologic-3.1.0.dev5027620150/graspologic/align/sign_flips.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/cluster/autogmm.py` & `graspologic-3.1.0.dev5027620150/graspologic/cluster/autogmm.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/cluster/base.py` & `graspologic-3.1.0.dev5027620150/graspologic/cluster/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/cluster/divisive_cluster.py` & `graspologic-3.1.0.dev5027620150/graspologic/cluster/divisive_cluster.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/cluster/gclust.py` & `graspologic-3.1.0.dev5027620150/graspologic/cluster/gclust.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/cluster/kclust.py` & `graspologic-3.1.0.dev5027620150/graspologic/cluster/kclust.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/base.py` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/drosophila/left_adjacency.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/drosophila/left_adjacency.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/drosophila/right_adjacency.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/drosophila/right_adjacency.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/atlas.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/atlas.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54776.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54776.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54777.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54777.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54779.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54779.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54781.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54781.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54790.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54790.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54793.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54793.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54794.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54794.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54797.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54797.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54811.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54811.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54813.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54813.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54815.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54815.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54817.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54817.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54821.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54821.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54823.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54823.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54829.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54829.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54831.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54831.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54833.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54833.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54835.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54835.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54842.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54842.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54847.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54847.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54849.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54849.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54851.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54851.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54853.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54853.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54855.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54855.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54864.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54864.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54866.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54866.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54868.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54868.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54870.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54870.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54883.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54883.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54885.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54885.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54887.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54887.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/features/54890.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/features/54890.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/datasets/mice/participants.csv` & `graspologic-3.1.0.dev5027620150/graspologic/datasets/mice/participants.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/embed/__init__.py` & `graspologic-3.1.0.dev5027620150/graspologic/embed/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/embed/ase.py` & `graspologic-3.1.0.dev5027620150/graspologic/embed/ase.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/embed/base.py` & `graspologic-3.1.0.dev5027620150/graspologic/embed/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/embed/case.py` & `graspologic-3.1.0.dev5027620150/graspologic/embed/case.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/embed/lse.py` & `graspologic-3.1.0.dev5027620150/graspologic/embed/lse.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/embed/mase.py` & `graspologic-3.1.0.dev5027620150/graspologic/embed/mase.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/embed/mds.py` & `graspologic-3.1.0.dev5027620150/graspologic/embed/mds.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/embed/mug2vec.py` & `graspologic-3.1.0.dev5027620150/graspologic/embed/mug2vec.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/embed/n2v.py` & `graspologic-3.1.0.dev5027620150/graspologic/embed/n2v.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/embed/omni.py` & `graspologic-3.1.0.dev5027620150/graspologic/embed/omni.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/embed/svd.py` & `graspologic-3.1.0.dev5027620150/graspologic/embed/svd.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/inference/binomial.py` & `graspologic-3.1.0.dev5027620150/graspologic/inference/binomial.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/inference/density_test.py` & `graspologic-3.1.0.dev5027620150/graspologic/inference/density_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/inference/group_connection_test.py` & `graspologic-3.1.0.dev5027620150/graspologic/inference/group_connection_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/inference/latent_distribution_test.py` & `graspologic-3.1.0.dev5027620150/graspologic/inference/latent_distribution_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/inference/latent_position_test.py` & `graspologic-3.1.0.dev5027620150/graspologic/inference/latent_position_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/inference/utils.py` & `graspologic-3.1.0.dev5027620150/graspologic/inference/utils.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/layouts/__main__.py` & `graspologic-3.1.0.dev5027620150/graspologic/layouts/__main__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/layouts/auto.py` & `graspologic-3.1.0.dev5027620150/graspologic/layouts/auto.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/layouts/colors.py` & `graspologic-3.1.0.dev5027620150/graspologic/layouts/colors.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/layouts/include/colors-100.json` & `graspologic-3.1.0.dev5027620150/graspologic/layouts/include/colors-100.json`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/layouts/nooverlap/_grid.py` & `graspologic-3.1.0.dev5027620150/graspologic/layouts/nooverlap/_grid.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/layouts/nooverlap/_node.py` & `graspologic-3.1.0.dev5027620150/graspologic/layouts/nooverlap/_node.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/layouts/nooverlap/_quad_node.py` & `graspologic-3.1.0.dev5027620150/graspologic/layouts/nooverlap/_quad_node.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/layouts/nooverlap/_quad_tree.py` & `graspologic-3.1.0.dev5027620150/graspologic/layouts/nooverlap/_quad_tree.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/layouts/nooverlap/nooverlap.py` & `graspologic-3.1.0.dev5027620150/graspologic/layouts/nooverlap/nooverlap.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/layouts/render.py` & `graspologic-3.1.0.dev5027620150/graspologic/layouts/render.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/match/solver.py` & `graspologic-3.1.0.dev5027620150/graspologic/match/solver.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/match/types.py` & `graspologic-3.1.0.dev5027620150/graspologic/match/types.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/match/wrappers.py` & `graspologic-3.1.0.dev5027620150/graspologic/match/wrappers.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/models/base.py` & `graspologic-3.1.0.dev5027620150/graspologic/models/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/models/edge_swaps.py` & `graspologic-3.1.0.dev5027620150/graspologic/models/edge_swaps.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/models/er.py` & `graspologic-3.1.0.dev5027620150/graspologic/models/er.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/models/rdpg.py` & `graspologic-3.1.0.dev5027620150/graspologic/models/rdpg.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/models/sbm_estimators.py` & `graspologic-3.1.0.dev5027620150/graspologic/models/sbm_estimators.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/nominate/VNviaSGM.py` & `graspologic-3.1.0.dev5027620150/graspologic/nominate/VNviaSGM.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/nominate/spectralVN.py` & `graspologic-3.1.0.dev5027620150/graspologic/nominate/spectralVN.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/partition/leiden.py` & `graspologic-3.1.0.dev5027620150/graspologic/partition/leiden.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/partition/modularity.py` & `graspologic-3.1.0.dev5027620150/graspologic/partition/modularity.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/pipeline/__init__.py` & `graspologic-3.1.0.dev5027620150/graspologic/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/pipeline/embed/__init__.py` & `graspologic-3.1.0.dev5027620150/graspologic/pipeline/embed/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/pipeline/embed/_elbow.py` & `graspologic-3.1.0.dev5027620150/graspologic/pipeline/embed/_elbow.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/pipeline/embed/adjacency_spectral_embedding.py` & `graspologic-3.1.0.dev5027620150/graspologic/pipeline/embed/adjacency_spectral_embedding.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/pipeline/embed/embeddings.py` & `graspologic-3.1.0.dev5027620150/graspologic/pipeline/embed/embeddings.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/pipeline/embed/laplacian_spectral_embedding.py` & `graspologic-3.1.0.dev5027620150/graspologic/pipeline/embed/laplacian_spectral_embedding.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/pipeline/embed/omnibus_embedding.py` & `graspologic-3.1.0.dev5027620150/graspologic/pipeline/embed/omnibus_embedding.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/pipeline/graph_builder.py` & `graspologic-3.1.0.dev5027620150/graspologic/pipeline/graph_builder.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/plot/__init__.py` & `graspologic-3.1.0.dev5027620150/graspologic/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/plot/plot.py` & `graspologic-3.1.0.dev5027620150/graspologic/plot/plot.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/plot/plot_matrix.py` & `graspologic-3.1.0.dev5027620150/graspologic/plot/plot_matrix.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/preconditions.py` & `graspologic-3.1.0.dev5027620150/graspologic/preconditions.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/preprocessing/__init__.py` & `graspologic-3.1.0.dev5027620150/graspologic/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/preprocessing/graph_cuts.py` & `graspologic-3.1.0.dev5027620150/graspologic/preprocessing/graph_cuts.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/simulations/rdpg_corr.py` & `graspologic-3.1.0.dev5027620150/graspologic/simulations/rdpg_corr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/simulations/simulations.py` & `graspologic-3.1.0.dev5027620150/graspologic/simulations/simulations.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/simulations/simulations_corr.py` & `graspologic-3.1.0.dev5027620150/graspologic/simulations/simulations_corr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/subgraph/sg.py` & `graspologic-3.1.0.dev5027620150/graspologic/subgraph/sg.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/types.py` & `graspologic-3.1.0.dev5027620150/graspologic/types.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/utils/__init__.py` & `graspologic-3.1.0.dev5027620150/graspologic/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/utils/ptr.py` & `graspologic-3.1.0.dev5027620150/graspologic/utils/ptr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/utils/utils.py` & `graspologic-3.1.0.dev5027620150/graspologic/utils/utils.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic/version.py` & `graspologic-3.1.0.dev5027620150/graspologic/version.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic.egg-info/PKG-INFO` & `graspologic-3.1.0.dev5027620150/graspologic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graspologic
-Version: 3.0.0.dev4997377482
+Version: 3.1.0.dev5027620150
 Summary: A set of python modules for graph statistics
 Home-page: https://github.com/microsoft/graspologic
 Author: Eric Bridgeford, Jaewon Chung, Benjamin Pedigo, Bijan Varjavand
 Author-email: j1c@jhu.edu
 Maintainer: Dax Pryce
 Maintainer-email: daxpryce@microsoft.com
 License: MIT
```

### Comparing `graspologic-3.0.0.dev4997377482/graspologic.egg-info/SOURCES.txt` & `graspologic-3.1.0.dev5027620150/graspologic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/graspologic.egg-info/requires.txt` & `graspologic-3.1.0.dev5027620150/graspologic.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/setup.cfg` & `graspologic-3.1.0.dev5027620150/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = graspologic
-version = 3.0.0
+version = 3.1.0
 description = A set of python modules for graph statistics
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Eric Bridgeford, Jaewon Chung, Benjamin Pedigo, Bijan Varjavand
 author_email = j1c@jhu.edu
 maintainer = Dax Pryce
 maintainer_email = daxpryce@microsoft.com
@@ -60,10 +60,10 @@
 	pytest-cov>=3.0.0
 	sphinx>=4.2.0
 	sphinxcontrib-rawfiles>=0.1.1
 	sphinx-rtd-theme>=1.0.0
 	testfixtures>=6.18.3
 
 [egg_info]
-tag_build = dev4997377482
+tag_build = dev5027620150
 tag_date = 0
```

### Comparing `graspologic-3.0.0.dev4997377482/tests/embed/test_n2v.py` & `graspologic-3.1.0.dev5027620150/tests/embed/test_n2v.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/tests/embed/test_omni.py` & `graspologic-3.1.0.dev5027620150/tests/embed/test_omni.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/tests/layouts/nooverlap/test_grid.py` & `graspologic-3.1.0.dev5027620150/tests/layouts/nooverlap/test_grid.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/tests/layouts/nooverlap/test_grid_cell_creation.py` & `graspologic-3.1.0.dev5027620150/tests/layouts/nooverlap/test_grid_cell_creation.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/tests/layouts/nooverlap/test_nooverlap.py` & `graspologic-3.1.0.dev5027620150/tests/layouts/nooverlap/test_nooverlap.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/tests/layouts/nooverlap/test_overlap_check.py` & `graspologic-3.1.0.dev5027620150/tests/layouts/nooverlap/test_overlap_check.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/tests/layouts/test_auto.py` & `graspologic-3.1.0.dev5027620150/tests/layouts/test_auto.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/tests/pipeline/test_graph_builder.py` & `graspologic-3.1.0.dev5027620150/tests/pipeline/test_graph_builder.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.0.0.dev4997377482/tests/preprocessing/graph_cuts.py` & `graspologic-3.1.0.dev5027620150/tests/preprocessing/graph_cuts.py`

 * *Files identical despite different names*

