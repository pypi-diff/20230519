# Comparing `tmp/pulumiverse_exoscale-0.47.0.tar.gz` & `tmp/pulumiverse_exoscale-0.48.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_exoscale-0.47.0.tar", last modified: Thu May  4 11:43:35 2023, max compression
+gzip compressed data, was "pulumiverse_exoscale-0.48.0.tar", last modified: Fri May 19 21:04:18 2023, max compression
```

## Comparing `pulumiverse_exoscale-0.47.0.tar` & `pulumiverse_exoscale-0.48.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:43:35.526572 pulumiverse_exoscale-0.47.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-04 11:43:35.526572 pulumiverse_exoscale-0.47.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:43:35.526572 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51270 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/anti_affinity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    59349 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    48316 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/compute_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:43:35.526572 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    40713 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    18856 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/elastic_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_anti_affinity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_instance_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_elastic_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_instance_pool_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_nlb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    19159 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_sks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    18631 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_sks_cluster_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_sks_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_sks_nodepool_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/iam_access_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    53079 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    37973 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/nic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/nlb.py
--rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/nlb_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    90177 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    16432 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/secondary_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    35942 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/security_group_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/security_group_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    39936 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/sks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/sks_kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    41557 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/sks_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/ssh_keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:43:35.526572 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:43:35.526572 pulumiverse_exoscale-0.47.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-04 11:43:35.000000 pulumiverse_exoscale-0.47.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:04:18.410469 pulumiverse_exoscale-0.48.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-19 21:04:18.410469 pulumiverse_exoscale-0.48.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:04:18.410469 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51270 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/anti_affinity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59349 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50320 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/compute_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:04:18.410469 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40713 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18856 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/elastic_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_anti_affinity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_instance_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_elastic_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_instance_pool_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_nlb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19159 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18631 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_cluster_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_nodepool_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/iam_access_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53079 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37973 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/nic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/nlb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/nlb_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90177 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16432 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/secondary_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39602 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/security_group_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/security_group_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39936 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/sks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/sks_kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41557 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/sks_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/ssh_keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:04:18.410469 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:04:18.410469 pulumiverse_exoscale-0.48.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-19 21:04:18.000000 pulumiverse_exoscale-0.48.0/setup.py
```

### Comparing `pulumiverse_exoscale-0.47.0/PKG-INFO` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumiverse_exoscale
-Version: 0.47.0
+Name: pulumiverse-exoscale
+Version: 0.48.0
 Summary: A Pulumi package for creating and managing exoscale cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-exoscale
 Keywords: pulumi exoscale category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_exoscale-0.47.0/README.md` & `pulumiverse_exoscale-0.48.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/__init__.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/_inputs.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/_utilities.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/affinity.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/affinity.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/anti_affinity_group.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/anti_affinity_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/compute.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/compute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/compute_instance.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/compute_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ipv6: Optional[pulumi.Input[bool]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_interfaces: Optional[pulumi.Input[Sequence[pulumi.Input['ComputeInstanceNetworkInterfaceArgs']]]] = None,
+                 private: Optional[pulumi.Input[bool]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ssh_key: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ComputeInstance resource.
@@ -44,14 +45,15 @@
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). **WARNING**: updating this attribute stops/restarts the instance.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The compute instance name.
         :param pulumi.Input[Sequence[pulumi.Input['ComputeInstanceNetworkInterfaceArgs']]] network_interfaces: Private network interfaces (may be specified multiple times). Structure is documented below.
+        :param pulumi.Input[bool] private: Whether the instance is private (no public IP addresses; default: false)
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
         :param pulumi.Input[str] ssh_key: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
         :param pulumi.Input[str] state: The instance state (`running` or `stopped`; default: `running`).
         :param pulumi.Input[str] user_data: [cloud-init](https://cloudinit.readthedocs.io/) configuration (no need to base64-encode or gzip it as the provider will
                take care of it).
         """
@@ -70,14 +72,16 @@
             pulumi.set(__self__, "ipv6", ipv6)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if network_interfaces is not None:
             pulumi.set(__self__, "network_interfaces", network_interfaces)
+        if private is not None:
+            pulumi.set(__self__, "private", private)
         if reverse_dns is not None:
             pulumi.set(__self__, "reverse_dns", reverse_dns)
         if security_group_ids is not None:
             pulumi.set(__self__, "security_group_ids", security_group_ids)
         if ssh_key is not None:
             pulumi.set(__self__, "ssh_key", ssh_key)
         if state is not None:
@@ -217,14 +221,26 @@
         return pulumi.get(self, "network_interfaces")
 
     @network_interfaces.setter
     def network_interfaces(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ComputeInstanceNetworkInterfaceArgs']]]]):
         pulumi.set(self, "network_interfaces", value)
 
     @property
+    @pulumi.getter
+    def private(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the instance is private (no public IP addresses; default: false)
+        """
+        return pulumi.get(self, "private")
+
+    @private.setter
+    def private(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "private", value)
+
+    @property
     @pulumi.getter(name="reverseDns")
     def reverse_dns(self) -> Optional[pulumi.Input[str]]:
         """
         Domain name for reverse DNS record.
         """
         return pulumi.get(self, "reverse_dns")
 
@@ -291,14 +307,15 @@
                  disk_size: Optional[pulumi.Input[int]] = None,
                  elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ipv6: Optional[pulumi.Input[bool]] = None,
                  ipv6_address: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_interfaces: Optional[pulumi.Input[Sequence[pulumi.Input['ComputeInstanceNetworkInterfaceArgs']]]] = None,
+                 private: Optional[pulumi.Input[bool]] = None,
                  private_network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  public_ip_address: Optional[pulumi.Input[str]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ssh_key: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  template_id: Optional[pulumi.Input[str]] = None,
@@ -314,14 +331,15 @@
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). **WARNING**: updating this attribute stops/restarts the instance.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[str] ipv6_address: The instance (main network interface) IPv6 address (if enabled).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The compute instance name.
         :param pulumi.Input[Sequence[pulumi.Input['ComputeInstanceNetworkInterfaceArgs']]] network_interfaces: Private network interfaces (may be specified multiple times). Structure is documented below.
+        :param pulumi.Input[bool] private: Whether the instance is private (no public IP addresses; default: false)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument
                instead.
         :param pulumi.Input[str] public_ip_address: The instance (main network interface) IPv4 address.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
         :param pulumi.Input[str] ssh_key: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
         :param pulumi.Input[str] state: The instance state (`running` or `stopped`; default: `running`).
@@ -349,14 +367,16 @@
             pulumi.set(__self__, "ipv6_address", ipv6_address)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if network_interfaces is not None:
             pulumi.set(__self__, "network_interfaces", network_interfaces)
+        if private is not None:
+            pulumi.set(__self__, "private", private)
         if private_network_ids is not None:
             warnings.warn("""Use the network_interface block instead.""", DeprecationWarning)
             pulumi.log.warn("""private_network_ids is deprecated: Use the network_interface block instead.""")
         if private_network_ids is not None:
             pulumi.set(__self__, "private_network_ids", private_network_ids)
         if public_ip_address is not None:
             pulumi.set(__self__, "public_ip_address", public_ip_address)
@@ -495,14 +515,26 @@
         return pulumi.get(self, "network_interfaces")
 
     @network_interfaces.setter
     def network_interfaces(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ComputeInstanceNetworkInterfaceArgs']]]]):
         pulumi.set(self, "network_interfaces", value)
 
     @property
+    @pulumi.getter
+    def private(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the instance is private (no public IP addresses; default: false)
+        """
+        return pulumi.get(self, "private")
+
+    @private.setter
+    def private(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "private", value)
+
+    @property
     @pulumi.getter(name="privateNetworkIds")
     def private_network_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument
         instead.
         """
         return pulumi.get(self, "private_network_ids")
@@ -632,14 +664,15 @@
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ipv6: Optional[pulumi.Input[bool]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_interfaces: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ComputeInstanceNetworkInterfaceArgs']]]]] = None,
+                 private: Optional[pulumi.Input[bool]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ssh_key: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  template_id: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
@@ -665,14 +698,15 @@
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). **WARNING**: updating this attribute stops/restarts the instance.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The compute instance name.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ComputeInstanceNetworkInterfaceArgs']]]] network_interfaces: Private network interfaces (may be specified multiple times). Structure is documented below.
+        :param pulumi.Input[bool] private: Whether the instance is private (no public IP addresses; default: false)
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
         :param pulumi.Input[str] ssh_key: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
         :param pulumi.Input[str] state: The instance state (`running` or `stopped`; default: `running`).
         :param pulumi.Input[str] template_id: The [exoscale_compute_template](../data-sources/compute_template.md) (ID) to use when creating the instance.
         :param pulumi.Input[str] type: The instance type (`<family>.<size>`, e.g. `standard.medium`; use the [Exoscale CLI](https://github.com/exoscale/cli/) -
                `exo compute instance-type list` - for the list of available types). **WARNING**: updating this attribute stops/restarts
@@ -719,14 +753,15 @@
                  deploy_target_id: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ipv6: Optional[pulumi.Input[bool]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_interfaces: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ComputeInstanceNetworkInterfaceArgs']]]]] = None,
+                 private: Optional[pulumi.Input[bool]] = None,
                  reverse_dns: Optional[pulumi.Input[str]] = None,
                  security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  ssh_key: Optional[pulumi.Input[str]] = None,
                  state: Optional[pulumi.Input[str]] = None,
                  template_id: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
@@ -744,14 +779,15 @@
             __props__.__dict__["deploy_target_id"] = deploy_target_id
             __props__.__dict__["disk_size"] = disk_size
             __props__.__dict__["elastic_ip_ids"] = elastic_ip_ids
             __props__.__dict__["ipv6"] = ipv6
             __props__.__dict__["labels"] = labels
             __props__.__dict__["name"] = name
             __props__.__dict__["network_interfaces"] = network_interfaces
+            __props__.__dict__["private"] = private
             __props__.__dict__["reverse_dns"] = reverse_dns
             __props__.__dict__["security_group_ids"] = security_group_ids
             __props__.__dict__["ssh_key"] = ssh_key
             __props__.__dict__["state"] = state
             if template_id is None and not opts.urn:
                 raise TypeError("Missing required property 'template_id'")
             __props__.__dict__["template_id"] = template_id
@@ -782,14 +818,15 @@
             disk_size: Optional[pulumi.Input[int]] = None,
             elastic_ip_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             ipv6: Optional[pulumi.Input[bool]] = None,
             ipv6_address: Optional[pulumi.Input[str]] = None,
             labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             network_interfaces: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ComputeInstanceNetworkInterfaceArgs']]]]] = None,
+            private: Optional[pulumi.Input[bool]] = None,
             private_network_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             public_ip_address: Optional[pulumi.Input[str]] = None,
             reverse_dns: Optional[pulumi.Input[str]] = None,
             security_group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             ssh_key: Optional[pulumi.Input[str]] = None,
             state: Optional[pulumi.Input[str]] = None,
             template_id: Optional[pulumi.Input[str]] = None,
@@ -810,14 +847,15 @@
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). **WARNING**: updating this attribute stops/restarts the instance.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elastic_ip_ids: A list of [exoscale_elastic_ip](./elastic_ip.md) (IDs) to attach to the instance.
         :param pulumi.Input[bool] ipv6: Enable IPv6 on the instance (boolean; default: `false`).
         :param pulumi.Input[str] ipv6_address: The instance (main network interface) IPv6 address (if enabled).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The compute instance name.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ComputeInstanceNetworkInterfaceArgs']]]] network_interfaces: Private network interfaces (may be specified multiple times). Structure is documented below.
+        :param pulumi.Input[bool] private: Whether the instance is private (no public IP addresses; default: false)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] private_network_ids: A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument
                instead.
         :param pulumi.Input[str] public_ip_address: The instance (main network interface) IPv4 address.
         :param pulumi.Input[str] reverse_dns: Domain name for reverse DNS record.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] security_group_ids: A list of [exoscale_security_group](./security_group.md) (IDs) to attach to the instance.
         :param pulumi.Input[str] ssh_key: The [exoscale_ssh_key](./ssh_key.md) (name) to authorize in the instance (may only be set at creation time).
         :param pulumi.Input[str] state: The instance state (`running` or `stopped`; default: `running`).
@@ -839,14 +877,15 @@
         __props__.__dict__["disk_size"] = disk_size
         __props__.__dict__["elastic_ip_ids"] = elastic_ip_ids
         __props__.__dict__["ipv6"] = ipv6
         __props__.__dict__["ipv6_address"] = ipv6_address
         __props__.__dict__["labels"] = labels
         __props__.__dict__["name"] = name
         __props__.__dict__["network_interfaces"] = network_interfaces
+        __props__.__dict__["private"] = private
         __props__.__dict__["private_network_ids"] = private_network_ids
         __props__.__dict__["public_ip_address"] = public_ip_address
         __props__.__dict__["reverse_dns"] = reverse_dns
         __props__.__dict__["security_group_ids"] = security_group_ids
         __props__.__dict__["ssh_key"] = ssh_key
         __props__.__dict__["state"] = state
         __props__.__dict__["template_id"] = template_id
@@ -933,14 +972,22 @@
     def network_interfaces(self) -> pulumi.Output[Optional[Sequence['outputs.ComputeInstanceNetworkInterface']]]:
         """
         Private network interfaces (may be specified multiple times). Structure is documented below.
         """
         return pulumi.get(self, "network_interfaces")
 
     @property
+    @pulumi.getter
+    def private(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Whether the instance is private (no public IP addresses; default: false)
+        """
+        return pulumi.get(self, "private")
+
+    @property
     @pulumi.getter(name="privateNetworkIds")
     def private_network_ids(self) -> pulumi.Output[Sequence[str]]:
         """
         A list of private networks (IDs) attached to the instance. Please use the `network_interface.*.network_id` argument
         instead.
         """
         return pulumi.get(self, "private_network_ids")
```

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/config/vars.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/database.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/database.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/domain.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/domain.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/domain_record.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/elastic_ip.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/elastic_ip.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_affinity.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_affinity.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_anti_affinity_group.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_anti_affinity_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_instance.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_instance.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_instance_list.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_instance_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_ip_address.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_compute_template.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_compute_template.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_domain.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_domain_record.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_elastic_ip.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_elastic_ip.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_instance_pool.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_instance_pool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_instance_pool_list.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_instance_pool_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_network.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_nlb.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_nlb.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_private_network.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_private_network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_security_group.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_sks_cluster.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_sks_cluster_list.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_cluster_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_sks_nodepool.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_nodepool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_sks_nodepool_list.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_sks_nodepool_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/get_template.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/get_template.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/iam_access_key.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/iam_access_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/instance_pool.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/instance_pool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/ip_address.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/network.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/nic.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/nic.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/nlb.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/nlb.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/nlb_service.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/nlb_service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/outputs.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/private_network.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/private_network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/provider.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/secondary_ip_address.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/secondary_ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/security_group.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/security_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/security_group_rule.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/security_group_rule.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,53 +17,58 @@
                  type: pulumi.Input[str],
                  cidr: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  end_port: Optional[pulumi.Input[int]] = None,
                  icmp_code: Optional[pulumi.Input[int]] = None,
                  icmp_type: Optional[pulumi.Input[int]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
+                 public_security_group: Optional[pulumi.Input[str]] = None,
                  security_group: Optional[pulumi.Input[str]] = None,
                  security_group_id: Optional[pulumi.Input[str]] = None,
                  start_port: Optional[pulumi.Input[int]] = None,
                  user_security_group: Optional[pulumi.Input[str]] = None,
                  user_security_group_id: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SecurityGroupRule resource.
         :param pulumi.Input[str] type: The traffic direction to match (`INGRESS` or `EGRESS`).
         :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
                notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
-               `user_security_group`/`user_security_group_id`).
+               `public_security_group`/`user_security_group`/`user_security_group_id`).
         :param pulumi.Input[str] description: A free-form text describing the security group rule.
         :param pulumi.Input[int] end_port: A `TCP`/`UDP` port range to match.
         :param pulumi.Input[int] icmp_code: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         :param pulumi.Input[int] icmp_type: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         :param pulumi.Input[str] protocol: The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
+        :param pulumi.Input[str] public_security_group: An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with
+               `cidr`/`user_security_group`/`user_security_group_id`).
         :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the
                [exoscale_security_group](../data-sources/security_group.md) data source instead.
         :param pulumi.Input[str] security_group_id: The parent [exoscale_security_group](./security_group.md) ID.
         :param pulumi.Input[int] start_port: A `TCP`/`UDP` port range to match.
         :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
-               `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
+               `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
                [exoscale_security_group](../data-sources/security_group.md) data source instead.
         :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
-               `cidr`/`user_security_group)`).
+               `cidr`/`public_security_group`/`user_security_group)`).
         """
         pulumi.set(__self__, "type", type)
         if cidr is not None:
             pulumi.set(__self__, "cidr", cidr)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if end_port is not None:
             pulumi.set(__self__, "end_port", end_port)
         if icmp_code is not None:
             pulumi.set(__self__, "icmp_code", icmp_code)
         if icmp_type is not None:
             pulumi.set(__self__, "icmp_type", icmp_type)
         if protocol is not None:
             pulumi.set(__self__, "protocol", protocol)
+        if public_security_group is not None:
+            pulumi.set(__self__, "public_security_group", public_security_group)
         if security_group is not None:
             warnings.warn("""Deprecated in favor of `security_group_id`""", DeprecationWarning)
             pulumi.log.warn("""security_group is deprecated: Deprecated in favor of `security_group_id`""")
         if security_group is not None:
             pulumi.set(__self__, "security_group", security_group)
         if security_group_id is not None:
             pulumi.set(__self__, "security_group_id", security_group_id)
@@ -91,15 +96,15 @@
 
     @property
     @pulumi.getter
     def cidr(self) -> Optional[pulumi.Input[str]]:
         """
         An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
         notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
-        `user_security_group`/`user_security_group_id`).
+        `public_security_group`/`user_security_group`/`user_security_group_id`).
         """
         return pulumi.get(self, "cidr")
 
     @cidr.setter
     def cidr(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cidr", value)
 
@@ -160,14 +165,27 @@
         return pulumi.get(self, "protocol")
 
     @protocol.setter
     def protocol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "protocol", value)
 
     @property
+    @pulumi.getter(name="publicSecurityGroup")
+    def public_security_group(self) -> Optional[pulumi.Input[str]]:
+        """
+        An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with
+        `cidr`/`user_security_group`/`user_security_group_id`).
+        """
+        return pulumi.get(self, "public_security_group")
+
+    @public_security_group.setter
+    def public_security_group(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "public_security_group", value)
+
+    @property
     @pulumi.getter(name="securityGroup")
     def security_group(self) -> Optional[pulumi.Input[str]]:
         """
         The parent security group name. Please use the `security_group_id` argument along the
         [exoscale_security_group](../data-sources/security_group.md) data source instead.
         """
         return pulumi.get(self, "security_group")
@@ -201,29 +219,29 @@
         pulumi.set(self, "start_port", value)
 
     @property
     @pulumi.getter(name="userSecurityGroup")
     def user_security_group(self) -> Optional[pulumi.Input[str]]:
         """
         An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
-        `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
+        `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
         [exoscale_security_group](../data-sources/security_group.md) data source instead.
         """
         return pulumi.get(self, "user_security_group")
 
     @user_security_group.setter
     def user_security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_security_group", value)
 
     @property
     @pulumi.getter(name="userSecurityGroupId")
     def user_security_group_id(self) -> Optional[pulumi.Input[str]]:
         """
         An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
-        `cidr`/`user_security_group)`).
+        `cidr`/`public_security_group`/`user_security_group)`).
         """
         return pulumi.get(self, "user_security_group_id")
 
     @user_security_group_id.setter
     def user_security_group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_security_group_id", value)
 
@@ -233,53 +251,58 @@
     def __init__(__self__, *,
                  cidr: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  end_port: Optional[pulumi.Input[int]] = None,
                  icmp_code: Optional[pulumi.Input[int]] = None,
                  icmp_type: Optional[pulumi.Input[int]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
+                 public_security_group: Optional[pulumi.Input[str]] = None,
                  security_group: Optional[pulumi.Input[str]] = None,
                  security_group_id: Optional[pulumi.Input[str]] = None,
                  start_port: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  user_security_group: Optional[pulumi.Input[str]] = None,
                  user_security_group_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SecurityGroupRule resources.
         :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
                notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
-               `user_security_group`/`user_security_group_id`).
+               `public_security_group`/`user_security_group`/`user_security_group_id`).
         :param pulumi.Input[str] description: A free-form text describing the security group rule.
         :param pulumi.Input[int] end_port: A `TCP`/`UDP` port range to match.
         :param pulumi.Input[int] icmp_code: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         :param pulumi.Input[int] icmp_type: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         :param pulumi.Input[str] protocol: The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
+        :param pulumi.Input[str] public_security_group: An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with
+               `cidr`/`user_security_group`/`user_security_group_id`).
         :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the
                [exoscale_security_group](../data-sources/security_group.md) data source instead.
         :param pulumi.Input[str] security_group_id: The parent [exoscale_security_group](./security_group.md) ID.
         :param pulumi.Input[int] start_port: A `TCP`/`UDP` port range to match.
         :param pulumi.Input[str] type: The traffic direction to match (`INGRESS` or `EGRESS`).
         :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
-               `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
+               `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
                [exoscale_security_group](../data-sources/security_group.md) data source instead.
         :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
-               `cidr`/`user_security_group)`).
+               `cidr`/`public_security_group`/`user_security_group)`).
         """
         if cidr is not None:
             pulumi.set(__self__, "cidr", cidr)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if end_port is not None:
             pulumi.set(__self__, "end_port", end_port)
         if icmp_code is not None:
             pulumi.set(__self__, "icmp_code", icmp_code)
         if icmp_type is not None:
             pulumi.set(__self__, "icmp_type", icmp_type)
         if protocol is not None:
             pulumi.set(__self__, "protocol", protocol)
+        if public_security_group is not None:
+            pulumi.set(__self__, "public_security_group", public_security_group)
         if security_group is not None:
             warnings.warn("""Deprecated in favor of `security_group_id`""", DeprecationWarning)
             pulumi.log.warn("""security_group is deprecated: Deprecated in favor of `security_group_id`""")
         if security_group is not None:
             pulumi.set(__self__, "security_group", security_group)
         if security_group_id is not None:
             pulumi.set(__self__, "security_group_id", security_group_id)
@@ -297,15 +320,15 @@
 
     @property
     @pulumi.getter
     def cidr(self) -> Optional[pulumi.Input[str]]:
         """
         An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
         notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
-        `user_security_group`/`user_security_group_id`).
+        `public_security_group`/`user_security_group`/`user_security_group_id`).
         """
         return pulumi.get(self, "cidr")
 
     @cidr.setter
     def cidr(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cidr", value)
 
@@ -366,14 +389,27 @@
         return pulumi.get(self, "protocol")
 
     @protocol.setter
     def protocol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "protocol", value)
 
     @property
+    @pulumi.getter(name="publicSecurityGroup")
+    def public_security_group(self) -> Optional[pulumi.Input[str]]:
+        """
+        An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with
+        `cidr`/`user_security_group`/`user_security_group_id`).
+        """
+        return pulumi.get(self, "public_security_group")
+
+    @public_security_group.setter
+    def public_security_group(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "public_security_group", value)
+
+    @property
     @pulumi.getter(name="securityGroup")
     def security_group(self) -> Optional[pulumi.Input[str]]:
         """
         The parent security group name. Please use the `security_group_id` argument along the
         [exoscale_security_group](../data-sources/security_group.md) data source instead.
         """
         return pulumi.get(self, "security_group")
@@ -419,29 +455,29 @@
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="userSecurityGroup")
     def user_security_group(self) -> Optional[pulumi.Input[str]]:
         """
         An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
-        `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
+        `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
         [exoscale_security_group](../data-sources/security_group.md) data source instead.
         """
         return pulumi.get(self, "user_security_group")
 
     @user_security_group.setter
     def user_security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_security_group", value)
 
     @property
     @pulumi.getter(name="userSecurityGroupId")
     def user_security_group_id(self) -> Optional[pulumi.Input[str]]:
         """
         An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
-        `cidr`/`user_security_group)`).
+        `cidr`/`public_security_group`/`user_security_group)`).
         """
         return pulumi.get(self, "user_security_group_id")
 
     @user_security_group_id.setter
     def user_security_group_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_security_group_id", value)
 
@@ -453,14 +489,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cidr: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  end_port: Optional[pulumi.Input[int]] = None,
                  icmp_code: Optional[pulumi.Input[int]] = None,
                  icmp_type: Optional[pulumi.Input[int]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
+                 public_security_group: Optional[pulumi.Input[str]] = None,
                  security_group: Optional[pulumi.Input[str]] = None,
                  security_group_id: Optional[pulumi.Input[str]] = None,
                  start_port: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  user_security_group: Optional[pulumi.Input[str]] = None,
                  user_security_group_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
@@ -477,30 +514,32 @@
 
          f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
                notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
-               `user_security_group`/`user_security_group_id`).
+               `public_security_group`/`user_security_group`/`user_security_group_id`).
         :param pulumi.Input[str] description: A free-form text describing the security group rule.
         :param pulumi.Input[int] end_port: A `TCP`/`UDP` port range to match.
         :param pulumi.Input[int] icmp_code: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         :param pulumi.Input[int] icmp_type: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         :param pulumi.Input[str] protocol: The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
+        :param pulumi.Input[str] public_security_group: An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with
+               `cidr`/`user_security_group`/`user_security_group_id`).
         :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the
                [exoscale_security_group](../data-sources/security_group.md) data source instead.
         :param pulumi.Input[str] security_group_id: The parent [exoscale_security_group](./security_group.md) ID.
         :param pulumi.Input[int] start_port: A `TCP`/`UDP` port range to match.
         :param pulumi.Input[str] type: The traffic direction to match (`INGRESS` or `EGRESS`).
         :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
-               `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
+               `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
                [exoscale_security_group](../data-sources/security_group.md) data source instead.
         :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
-               `cidr`/`user_security_group)`).
+               `cidr`/`public_security_group`/`user_security_group)`).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SecurityGroupRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -534,14 +573,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cidr: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  end_port: Optional[pulumi.Input[int]] = None,
                  icmp_code: Optional[pulumi.Input[int]] = None,
                  icmp_type: Optional[pulumi.Input[int]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
+                 public_security_group: Optional[pulumi.Input[str]] = None,
                  security_group: Optional[pulumi.Input[str]] = None,
                  security_group_id: Optional[pulumi.Input[str]] = None,
                  start_port: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  user_security_group: Optional[pulumi.Input[str]] = None,
                  user_security_group_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
@@ -555,14 +595,15 @@
 
             __props__.__dict__["cidr"] = cidr
             __props__.__dict__["description"] = description
             __props__.__dict__["end_port"] = end_port
             __props__.__dict__["icmp_code"] = icmp_code
             __props__.__dict__["icmp_type"] = icmp_type
             __props__.__dict__["protocol"] = protocol
+            __props__.__dict__["public_security_group"] = public_security_group
             if security_group is not None and not opts.urn:
                 warnings.warn("""Deprecated in favor of `security_group_id`""", DeprecationWarning)
                 pulumi.log.warn("""security_group is deprecated: Deprecated in favor of `security_group_id`""")
             __props__.__dict__["security_group"] = security_group
             __props__.__dict__["security_group_id"] = security_group_id
             __props__.__dict__["start_port"] = start_port
             if type is None and not opts.urn:
@@ -585,14 +626,15 @@
             opts: Optional[pulumi.ResourceOptions] = None,
             cidr: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             end_port: Optional[pulumi.Input[int]] = None,
             icmp_code: Optional[pulumi.Input[int]] = None,
             icmp_type: Optional[pulumi.Input[int]] = None,
             protocol: Optional[pulumi.Input[str]] = None,
+            public_security_group: Optional[pulumi.Input[str]] = None,
             security_group: Optional[pulumi.Input[str]] = None,
             security_group_id: Optional[pulumi.Input[str]] = None,
             start_port: Optional[pulumi.Input[int]] = None,
             type: Optional[pulumi.Input[str]] = None,
             user_security_group: Optional[pulumi.Input[str]] = None,
             user_security_group_id: Optional[pulumi.Input[str]] = None) -> 'SecurityGroupRule':
         """
@@ -600,56 +642,59 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cidr: An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
                notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
-               `user_security_group`/`user_security_group_id`).
+               `public_security_group`/`user_security_group`/`user_security_group_id`).
         :param pulumi.Input[str] description: A free-form text describing the security group rule.
         :param pulumi.Input[int] end_port: A `TCP`/`UDP` port range to match.
         :param pulumi.Input[int] icmp_code: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         :param pulumi.Input[int] icmp_type: An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
         :param pulumi.Input[str] protocol: The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
+        :param pulumi.Input[str] public_security_group: An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with
+               `cidr`/`user_security_group`/`user_security_group_id`).
         :param pulumi.Input[str] security_group: The parent security group name. Please use the `security_group_id` argument along the
                [exoscale_security_group](../data-sources/security_group.md) data source instead.
         :param pulumi.Input[str] security_group_id: The parent [exoscale_security_group](./security_group.md) ID.
         :param pulumi.Input[int] start_port: A `TCP`/`UDP` port range to match.
         :param pulumi.Input[str] type: The traffic direction to match (`INGRESS` or `EGRESS`).
         :param pulumi.Input[str] user_security_group: An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
-               `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
+               `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
                [exoscale_security_group](../data-sources/security_group.md) data source instead.
         :param pulumi.Input[str] user_security_group_id: An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
-               `cidr`/`user_security_group)`).
+               `cidr`/`public_security_group`/`user_security_group)`).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SecurityGroupRuleState.__new__(_SecurityGroupRuleState)
 
         __props__.__dict__["cidr"] = cidr
         __props__.__dict__["description"] = description
         __props__.__dict__["end_port"] = end_port
         __props__.__dict__["icmp_code"] = icmp_code
         __props__.__dict__["icmp_type"] = icmp_type
         __props__.__dict__["protocol"] = protocol
+        __props__.__dict__["public_security_group"] = public_security_group
         __props__.__dict__["security_group"] = security_group
         __props__.__dict__["security_group_id"] = security_group_id
         __props__.__dict__["start_port"] = start_port
         __props__.__dict__["type"] = type
         __props__.__dict__["user_security_group"] = user_security_group
         __props__.__dict__["user_security_group_id"] = user_security_group_id
         return SecurityGroupRule(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def cidr(self) -> pulumi.Output[Optional[str]]:
         """
         An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR
         notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with
-        `user_security_group`/`user_security_group_id`).
+        `public_security_group`/`user_security_group`/`user_security_group_id`).
         """
         return pulumi.get(self, "cidr")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
@@ -686,14 +731,23 @@
     def protocol(self) -> pulumi.Output[Optional[str]]:
         """
         The network protocol to match (`TCP`, `UDP`, `ICMP`, `ICMPv6`, `AH`, `ESP`, `GRE`, `IPIP` or `ALL`)
         """
         return pulumi.get(self, "protocol")
 
     @property
+    @pulumi.getter(name="publicSecurityGroup")
+    def public_security_group(self) -> pulumi.Output[str]:
+        """
+        An (`INGRESS`) source / (`EGRESS`) destination public security group name to match (conflicts with
+        `cidr`/`user_security_group`/`user_security_group_id`).
+        """
+        return pulumi.get(self, "public_security_group")
+
+    @property
     @pulumi.getter(name="securityGroup")
     def security_group(self) -> pulumi.Output[str]:
         """
         The parent security group name. Please use the `security_group_id` argument along the
         [exoscale_security_group](../data-sources/security_group.md) data source instead.
         """
         return pulumi.get(self, "security_group")
@@ -723,21 +777,21 @@
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="userSecurityGroup")
     def user_security_group(self) -> pulumi.Output[str]:
         """
         An (`INGRESS`) source / (`EGRESS`) destination security group name to match (conflicts with
-        `cidr`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
+        `cidr`/`public_security_group`/`user_security_group_id`). Please use the `user_security_group_id` argument along the
         [exoscale_security_group](../data-sources/security_group.md) data source instead.
         """
         return pulumi.get(self, "user_security_group")
 
     @property
     @pulumi.getter(name="userSecurityGroupId")
     def user_security_group_id(self) -> pulumi.Output[Optional[str]]:
         """
         An (`INGRESS`) source / (`EGRESS`) destination security group ID to match (conflicts with
-        `cidr`/`user_security_group)`).
+        `cidr`/`public_security_group`/`user_security_group)`).
         """
         return pulumi.get(self, "user_security_group_id")
```

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/security_group_rules.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/security_group_rules.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/sks_cluster.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/sks_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/sks_kubeconfig.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/sks_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/sks_nodepool.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/sks_nodepool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/ssh_key.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale/ssh_keypair.py` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale/ssh_keypair.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/PKG-INFO` & `pulumiverse_exoscale-0.48.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumiverse-exoscale
-Version: 0.47.0
+Name: pulumiverse_exoscale
+Version: 0.48.0
 Summary: A Pulumi package for creating and managing exoscale cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-exoscale
 Keywords: pulumi exoscale category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_exoscale-0.47.0/pulumiverse_exoscale.egg-info/SOURCES.txt` & `pulumiverse_exoscale-0.48.0/pulumiverse_exoscale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.47.0/setup.py` & `pulumiverse_exoscale-0.48.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.47.0"
-PLUGIN_VERSION = "0.47.0"
+VERSION = "0.48.0"
+PLUGIN_VERSION = "0.48.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'exoscale', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse/pulumi-exoscale'])
         except OSError as error:
```

