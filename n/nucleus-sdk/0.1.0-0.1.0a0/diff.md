# Comparing `tmp/nucleus-sdk-0.1.0.tar.gz` & `tmp/nucleus-sdk-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucleus-sdk-0.1.0.tar", last modified: Thu May 18 20:17:02 2023, max compression
+gzip compressed data, was "nucleus-sdk-0.1.0a0.tar", last modified: Fri May 19 16:51:14 2023, max compression
```

## Comparing `nucleus-sdk-0.1.0.tar` & `nucleus-sdk-0.1.0a0.tar`

### file list

```diff
@@ -1,106 +1,108 @@
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.608706 nucleus-sdk-0.1.0/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)    34523 2021-10-21 21:17:05.000000 nucleus-sdk-0.1.0/LICENSE
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      246 2023-05-18 20:17:02.608706 nucleus-sdk-0.1.0/PKG-INFO
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     5838 2023-05-18 13:00:25.000000 nucleus-sdk-0.1.0/README.md
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.596706 nucleus-sdk-0.1.0/nucleus/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)        0 2023-05-18 19:44:44.000000 nucleus-sdk-0.1.0/nucleus/__init__.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.596706 nucleus-sdk-0.1.0/nucleus/core/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)        0 2023-05-18 19:41:08.000000 nucleus-sdk-0.1.0/nucleus/core/__init__.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.596706 nucleus-sdk-0.1.0/nucleus/core/blockchain/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)        0 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/blockchain/__init__.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      402 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/blockchain/constants.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      558 2023-05-17 19:34:07.000000 nucleus-sdk-0.1.0/nucleus/core/blockchain/crypto.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     1173 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/blockchain/types.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.596706 nucleus-sdk-0.1.0/nucleus/core/cache/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      161 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/cache/__init__.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      315 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/cache/constants.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     1744 2023-05-18 17:21:48.000000 nucleus-sdk-0.1.0/nucleus/core/cache/database.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)       76 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/cache/types.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)       90 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/constants.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      640 2023-05-17 21:11:55.000000 nucleus-sdk-0.1.0/nucleus/core/dataclass.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      625 2023-05-17 19:34:07.000000 nucleus-sdk-0.1.0/nucleus/core/decorators.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     1021 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/exceptions.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.600706 nucleus-sdk-0.1.0/nucleus/core/http/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      218 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/http/__init__.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      419 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/http/partials.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      925 2023-05-18 17:21:48.000000 nucleus-sdk-0.1.0/nucleus/core/http/session.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)       96 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/http/types.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.600706 nucleus-sdk-0.1.0/nucleus/core/ipfs/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      143 2023-05-17 19:34:07.000000 nucleus-sdk-0.1.0/nucleus/core/ipfs/__init__.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.600706 nucleus-sdk-0.1.0/nucleus/core/ipfs/cmd/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      268 2023-05-18 17:21:49.000000 nucleus-sdk-0.1.0/nucleus/core/ipfs/cmd/__init__.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      950 2023-05-18 16:42:30.000000 nucleus-sdk-0.1.0/nucleus/core/ipfs/cmd/add.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      980 2023-05-18 17:21:49.000000 nucleus-sdk-0.1.0/nucleus/core/ipfs/cmd/block.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      189 2023-05-17 19:34:07.000000 nucleus-sdk-0.1.0/nucleus/core/ipfs/cmd/constants.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      985 2023-05-18 17:21:49.000000 nucleus-sdk-0.1.0/nucleus/core/ipfs/cmd/dag.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      896 2023-05-17 19:34:07.000000 nucleus-sdk-0.1.0/nucleus/core/ipfs/cmd/options.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      571 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/ipfs/connect.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)       48 2023-04-24 16:49:26.000000 nucleus-sdk-0.1.0/nucleus/core/ipfs/constants.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     1629 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/ipfs/rpc.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      724 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/ipfs/types.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      875 2023-05-17 19:34:07.000000 nucleus-sdk-0.1.0/nucleus/core/logger.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.600706 nucleus-sdk-0.1.0/nucleus/core/subprocess/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      107 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/subprocess/__init__.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)       97 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/subprocess/constants.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      206 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/subprocess/exec.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     4006 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/subprocess/ipc.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     1399 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/subprocess/protocol.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      295 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/core/subprocess/types.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     5557 2023-05-18 16:43:14.000000 nucleus-sdk-0.1.0/nucleus/core/types.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.600706 nucleus-sdk-0.1.0/nucleus/sdk/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)        0 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/sdk/__init__.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     1930 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/sdk/exceptions.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.604706 nucleus-sdk-0.1.0/nucleus/sdk/expose/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      477 2023-05-18 14:29:17.000000 nucleus-sdk-0.1.0/nucleus/sdk/expose/__init__.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     1659 2023-05-18 17:21:45.000000 nucleus-sdk-0.1.0/nucleus/sdk/expose/crypto.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     1670 2023-05-18 16:44:10.000000 nucleus-sdk-0.1.0/nucleus/sdk/expose/key.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     4176 2023-05-18 17:21:43.000000 nucleus-sdk-0.1.0/nucleus/sdk/expose/marshall.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      762 2023-05-13 00:48:14.000000 nucleus-sdk-0.1.0/nucleus/sdk/expose/metadata.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      707 2023-05-18 15:31:41.000000 nucleus-sdk-0.1.0/nucleus/sdk/expose/partials.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     2671 2023-05-18 16:43:40.000000 nucleus-sdk-0.1.0/nucleus/sdk/expose/sep.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     2472 2023-05-18 16:44:10.000000 nucleus-sdk-0.1.0/nucleus/sdk/expose/types.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.604706 nucleus-sdk-0.1.0/nucleus/sdk/harvest/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      551 2023-05-17 19:33:30.000000 nucleus-sdk-0.1.0/nucleus/sdk/harvest/__init__.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     1803 2023-05-18 17:21:47.000000 nucleus-sdk-0.1.0/nucleus/sdk/harvest/collectors.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      372 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/sdk/harvest/constants.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      593 2023-05-15 20:49:38.000000 nucleus-sdk-0.1.0/nucleus/sdk/harvest/media.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     4693 2023-05-18 17:21:46.000000 nucleus-sdk-0.1.0/nucleus/sdk/harvest/models.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     1011 2023-05-17 19:33:30.000000 nucleus-sdk-0.1.0/nucleus/sdk/harvest/partials.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      644 2023-05-17 19:33:30.000000 nucleus-sdk-0.1.0/nucleus/sdk/harvest/types.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.604706 nucleus-sdk-0.1.0/nucleus/sdk/processing/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      350 2023-05-17 19:33:30.000000 nucleus-sdk-0.1.0/nucleus/sdk/processing/__init__.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     5210 2023-05-18 17:21:44.000000 nucleus-sdk-0.1.0/nucleus/sdk/processing/engines.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.604706 nucleus-sdk-0.1.0/nucleus/sdk/processing/image/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)       90 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/sdk/processing/image/__init__.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     2152 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/sdk/processing/image/options.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      993 2023-05-17 19:34:07.000000 nucleus-sdk-0.1.0/nucleus/sdk/processing/process.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     3089 2023-05-18 16:42:30.000000 nucleus-sdk-0.1.0/nucleus/sdk/processing/types.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.608706 nucleus-sdk-0.1.0/nucleus/sdk/processing/video/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      303 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/sdk/processing/video/__init__.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     2529 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/sdk/processing/video/codecs.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      880 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/sdk/processing/video/constants.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      763 2023-05-17 19:34:07.000000 nucleus-sdk-0.1.0/nucleus/sdk/processing/video/ffprobe.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     2376 2023-04-29 17:07:19.000000 nucleus-sdk-0.1.0/nucleus/sdk/processing/video/options.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      624 2023-05-15 21:05:06.000000 nucleus-sdk-0.1.0/nucleus/sdk/processing/video/protocols.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      623 2023-05-18 16:42:30.000000 nucleus-sdk-0.1.0/nucleus/sdk/processing/video/types.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.608706 nucleus-sdk-0.1.0/nucleus/sdk/retrieval/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)       48 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/sdk/retrieval/__init__.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      437 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/sdk/retrieval/cmd.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)        0 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/sdk/retrieval/unmarshall.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.608706 nucleus-sdk-0.1.0/nucleus/sdk/storage/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      352 2023-05-17 19:33:30.000000 nucleus-sdk-0.1.0/nucleus/sdk/storage/__init__.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     3234 2023-05-12 23:39:14.000000 nucleus-sdk-0.1.0/nucleus/sdk/storage/clients.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      111 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/sdk/storage/constants.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      696 2023-05-18 01:34:38.000000 nucleus-sdk-0.1.0/nucleus/sdk/storage/edge.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      200 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/sdk/storage/partials.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      313 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0/nucleus/sdk/storage/services.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     3015 2023-05-18 17:21:46.000000 nucleus-sdk-0.1.0/nucleus/sdk/storage/store.py
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     1984 2023-05-18 01:35:00.000000 nucleus-sdk-0.1.0/nucleus/sdk/storage/types.py
-drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-18 20:17:02.608706 nucleus-sdk-0.1.0/nucleus_sdk.egg-info/
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      246 2023-05-18 20:17:01.000000 nucleus-sdk-0.1.0/nucleus_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 gmena     (1000) gmena     (1000)     2657 2023-05-18 20:17:02.000000 nucleus-sdk-0.1.0/nucleus_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 gmena     (1000) gmena     (1000)        1 2023-05-18 20:17:02.000000 nucleus-sdk-0.1.0/nucleus_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 gmena     (1000) gmena     (1000)        1 2023-05-18 20:17:01.000000 nucleus-sdk-0.1.0/nucleus_sdk.egg-info/not-zip-safe
--rw-rw-r--   0 gmena     (1000) gmena     (1000)        8 2023-05-18 20:17:02.000000 nucleus-sdk-0.1.0/nucleus_sdk.egg-info/top_level.txt
--rw-rw-r--   0 gmena     (1000) gmena     (1000)       38 2023-05-18 20:17:02.608706 nucleus-sdk-0.1.0/setup.cfg
--rw-rw-r--   0 gmena     (1000) gmena     (1000)      536 2023-05-18 20:16:51.000000 nucleus-sdk-0.1.0/setup.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.150583 nucleus-sdk-0.1.0a0/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)    34523 2021-10-21 21:17:05.000000 nucleus-sdk-0.1.0a0/LICENSE
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     7089 2023-05-19 16:51:14.150583 nucleus-sdk-0.1.0a0/PKG-INFO
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     5931 2023-05-19 15:22:15.000000 nucleus-sdk-0.1.0a0/README.md
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.134583 nucleus-sdk-0.1.0a0/nucleus/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)       51 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/__init__.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.134583 nucleus-sdk-0.1.0a0/nucleus/core/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)        0 2023-05-18 19:41:08.000000 nucleus-sdk-0.1.0a0/nucleus/core/__init__.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.134583 nucleus-sdk-0.1.0a0/nucleus/core/blockchain/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)        0 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0a0/nucleus/core/blockchain/__init__.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      403 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/blockchain/constants.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      560 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/blockchain/crypto.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     1173 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/blockchain/types.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.134583 nucleus-sdk-0.1.0a0/nucleus/core/cache/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      161 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/cache/__init__.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      316 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/cache/constants.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     1732 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/cache/database.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)       75 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/cache/types.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)       90 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0a0/nucleus/core/constants.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      619 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/dataclass.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      588 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/decorators.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     1021 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/exceptions.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.138583 nucleus-sdk-0.1.0a0/nucleus/core/http/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      282 2023-05-19 16:36:01.000000 nucleus-sdk-0.1.0a0/nucleus/core/http/__init__.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      420 2023-05-19 15:50:48.000000 nucleus-sdk-0.1.0a0/nucleus/core/http/partials.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      909 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/http/session.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)       96 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0a0/nucleus/core/http/types.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.138583 nucleus-sdk-0.1.0a0/nucleus/core/ipfs/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      167 2023-05-19 16:36:01.000000 nucleus-sdk-0.1.0a0/nucleus/core/ipfs/__init__.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.138583 nucleus-sdk-0.1.0a0/nucleus/core/ipfs/cmd/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      162 2023-05-19 15:52:19.000000 nucleus-sdk-0.1.0a0/nucleus/core/ipfs/cmd/__init__.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      950 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/ipfs/cmd/add.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      944 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/ipfs/cmd/block.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      189 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/ipfs/cmd/constants.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      949 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/ipfs/cmd/dag.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      867 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/ipfs/cmd/options.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      570 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/ipfs/connect.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)       48 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/ipfs/constants.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     1603 2023-05-19 15:53:40.000000 nucleus-sdk-0.1.0a0/nucleus/core/ipfs/rpc.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      724 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0a0/nucleus/core/ipfs/types.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      840 2023-05-19 15:54:12.000000 nucleus-sdk-0.1.0a0/nucleus/core/logger.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.138583 nucleus-sdk-0.1.0a0/nucleus/core/subprocess/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      107 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/subprocess/__init__.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)       97 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0a0/nucleus/core/subprocess/constants.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      206 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0a0/nucleus/core/subprocess/exec.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     3984 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/subprocess/ipc.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     1400 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/subprocess/protocol.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      295 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/core/subprocess/types.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     5586 2023-05-19 16:11:34.000000 nucleus-sdk-0.1.0a0/nucleus/core/types.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.138583 nucleus-sdk-0.1.0a0/nucleus/sdk/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)        0 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/__init__.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     1848 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/exceptions.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.142583 nucleus-sdk-0.1.0a0/nucleus/sdk/expose/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      413 2023-05-19 16:36:01.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/expose/__init__.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     1626 2023-05-19 16:15:59.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/expose/crypto.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     1670 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/expose/key.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     4176 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/expose/marshall.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      762 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/expose/metadata.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      696 2023-05-19 16:20:02.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/expose/partials.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     2671 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/expose/sep.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     2472 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/expose/types.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.142583 nucleus-sdk-0.1.0a0/nucleus/sdk/harvest/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      539 2023-05-19 16:44:26.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/harvest/__init__.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     1790 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/harvest/collectors.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      372 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/harvest/constants.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      594 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/harvest/media.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     4635 2023-05-19 15:38:02.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/harvest/models.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      990 2023-05-19 15:38:02.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/harvest/partials.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      644 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/harvest/types.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.142583 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      593 2023-05-19 16:44:27.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/__init__.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     5121 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/engines.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.142583 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/image/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      106 2023-05-19 16:27:49.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/image/__init__.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     2152 2023-05-19 16:36:29.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/image/options.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      994 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/process.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     3108 2023-05-19 16:37:55.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/types.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.146583 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/video/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      328 2023-05-19 16:42:01.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/video/__init__.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     2544 2023-05-19 16:38:26.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/video/codecs.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      880 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/video/constants.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      763 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/video/ffprobe.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     2352 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/video/options.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      625 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/video/protocols.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      624 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/processing/video/types.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.146583 nucleus-sdk-0.1.0a0/nucleus/sdk/retrieval/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)       48 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/retrieval/__init__.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      437 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/retrieval/cmd.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)        0 2023-04-16 12:45:23.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/retrieval/unmarshall.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.146583 nucleus-sdk-0.1.0a0/nucleus/sdk/storage/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      328 2023-05-19 16:40:17.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/storage/__init__.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     3204 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/storage/clients.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      111 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/storage/constants.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      696 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/storage/edge.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      200 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/storage/partials.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      314 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/storage/services.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     3003 2023-05-19 14:22:46.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/storage/store.py
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     1925 2023-05-19 16:44:57.000000 nucleus-sdk-0.1.0a0/nucleus/sdk/storage/types.py
+drwxrwxr-x   0 gmena     (1000) gmena     (1000)        0 2023-05-19 16:51:14.146583 nucleus-sdk-0.1.0a0/nucleus_sdk.egg-info/
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     7089 2023-05-19 16:51:14.000000 nucleus-sdk-0.1.0a0/nucleus_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     2706 2023-05-19 16:51:14.000000 nucleus-sdk-0.1.0a0/nucleus_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)        1 2023-05-19 16:51:14.000000 nucleus-sdk-0.1.0a0/nucleus_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)        1 2023-05-19 16:51:13.000000 nucleus-sdk-0.1.0a0/nucleus_sdk.egg-info/not-zip-safe
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)      162 2023-05-19 16:51:14.000000 nucleus-sdk-0.1.0a0/nucleus_sdk.egg-info/requires.txt
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)        8 2023-05-19 16:51:14.000000 nucleus-sdk-0.1.0a0/nucleus_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     6164 2023-05-19 16:51:08.000000 nucleus-sdk-0.1.0a0/pyproject.toml
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)       38 2023-05-19 16:51:14.150583 nucleus-sdk-0.1.0a0/setup.cfg
+-rw-rw-r--   0 gmena     (1000) gmena     (1000)     1081 2023-05-19 13:18:36.000000 nucleus-sdk-0.1.0a0/setup.py
```

### Comparing `nucleus-sdk-0.1.0/LICENSE` & `nucleus-sdk-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `nucleus-sdk-0.1.0/README.md` & `nucleus-sdk-0.1.0a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Nucleus
 
 [![Slack](https://camo.githubusercontent.com/552ad37eb845d5e54e1bef55f3ea7adb185f36c845a6b676eec85e97122b2fcd/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f736c61636b2d6a6f696e2d6f72616e67652e737667)](https://join.slack.com/t/synapse-media/shared_invite/zt-1vbnai6ee-zxOs1Outt2oGMA7Sh1CXgQ)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
 [![CI](https://github.com/ZorrillosDev/watchit-toolkit/actions/workflows/ci.yml/badge.svg)](https://github.com/ZorrillosDev/watchit-toolkit/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/SynapseMedia/nucleus/branch/main/graph/badge.svg?token=M9FF5B6UNA)](https://codecov.io/gh/SynapseMedia/nucleus)
+[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
 <div align="center">
   <img src="arch.png" style="margin: 20px auto"/>
   <hr/>
 </div>
 
 ***NOTE!*** Nucleus is **alpha-stage** software. It means nucleus hasn't been security audited and programming APIs and data formats can still change.
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/blockchain/crypto.py` & `nucleus-sdk-0.1.0a0/nucleus/core/blockchain/crypto.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # Convention for importing types
 from web3 import Web3
-from nucleus.core.types import Primitives, HexStr, CID
+
+from nucleus.core.types import CID, HexStr, Primitives
 
 
 def to_hex(input_: Primitives) -> HexStr:
     """Convert input to hex representation
 
     :param input:
     :return: hexadecimal string
     :rtype: str
     """
-    return HexStr(Web3.toHex(input_))
+    return HexStr(Web3.to_hex(input_))
 
 
 def cid_to_uint256(cid_: CID) -> int:
     """Encode cid to uint256
 
     :param cid: IPFS cid
     :return: uint256 cid representation
     :rtype: int
     """
-    cid_base16 = cid_.format().encode("base16")
-    return int("0x" + cid_base16[1:], 0)
+    cid_base16 = cid_.format().encode('base16')
+    return int('0x' + cid_base16[1:], 0)
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/blockchain/types.py` & `nucleus-sdk-0.1.0a0/nucleus/core/blockchain/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from nucleus.core.types import (
+    JSON,
     URL,
-    HexStr,
     Any,
-    Protocol,
-    Union,
+    Callable,
+    HexStr,
+    NamedTuple,
     NewType,
+    Protocol,
     TypedDict,
-    NamedTuple,
-    Callable,
-    JSON,
+    Union,
 )
 
 Address = Union[HexStr, str]
-Abi = NewType("Abi", JSON)
+Abi = NewType('Abi', JSON)
 Connector = Callable[[URL], Any]
 PrivateKey = Union[Address, int]
 TxCall = Union[NamedTuple, TypedDict]
 TxAnswer = Union[NamedTuple, TypedDict]
-SignedTransaction = NewType("SignedTransaction", NamedTuple)
+SignedTransaction = NewType('SignedTransaction', NamedTuple)
 
 
 class Chain(Protocol):
     """Chain abstract class.
     Use this class to create chain subtypes.
 
     Usage:
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/cache/database.py` & `nucleus-sdk-0.1.0a0/nucleus/core/cache/database.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import sqlite3
 import contextlib
+import sqlite3
 
 from nucleus.core.exceptions import DatabaseError
-from nucleus.core.types import Iterator, Any
+from nucleus.core.types import Any, Iterator
+
 from .constants import DB_DEFAULT
 from .types import Connection
 
 
 def connect(db_path: str = DB_DEFAULT, **kwargs: Any):
     """Db connection factory.
     If path is not found, a new database file is created.
@@ -25,16 +26,15 @@
         return sqlite3.connect(
             db_path,
             detect_types=sqlite3.PARSE_DECLTYPES,
             **kwargs,
         )
     except sqlite3.Error as e:
         # proxy exception raising
-        raise DatabaseError(
-            f"error while trying to connect to database: {str(e)}")
+        raise DatabaseError(f'error while trying to connect to database: {str(e)}')
 
 
 @contextlib.contextmanager
 def connection(db_path: str = DB_DEFAULT, **k: Any) -> Iterator[Connection]:
     """Context db connection
 
     :param db_path: sqlite file path
@@ -52,8 +52,8 @@
     :return: true if connection is open or False otherwise
     :rtype: bool
     """
     cursor = conn.cursor()
     return cursor is not None  # type: ignore
 
 
-__all__ = ["connect", "connection", "is_open"]
+__all__ = ['connect', 'connection', 'is_open']
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/dataclass.py` & `nucleus-sdk-0.1.0a0/nucleus/core/dataclass.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import asdict
+
 from nucleus.core.types import Any, Raw, Tuple
 
 # TODO write test
 
 
 def asdict_sanitize(obj: Any, exclude: Tuple[str]) -> Raw:
     """Does the same as asdict with the exception that it excludes some elements in the conversion.
@@ -11,11 +12,9 @@
     :param obj: dataclass object
     :param exclude: the list of fields to exclude in dict
     :return: dataclass dict with excluded fields
     :rtype: Raw
     """
     return asdict(
         obj,
-        dict_factory=lambda x: {
-            k.replace("_", "-"): v for k, v in x if k not in exclude
-        },
+        dict_factory=lambda x: {k.replace('_', '-'): v for k, v in x if k not in exclude},
     )
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/decorators.py` & `nucleus-sdk-0.1.0a0/nucleus/core/decorators.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import functools
-from nucleus.core.types import Any, Func, ExceptionType
+
+from nucleus.core.types import Any, ExceptionType, Func
 
 
 def proxy_exception(*, expected: ExceptionType, target: ExceptionType) -> Func:
     """It decorate underlying raised exceptions and raise a new standard exception"""
 
     def decorator(func: Func):
         @functools.wraps(func)
         def wrapper(*args: Any, **kwargs: Any):
             try:
                 return func(*args, **kwargs)
             except expected as e:
-                raise target(
-                    f"raised exception during call to `{func.__name__}`: {str(e)}"
-                )
+                raise target(f'raised exception during call to `{func.__name__}`: {str(e)}')
 
         return wrapper
 
     return decorator
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/exceptions.py` & `nucleus-sdk-0.1.0a0/nucleus/core/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 """
 
 
 class HttpError(Exception):
     """Exception raised for errors relation to http operations."""
 
     def __init__(self, message: str):
-        self.message = f"Core :: Http -> {message}"
+        self.message = f'Core :: Http -> {message}'
 
 
 class IPFSRuntimeError(Exception):
     """Exception raised for errors related to ipfs API."""
 
     def __init__(self, message: str):
-        self.message = f"Core :: IPFS -> {message}"
+        self.message = f'Core :: IPFS -> {message}'
 
 
 class DatabaseError(Exception):
     """Exception raised for errors that are related to the database."""
 
     def __init__(self, message: str):
-        self.message = f"Core :: Cache -> {message}"
+        self.message = f'Core :: Cache -> {message}'
 
 
 class DatabaseTransactionError(DatabaseError):
     """Exception raised for errors that are related to database transaction.
     DatabaseTransactionError error is a subclass from DatabaseError.
     """
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/http/session.py` & `nucleus-sdk-0.1.0a0/nucleus/core/http/session.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from urllib.parse import urljoin
+
 import requests
 
-from urllib.parse import urljoin
-from nucleus.core.types import Any
 from nucleus.core.exceptions import HttpError
+from nucleus.core.types import Any
 
 
 class LiveSession(requests.Session):
     """Enhance the session behavior by adding the default base url into requests"""
 
     _base_url: str
 
@@ -19,9 +20,8 @@
 
         # auto concatenate base url with request path
         joined_url = urljoin(self._base_url, url)  # type: ignore
 
         try:
             return super().request(method, joined_url, *args, **kwargs)
         except requests.exceptions.RequestException as e:
-            raise HttpError(
-                f"error trying to make a request to {joined_url}: {str(e)}")
+            raise HttpError(f'error trying to make a request to {joined_url}: {str(e)}')
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/ipfs/cmd/add.py` & `nucleus-sdk-0.1.0a0/nucleus/core/ipfs/cmd/add.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import nucleus.core.dataclass as dc
-
 from dataclasses import dataclass
-from nucleus.core.types import Settings
+
+import nucleus.core.dataclass as dc
 from nucleus.core.http import LiveSession
+from nucleus.core.types import Settings
 
 from .constants import IPFS_API_ADD
 
 
 @dataclass(slots=True)
 class Add:
     """Add files or text to ipfs.
     Each input setting is expected to iter arguments for post requests
     ref: https://docs.ipfs.io/reference/cli/#ipfs-add
     """
 
     input: Settings
     pin: bool = False
     quieter: bool = True
-    hash: str = "blake2b-208"
+    hash: str = 'blake2b-208'
     cid_version: int = 1
 
     def __call__(self, session: LiveSession):
         # convert dataclass to request IPFS 'add endpoint' attributes.
         # we don't want `input` into params
-        params = dc.asdict_sanitize(self, ("input",))
+        params = dc.asdict_sanitize(self, ('input',))
         compiled_settings = dict(self.input)
         # post request to /add endpoint using defined params and settings
         return session.post(IPFS_API_ADD, params=params, **compiled_settings)
 
 
-__all__ = ("Add",)
+__all__ = ('Add',)
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/ipfs/cmd/dag.py` & `nucleus-sdk-0.1.0a0/nucleus/core/ipfs/cmd/dag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-import nucleus.core.dataclass as dc
-
 from dataclasses import dataclass
-from nucleus.core.types import Settings
+
+import nucleus.core.dataclass as dc
 from nucleus.core.http import LiveSession
+from nucleus.core.types import Settings
+
 from .constants import IPFS_API_DAG_PUT
 
 
 @dataclass(slots=True)
 class DagPut:
     """Put data in dag.
     ref: http://docs.ipfs.tech/reference/kubo/rpc/#api-v0-block-put
     """
 
     input: Settings
     pin: bool = True
-    hash: str = "sha2-256"
-    store_codec: str = "dag-jose"
-    input_codec: str = "dag-json"
+    hash: str = 'sha2-256'
+    store_codec: str = 'dag-jose'
+    input_codec: str = 'dag-json'
     allow_big_block: bool = False
 
     def __call__(self, session: LiveSession):
         # convert dataclass to request IPFS 'add endpoint' attributes.
         # we don't want `input` into params
-        params = dc.asdict_sanitize(self, ("input",))
+        params = dc.asdict_sanitize(self, ('input',))
         compiled_settings = dict(self.input)
         # post request to /dag/put endpoint using defined params and settings
-        return session.post(
-            IPFS_API_DAG_PUT,
-            params=params,
-            **compiled_settings)
+        return session.post(IPFS_API_DAG_PUT, params=params, **compiled_settings)
 
 
-__all__ = ("DagPut",)
+__all__ = ('DagPut',)
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/ipfs/cmd/options.py` & `nucleus-sdk-0.1.0a0/nucleus/core/ipfs/cmd/options.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from dataclasses import dataclass
-from nucleus.core.types import Path
+
 from nucleus.core.exceptions import IPFSRuntimeError
+from nucleus.core.types import Path
 
 
 @dataclass(slots=True)
 class File:
     """File represent "files" params in request based on input path.
     :raises IPFSRuntimeError if file does not exist.
     """
 
     path: Path
 
     def __post_init__(self):
         if not self.path.exists():
-            raise IPFSRuntimeError(
-                f"raised trying to execute `add` directory with an invalid path {self.path}"
-            )
+            raise IPFSRuntimeError(f'raised trying to execute `add` directory with an invalid path {self.path}')
 
     def __iter__(self):
         file_name = self.path.name
         blob = self.path.read_bytes()
-        yield "files", {"file": (file_name, blob)}
+        yield 'files', {'file': (file_name, blob)}
 
 
 @dataclass(slots=True)
 class Text:
     """Text represent "data" param in request based on input text."""
 
     input: bytes
 
     def __iter__(self):
-        yield "files", {"file": ("meta", self.input)}
+        yield 'files', {'file': ('meta', self.input)}
 
 
-__all__ = ("File", "Text")
+__all__ = ('File', 'Text')
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/ipfs/connect.py` & `nucleus-sdk-0.1.0a0/nucleus/core/ipfs/connect.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import nucleus.core.http as http
-
 from nucleus.core.types import Optional
 
 from .constants import IPFS_DEFAULT_ENDPOINT
 from .rpc import RPC
 
 
 def rpc(endpoint: Optional[str] = None):
@@ -14,8 +13,8 @@
     :return: a new ipfs api interface object
     :rtype: IPFSApi
     """
     endpoint = endpoint or IPFS_DEFAULT_ENDPOINT
     return RPC(http.live_session(endpoint))
 
 
-__all__ = ("rpc",)
+__all__ = ('rpc',)
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/ipfs/rpc.py` & `nucleus-sdk-0.1.0a0/nucleus/core/ipfs/rpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from nucleus.core.exceptions import IPFSRuntimeError
 from nucleus.core.http import LiveSession
 from nucleus.core.types import JSON
+
 from .types import RPCCommand
 
 
 class RPC:
 
     """IPFS strategically interact with different rpc command and execute them in a safe manner.
-    Each http call is preset with base url and version and the complement of the url is added during runtime based on each rpc command implementation.
+    Each http call is preset with base url and version and the complement of the url is added during runtime
+    based on each rpc command implementation.
         eg. localhost:5001/api/v0 + /add, /config, ...
 
     """
 
     _http: LiveSession
 
     def __init__(self, http_client: LiveSession):
@@ -34,18 +36,15 @@
 
         # we pass an out of the box http session
         response = command(self._http)
         json_response = response.json()
 
         # check if request was successful
         if not response.ok:
-
-            error_details = json_response.get("Message")
-            raise IPFSRuntimeError(
-                f"error trying to execute IPFS command `{type(command).__name__}`: {error_details}"
-            )
+            error_details = json_response.get('Message')
+            raise IPFSRuntimeError(f'error trying to execute IPFS command `{type(command).__name__}`: {error_details}')
 
         # ready to use response
         return json_response
 
 
-__all__ = ("RPC",)
+__all__ = ('RPC',)
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/ipfs/types.py` & `nucleus-sdk-0.1.0a0/nucleus/core/ipfs/types.py`

 * *Files identical despite different names*

### Comparing `nucleus-sdk-0.1.0/nucleus/core/logger.py` & `nucleus-sdk-0.1.0a0/nucleus/core/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-import os
 import logging
-import rich
+import os
 
-from rich import *  # type: ignore
+import rich
 from rich.logging import RichHandler
 
 # Get log level from env vars
-LOG_LEVEL = os.environ.get("LOGLEVEL", "DEBUG")
+LOG_LEVEL = os.environ.get('LOGLEVEL', 'DEBUG')
 
 
 # ref: https://rich.readthedocs.io/en/stable/console.html
 console = rich.console.Console(record=True)
 handler = RichHandler(
     rich_tracebacks=False,
     tracebacks_show_locals=False,
     console=console,
 )
 
 
 def factory(name: str, level: str = LOG_LEVEL):
     # create logger
-    fmt = "%(message)s"
+    fmt = '%(message)s'
     formatter = logging.Formatter(fmt)
     logger = logging.getLogger(name)
 
     if not logger.hasHandlers():
         logger.setLevel(level)
         handler.setFormatter(formatter)
         logger.addHandler(handler)
     return logger
 
 
 # Default logging
-core = factory("CORE")
-sdk = factory("SDK")
+core = factory('CORE')
+sdk = factory('SDK')
 
 __all__ = (
-    "core",
-    "sdk",
-    "logging",
-    "factory",
-    "console",
+    'core',
+    'sdk',
+    'logging',
+    'factory',
+    'console',
 )
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/subprocess/ipc.py` & `nucleus-sdk-0.1.0a0/nucleus/core/subprocess/ipc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import re
-import os
 import asyncio
-import subprocess
 import functools
+import os
+import re
+import subprocess
 
-from nucleus.core.types import Sequence, List, Union
+from nucleus.core.types import List, Sequence, Union
 
-from .protocol import StreamProtocol
-from .types import Reader, Loop, SubProcess, StdOut
 from .constants import EXIT_FAILURE, EXIT_SUCCESS
+from .protocol import StreamProtocol
+from .types import Loop, Reader, StdOut, SubProcess
 
 
 def _decode_bytes(b: bytes) -> str:
     """Helper function to decode bytes to string
 
     :param b: bytes to decode
     :return: string decoded
@@ -28,15 +28,15 @@
     :param line: input line to analyze
     :return: if process failed True is returned otherwise False.
     :rtype: str | None
     """
 
     for line in lines:
         # try find a fault in log lines
-        pattern = r"(\w+)?(Error|\[ERROR\])"  # what should we find?
+        pattern = r'(\w+)?(Error|\[ERROR\])'  # what should we find?
         match_found = re.search(pattern, line)
         if match_found:
             return line
 
     return None
 
 
@@ -48,15 +48,15 @@
     :rtype: StdOut
 
     """
 
     logs: List[str] = []
 
     async for lines in stream:
-        raw_lines = lines.split(b"\n")
+        raw_lines = lines.split(b'\n')
         decoded_lines = map(_decode_bytes, raw_lines)
         cleaned_lines = tuple(filter(len, decoded_lines))
         match_found = _match_faulty_line(cleaned_lines)
 
         if match_found:
             # even if the process do not exit with failure,
             # we can force return as failure if we find a fault error.
@@ -114,30 +114,28 @@
         We use a custom factory to stream process output.
 
         :return: subprocess instance
         :rtype: SubProcess
         """
 
         # execute nodejs command and communicate the data input
-        protocol_factory = functools.partial(
-            StreamProtocol, self._stream, loop=self._loop
-        )
+        protocol_factory = functools.partial(StreamProtocol, self._stream, loop=self._loop)
 
         # run the cmd shell command + return a Process instance.
         transport, protocol = await self._loop.subprocess_shell(
             protocol_factory,
             self._cmd,
             stderr=subprocess.PIPE,
             stdout=subprocess.PIPE,
             env=os.environ.copy(),
         )
 
         return SubProcess(transport, protocol, self._loop)
 
-    def communicate(self, data: bytes = b"") -> StdOut:
+    def communicate(self, data: bytes = b'') -> StdOut:
         """Communicate with process
 
         :param data: message sent to process
         :return: resulting output
         :rtype: Any
         """
         routine = asyncio.gather(self.pipe(data))
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/subprocess/protocol.py` & `nucleus-sdk-0.1.0a0/nucleus/core/subprocess/protocol.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 
 # Convention for importing types
 from nucleus.core.types import Any
-from .types import Reader, Loop
+
 from .constants import FILE_NO
+from .types import Loop, Reader
 
 
 class StreamProtocol(asyncio.subprocess.SubprocessStreamProtocol):
     """Like StreamReaderProtocol, but for a subprocess.
     ref: https://docs.python.org/3.6/library/asyncio-stream.html
     """
```

### Comparing `nucleus-sdk-0.1.0/nucleus/core/types.py` & `nucleus-sdk-0.1.0a0/nucleus/core/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from __future__ import annotations
 
-"""
-Types bridge "inherit" from global typing
-Use this `types` to handle global standard type definition
-
-Note: The Python runtime does not enforce function and variable type annotations.
-They can be used by third party tools such as type checkers, IDEs, linters, etc.
-
-refs:
-- https://docs.python.org/3/library/typing.html#module-typing
-- https://peps.python.org/pep-0544/#protocol-members
-- https://google.github.io/pytype/errors.html#bad-return-type
-
-"""
-
 import json
 import pathlib
 import urllib.parse as parse
-
 from collections import UserDict
+from types import *  # noqa: F403
+
+# "inherit" from global typing
+from typing import *  # noqa: F403
+
 from hexbytes import HexBytes
 from multiformats import CID as MultiFormatCID
 
-# "inherit" from global typing
-from typing import *  # type: ignore
-from types import *  # type: ignore
+"""
+    Types bridge "inherit" from global typing
+    Use this `types` to handle global standard type definition
+
+    Note: The Python runtime does not enforce function and variable type annotations.
+    They can be used by third party tools such as type checkers, IDEs, linters, etc.
+
+    refs:
+    - https://docs.python.org/3/library/typing.html#module-typing
+    - https://peps.python.org/pep-0544/#protocol-members
+    - https://google.github.io/pytype/errors.html#bad-return-type
+
+"""
+
 
 # https://docs.python.org/3/library/typing.html#typing.TypeVar
-T = TypeVar("T")
-T_contra = TypeVar("T_contra", contravariant=True)
-T_co = TypeVar("T_co", covariant=True)
+T = TypeVar('T')
+T_contra = TypeVar('T_contra', contravariant=True)
+T_co = TypeVar('T_co', covariant=True)
 
 Raw = Dict[Any, Any]
 ExceptionType = Type[Exception]
-HexStr = NewType("HexStr", str)
-Hash32 = NewType("Hash32", bytes)
+HexStr = NewType('HexStr', str)
+Hash32 = NewType('Hash32', bytes)
 Primitives = Union[bytes, int, bool]
 Hash = Union[HexBytes, Hash32]
 Func = Callable[..., Any]
 Dynamic = SimpleNamespace
 Setting = Iterator[Tuple[str, Any]]
 
 
@@ -106,29 +107,29 @@
         self._parsed = parse.urlparse(value)
 
     def __getattr__(self, name: str) -> str:
         """Proxy handling urlparse features"""
         return getattr(self._parsed, name)
 
     def valid(self) -> bool:
-        allowed_schemes = {"http", "https"}
+        allowed_schemes = {'http', 'https'}
         valid_scheme = self.scheme in allowed_schemes
         # contains a valid scheme and valid domain
         # ref: https://docs.python.org/3/library/urllib.parse.html
         return all((valid_scheme, self.netloc))
 
     @classmethod
     def __get_validators__(cls):
         """Add compat with pydantic validators"""
         yield cls.validate
 
     @classmethod
     def validate(cls, v: str):
         if not cls(v).valid():
-            raise ValueError("string must be a URL")
+            raise ValueError('string must be a URL')
 
 
 class Path(_ExtensibleStr):
 
     """Enhanced bridge string type extended with features needed to handle paths"""
 
     _path: pathlib.Path
@@ -148,28 +149,28 @@
     def __get_validators__(cls):
         """Add compat with pydantic validators"""
         yield cls.validate
 
     @classmethod
     def validate(cls, v: str):
         if not cls(v).exists():
-            raise ValueError("string must be a Path")
+            raise ValueError('string must be a Path')
 
 
 class JSON(UserDict[Any, Any]):
 
     """Enhanced bridge dict type extended with features needed to handle json structure"""
 
     def __str__(self) -> str:
         """Return json as json string"""
         return json.dumps(dict(self))
 
     def __bytes__(self) -> bytes:
         """Return json as bytes"""
-        return bytes(str(self), "utf-8")
+        return bytes(str(self), 'utf-8')
 
     def parse(self):
         return json.loads(str(self))
 
     def write(self, path: Path):
         """Create an output json file into output file with self
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/exceptions.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from nucleus.core.types import Any
 
 
 class HarvestingError(Exception):
     """Exception raised for errors related to harvesting tasks"""
 
     def __init__(self, message: str, *args: Any, **kwargs: Any):
-        self.message = f"SDK :: Harvesting -> {message}"
-        super(HarvestingError, self).__init__(self.message, *args, **kwargs)
+        self.message = f'SDK :: Harvesting -> {message}'
+        super().__init__(self.message, *args, **kwargs)
 
 
 class ProcessingError(Exception):
     """Exception raised for errors related to processing tasks"""
 
     def __init__(self, message: str, *args: Any, **kwargs: Any):
-        self.message = f"SDK :: Processing -> {message}"
-        super(ProcessingError, self).__init__(self.message, *args, **kwargs)
+        self.message = f'SDK :: Processing -> {message}'
+        super().__init__(self.message, *args, **kwargs)
 
 
 class StorageError(Exception):
     """Exception raised for errors related to storage tasks"""
 
     def __init__(self, message: str, *args: Any, **kwargs: Any):
-        self.message = f"SDK :: Storage -> {message}"
-        super(StorageError, self).__init__(
-            self.message, *args, **kwargs
-        )  # type: ignore
+        self.message = f'SDK :: Storage -> {message}'
+        super().__init__(self.message, *args, **kwargs)  # type: ignore
 
 
 class ModelManagerError(HarvestingError):
     """Raised when a model fails to persist or interact with the underlying cache.
     ModelManagerError error is a subclass from HarvestingError.
     """
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/expose/crypto.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/expose/crypto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
+
 from jwcrypto.common import json_encode  # type: ignore
+
 from nucleus.core.types import Raw
 
 from .key import KeyRing
 from .types import JWS, Serializer
 
 
 @dataclass(slots=True)
@@ -15,18 +17,18 @@
 
     # attach serializer as subscriber
     _s8r: Serializer
     # internal JWS interface
     _jws: JWS = field(init=False)
     # filter included members in jwk object
     __allowed__ = (
-        "crv",
-        "kty",
-        "x",
-        "y",
+        'crv',
+        'kty',
+        'x',
+        'y',
     )
 
     def __post_init__(self):
         """Initialize JWS instance
         ref: https://jwcrypto.readthedocs.io/en/latest/jws.html
         """
         self._jws = JWS(bytes(self._s8r))
@@ -35,20 +37,17 @@
         """Bind signers to JWS
 
         :param kr: keyring to assoc with signature
         :return: JWS object
         :rtype: JWS
         """
 
-        jwk: Raw = {
-            k: v for k, v in kr.jwk.items() if k in self.__allowed__
-        }  # type: ignore
-        header = {**{"alg": kr.alg.value, "jwk": jwk}, **dict(self._s8r)}
-        self._jws.add_signature(
-            kr.jwk, None, json_encode(header))  # type: ignore
+        jwk: Raw = {k: v for k, v in kr.jwk.items() if k in self.__allowed__}  # type: ignore
+        header = {**{'alg': kr.alg.value, 'jwk': jwk}, **dict(self._s8r)}
+        self._jws.add_signature(kr.jwk, None, json_encode(header))  # type: ignore
         return self
 
     def serialize(self) -> Serializer:
         """Trigger and notify to underneath serializer for JWS post-processing .
         In this step additional data could be added/modified into JWS.
 
         :return: an out of the box serializer
@@ -58,8 +57,8 @@
 
 
 class Cypher(Sign):
     # TODO pending implementation
     ...
 
 
-__all__ = ("Sign", "Cypher")
+__all__ = ('Sign', 'Cypher')
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/expose/key.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/expose/key.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from enum import Enum
-from .types import JWK
 
+from .types import JWK
 
 """
 We can support more
 ref: https://www.rfc-editor.org/rfc/rfc7518#section-3.1
 HS256	HMAC using SHA-256	Required
 HS384	HMAC using SHA-384	Optional
 HS512	HMAC using SHA-512	Optional
@@ -22,34 +22,34 @@
 PS512	RSASSA-PSS using SHA-512 and MGF1 with SHA-512	Optional
 none	No digital signature or MAC performed	Optional
 
 """
 
 
 class Use(str, Enum):
-    SIG = "sig"
-    ENC = "enc"
+    SIG = 'sig'
+    ENC = 'enc'
 
 
 class KeyType(str, Enum):
-    RSA = "RSA"
-    EllipticCurve = "EC"
+    RSA = 'RSA'
+    EllipticCurve = 'EC'
 
 
 class Curve(str, Enum):
-    HMAC = "HMAC"
-    P256 = "P-256"
-    ED25519 = "ED25519"
-    Secp256k1 = "secp256k1"
+    HMAC = 'HMAC'
+    P256 = 'P-256'
+    ED25519 = 'ED25519'
+    Secp256k1 = 'secp256k1'
 
 
 class Algorithm(str, Enum):
-    H256 = "H256"
-    ES256 = "ES256"
-    ES256K = "ES256K"
+    H256 = 'H256'
+    ES256 = 'ES256'
+    ES256K = 'ES256K'
 
 
 @dataclass(slots=True)
 class KeyRing:
     alg: Algorithm
     key_type: KeyType
     curve: Curve
@@ -64,8 +64,8 @@
             alg=self.alg.value,
             kty=self.key_type.value,
             curve=self.curve.value,
             use=self.use.value,
         )
 
 
-__all__ = ("KeyRing", "Algorithm", "Curve", "KeyType", "Use")
+__all__ = ('KeyRing', 'Algorithm', 'Curve', 'KeyType', 'Use')
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/expose/marshall.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/expose/marshall.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 from __future__ import annotations
 
-
 import hashlib
-import dag_cbor
 
+import dag_cbor
 from jwcrypto.common import json_decode  # type: ignore
-from nucleus.core.types import JSON, Raw, CID, Union, List
-from nucleus.sdk.storage import Store, Object
 
-from .types import JWS, JWE, Standard
+from nucleus.core.types import CID, JSON, List, Raw, Union
+from nucleus.sdk.storage import Object, Store
+
+from .types import JWE, JWS, Standard
 
 
-def cid_from_bytes(data: bytes, codec: str = "raw") -> CID:
+def cid_from_bytes(data: bytes, codec: str = 'raw') -> CID:
     """Return a new CIDv1 base32 based on data hash and codec.
 
     :param data: the data to create a new CID
     :param codec: the codec to use for the new CID
     :return: the new multi format cid object
     :rtype: CID
     """
     digest = hashlib.sha256(data).digest()
-    return CID.create("base32", 1, codec, ("sha2-256", digest))
+    return CID.create('base32', 1, codec, ('sha2-256', digest))
 
 
 class DagJose:
     """Dag-JOSE Serialization observer"""
 
     _cid: CID
     _s11n: JSON
     _cbor: bytes
     _header: Raw
     _std: Standard
 
     def __init__(self, standard: Standard):
         self._header = standard.header()
         self._cbor = dag_cbor.encode(standard.payload())
-        self._cid = cid_from_bytes(self._cbor, "dag-cbor")
+        self._cid = cid_from_bytes(self._cbor, 'dag-cbor')
 
     def __iter__(self):
         return iter(self._header.items())
 
     def __str__(self):
         return str(self._s11n)
 
@@ -49,15 +49,15 @@
         """
         return bytes(self._cid)
 
     def update(self, jwt: Union[JWS, JWE]) -> DagJose:
         """Encode JWS/JWE general serialization to dag-jose when crypto process get ready"""
         general_json = json_decode(jwt.serialize(False))  # type: ignore
         # set new state for serialization attribute
-        self._s11n = JSON({"link": self._cid, **general_json})
+        self._s11n = JSON({'link': self._cid, **general_json})
         return self
 
     def save_to(self, store: Store) -> Object:
         # 1. store cbor in blocks
         # 2. store serialization and return
         store(self._cbor)
         return store(self._s11n)
@@ -129,8 +129,8 @@
     def __bytes__(self) -> bytes:
         """SEP as compact serialization
         ref: https://www.rfc-editor.org/rfc/rfc7515#section-3.1
         """
         return bytes(self._payload)
 
 
-__all__ = ("DagJose", "Compact")
+__all__ = ('DagJose', 'Compact')
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/expose/metadata.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/expose/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from nucleus.core.types import CID, Optional, Dynamic
+from nucleus.core.types import CID, Dynamic, Optional
 
 
 class Structural(Dynamic):
     """Structural metadata implementation.
     https://github.com/SynapseMedia/sep/blob/main/SEP/SEP-001.md
     """
 
     cid: CID
     path: Optional[str] = None
 
     def __str__(self):
-        return "s"
+        return 's'
 
 
 class Descriptive(Dynamic):
     """Descriptive metadata implementation.
     https://github.com/SynapseMedia/sep/blob/main/SEP/SEP-001.md
     """
 
     name: str
     desc: str
 
     def __str__(self):
-        return "d"
+        return 'd'
 
 
 class Technical(Dynamic):
     """Technical metadata implementation.
     https://github.com/SynapseMedia/sep/blob/main/SEP/SEP-001.md
     """
 
     size: int
 
     def __str__(self):
-        return "t"
+        return 't'
 
 
-__all__ = ["Structural", "Descriptive", "Technical"]
+__all__ = ['Structural', 'Descriptive', 'Technical']
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/expose/partials.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/expose/partials.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from .key import Algorithm, Curve, KeyRing, KeyType, Use
 from .sep import SEP001, Header, Payload
-from .key import KeyRing, Algorithm, Curve, Use, KeyType
 
 
 def standard(type: str) -> SEP001:
     """SEP001 factory
 
     :param type: the type of media to expose
     :return: new standard implementation sep-001 object
@@ -25,11 +25,8 @@
         alg=Algorithm.ES256,
         key_type=KeyType.EllipticCurve,
         curve=Curve.P256,
         use=Use.SIG,
     )
 
 
-__all__ = (
-    "standard",
-    "es256",
-)
+__all__ = ('standard', 'es256')
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/expose/sep.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/expose/sep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
-
 from dataclasses import dataclass
-from nucleus.core.types import Raw, Optional, CID, Type
 
-from .key import KeyRing
+from nucleus.core.types import CID, Optional, Raw, Type
+
 from .crypto import Sign
+from .key import KeyRing
 from .marshall import DagJose
 from .types import Metadata, Serializer
 
 """Standard implementation for SEP-001 .
 ref: https://github.com/SynapseMedia/sep/blob/main/SEP/SEP-001.mdhttps://github.com/SynapseMedia/sep/blob/main/SEP/SEP-001.md
 """
 
@@ -89,8 +89,8 @@
         :param meta: the metadata type to store in payload
         :return: none
         :rtype: None
         """
         self._payload.add(meta)
 
 
-__all__ = ("SEP001", "Header", "Payload")
+__all__ = ('SEP001', 'Header', 'Payload')
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/expose/types.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/expose/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
-from nucleus.core.types import Protocol, Literal, Raw, Union, Setting
-from nucleus.sdk.storage import Store, Object
+from jwcrypto import jwe, jwk, jws
 
-from jwcrypto import jwk, jws, jwe
+from nucleus.core.types import Literal, Protocol, Raw, Setting, Union
+from nucleus.sdk.storage import Object, Store
 
-Claims = Literal["s", "d", "t"]
+Claims = Literal['s', 'd', 't']
 
 JWK = jwk.JWK
 JWS = jws.JWS
 JWE = jwe.JWE
 
 
 class Metadata(Protocol):
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/harvest/collectors.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/harvest/collectors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import pkgutil
 import inspect
 import itertools
+import pkgutil
+from collections import defaultdict
 
+from nucleus.core.types import JSON, Any, Iterator, Mapping
 
-from collections import defaultdict
-from nucleus.core.types import Iterator, Any, Mapping, JSON
 from .constants import COLLECTORS_PATH
 from .types import Collector
 
 
 def map(collectors: Iterator[Collector]) -> Mapping[str, Iterator[JSON]]:
     """Returns a map of collectors.
     Map collectors using name as key and the metadata content as value list.
@@ -41,18 +41,17 @@
 
     :param path: the path to search for submodules.
     :return: iterator of matched modules.
     :rtype: Iterator[Collector]
     """
 
     for module_finder, name, _ in pkgutil.iter_modules([path]):
-        module = module_finder.find_module(
-            name).load_module(name)  # type: ignore
+        module = module_finder.find_module(name).load_module(name)  # type: ignore
 
         # Get the module collector class
         for _, obj in inspect.getmembers(module):
             if not inspect.isabstract(obj) and inspect.isclass(obj):
                 if issubclass(obj, Collector):
                     yield obj()  # yield an instance of collector
 
 
-__all__ = ("load", "map", "merge")
+__all__ = ('load', 'map', 'merge')
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/harvest/media.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/harvest/media.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from nucleus.core.types import Path, Union, URL
+from nucleus.core.types import URL, Path, Union
+
 from .models import Media
 
 """
 Each specification defines how media types are processed and stored.
 The behavior of media types in the context of processing and storage is defined by each specification.
 """
 
@@ -19,10 +20,10 @@
 class Image(Collectable):
     """Image class establishes how the images should be processed"""
 
     ...
 
 
 __all__ = (
-    "Image",
-    "Video",
+    'Image',
+    'Video',
 )
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/harvest/models.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/harvest/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 from __future__ import annotations
 
-import pydantic
-import sqlite3
 import pickle
-import nucleus.core.cache as cache
-import nucleus.core.decorators as decorators
+import sqlite3
 
+import pydantic
 from pydantic import ValidationError
-from nucleus.core.cache import Connection
-from nucleus.core.types import Any, Union, Iterator, Path, Generic, T
 
+import nucleus.core.cache as cache
+import nucleus.core.decorators as decorators
+from nucleus.core.cache import Connection
+from nucleus.core.types import Any, Generic, Iterator, Path, T, Union
 from nucleus.sdk.exceptions import ModelManagerError, ModelValidationError
-from .constants import MIGRATE, INSERT, FETCH, MODELS_PATH
+
+from .constants import FETCH, INSERT, MIGRATE, MODELS_PATH
 
 
 class _Manager(pydantic.main.ModelMetaclass):
     """Database manager behavior.
 
     Each database file is created based on the class name.
     This metaclass prepare the connection to query to the right database according to the class name.
     """
 
     def __new__(mcs, name: Any, bases: Any, attrs: Any, **kwargs: Any):  # type: ignore
         """Start a new connection to cache database and ensure that the database is ready to receive requests."""
         db_path = Path(MODELS_PATH)
-        db_file = f"{db_path}/{name}.db"
+        db_file = f'{db_path}/{name}.db'
 
         super_new = super().__new__  # type: ignore
         # Ensure initialization is only performed for subclasses of _Model
-        is_subclass_instance = any(
-            map(lambda x: isinstance(x, _Manager), bases))
+        is_subclass_instance = any(map(lambda x: isinstance(x, _Manager), bases))
         if not is_subclass_instance:
             return super_new(mcs, name, bases, attrs, **kwargs)  # type: ignore
 
         # ensure that model directory exists
         if not db_path.exists():
             db_path.mkdir(parents=True)
 
         # connect and run migrations for model database
         conn = cache.connect(db_path=db_file)
         conn.execute(MIGRATE % (name, name))
         # add new attributes to class
-        new_attrs = {**{"_conn": conn, "_alias": name}, **attrs}
+        new_attrs = {**{'_conn': conn, '_alias': name}, **attrs}
         return super_new(mcs, name, bases, new_attrs, **kwargs)  # type: ignore
 
 
 class _BaseModel(pydantic.BaseModel, metaclass=_Manager):
     """This model defines a template to handle cache associated with each derived model"""
 
     _alias: str
@@ -58,19 +58,17 @@
         smart_union = True
         use_enum_values = True
         arbitrary_types_allowed = True
         anystr_strip_whitespace = True
 
     def __init__(self, *args: Any, **kwargs: Any):
         try:
-            super(_BaseModel, self).__init__(*args, **kwargs)
+            super().__init__(*args, **kwargs)
         except ValidationError as e:
-            raise ModelValidationError(
-                f"raised exception during model initialization: {str(e)}"
-            )
+            raise ModelValidationError(f'raised exception during model initialization: {str(e)}')
 
         sqlite3.register_converter(self._alias, pickle.loads)
         sqlite3.register_adapter(type(self), pickle.dumps)
 
     @classmethod
     @decorators.proxy_exception(
         expected=sqlite3.ProgrammingError,
@@ -145,8 +143,8 @@
 
         process(video)
     """
 
     path: T
 
 
-__all__ = ("Model", "Media")
+__all__ = ('Model', 'Media')
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/harvest/types.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/harvest/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
-
 # Convention for importing constants/types
 from abc import ABC, abstractmethod
-from nucleus.core.types import Iterator, JSON
+
+from nucleus.core.types import JSON, Iterator
 
 
 class Collector(ABC):
     """Abstract class for metadata collection.
     Collector define an abstraction with methods needed to handle metadata collection process.
     Subclasses should implement the __iter__ method to collect metadata from various data inputs.
     Use this class to create collector subtypes.
@@ -15,8 +15,8 @@
 
     @abstractmethod
     def __iter__(self) -> Iterator[JSON]:
         """Collect metadata from any kind of data input"""
         ...
 
 
-__all__ = ("Collector",)
+__all__ = ('Collector',)
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/processing/engines.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/processing/engines.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
-import re
 import inspect
 import mimetypes
-import PIL.Image
-import nucleus.sdk.processing as processing
-
+import re
 from collections import ChainMap
-from PIL.Image import Image as Pillow
+
+import PIL.Image
 from ffmpeg.nodes import FilterableStream as FFMPEG
+from PIL.Image import Image as Pillow
 
-from nucleus.core.types import Path, Any, no_type_check, Dynamic
+import nucleus.sdk.processing as processing
+from nucleus.core.types import Any, Dynamic, Path, no_type_check
 from nucleus.sdk.exceptions import ProcessingEngineError
+
 from .types import Engine, File, Introspection
 
 
 @no_type_check
 def _to_object(data: Any) -> Any:
     """Recursively convert a nested JSON as Dynamic object
 
@@ -71,36 +72,34 @@
             self._library.output(path, **output_args).run()  # type: ignore
 
             # after low level processing happen!!
             i8t = self.introspect(path)
             return File(path=path, meta=i8t)
         except Exception as e:
             # Standard exceptions raised
-            raise ProcessingEngineError(
-                f"error while trying to save video output: {str(e)}"
-            )
+            raise ProcessingEngineError(f'error while trying to save video output: {str(e)}')
 
 
 class ImageEngine(Engine):
     """Engine adapt Pillow to support image processing
     ref: https://pillow.readthedocs.io/en/stable/reference/Image.html
     """
 
     def __init__(self, lib: Pillow):
         # compile the pattern to avoid overhead in loop and bind underlying lib
-        self._pattern = re.compile(r"(?<!^)(?=[A-Z])")
+        self._pattern = re.compile(r'(?<!^)(?=[A-Z])')
         super().__init__(lib)
 
     def _to_snake_case(self, class_name: str) -> str:
         """Transform PascalCase class definition to snake_case method name
 
         :para name: the class name to parse
         :return: the snake case version for class name
         """
-        return self._pattern.sub("_", class_name).lower()
+        return self._pattern.sub('_', class_name).lower()
 
     def _setup_methods(self):
         """Call and chain methods based on configured options"""
         for class_name, params in self.compile():
             # The method to call should be the same as the option name.
             method = self._to_snake_case(class_name)
             func = getattr(self._library, method)
@@ -111,21 +110,19 @@
             self._library = func(**dict(params))
 
     def introspect(self, path: Path) -> Introspection:
         # fet the mime type from file path
         (mime_type, _) = mimetypes.guess_type(path)
         # get attributes from PIL.Image object
         members = inspect.getmembers(PIL.Image.open(path))
-        filter_private = filter(lambda x: not x[0].startswith("_"), members)
-        filter_method = filter(
-            lambda x: not inspect.ismethod(
-                x[1]), filter_private)
+        filter_private = filter(lambda x: not x[0].startswith('_'), members)
+        filter_method = filter(lambda x: not inspect.ismethod(x[1]), filter_private)
         image_introspection = _to_object(dict(filter_method))
         # patch to avoid size conflict keyword
-        delattr(image_introspection, "size")
+        delattr(image_introspection, 'size')
 
         # extend introspection with custom PIL.Image attributes
         return Introspection(
             size=path.size(),
             type=str(mime_type),
             **vars(image_introspection),
         )
@@ -137,13 +134,11 @@
             self._library.save(path)
 
             # after low level processing happen!!
             i8t = self.introspect(path)
             return File(path=path, meta=i8t)
         except Exception as e:
             # Standard exceptions raised
-            raise ProcessingEngineError(
-                f"error while trying to save image output: {str(e)}"
-            )
+            raise ProcessingEngineError(f'error while trying to save image output: {str(e)}')
 
 
-__all__ = ("VideoEngine", "ImageEngine")
+__all__ = ('VideoEngine', 'ImageEngine')
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/processing/image/options.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/processing/image/options.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from PIL.Image import Resampling
 from dataclasses import dataclass, field
+
+from PIL.Image import Resampling
+
 from nucleus.core.types import Tuple
 
 """All these settings are defined by pillow library.
-Option classes should be named in correspondence to the methods of the Pillow Image object and using the Python class naming convention.
+Option classes should be named in correspondence to the methods of the Pillow Image object 
+using the Python class naming convention.
+
 Underneath each class is parsed as a method to setup pillow image object.
 ref: https://pillow.readthedocs.io/en/stable/reference/Image.html#PIL.Image.Image.resize
 
 eg:
     # after parsing
     class RemapPalette(Option) = image.remap_palette(...)
         ...
@@ -35,15 +39,15 @@
     """Crop image returns a rectangular region from this image
     ref: https://pillow.readthedocs.io/en/stable/reference/Image.html#PIL.Image.Image.crop
     """
 
     box: Coord
 
     def __iter__(self):
-        yield "box", (
+        yield 'box', (
             self.box.left,
             self.box.top,
             self.box.right,
             self.box.bottom,
         )
 
 
@@ -68,13 +72,13 @@
     def crop(self, box: Coord):
         self._box = (box.left, box.top, box.right, box.bottom)
 
     def resample(self, resample: Resampling):
         self._resample = resample
 
     def __iter__(self):
-        yield "size", self._size
-        yield "resample", self._resample
-        yield "box", self._box
+        yield 'size', self._size
+        yield 'resample', self._resample
+        yield 'box', self._box
 
 
-__all__ = ("Crop", "Coord", "Resize", "Resampling")
+__all__ = ('Crop', 'Coord', 'Resize', 'Resampling')
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/processing/process.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/processing/process.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-import ffmpeg
 import functools
+
+import ffmpeg
 import PIL.Image as PIL
 
 from nucleus.core.types import Path
-from nucleus.sdk.harvest import Video, Image
+from nucleus.sdk.harvest import Image, Video
 
-from .engines import VideoEngine, ImageEngine
+from .engines import ImageEngine, VideoEngine
 from .types import Engine, Processable
 
 
 @functools.singledispatch
 def engine(media: Processable) -> Engine:
     """Engine single dispatch factory.
     Use the media input to infer the right engine.
 
     :param media: the media to dispatch
     :param kwargs: these args are passed directly to library.
     :return: engine instance
     :rtype: Engine
     """
-    raise NotImplementedError(f"cannot process not registered media `{media}")
+    raise NotImplementedError(f'cannot process not registered media `{media}')
 
 
 @engine.register
 def _(media: Video) -> VideoEngine:
     input_path = Path(media.path)
     library = ffmpeg.input(input_path)  # type: ignore
     return VideoEngine(library)  # type: ignore
@@ -32,8 +33,8 @@
 @engine.register
 def _(media: Image) -> ImageEngine:
     input_path = Path(media.path)
     library = PIL.open(input_path)
     return ImageEngine(library)
 
 
-__all__ = ("engine",)
+__all__ = ('engine',)
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/processing/types.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/processing/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from __future__ import annotations
-from abc import abstractmethod, ABC
-from nucleus.sdk.harvest import Media
+
+from abc import ABC, abstractmethod
+
 from nucleus.core.types import (
-    Path,
-    Iterator,
     URL,
-    Union,
-    List,
-    Tuple,
     Any,
-    Settings,
     Dynamic,
+    Iterator,
+    List,
+    Path,
+    Settings,
+    Tuple,
+    Union,
 )
-
+from nucleus.sdk.harvest import Media
 
 # Alias for allowed engine inputs
 Processable = Media[Union[Path, URL]]
 Compilation = Iterator[Tuple[str, Any]]
 
 
 class Introspection(Dynamic):
     """Introspection hold internal media information/metadata.
-    For each result the media metadata is associated as `meta` and it could change based on media type and underneath library.
+    For each result the media metadata is associated as `meta` and it could change
+    based on media type and underneath library.
 
     eg.
         # could be related to ffprobe video info or PIL.Image, etc
         video = Introspection(**ffprobe)
         image = Introspection(**PIL.Image)
 
         # in this case introspection dynamically receive all the metadata from the underneath library output
-        # the "WARNING" here is that based on media type the introspection content could change and needs an extra review.
+        # the "WARNING" here is that based on media type
+        # the introspection content could change and needs an extra review.
     """
 
     size: int
     # we expect to fill this field with IANA Media types
     # https://www.iana.org/assignments/media-types/media-types.xhtml
     type: str
 
@@ -46,15 +49,16 @@
     # associated file introspection
     meta: Introspection
     ...
 
 
 class Engine(ABC):
     """Engine implements a media engine template/adapter.
-    It uses an underlying library as an interface to process media files and produce output based on the provided settings.
+    It uses an underlying library as an interface to process media files.
+    It produce output based on the provided settings.
     Use this class to create engine subtypes.
     """
 
     _library: Any
     _settings: List[Settings]
 
     def __init__(self, lib: Any):
@@ -100,8 +104,8 @@
         :return: new media path
         :rtype: File
         :raises ProcessingEngineError: if any exception is captured during processing
         """
         ...
 
 
-__all__ = ("Engine", "File", "Introspection")
+__all__ = ('Engine', 'File', 'Introspection')
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/processing/video/codecs.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/processing/video/codecs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,92 @@
 from nucleus.core.types import Literal
+
 from .constants import (
-    DEFAULT_KEY_MIN,
-    DEFAULT_GOP,
+    DEFAULT_AUDIO_CODEC,
     DEFAULT_CRF,
+    DEFAULT_GOP,
+    DEFAULT_KEY_MIN,
     DEFAULT_SC_THRESHOLD,
-    DEFAULT_AUDIO_CODEC,
 )
 
 
 class Copy:
     """Format used to `copy` the codec from the source to the output.
     Special value copy (output only) to indicate that the stream is not to be re-encoded.
     ref: https://ffmpeg.org/ffmpeg.html#Main-options
 
     """
 
     _stream_specifier: str
 
-    def __init__(self, stream: Literal["v", "a"] = "v"):
+    def __init__(self, stream: Literal['v', 'a'] = 'v'):  # noqa: F821
         self._stream_specifier = stream
 
     def __contains__(self, codec: str) -> bool:
         ...
 
     def __iter__(self):
-        yield f"c:{self._stream_specifier}", "copy"
+        yield f'c:{self._stream_specifier}', 'copy'
 
 
 class H264:
     """Represent H264 codec with default options.
     ref: https://trac.ffmpeg.org/wiki/Encode/H.264
 
     """
 
     def __contains__(self, codec: str) -> bool:
-        videos = ["libx264", "h264", "h264_afm", "h264_nvenc"]
-        audios = ["aac", "libvo_aacenc", "libfaac", "libmp3lame", "libfdk_aac"]
+        videos = ['libx264', 'h264', 'h264_afm', 'h264_nvenc']
+        audios = ['aac', 'libvo_aacenc', 'libfaac', 'libmp3lame', 'libfdk_aac']
         allowed_codecs = videos + audios
         return codec in allowed_codecs
 
     def __iter__(self):
-        yield "bf", 1
-        yield "g", DEFAULT_GOP
-        yield "crf", DEFAULT_CRF
-        yield "keyint_min", DEFAULT_KEY_MIN
-        yield "sc_threshold", DEFAULT_SC_THRESHOLD
-        yield "c:a", DEFAULT_AUDIO_CODEC
-        yield "c:v", "libx264"
+        yield 'bf', 1
+        yield 'g', DEFAULT_GOP
+        yield 'crf', DEFAULT_CRF
+        yield 'keyint_min', DEFAULT_KEY_MIN
+        yield 'sc_threshold', DEFAULT_SC_THRESHOLD
+        yield 'c:a', DEFAULT_AUDIO_CODEC
+        yield 'c:v', 'libx264'
 
 
 class HEVC:
     """Represent HEVC codec with default options.
     ref: https://trac.ffmpeg.org/wiki/Encode/H.265
 
     """
 
     def __contains__(self, codec: str) -> bool:
-        videos = ["libx265", "h265"]
-        audios = ["aac", "libvo_aacenc", "libfaac", "libmp3lame", "libfdk_aac"]
+        videos = ['libx265', 'h265']
+        audios = ['aac', 'libvo_aacenc', 'libfaac', 'libmp3lame', 'libfdk_aac']
         allowed_codecs = videos + audios
         return codec in allowed_codecs
 
     def __iter__(self):
-        yield "g", DEFAULT_GOP
-        yield "crf", DEFAULT_CRF
-        yield "keyint_min", DEFAULT_KEY_MIN
-        yield "sc_threshold", DEFAULT_SC_THRESHOLD
-        yield "c:a", DEFAULT_AUDIO_CODEC
-        yield "c:v", "libx265"
-        yield "x265-params", "lossless=1"
+        yield 'g', DEFAULT_GOP
+        yield 'crf', DEFAULT_CRF
+        yield 'keyint_min', DEFAULT_KEY_MIN
+        yield 'sc_threshold', DEFAULT_SC_THRESHOLD
+        yield 'c:a', DEFAULT_AUDIO_CODEC
+        yield 'c:v', 'libx265'
+        yield 'x265-params', 'lossless=1'
 
 
 class VP9:
     """Represent Vp9 codec with default options.
     ref: https://trac.ffmpeg.org/wiki/Encode/VP9
 
     """
 
     def __contains__(self, codec: str) -> bool:
-        videos = ["libvpx", "libvpx-vp9"]
-        audios = ["aac", "libvo_aacenc", "libfaac", "libmp3lame", "libfdk_aac"]
+        videos = ['libvpx', 'libvpx-vp9']
+        audios = ['aac', 'libvo_aacenc', 'libfaac', 'libmp3lame', 'libfdk_aac']
         allowed_codecs = videos + audios
         return codec in allowed_codecs
 
     def __iter__(self):
-        yield "c:a", DEFAULT_AUDIO_CODEC
-        yield "c:v", "libvpx-vp9"
+        yield 'c:a', DEFAULT_AUDIO_CODEC
+        yield 'c:v', 'libvpx-vp9'
 
 
-__all__ = ("HEVC", "VP9", "H264", "Copy")
+__all__ = ('HEVC', 'VP9', 'H264', 'Copy')
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/processing/video/constants.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/processing/video/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # ref:
 # https://developer.apple.com/documentation/http_live_streaming/http_live_streaming_hls_authoring_specification_for_apple_devices
 
 # Transcode constants
 HLS_TIME = 10
 HLS_LIST_SIZE = 0
-HLS_TAG_VIDEO_FORMAT = "hvc1"
-HLS_PLAYLIST_TYPE = "vod"
+HLS_TAG_VIDEO_FORMAT = 'hvc1'
+HLS_PLAYLIST_TYPE = 'vod'
 
 
-DEFAULT_AUDIO_CODEC = "aac"
+DEFAULT_AUDIO_CODEC = 'aac'
 # The range of the CRF scale is 0–51, where 0 is lossless (higher quality)
 DEFAULT_CRF = 0
 # The preset determines compression efficiency and therefore affects encoding speed
 # This option itemizes a range of choices from veryfast (best speed) to
 # veryslow (best quality).
-DEFAULT_PRESET = "slow"
+DEFAULT_PRESET = 'slow'
 # keyframes minimum every 100 frames
 DEFAULT_KEY_MIN = 25
 # maximum amount of GOP size, maximum every 100 frames there will be a
 # keyframe, together with -keyint_min this gives a keyframe every 100
 # frames
 DEFAULT_GOP = 250
 # ffmpeg has scene detection. 0 (stands for false)
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/processing/video/ffprobe.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/processing/video/ffprobe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ffmpeg
 
 # Convention for importing types
-from nucleus.core.types import Path, Any, JSON
+from nucleus.core.types import JSON, Any, Path
 from nucleus.sdk.exceptions import FFProbeError
 
 
 # TODO add auto_probe feature to encoding step
 # TODO set video->0, audio->1 streams methods
 def probe(path: Path, **kwargs: Any) -> JSON:
     """Run ffprobe on the specified file and return a JSON representation of the output.
@@ -14,11 +14,11 @@
     :return: JSON representation of the output
     :rtype: JSON
     :raises FFProbeError: if the file path does not exist
     """
     try:
         return JSON(ffmpeg.probe(path, **kwargs))  # type: ignore
     except ffmpeg._run.Error as e:  # type: ignore
-        raise FFProbeError(f"error during ffprobe command call: {str(e)}")
+        raise FFProbeError(f'error during ffprobe command call: {str(e)}')
 
 
-__all__ = ("probe",)
+__all__ = ('probe',)
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/processing/video/options.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/processing/video/options.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
-from nucleus.core.types import Mapping, Any
+
+from nucleus.core.types import Any, Mapping
 
 """
 aspect ratio	H.264/AVC kb/s	Frame rate
 416 x 234	    145 	        ≤ 30 fps
 640 x 360	    365             ≤ 30 fps
 768 x 432	    730, 1100       ≤ 30 fps
 960 x 540	    2000	        same as source
@@ -26,63 +27,62 @@
 
     _custom: Mapping[str, Any]
 
     def __init__(self, **kwargs: Any):
         self._custom = kwargs
 
     def __iter__(self):
-        for k, v in self._custom.items():
-            yield k, v
+        yield from self._custom.items()
 
 
 @dataclass(slots=True)
 class FrameSize:
     """Set frame size.
     ref: https://ffmpeg.org/ffmpeg.html#Main-options
     """
 
     width: int
     height: int
 
     def __str__(self) -> str:
-        return f"{self.width}x{self.height}"
+        return f'{self.width}x{self.height}'
 
     def __iter__(self):
-        yield "s", str(self)
+        yield 's', str(self)
 
 
 @dataclass(slots=True)
 class FPS:
     """Set frame rate (Hz value, fraction or abbreviation).
     ref: https://ffmpeg.org/ffmpeg.html#Main-options
     """
 
     fps: float
 
     def __iter__(self):
-        yield "r", self.fps
+        yield 'r', self.fps
 
 
 @dataclass(slots=True)
 class BR:
     """Video/Audio bitrate
     ref: https://ffmpeg.org/ffmpeg.html#Main-options
     """
 
     video: int
     audio: int = 0
 
     def __iter__(self):
         # if we only receive video bitrate, we consider it as overall bitrate
         if self.video and not self.audio:
-            yield "b", f"{self.video}k"
+            yield 'b', f'{self.video}k'
             return
 
-        yield "b:v", f"{self.video}k"
-        yield "b:a", f"{self.audio}k"
+        yield 'b:v', f'{self.video}k'
+        yield 'b:a', f'{self.audio}k'
 
 
 @dataclass(frozen=True)
 class Bitrate:
     B240 = BR(150, 94)
     B360 = BR(276, 128)
     B480 = BR(750, 192)
@@ -99,8 +99,8 @@
     Q480 = FrameSize(854, 480)
     Q720 = FrameSize(1280, 720)
     Q1080 = FrameSize(1920, 1080)
     Q2k = FrameSize(2560, 1440)
     Q4k = FrameSize(3840, 2160)
 
 
-__all__ = ("FPS", "FrameSize", "Screen", "Bitrate", "BR", "Custom")
+__all__ = ('FPS', 'FrameSize', 'Screen', 'Bitrate', 'BR', 'Custom')
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/processing/video/types.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/processing/video/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from nucleus.core.types import Protocol, Settings
 
 
 class Codec(Settings, Protocol):
     """Codec compression abstraction.
     ref: https://trac.ffmpeg.org/wiki/Encode/VP9
     ref: https://trac.ffmpeg.org/wiki/Encode/H.265
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/storage/clients.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/storage/clients.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import nucleus.core.http as http_client
-
 from dataclasses import dataclass
+
+import nucleus.core.http as http_client
 from nucleus.core.http import Response
-from nucleus.core.types import CID, Any, JSON, URL
+from nucleus.core.types import CID, JSON, URL, Any
 from nucleus.sdk.exceptions import StorageServiceError
 
-from .types import Pin, Object
 from .constants import ESTUARY_API_PIN, ESTUARY_API_PUBLIC
+from .types import Object, Pin
 
 
 @dataclass
 class EstuaryClient:
     """Estuary client implements Service"""
 
     endpoint: URL
     key: str
 
     def __post_init__(self):
         self._http = http_client.live_session(self.endpoint)
-        self._http.headers.update({"Authorization": f"Bearer {self.key}"})
+        self._http.headers.update({'Authorization': f'Bearer {self.key}'})
 
     def _safe_request(self, res: Response) -> JSON:
         """Amplifier helper method to handle response from Estuary API
 
         :param res: expected response
         :return: json response
         :rtype: JSON
@@ -38,68 +38,66 @@
             Observable behavior:
                 {
                     "code": 0,
                     "details": "string",
                     "reason": "string"
                 }
             """
-            error_description = response["error"]["details"]
-            raise StorageServiceError(
-                f"exception raised during request: {error_description}"
-            )
+            error_description = response['error']['details']
+            raise StorageServiceError(f'exception raised during request: {error_description}')
 
         return JSON(response)
 
     def _content_by_cid(self, cid: CID) -> JSON:
         """Collect details from estuary based on CID
         ref: https://docs.estuary.tech/Reference/SwaggerUI#/public/get_public_by_cid__cid_
 
         :param cid: cid to retrieve content details
         :return: cid content details
         :rtype: JSON
         :raises EdgePinException: if pin request fails
         """
 
-        content_uri = f"{ESTUARY_API_PUBLIC}/by-cid/{cid}"
+        content_uri = f'{ESTUARY_API_PUBLIC}/by-cid/{cid}'
         req = self._http.get(content_uri)
 
         # expected response as json
         response = self._safe_request(req)
-        return response.get("content", {})
+        return response.get('content', {})
 
     def pin(self, obj: Object, **kwargs: Any) -> Pin:
         """Pin cid into estuary
 
         :param obj: object to pin
         :return: pin object
         :rtype: Pin
         :raises StorageServiceError: if pin request fails
         """
         # ref:
         # https://docs.estuary.tech/Reference/SwaggerUI#/pinning/post_pinning_pins
-        data = {"cid": obj.hash, **kwargs}
+        data = {'cid': obj.hash, **kwargs}
         req = self._http.post(ESTUARY_API_PIN, data=data)
         json_response = self._safe_request(req)
 
         return Pin(
-            cid=json_response["cid"],
-            name=json_response["name"],
-            status="pending",
+            cid=json_response['cid'],
+            name=json_response['name'],
+            status='pending',
         )
 
     def unpin(self, obj: Object) -> CID:
         """Remove pin from estuary
 
         :param obj: object to remove from service
         :return: just removed CID
         :rtype: CID
         :raises StorageServiceError: if an error occurs during request
         """
         # content id is same as pin id
-        pin_id = self._content_by_cid(obj.hash).get("id")
-        response = self._http.delete(f"{ESTUARY_API_PIN}/{pin_id}")
+        pin_id = self._content_by_cid(obj.hash).get('id')
+        response = self._http.delete(f'{ESTUARY_API_PIN}/{pin_id}')
         # If error happens then raise standard exception.
         self._safe_request(response)
         return obj.hash
 
 
-__all__ = ["EstuaryClient"]
+__all__ = ['EstuaryClient']
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/storage/edge.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/storage/edge.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import functools
 
-from .services import Estuary
 from .clients import EstuaryClient
-from .types import Service, Client
+from .services import Estuary
+from .types import Client, Service
 
 
 @functools.singledispatch
 def client(svc: Service) -> Client:
     """Client single dispatch factory.
     Use the model input to infer the right storage service.
 
     :param model: the model to dispatch
     :return: edge service client instance
     :rtype: Edge
     """
-    raise NotImplementedError(f"cannot process not registered storable `{svc}")
+    raise NotImplementedError(f'cannot process not registered storable `{svc}')
 
 
 @client.register
 def _(svc: Estuary):
     """Return a estuary api client with the specified service settings."""
     return EstuaryClient(
         endpoint=svc.endpoint(),
         key=svc.key(),
     )
 
 
-__all__ = ("client",)
+__all__ = ('client',)
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/storage/store.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/storage/store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import functools
-import nucleus.core.ipfs as ipfs_
 
-from nucleus.core.types import CID, Optional, JSON
-from nucleus.core.ipfs import File, Text, Add, BlockPut, DagPut
+import nucleus.core.ipfs as ipfs_
+from nucleus.core.ipfs import Add, BlockPut, DagPut, File, Text
+from nucleus.core.types import CID, JSON, Optional
 from nucleus.sdk.processing import File as FileType
-from .types import Storable, Object, Store
+
+from .types import Object, Storable, Store
 
 
 def ipfs(endpoint: Optional[str] = None) -> Store:
     """HOF to handle storage endpoint and return a singledispatch generic function.
     A form of generic function dispatch where the implementation is chosen based on the type of a single argument.
     ref: https://docs.python.org/3/glossary.html#term-single-dispatch
 
@@ -25,16 +26,15 @@
         """Storage single dispatch factory.
         Use the data input type to infer the right storage strategy.
 
         :param data: the model to dispatch
         :return: Object instance
         :rtype: Object
         """
-        raise NotImplementedError(
-            f"cannot process not registered storable `{data}")
+        raise NotImplementedError(f'cannot process not registered storable `{data}')
 
     @store.register
     def _(data: FileType) -> Object:
         """Add a file to IPFS
 
         :param data: the file model to store
         :return: stored instance
@@ -43,17 +43,17 @@
         """
         command = Add(File(data.path))
         # expected /add output from API
         # {Hash: .., Name: .., Size: ...}
         file_output = api(command)
 
         return Object(
-            name=file_output["Name"],
-            hash=CID(file_output["Hash"]),
-            size=int(file_output["Size"]),
+            name=file_output['Name'],
+            hash=CID(file_output['Hash']),
+            size=int(file_output['Size']),
         )
 
     @store.register
     def _(data: bytes) -> Object:
         """Add bytes to ipfs
 
         :param data: bytes to store
@@ -63,29 +63,29 @@
 
         command = BlockPut(Text(data))
         # expected block/put output from API
         # {Key: .., Size: ..}
         output = api(command)
 
         return Object(
-            name=output["Key"],
-            hash=CID(output["Key"]),
+            name=output['Key'],
+            hash=CID(output['Key']),
             size=len(data),
         )
 
     @store.register
     def _(data: str) -> Object:
         """Add JSON metadata representation to ipfs
 
         :param data: string to store
         :return: object instance
         :rtype: Object
         """
 
-        bytes_ = data.encode("utf-8")
+        bytes_ = data.encode('utf-8')
         return store(bytes_)
 
     @store.register
     def _(data: JSON) -> Object:
         """Add JSON metadata representation to ipfs
 
         :param data: json to store
@@ -94,19 +94,19 @@
         """
 
         bytes_ = bytes(data)
         command = DagPut(Text(bytes_))
         # expected block/put output from API
         # {"Cid": { "/": "<cid-string>" }}
         output = api(command)
-        raw_cid = output["Cid"]["/"]
+        raw_cid = output['Cid']['/']
 
         return Object(
             name=raw_cid,
             hash=CID(raw_cid),
             size=len(data),
         )
 
     return store
 
 
-__all__ = ("ipfs",)
+__all__ = ('ipfs',)
```

### Comparing `nucleus-sdk-0.1.0/nucleus/sdk/storage/types.py` & `nucleus-sdk-0.1.0a0/nucleus/sdk/storage/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from dataclasses import dataclass
 from nucleus.sdk.processing import File
 from nucleus.core.types import (
-    Protocol,
     CID,
+    JSON,
+    URL,
+    Callable,
     NewType,
     Optional,
+    Protocol,
     Union,
-    URL,
-    Callable,
-    JSON,
     runtime_checkable,
 )
 
 
+
 @dataclass(slots=True)
 class Object:
     """Distributed/Stored media representation.
     This class is used to infer any media decentralized and already stored in IPFS
     """
 
     hash: CID
@@ -30,15 +31,15 @@
 
     cid: CID
     status: str
     name: Optional[str]
 
 
 # Alias for allowed media to store
-ID = NewType("ID", str)
+ID = NewType('ID', str)
 Storable = Union[File, JSON, str, bytes]
 Store = Callable[[Storable], Object]
 
 
 @runtime_checkable
 class Service(Protocol):
     """Storage abstraction to manage the configuration needed to connect to services.
@@ -60,15 +61,15 @@
         :rtype: str
         """
         ...
 
 
 class Client(Protocol):
     """Client provides an standard interface to handle ipfs storage services.
-    Each storage service represent a remote cache service like 'pinata', 'filebase' or any service that support remote pinning service.
+    Each storage service represent a remote cache service like eg. estuary'
     Use this class to create edge services subtypes.
     """
 
     def pin(self, obj: Object) -> Pin:
         """Pin cid into remote storage
 
         :param obj: object to pin
@@ -83,8 +84,8 @@
         :param obj: object to remove from service
         :return: just removed object cid
         :rtype: CID
         """
         ...
 
 
-__all__ = ("Pin", "Service", "Storable", "Store", "Client", "Object")
+__all__ = ('Pin', 'Service', 'Storable', 'Store', 'Client', 'Object')
```

### Comparing `nucleus-sdk-0.1.0/nucleus_sdk.egg-info/SOURCES.txt` & `nucleus-sdk-0.1.0a0/nucleus_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 nucleus/__init__.py
 nucleus/core/__init__.py
 nucleus/core/constants.py
 nucleus/core/dataclass.py
 nucleus/core/decorators.py
 nucleus/core/exceptions.py
@@ -79,8 +80,9 @@
 nucleus/sdk/storage/services.py
 nucleus/sdk/storage/store.py
 nucleus/sdk/storage/types.py
 nucleus_sdk.egg-info/PKG-INFO
 nucleus_sdk.egg-info/SOURCES.txt
 nucleus_sdk.egg-info/dependency_links.txt
 nucleus_sdk.egg-info/not-zip-safe
+nucleus_sdk.egg-info/requires.txt
 nucleus_sdk.egg-info/top_level.txt
```

