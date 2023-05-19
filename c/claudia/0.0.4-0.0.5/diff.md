# Comparing `tmp/claudia-0.0.4.tar.gz` & `tmp/claudia-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claudia-0.0.4.tar", last modified: Thu May 18 02:41:02 2023, max compression
+gzip compressed data, was "claudia-0.0.5.tar", last modified: Fri May 19 00:32:31 2023, max compression
```

## Comparing `claudia-0.0.4.tar` & `claudia-0.0.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.697970 claudia-0.0.4/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1073 2023-05-11 10:47:00.000000 claudia-0.0.4/LICENSE
--rw-r--r--   0 ksaxena    (502) staff       (20)     1866 2023-05-18 02:41:02.697748 claudia-0.0.4/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)     3088 2023-05-15 19:36:08.000000 claudia-0.0.4/README.md
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.676966 claudia-0.0.4/claudia.egg-info/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1866 2023-05-18 02:41:02.000000 claudia-0.0.4/claudia.egg-info/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)     2610 2023-05-18 02:41:02.000000 claudia-0.0.4/claudia.egg-info/SOURCES.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-05-18 02:41:02.000000 claudia-0.0.4/claudia.egg-info/dependency_links.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-18 02:41:02.000000 claudia-0.0.4/claudia.egg-info/entry_points.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       79 2023-05-18 02:41:02.000000 claudia-0.0.4/claudia.egg-info/requires.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-05-18 02:41:02.000000 claudia-0.0.4/claudia.egg-info/top_level.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-05-18 02:41:02.698034 claudia-0.0.4/setup.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)     1477 2023-05-18 02:38:59.000000 claudia-0.0.4/setup.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.670291 claudia-0.0.4/src/
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.678304 claudia-0.0.4/src/claudia/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1517 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/README.md
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    10376 2023-05-16 20:58:51.000000 claudia-0.0.4/src/claudia/claudia.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.679544 claudia-0.0.4/src/claudia/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/features/nft_burn_mint.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/features/payments.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/features/trustline.feature
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.681920 claudia-0.0.4/src/claudia/javascript/
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/cleanup
--rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/cucumber.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.682267 claudia-0.0.4/src/claudia/javascript/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1226 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/features/context.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.682550 claudia-0.0.4/src/claudia/javascript/features/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)     2106 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/features/lib/ObjFactory.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.684437 claudia-0.0.4/src/claudia/javascript/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    38728 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/features/steps/common.js
--rw-r--r--   0 ksaxena    (502) staff       (20)      300 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/features/steps/constants.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/features/steps/nft_mint_burn.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/features/steps/payments.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/features/steps/trustline.js
--rw-r--r--   0 ksaxena    (502) staff       (20)   129466 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/package-lock.json
--rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/package.json
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      869 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     4674 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/runTest
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.685079 claudia-0.0.4/src/claudia/network_setup/
--rw-rw-r--   0 ksaxena    (502) staff       (20)      251 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/Dockerfile
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.685889 claudia-0.0.4/src/claudia/network_setup/configs/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     1520 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled.cfg
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.686599 claudia-0.0.4/src/claudia/network_setup/configs/rippled_1/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2150 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_1/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_1/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.687178 claudia-0.0.4/src/claudia/network_setup/configs/rippled_2/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_2/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_2/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.687893 claudia-0.0.4/src/claudia/network_setup/configs/rippled_3/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_3/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_3/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.688610 claudia-0.0.4/src/claudia/network_setup/configs/rippled_4/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2190 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_4/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_4/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.689721 claudia-0.0.4/src/claudia/network_setup/configs/rippled_5/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2226 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_5/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_5/validators.txt
--rw-rw-r--   0 ksaxena    (502) staff       (20)      279 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.691228 claudia-0.0.4/src/claudia/network_setup/lib/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     1619 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/lib/build_rippled.sh
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2161 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/lib/rippled_network.yml
--rw-rw-r--   0 ksaxena    (502) staff       (20)     8966 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/lib/setup_helper.sh
--rw-rw-r--   0 ksaxena    (502) staff       (20)     5094 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/lib/validate_network.py
--rw-rw-r--   0 ksaxena    (502) staff       (20)     3784 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/setup.sh
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.692897 claudia-0.0.4/src/claudia/python/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/behave.ini
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/cleanup
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.693446 claudia-0.0.4/src/claudia/python/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     2977 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/environment.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.694327 claudia-0.0.4/src/claudia/python/features/exceptions/
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/exceptions/InvalidInputException.py
--rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/exceptions/UnconfiguredEnvironmentException.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.695236 claudia-0.0.4/src/claudia/python/features/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)      301 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/lib/Helpers.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     7674 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/lib/ObjFactory.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.697333 claudia-0.0.4/src/claudia/python/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    24750 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/steps/common.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/steps/constants.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    66340 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/steps/nft_mint_burn.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    21822 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/steps/payments.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    54620 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/steps/trustline.py
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     1381 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     5634 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/runTest
--rw-r--r--   0 ksaxena    (502) staff       (20)       79 2023-05-16 18:21:22.000000 claudia-0.0.4/src/claudia/requirements.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.395634 claudia-0.0.5/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1073 2023-05-11 10:47:00.000000 claudia-0.0.5/LICENSE
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1918 2023-05-19 00:32:31.395452 claudia-0.0.5/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)     3140 2023-05-18 03:10:36.000000 claudia-0.0.5/README.md
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.374537 claudia-0.0.5/claudia.egg-info/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1918 2023-05-19 00:32:31.000000 claudia-0.0.5/claudia.egg-info/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2610 2023-05-19 00:32:31.000000 claudia-0.0.5/claudia.egg-info/SOURCES.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-05-19 00:32:31.000000 claudia-0.0.5/claudia.egg-info/dependency_links.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-19 00:32:31.000000 claudia-0.0.5/claudia.egg-info/entry_points.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       79 2023-05-19 00:32:31.000000 claudia-0.0.5/claudia.egg-info/requires.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-05-19 00:32:31.000000 claudia-0.0.5/claudia.egg-info/top_level.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-05-19 00:32:31.395682 claudia-0.0.5/setup.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1477 2023-05-18 21:58:41.000000 claudia-0.0.5/setup.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.366269 claudia-0.0.5/src/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.376112 claudia-0.0.5/src/claudia/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1569 2023-05-18 03:11:01.000000 claudia-0.0.5/src/claudia/README.md
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    10512 2023-05-19 00:29:17.000000 claudia-0.0.5/src/claudia/claudia.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.377618 claudia-0.0.5/src/claudia/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/features/nft_burn_mint.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/features/payments.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/features/trustline.feature
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.379963 claudia-0.0.5/src/claudia/javascript/
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/javascript/cleanup
+-rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/javascript/cucumber.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.380356 claudia-0.0.5/src/claudia/javascript/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1226 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/javascript/features/context.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.380721 claudia-0.0.5/src/claudia/javascript/features/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2106 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/javascript/features/lib/ObjFactory.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.382543 claudia-0.0.5/src/claudia/javascript/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    38728 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/javascript/features/steps/common.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)      300 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/javascript/features/steps/constants.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/javascript/features/steps/nft_mint_burn.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/javascript/features/steps/payments.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/javascript/features/steps/trustline.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)   129466 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/javascript/package-lock.json
+-rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/javascript/package.json
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      869 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/javascript/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     4674 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/javascript/runTest
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.383355 claudia-0.0.5/src/claudia/network_setup/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      251 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/Dockerfile
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.384145 claudia-0.0.5/src/claudia/network_setup/configs/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     1520 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/configs/rippled.cfg
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.384932 claudia-0.0.5/src/claudia/network_setup/configs/rippled_1/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2150 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/configs/rippled_1/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/configs/rippled_1/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.385541 claudia-0.0.5/src/claudia/network_setup/configs/rippled_2/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/configs/rippled_2/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/configs/rippled_2/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.386189 claudia-0.0.5/src/claudia/network_setup/configs/rippled_3/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/configs/rippled_3/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/configs/rippled_3/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.386817 claudia-0.0.5/src/claudia/network_setup/configs/rippled_4/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2190 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/configs/rippled_4/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/configs/rippled_4/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.387347 claudia-0.0.5/src/claudia/network_setup/configs/rippled_5/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2226 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/configs/rippled_5/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/configs/rippled_5/validators.txt
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      279 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/configs/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.388641 claudia-0.0.5/src/claudia/network_setup/lib/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     1619 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/lib/build_rippled.sh
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2161 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/lib/rippled_network.yml
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     8966 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/lib/setup_helper.sh
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     5094 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/lib/validate_network.py
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     3784 2023-05-18 02:32:34.000000 claudia-0.0.5/src/claudia/network_setup/setup.sh
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.390394 claudia-0.0.5/src/claudia/python/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/behave.ini
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/cleanup
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.390897 claudia-0.0.5/src/claudia/python/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/features/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2977 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/features/environment.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.391673 claudia-0.0.5/src/claudia/python/features/exceptions/
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/features/exceptions/InvalidInputException.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/features/exceptions/UnconfiguredEnvironmentException.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.392686 claudia-0.0.5/src/claudia/python/features/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)      301 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/features/lib/Helpers.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     7674 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/features/lib/ObjFactory.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 00:32:31.395042 claudia-0.0.5/src/claudia/python/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    24750 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/features/steps/common.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/features/steps/constants.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    66340 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/features/steps/nft_mint_burn.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    21822 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/features/steps/payments.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    54620 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/features/steps/trustline.py
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     1381 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     5634 2023-05-15 18:14:02.000000 claudia-0.0.5/src/claudia/python/runTest
+-rw-r--r--   0 ksaxena    (502) staff       (20)       79 2023-05-16 18:21:22.000000 claudia-0.0.5/src/claudia/requirements.txt
```

### Comparing `claudia-0.0.4/LICENSE` & `claudia-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/PKG-INFO` & `claudia-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claudia
-Version: 0.0.4
+Version: 0.0.5
 Summary: Run XRPL Automated Tests
 Home-page: https://xrpl.org/
 Download-URL: https://gitlab.ops.ripple.com/xrpledger/xrpl-nocode-automation
 Author: Kausty Saxena
 Author-email: ksaxena@ripple.com
 Keywords: ripple xrpl python javascript
 Description-Content-Type: text/markdown
@@ -15,14 +15,15 @@
 
 ---
 
 ## General prerequisites
 Please have the following installed on your machine before proceeding further:
 - [Python3](https://www.python.org/downloads/)
 - [pip](https://pip.pypa.io/en/stable/installation/)
+- [docker](https://docs.docker.com/engine/install/)
 -  Following is only required if you intend to run Javascript tests.
    - [node](https://nodejs.org/en/download)
    - [npm](https://www.npmjs.com/package/download)
 
 ---
 
 ## Installation
```

### Comparing `claudia-0.0.4/README.md` & `claudia-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 ---
 
 ## General prerequisites
 Please have the following installed on your machine before proceeding further:
 - [Python3](https://www.python.org/downloads/)
 - [pip](https://pip.pypa.io/en/stable/installation/)
+- [docker](https://docs.docker.com/engine/install/)
 -  Following is only required if you intend to run Javascript tests.
    - [node](https://nodejs.org/en/download)
    - [npm](https://www.npmjs.com/package/download)
 
 ---
 
 ## Build Rippled
```

### Comparing `claudia-0.0.4/claudia.egg-info/PKG-INFO` & `claudia-0.0.5/claudia.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claudia
-Version: 0.0.4
+Version: 0.0.5
 Summary: Run XRPL Automated Tests
 Home-page: https://xrpl.org/
 Download-URL: https://gitlab.ops.ripple.com/xrpledger/xrpl-nocode-automation
 Author: Kausty Saxena
 Author-email: ksaxena@ripple.com
 Keywords: ripple xrpl python javascript
 Description-Content-Type: text/markdown
@@ -15,14 +15,15 @@
 
 ---
 
 ## General prerequisites
 Please have the following installed on your machine before proceeding further:
 - [Python3](https://www.python.org/downloads/)
 - [pip](https://pip.pypa.io/en/stable/installation/)
+- [docker](https://docs.docker.com/engine/install/)
 -  Following is only required if you intend to run Javascript tests.
    - [node](https://nodejs.org/en/download)
    - [npm](https://www.npmjs.com/package/download)
 
 ---
 
 ## Installation
```

### Comparing `claudia-0.0.4/claudia.egg-info/SOURCES.txt` & `claudia-0.0.5/claudia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/setup.py` & `claudia-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         requirements = content.split('\n')
 
     return requirements
 
 
 setup(
     name='claudia',
-    version='0.0.4',
+    version='0.0.5',
     description='Run XRPL Automated Tests',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     author="Kausty Saxena",
     author_email="ksaxena@ripple.com",
     keywords="ripple xrpl python javascript",
     url='https://xrpl.org/',
```

### Comparing `claudia-0.0.4/src/claudia/README.md` & `claudia-0.0.5/src/claudia/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 ---
 
 ## General prerequisites
 Please have the following installed on your machine before proceeding further:
 - [Python3](https://www.python.org/downloads/)
 - [pip](https://pip.pypa.io/en/stable/installation/)
+- [docker](https://docs.docker.com/engine/install/)
 -  Following is only required if you intend to run Javascript tests.
    - [node](https://nodejs.org/en/download)
    - [npm](https://www.npmjs.com/package/download)
 
 ---
 
 ## Installation
```

### Comparing `claudia-0.0.4/src/claudia/claudia.py` & `claudia-0.0.5/src/claudia/claudia.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,50 +9,98 @@
             cls.instance = super(SingletonClass, cls).__new__(cls)
         return cls.instance
 
 
 singleton = SingletonClass()
 singleton.PROJECT_ROOT_DIR = os.path.dirname(__file__)
 
+
+def set_to_js_wd():
+    os.chdir("{}/javascript/".format(singleton.PROJECT_ROOT_DIR))
+
+
+def set_to_py_wd():
+    os.chdir("{}/python/".format(singleton.PROJECT_ROOT_DIR))
+
+
+def set_to_project_root_wd():
+    os.chdir(singleton.PROJECT_ROOT_DIR)
+
+
+def python(context, client_type, network, tag, feature):
+    set_to_py_wd()
+    try:
+        set_python_launch_vars(network, client_type)
+        load_feature_files()
+        launch_behave(tag, feature)
+        unload_feature_files()
+    except Exception as e:
+        set_to_project_root_wd()
+        raise e
+
+
+def javascript(context, network, tag, feature, invalidate_cache):
+    set_to_js_wd()
+    try:
+        if invalidate_cache != 'false':
+            invalidate_cache_and_rebuild()
+        elif not os.path.isdir('./node_modules'):
+            first_time_build()
+
+        set_javascript_launch_vars(network)
+        load_feature_files()
+        launch_cucumber(tag, feature)
+        unload_feature_files()
+        set_to_project_root_wd()
+    except Exception as e:
+        set_to_project_root_wd()
+        raise e
+
+def compose_feature_helper_message():
+    set_to_project_root_wd()
+    message = "Feature file to be used for the test run. Allowed values are "
+    features = os.listdir('./features/')
+    for i in range(0, len(features)):
+        message += "'{}', ".format(features[i].replace(".feature", ""))
+    message += "and 'all' and is defaulted to 'payments'. \n\nMore information: https://behave.readthedocs.io/en/latest/tutorial.html?highlight=feature#feature-files."
+    return message
+
 @click.group()
 def main():
     """Claudia says hi! Please choose a command to perform an action. A command can have multiple sub-commands and options. Use '--help' option for more information."""
 
+@main.group()
+def rippled():
+    """Build or install rippled"""
+
+@main.group()
+def network():
+    """Setup Rippled Network"""
 
 @main.group()
 @click.pass_context
 def run(context):
-    """This command allows you to run XRPL automated tests."""
+    """Run XRPL automated tests"""
 
 
-@main.command()
-# @click.pass_context
+@rippled.command()
 @click.option('--repo', required=True, help="The path to a local rippled repo")
 def build(repo):
     """Build rippled from source"""
-    # click.echo("Hellow12")
     set_to_project_root_wd()
-    # click.echo("Hellow")
     command = "sh network_setup/setup.sh --buildRippled --rippledRepo {}".format(repo)
     subprocess.call(command, shell=True)
 
 
-@main.group()
-# @click.pass_context
+@rippled.command()
 def install():
     """Install rippled packages"""
     click.echo("Currently not supported")
 
 
-@main.group()
-# @click.pass_context
-def network():
-    """Setup Rippled Network"""
-
-
 @network.command()
 @click.option('--repo', required=True,
               help="path to rippled repo")
 def start(repo):
     """Start a new rippled network"""
     set_to_project_root_wd()
     command = "sh ./network_setup/setup.sh --networkStart  --rippledRepo {}".format(repo)
@@ -70,73 +118,49 @@
 @network.command()
 def status():
     """rippled network status"""
     set_to_project_root_wd()
     command = "sh ./network_setup/setup.sh --networkStatus"
     subprocess.call(command, shell=True)
 
-
 @run.command()
 @click.pass_context
+@click.option('--lib', default='py',
+              help="The type of client library to be used for running the tests. Allowed values are 'py' and 'js' and is defaulted to 'py'.  \n\nMore information: https://xrpl.org/client-libraries.html#client-libraries")
 @click.option('--client_type', default='websocket',
-              help="The type of client to be used. Allowed values are 'websocket' and 'jsonrpc' and is defaulted to 'websocket'. More information: \n\nhttps://xrpl.org/get-started-using-http-websocket-apis.html#differences-between-json-rpc-and-websocket")
+              help="The type of client to be used. This flag should only be used with 'py' library. Allowed values are 'websocket' and 'jsonrpc' and is defaulted to 'websocket'.  \n\nMore information: https://xrpl.org/get-started-using-http-websocket-apis.html#differences-between-json-rpc-and-websocket")
 @click.option('--network', default='local',
-              help="The type of client to be used. Allowed values are 'websocket' and 'jsonrpc' and is defaulted to 'local'. More information: \n\nhttps://xrpl.org/get-started-using-http-websocket-apis.html#differences-between-json-rpc-and-websocket")
+              help="The type of network to be used. Allowed values are 'devnet', 'testnet', and 'local' and is defaulted to 'local'.  \n\nMore information: https://xrpl.org/get-started-using-http-websocket-apis.html#differences-between-json-rpc-and-websocket")
 @click.option('--tag', default='smoke',
-              help="Tag name of the all the tests to be included in the test run. Allowed values are 'smoke', 'regression' and 'time_intensive' and is defaulted to 'smoke'. More information: \n\nhttps://behave.readthedocs.io/en/latest/tag_expressions.html")
+              help="Tag name of the all the tests to be included in the test run. Allowed values are 'smoke', 'regression' and 'time_intensive' and is defaulted to 'smoke'.  \n\nMore information: https://behave.readthedocs.io/en/latest/tag_expressions.html")
 @click.option('--feature', default='payments',
-              help="Feature file to be used for the test run. Allowed values are 'payments', 'trustline', 'nft_mint_burn', and 'all' and is defaulted to 'payments''. More information: \n\nhttps://behave.readthedocs.io/en/latest/tutorial.html?highlight=feature#feature-files")
-def python(context, client_type, network, tag, feature):
-    """Launch XRPL Automated tests using the Python client. Please choose your options wisely."""
-    set_to_py_wd()
-    try:
-        set_python_launch_vars(network, client_type)
-        load_feature_files()
-        launch_behave(tag, feature)
-        unload_feature_files()
-    except Exception as e:
-        set_to_project_root_wd()
-        raise e
-
-
-@run.command()
-@click.pass_context
-@click.option('--network', default='local',
-              help="The type of client to be used. Allowed values are 'websocket' and 'jsonrpc' and is defaulted to 'local'. More information: \n\nhttps://xrpl.org/get-started-using-http-websocket-apis.html#differences-between-json-rpc-and-websocket")
-@click.option('--tag', default='smoke',
-              help="Tag name of the all the tests to be included in the test run. Allowed values are 'smoke', 'regression' and 'time_intensive' and is defaulted to 'smoke'. More information: \n\nhttps://behave.readthedocs.io/en/latest/tag_expressions.html")
-@click.option('--feature', default='payments',
-              help="Feature file to be used for the test run. Allowed values are 'payments', 'trustline', 'nft_mint_burn', and 'all' and is defaulted to 'payments''. More information: \n\nhttps://behave.readthedocs.io/en/latest/tutorial.html?highlight=feature#feature-files")
+              help=compose_feature_helper_message())
 @click.option('--invalidate_cache', default='false',
-              help="Forces ignoring cache, and reinstalling dependencies. Allowed values are 'true' and 'false' and is defaulted to 'false'.")
-def javascript(context, network, tag, feature, invalidate_cache):
-    """Launch XRPL Automated tests using the Javascript client. Please choose your options wisely."""
-    set_to_js_wd()
-    try:
-        if invalidate_cache != 'false':
-            invalidate_cache_and_rebuild()
-        elif not os.path.isdir('./node_modules'):
-            first_time_build()
-        set_javascript_launch_vars(network)
-        load_feature_files()
-        launch_cucumber(tag, feature)
-        unload_feature_files()
-        set_to_project_root_wd()
-    except Exception as e:
-        set_to_project_root_wd()
-        raise e
+              help="Forces ignoring cache, and reinstalling dependencies. This flag should only be used with 'js library. Allowed values are 'true' and 'false' and is defaulted to 'false'.")
+def e2etests(context, lib, client_type, network, tag, feature, invalidate_cache):
+    """Launch XRPL Automated tests using XRPL library client. Please choose your options wisely."""
+    if(lib == 'py'):
+        if (invalidate_cache != 'false'):
+            raise Exception("--invalidate_cache flag is supported not with {} library client.".format(lib))
+        python(context, client_type, network, tag, feature)
+    elif(lib == 'js'):
+        if (client_type != 'websocket'):
+            raise Exception("Client Type {} is not supported with {} library client.".format(client_type, lib))
+        javascript(context, network, tag, feature, invalidate_cache)
+    else:
+        raise Exception("Invalid library type: {}".format(lib))
 
 
-@run.command()
-@click.pass_context
-@click.argument("text")
-def customcommand(context, text):
-    """Run a debug command"""
-    click.echo("Running command: {}".format(text))
-    subprocess.call(text, shell=True)
+# @run.command()
+# @click.pass_context
+# @click.argument("text")
+# def customcommand(context, text):
+#     """Run a debug command"""
+#     click.echo("Running command: {}".format(text))
+#     subprocess.call(text, shell=True)
 
 
 def invalidate_cache_and_rebuild():
     print("Invalidating cache...")
     os.popen('rm -rf ./node_modules')
     install_js_dependencies_if_needed()
 
@@ -153,37 +177,37 @@
             connectionURL = "127.0.0.5:6001"
             connectionType = "websocket"
         elif client_type == "jsonrpc":
             connectionScheme = "http"
             connectionURL = "127.0.0.5:5001"
             connectionType = "jsonrpc"
         else:
-            raise Exception("{} is not a valid connectionType".format(client_type))
+            raise Exception("{} is not a valid client_type".format(client_type))
     elif network == "devnet":
         if client_type == "websocket":
             connectionScheme = "wss"
             connectionURL = "s.devnet.rippletest.net:51233"
             connectionType = "websocket"
         elif client_type == "jsonrpc":
             connectionScheme = "https"
             connectionURL = "s.devnet.rippletest.net:51234"
             connectionType = "jsonrpc"
         else:
-            raise Exception("{} is not a valid connectionType".format(client_type))
+            raise Exception("{} is not a valid client_type".format(client_type))
     elif network == "testnet":
         if client_type == "websocket":
             connectionScheme = "wss"
             connectionURL = "s.altnet.rippletest.net:51233"
             connectionType = "websocket"
         elif client_type == "jsonrpc":
             connectionScheme = "https"
             connectionURL = "s.altnet.rippletest.net:51234"
             connectionType = "jsonrpc"
         else:
-            raise Exception("{} is not a valid connectionType".format(client_type))
+            raise Exception("{} is not a valid client_type".format(client_type))
     else:
         raise Exception("{} is not a valid network".format(network))
 
     os.environ['CONNECTION_SCHEME'] = connectionScheme
     os.environ['CONNECTION_URL'] = connectionURL
     os.environ['CONNECTION_TYPE'] = connectionType
     click.echo("Setting CONNECTION_SCHEME='{}', CONNECTION_URL='{}' and CONNECTION_TYPE='{}'".format(connectionScheme,
@@ -233,25 +257,14 @@
 
 
 def install_js_dependencies_if_needed():
     command = "sh ./runSetup"
     subprocess.call(command, shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
 
 
-def set_to_js_wd():
-    os.chdir("{}/javascript/".format(singleton.PROJECT_ROOT_DIR))
-
-
-def set_to_py_wd():
-    os.chdir("{}/python/".format(singleton.PROJECT_ROOT_DIR))
-
-
-def set_to_project_root_wd():
-    os.chdir(singleton.PROJECT_ROOT_DIR)
-
 
 def launch_cucumber(tag, feature):
     if feature == "all":
         command = "npx cucumber-js --format @cucumber/pretty-formatter --tags @{}".format(tag)
     else:
         command = "npx cucumber-js --format @cucumber/pretty-formatter --tags @{} ./features/{}.feature".format(tag,
                                                                                                                 feature)
```

### Comparing `claudia-0.0.4/src/claudia/features/nft_burn_mint.feature` & `claudia-0.0.5/src/claudia/features/nft_burn_mint.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/features/payments.feature` & `claudia-0.0.5/src/claudia/features/payments.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/features/trustline.feature` & `claudia-0.0.5/src/claudia/features/trustline.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/javascript/features/context.js` & `claudia-0.0.5/src/claudia/javascript/features/context.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/javascript/features/lib/ObjFactory.js` & `claudia-0.0.5/src/claudia/javascript/features/lib/ObjFactory.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/javascript/features/steps/common.js` & `claudia-0.0.5/src/claudia/javascript/features/steps/common.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/javascript/features/steps/nft_mint_burn.js` & `claudia-0.0.5/src/claudia/javascript/features/steps/nft_mint_burn.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/javascript/features/steps/payments.js` & `claudia-0.0.5/src/claudia/javascript/features/steps/payments.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/javascript/features/steps/trustline.js` & `claudia-0.0.5/src/claudia/javascript/features/steps/trustline.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/javascript/package-lock.json` & `claudia-0.0.5/src/claudia/javascript/package-lock.json`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/javascript/runSetup` & `claudia-0.0.5/src/claudia/javascript/runSetup`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/javascript/runTest` & `claudia-0.0.5/src/claudia/javascript/runTest`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/network_setup/configs/rippled.cfg` & `claudia-0.0.5/src/claudia/network_setup/configs/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/network_setup/configs/rippled_1/rippled.cfg` & `claudia-0.0.5/src/claudia/network_setup/configs/rippled_1/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/network_setup/configs/rippled_2/rippled.cfg` & `claudia-0.0.5/src/claudia/network_setup/configs/rippled_2/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/network_setup/configs/rippled_3/rippled.cfg` & `claudia-0.0.5/src/claudia/network_setup/configs/rippled_3/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/network_setup/configs/rippled_4/rippled.cfg` & `claudia-0.0.5/src/claudia/network_setup/configs/rippled_4/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/network_setup/configs/rippled_5/rippled.cfg` & `claudia-0.0.5/src/claudia/network_setup/configs/rippled_5/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/network_setup/lib/build_rippled.sh` & `claudia-0.0.5/src/claudia/network_setup/lib/build_rippled.sh`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/network_setup/lib/rippled_network.yml` & `claudia-0.0.5/src/claudia/network_setup/lib/rippled_network.yml`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/network_setup/lib/setup_helper.sh` & `claudia-0.0.5/src/claudia/network_setup/lib/setup_helper.sh`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/network_setup/lib/validate_network.py` & `claudia-0.0.5/src/claudia/network_setup/lib/validate_network.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/network_setup/setup.sh` & `claudia-0.0.5/src/claudia/network_setup/setup.sh`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/python/features/environment.py` & `claudia-0.0.5/src/claudia/python/features/environment.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/python/features/lib/ObjFactory.py` & `claudia-0.0.5/src/claudia/python/features/lib/ObjFactory.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/python/features/steps/common.py` & `claudia-0.0.5/src/claudia/python/features/steps/common.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/python/features/steps/nft_mint_burn.py` & `claudia-0.0.5/src/claudia/python/features/steps/nft_mint_burn.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/python/features/steps/payments.py` & `claudia-0.0.5/src/claudia/python/features/steps/payments.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/python/features/steps/trustline.py` & `claudia-0.0.5/src/claudia/python/features/steps/trustline.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/python/runSetup` & `claudia-0.0.5/src/claudia/python/runSetup`

 * *Files identical despite different names*

### Comparing `claudia-0.0.4/src/claudia/python/runTest` & `claudia-0.0.5/src/claudia/python/runTest`

 * *Files identical despite different names*

