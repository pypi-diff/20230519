# Comparing `tmp/rnspure-0.5.2.tar.gz` & `tmp/rnspure-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnspure-0.5.2.tar", last modified: Fri May 12 10:36:54 2023, max compression
+gzip compressed data, was "rnspure-0.5.3.tar", last modified: Fri May 19 09:34:49 2023, max compression
```

## Comparing `rnspure-0.5.2.tar` & `rnspure-0.5.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:54.397606 rnspure-0.5.2/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1110 2022-10-20 15:25:41.000000 rnspure-0.5.2/LICENSE
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18698 2023-05-12 10:36:54.397606 rnspure-0.5.2/PKG-INFO
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    17959 2023-05-05 09:14:48.000000 rnspure-0.5.2/README.md
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:54.390940 rnspure-0.5.2/RNS/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10508 2023-05-10 16:48:56.000000 rnspure-0.5.2/RNS/Buffer.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24440 2023-05-11 19:18:34.000000 rnspure-0.5.2/RNS/Channel.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:54.390940 rnspure-0.5.2/RNS/Cryptography/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2735 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/AES.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      988 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/Ed25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3705 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/Fernet.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1961 2023-03-02 11:05:06.000000 rnspure-0.5.2/RNS/Cryptography/HKDF.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6885 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/HMAC.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      769 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/Hashes.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1541 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/PKCS7.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      794 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/Provider.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2611 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/Proxies.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4777 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/SHA256.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5589 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/SHA512.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4917 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/X25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      929 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/__init__.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:54.390940 rnspure-0.5.2/RNS/Cryptography/aes/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       20 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/aes/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8905 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/aes/aes.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7045 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/aes/utils.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:54.390940 rnspure-0.5.2/RNS/Cryptography/pure25519/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        0 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/pure25519/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1939 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/pure25519/_ed25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13056 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/pure25519/basic.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8193 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/pure25519/ed25519_oop.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3156 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Cryptography/pure25519/eddsa.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    20638 2023-02-09 10:50:55.000000 rnspure-0.5.2/RNS/Destination.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24033 2022-12-21 18:12:50.000000 rnspure-0.5.2/RNS/Identity.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:54.394273 rnspure-0.5.2/RNS/Interfaces/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14502 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Interfaces/AX25KISSInterface.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:54.394273 rnspure-0.5.2/RNS/Interfaces/Android/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    16723 2022-10-20 17:46:53.000000 rnspure-0.5.2/RNS/Interfaces/Android/KISSInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    49037 2023-05-02 15:44:28.000000 rnspure-0.5.2/RNS/Interfaces/Android/RNodeInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10335 2022-10-20 17:46:58.000000 rnspure-0.5.2/RNS/Interfaces/Android/SerialInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1290 2022-10-20 17:28:52.000000 rnspure-0.5.2/RNS/Interfaces/Android/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    20327 2023-05-11 17:33:15.000000 rnspure-0.5.2/RNS/Interfaces/AutoInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    41416 2022-11-03 21:46:26.000000 rnspure-0.5.2/RNS/Interfaces/I2PInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     3654 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Interfaces/Interface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13773 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Interfaces/KISSInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12932 2023-05-10 13:51:28.000000 rnspure-0.5.2/RNS/Interfaces/LocalInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6583 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Interfaces/PipeInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    30633 2023-05-02 15:44:01.000000 rnspure-0.5.2/RNS/Interfaces/RNodeInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7408 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Interfaces/SerialInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    21620 2023-05-04 21:14:01.000000 rnspure-0.5.2/RNS/Interfaces/TCPInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4206 2023-05-04 21:15:49.000000 rnspure-0.5.2/RNS/Interfaces/UDPInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     1321 2022-10-21 23:31:41.000000 rnspure-0.5.2/RNS/Interfaces/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    52943 2023-05-11 14:21:07.000000 rnspure-0.5.2/RNS/Link.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    22263 2023-05-11 13:48:09.000000 rnspure-0.5.2/RNS/Packet.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    45887 2023-05-10 13:26:58.000000 rnspure-0.5.2/RNS/Resource.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    65220 2023-05-05 08:37:31.000000 rnspure-0.5.2/RNS/Reticulum.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)   129920 2023-05-11 13:43:33.000000 rnspure-0.5.2/RNS/Transport.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:54.394273 rnspure-0.5.2/RNS/Utilities/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1291 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Utilities/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14872 2023-02-02 12:40:06.000000 rnspure-0.5.2/RNS/Utilities/rncp.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    25425 2023-05-09 18:30:37.000000 rnspure-0.5.2/RNS/Utilities/rnid.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)   208355 2023-05-09 13:30:30.000000 rnspure-0.5.2/RNS/Utilities/rnodeconf.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12583 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Utilities/rnpath.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6588 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/Utilities/rnprobe.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    12818 2023-05-02 14:47:11.000000 rnspure-0.5.2/RNS/Utilities/rnsd.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9818 2023-03-08 12:57:44.000000 rnspure-0.5.2/RNS/Utilities/rnstatus.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    26422 2023-02-02 12:55:50.000000 rnspure-0.5.2/RNS/Utilities/rnx.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7088 2023-03-04 17:36:37.000000 rnspure-0.5.2/RNS/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       22 2023-05-09 21:07:38.000000 rnspure-0.5.2/RNS/_version.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:54.394273 rnspure-0.5.2/RNS/vendor/
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)      166 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/vendor/__init__.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    89634 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/vendor/configobj.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:54.394273 rnspure-0.5.2/RNS/vendor/i2plib/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      667 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/vendor/i2plib/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      316 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/vendor/i2plib/__version__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9939 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/vendor/i2plib/aiosam.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1158 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/vendor/i2plib/exceptions.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      122 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/vendor/i2plib/log.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4397 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/vendor/i2plib/sam.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8983 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/vendor/i2plib/tunnel.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1203 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/vendor/i2plib/utils.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:54.394273 rnspure-0.5.2/RNS/vendor/ifaddr/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1432 2023-05-05 08:23:36.000000 rnspure-0.5.2/RNS/vendor/ifaddr/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3646 2023-05-05 08:19:48.000000 rnspure-0.5.2/RNS/vendor/ifaddr/_posix.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7321 2023-05-05 08:20:00.000000 rnspure-0.5.2/RNS/vendor/ifaddr/_shared.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5107 2023-05-05 08:20:05.000000 rnspure-0.5.2/RNS/vendor/ifaddr/_win32.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1141 2023-05-05 08:36:33.000000 rnspure-0.5.2/RNS/vendor/ifaddr/niwrapper.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1184 2022-10-21 23:31:14.000000 rnspure-0.5.2/RNS/vendor/platformutils.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    34549 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/vendor/six.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    43449 2022-10-20 15:25:41.000000 rnspure-0.5.2/RNS/vendor/umsgpack.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-12 10:36:54.397606 rnspure-0.5.2/rnspure.egg-info/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18698 2023-05-12 10:36:54.000000 rnspure-0.5.2/rnspure.egg-info/PKG-INFO
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2231 2023-05-12 10:36:54.000000 rnspure-0.5.2/rnspure.egg-info/SOURCES.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        1 2023-05-12 10:36:54.000000 rnspure-0.5.2/rnspure.egg-info/dependency_links.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      292 2023-05-12 10:36:54.000000 rnspure-0.5.2/rnspure.egg-info/entry_points.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        4 2023-05-12 10:36:54.000000 rnspure-0.5.2/rnspure.egg-info/top_level.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       38 2023-05-12 10:36:54.397606 rnspure-0.5.2/setup.cfg
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1970 2023-05-04 15:54:21.000000 rnspure-0.5.2/setup.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-19 09:34:49.138155 rnspure-0.5.3/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1110 2022-10-20 15:25:41.000000 rnspure-0.5.3/LICENSE
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18698 2023-05-19 09:34:49.138155 rnspure-0.5.3/PKG-INFO
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    17959 2023-05-05 09:14:48.000000 rnspure-0.5.3/README.md
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-19 09:34:49.128155 rnspure-0.5.3/RNS/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10926 2023-05-18 23:54:43.000000 rnspure-0.5.3/RNS/Buffer.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24736 2023-05-18 23:37:50.000000 rnspure-0.5.3/RNS/Channel.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-19 09:34:49.131489 rnspure-0.5.3/RNS/Cryptography/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2735 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/AES.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      988 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/Ed25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3705 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/Fernet.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1961 2023-03-02 11:05:06.000000 rnspure-0.5.3/RNS/Cryptography/HKDF.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6885 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/HMAC.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      769 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/Hashes.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1541 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/PKCS7.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      794 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/Provider.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2611 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/Proxies.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4777 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/SHA256.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5589 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/SHA512.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4917 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/X25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      929 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/__init__.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-19 09:34:49.131489 rnspure-0.5.3/RNS/Cryptography/aes/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       20 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/aes/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8905 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/aes/aes.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7045 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/aes/utils.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-19 09:34:49.131489 rnspure-0.5.3/RNS/Cryptography/pure25519/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        0 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/pure25519/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1939 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/pure25519/_ed25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13056 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/pure25519/basic.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8193 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/pure25519/ed25519_oop.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3156 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Cryptography/pure25519/eddsa.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    20638 2023-02-09 10:50:55.000000 rnspure-0.5.3/RNS/Destination.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24033 2022-12-21 18:12:50.000000 rnspure-0.5.3/RNS/Identity.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-19 09:34:49.134822 rnspure-0.5.3/RNS/Interfaces/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14502 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Interfaces/AX25KISSInterface.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-19 09:34:49.134822 rnspure-0.5.3/RNS/Interfaces/Android/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    16723 2022-10-20 17:46:53.000000 rnspure-0.5.3/RNS/Interfaces/Android/KISSInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    49037 2023-05-02 15:44:28.000000 rnspure-0.5.3/RNS/Interfaces/Android/RNodeInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10335 2022-10-20 17:46:58.000000 rnspure-0.5.3/RNS/Interfaces/Android/SerialInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1290 2022-10-20 17:28:52.000000 rnspure-0.5.3/RNS/Interfaces/Android/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    20327 2023-05-11 17:33:15.000000 rnspure-0.5.3/RNS/Interfaces/AutoInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    41416 2022-11-03 21:46:26.000000 rnspure-0.5.3/RNS/Interfaces/I2PInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     3654 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Interfaces/Interface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13773 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Interfaces/KISSInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12932 2023-05-10 13:51:28.000000 rnspure-0.5.3/RNS/Interfaces/LocalInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6583 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Interfaces/PipeInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    30633 2023-05-02 15:44:01.000000 rnspure-0.5.3/RNS/Interfaces/RNodeInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7408 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Interfaces/SerialInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    21620 2023-05-04 21:14:01.000000 rnspure-0.5.3/RNS/Interfaces/TCPInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4206 2023-05-04 21:15:49.000000 rnspure-0.5.3/RNS/Interfaces/UDPInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     1321 2022-10-21 23:31:41.000000 rnspure-0.5.3/RNS/Interfaces/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    52943 2023-05-18 13:47:11.000000 rnspure-0.5.3/RNS/Link.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    22263 2023-05-18 14:48:32.000000 rnspure-0.5.3/RNS/Packet.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    45887 2023-05-10 13:26:58.000000 rnspure-0.5.3/RNS/Resource.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    65220 2023-05-05 08:37:31.000000 rnspure-0.5.3/RNS/Reticulum.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)   129986 2023-05-18 19:32:45.000000 rnspure-0.5.3/RNS/Transport.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-19 09:34:49.134822 rnspure-0.5.3/RNS/Utilities/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1291 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Utilities/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14872 2023-02-02 12:40:06.000000 rnspure-0.5.3/RNS/Utilities/rncp.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    25425 2023-05-09 18:30:37.000000 rnspure-0.5.3/RNS/Utilities/rnid.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)   208355 2023-05-09 13:30:30.000000 rnspure-0.5.3/RNS/Utilities/rnodeconf.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    12583 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Utilities/rnpath.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6588 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/Utilities/rnprobe.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    12818 2023-05-02 14:47:11.000000 rnspure-0.5.3/RNS/Utilities/rnsd.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9818 2023-03-08 12:57:44.000000 rnspure-0.5.3/RNS/Utilities/rnstatus.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    26422 2023-02-02 12:55:50.000000 rnspure-0.5.3/RNS/Utilities/rnx.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7088 2023-03-04 17:36:37.000000 rnspure-0.5.3/RNS/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       22 2023-05-19 09:18:07.000000 rnspure-0.5.3/RNS/_version.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-19 09:34:49.134822 rnspure-0.5.3/RNS/vendor/
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)      166 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/vendor/__init__.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    89634 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/vendor/configobj.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-19 09:34:49.134822 rnspure-0.5.3/RNS/vendor/i2plib/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      667 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/vendor/i2plib/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      316 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/vendor/i2plib/__version__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9939 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/vendor/i2plib/aiosam.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1158 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/vendor/i2plib/exceptions.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      122 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/vendor/i2plib/log.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4397 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/vendor/i2plib/sam.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8983 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/vendor/i2plib/tunnel.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1203 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/vendor/i2plib/utils.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-19 09:34:49.138155 rnspure-0.5.3/RNS/vendor/ifaddr/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1432 2023-05-05 08:23:36.000000 rnspure-0.5.3/RNS/vendor/ifaddr/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3646 2023-05-05 08:19:48.000000 rnspure-0.5.3/RNS/vendor/ifaddr/_posix.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7321 2023-05-05 08:20:00.000000 rnspure-0.5.3/RNS/vendor/ifaddr/_shared.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5107 2023-05-05 08:20:05.000000 rnspure-0.5.3/RNS/vendor/ifaddr/_win32.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1141 2023-05-05 08:36:33.000000 rnspure-0.5.3/RNS/vendor/ifaddr/niwrapper.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1184 2022-10-21 23:31:14.000000 rnspure-0.5.3/RNS/vendor/platformutils.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    34549 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/vendor/six.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    43449 2022-10-20 15:25:41.000000 rnspure-0.5.3/RNS/vendor/umsgpack.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2023-05-19 09:34:49.138155 rnspure-0.5.3/rnspure.egg-info/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    18698 2023-05-19 09:34:49.000000 rnspure-0.5.3/rnspure.egg-info/PKG-INFO
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2231 2023-05-19 09:34:49.000000 rnspure-0.5.3/rnspure.egg-info/SOURCES.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        1 2023-05-19 09:34:49.000000 rnspure-0.5.3/rnspure.egg-info/dependency_links.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      292 2023-05-19 09:34:49.000000 rnspure-0.5.3/rnspure.egg-info/entry_points.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        4 2023-05-19 09:34:49.000000 rnspure-0.5.3/rnspure.egg-info/top_level.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       38 2023-05-19 09:34:49.138155 rnspure-0.5.3/setup.cfg
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1970 2023-05-04 15:54:21.000000 rnspure-0.5.3/setup.py
```

### Comparing `rnspure-0.5.2/LICENSE` & `rnspure-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/PKG-INFO` & `rnspure-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rnspure
-Version: 0.5.2
+Version: 0.5.3
 Summary: Self-configuring, encrypted and resilient mesh networking stack for LoRa, packet radio, WiFi and everything in between
 Home-page: https://reticulum.network/
 Author: Mark Qvist
 Author-email: mark@unsigned.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rnspure-0.5.2/README.md` & `rnspure-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Buffer.py` & `rnspure-0.5.3/RNS/Buffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 import bz2
 import sys
+import time
 import threading
 from threading import RLock
 import struct
 from RNS.Channel import Channel, MessageBase, SystemMessageTypes
 import RNS
 from io import RawIOBase, BufferedRWPair, BufferedReader, BufferedWriter
 from typing import Callable
@@ -61,14 +62,15 @@
 
     def unpack(self, raw):
         self.stream_id = struct.unpack(">H", raw[:2])[0]
         self.eof = (0x8000 & self.stream_id) > 0
         self.compressed = (0x4000 & self.stream_id) > 0
         self.stream_id = self.stream_id & 0x3fff
         self.data = raw[2:]
+
         if self.compressed:
             self.data = bz2.decompress(self.data)
 
 
 class RawChannelReader(RawIOBase, AbstractContextManager):
     """
     An implementation of RawIOBase that receives
@@ -125,15 +127,15 @@
                 with self._lock:
                     if message.data is not None:
                         self._buffer.extend(message.data)
                     if message.eof:
                         self._eof = True
                     for listener in self._listeners:
                         try:
-                            listener(len(self._buffer))
+                            threading.Thread(target=listener, name="Message Callback", args=[len(self._buffer)], daemon=True).start()
                         except Exception as ex:
                             RNS.log("Error calling RawChannelReader(" + str(self._stream_id) + ") callback: " + str(ex))
                     return True
         return False
 
     def _read(self, __size: int) -> bytes | None:
         with self._lock:
@@ -203,14 +205,23 @@
             return len(chunk)
         except RNS.Channel.ChannelException as cex:
             if cex.type != RNS.Channel.CEType.ME_LINK_NOT_READY:
                 raise
         return 0
 
     def close(self):
+        try:
+            link_rtt = self._channel._outlet.link.rtt
+            timeout = time.time() + (link_rtt * len(self._channel._tx_ring) * 1)
+        except Exception as e:
+            timeout = time.time() + 15
+
+        while time.time() < timeout and not self._channel.is_ready_to_send():
+            time.sleep(0.05)
+
         self._eof = True
         self.write(bytes())
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
```

### Comparing `rnspure-0.5.2/RNS/Channel.py` & `rnspure-0.5.3/RNS/Channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,32 +172,38 @@
         msgtype, self.sequence, length = struct.unpack(">HHH", self.raw[:6])
         raw = self.raw[6:]
         ctor = message_factories.get(msgtype, None)
         if ctor is None:
             raise ChannelException(CEType.ME_NOT_REGISTERED, f"Unable to find constructor for Channel MSGTYPE {hex(msgtype)}")
         message = ctor()
         message.unpack(raw)
+        self.unpacked = True
+        self.message = message
+
         return message
 
     def pack(self) -> bytes:
         if self.message.__class__.MSGTYPE is None:
             raise ChannelException(CEType.ME_NO_MSG_TYPE, f"{self.message.__class__} lacks MSGTYPE")
         data = self.message.pack()
         self.raw = struct.pack(">HHH", self.message.MSGTYPE, self.sequence, len(data)) + data
+        self.packed = True
         return self.raw
 
     def __init__(self, outlet: ChannelOutletBase, message: MessageBase = None, raw: bytes = None, sequence: int = None):
         self.ts = time.time()
         self.id = id(self)
         self.message = message
         self.raw = raw
         self.packet: TPacket = None
         self.sequence = sequence
         self.outlet = outlet
         self.tries = 0
+        self.unpacked = False
+        self.packed = False
         self.tracked = False
 
 
 class Channel(contextlib.AbstractContextManager):
     """
     Provides reliable delivery of messages over
     a link.
@@ -367,30 +373,37 @@
                     self._outlet.set_packet_delivered_callback(envelope.packet, None)
             self._tx_ring.clear()
             self._rx_ring.clear()
 
     def _emplace_envelope(self, envelope: Envelope, ring: collections.deque[Envelope]) -> bool:
         with self._lock:
             i = 0
+            
+            window_overflow = (self._next_rx_sequence+Channel.WINDOW_MAX) % Channel.SEQ_MODULUS
             for existing in ring:
-                if existing.sequence > envelope.sequence \
-                   and not existing.sequence // 2 > envelope.sequence:  # account for overflow
-                    ring.insert(i, envelope)
-                    return True
-                if existing.sequence == envelope.sequence:
+
+                if envelope.sequence == existing.sequence:
                     RNS.log(f"Envelope: Emplacement of duplicate envelope with sequence "+str(envelope.sequence), RNS.LOG_EXTREME)
                     return False
+                
+                if envelope.sequence < existing.sequence and not envelope.sequence < window_overflow:
+                    ring.insert(i, envelope)
+                    RNS.log("Inserted seq "+str(envelope.sequence)+" at "+str(i), RNS.LOG_DEBUG)
+
+                    envelope.tracked = True
+                    return True
+                
                 i += 1
+            
             envelope.tracked = True
             ring.append(envelope)
             return True
 
     def _run_callbacks(self, message: MessageBase):
-        with self._lock:
-            cbs = self._message_callbacks.copy()
+        cbs = self._message_callbacks.copy()
 
         for cb in cbs:
             try:
                 if cb(message):
                     return
             except Exception as e:
                 RNS.log("Channel "+str(self)+" experienced an error while running a message callback. The contained exception was: "+str(e), RNS.LOG_ERROR)
@@ -401,20 +414,19 @@
             with self._lock:
                 message = envelope.unpack(self._message_factories)
 
                 if envelope.sequence < self._next_rx_sequence:
                     window_overflow = (self._next_rx_sequence+Channel.WINDOW_MAX) % Channel.SEQ_MODULUS
                     if window_overflow < self._next_rx_sequence:
                         if envelope.sequence > window_overflow:
-                            RNS.log("Invalid packet sequence ("+str(envelope.sequence)+") received on channel "+str(self), RNS.LOG_DEBUG)
+                            RNS.log("Invalid packet sequence ("+str(envelope.sequence)+") received on channel "+str(self), RNS.LOG_EXTREME)
                             return
                     else:
-                        if envelope.sequence < self._next_rx_sequence:
-                            RNS.log("Invalid packet sequence ("+str(envelope.sequence)+") received on channel "+str(self), RNS.LOG_DEBUG)
-                            return
+                        RNS.log("Invalid packet sequence ("+str(envelope.sequence)+") received on channel "+str(self), RNS.LOG_EXTREME)
+                        return
 
                 is_new = self._emplace_envelope(envelope, self._rx_ring)
 
             if not is_new:
                 RNS.log("Duplicate message received on channel "+str(self), RNS.LOG_EXTREME)
                 return
             else:            
@@ -422,17 +434,21 @@
                     contigous = []
                     for e in self._rx_ring:
                         if e.sequence == self._next_rx_sequence:
                             contigous.append(e)
                             self._next_rx_sequence = (self._next_rx_sequence + 1) % Channel.SEQ_MODULUS
 
                     for e in contigous:
-                        m = e.unpack(self._message_factories)
+                        if not e.unpacked:
+                            m = e.unpack(self._message_factories)
+                        else:
+                            m = e.message
+                            
                         self._rx_ring.remove(e)
-                        threading.Thread(target=self._run_callbacks, name="Message Callback", args=[m], daemon=True).start()
+                        self._run_callbacks(m)
 
         except Exception as e:
             RNS.log("An error ocurred while receiving data on "+str(self)+". The contained exception was: "+str(e), RNS.LOG_ERROR)
 
     def is_ready_to_send(self) -> bool:
         """
         Check if ``Channel`` is ready to send.
@@ -465,41 +481,39 @@
 
                     if self.window < self.window_max:
                         self.window += 1
                         if (self.window - self.window_min) > (self.window_flexibility-1):
                             self.window_min += 1
 
                         # TODO: Remove at some point
-                        RNS.log("Increased "+str(self)+" window to "+str(self.window), RNS.LOG_DEBUG)
+                        # RNS.log("Increased "+str(self)+" window to "+str(self.window), RNS.LOG_EXTREME)
 
                     if self._outlet.rtt != 0:
                         if self._outlet.rtt > Channel.RTT_FAST:
                             self.fast_rate_rounds = 0
 
                             if self._outlet.rtt > Channel.RTT_MEDIUM:
                                 self.medium_rate_rounds = 0
 
                             else:
                                 self.medium_rate_rounds += 1
                                 if self.window_max < Channel.WINDOW_MAX_MEDIUM and self.medium_rate_rounds == Channel.FAST_RATE_THRESHOLD:
                                     self.window_max = Channel.WINDOW_MAX_MEDIUM
                                     # TODO: Remove at some point
-                                    RNS.log("Increased "+str(self)+" max window to "+str(self.window_max), RNS.LOG_EXTREME)
+                                    # RNS.log("Increased "+str(self)+" max window to "+str(self.window_max), RNS.LOG_EXTREME)
                             
                         else:
                             self.fast_rate_rounds += 1
                             if self.window_max < Channel.WINDOW_MAX_FAST and self.fast_rate_rounds == Channel.FAST_RATE_THRESHOLD:
                                 self.window_max = Channel.WINDOW_MAX_FAST                                
                                 # TODO: Remove at some point
-                                RNS.log("Increased "+str(self)+" max window to "+str(self.window_max), RNS.LOG_EXTREME)
-
-
+                                # RNS.log("Increased "+str(self)+" max window to "+str(self.window_max), RNS.LOG_EXTREME)
 
                 else:
-                    RNS.log("Envelope not found in TX ring for "+str(self), RNS.LOG_DEBUG)
+                    RNS.log("Envelope not found in TX ring for "+str(self), RNS.LOG_EXTREME)
         if not envelope:
             RNS.log("Spurious message received on "+str(self), RNS.LOG_EXTREME)
 
     def _packet_delivered(self, packet: TPacket):
         self._packet_tx_op(packet, lambda env: True)
 
     def _get_packet_timeout_time(self, tries: int) -> float:
@@ -521,15 +535,15 @@
                 self.window -= 1
                 if self.window_max > self.window_min:
                     self.window_max -= 1
                     if (self.window_max - self.window) > (self.window_flexibility-1):
                         self.window_max -= 1
 
                 # TODO: Remove at some point
-                RNS.log("Decreased "+str(self)+" window to "+str(self.window), RNS.LOG_EXTREME)
+                # RNS.log("Decreased "+str(self)+" window to "+str(self.window), RNS.LOG_EXTREME)
 
             return False
 
         if self._outlet.get_packet_state(packet) != MessageState.MSGSTATE_DELIVERED:
             self._packet_tx_op(packet, retry_envelope)
 
     def send(self, message: MessageBase) -> Envelope:
@@ -539,24 +553,26 @@
 
         :param message: an instance of a ``MessageBase`` subclass
         """
         envelope: Envelope | None = None
         with self._lock:
             if not self.is_ready_to_send():
                 raise ChannelException(CEType.ME_LINK_NOT_READY, f"Link is not ready")
+        
             envelope = Envelope(self._outlet, message=message, sequence=self._next_sequence)
             self._next_sequence = (self._next_sequence + 1) % Channel.SEQ_MODULUS
-
             self._emplace_envelope(envelope, self._tx_ring)
+
         if envelope is None:
             raise BlockingIOError()
 
         envelope.pack()
         if len(envelope.raw) > self._outlet.mdu:
             raise ChannelException(CEType.ME_TOO_BIG, f"Packed message too big for packet: {len(envelope.raw)} > {self._outlet.mdu}")
+        
         envelope.packet = self._outlet.send(envelope.raw)
         envelope.tries += 1
         self._outlet.set_packet_delivered_callback(envelope.packet, self._packet_delivered)
         self._outlet.set_packet_timeout_callback(envelope.packet, self._packet_timeout, self._get_packet_timeout_time(envelope.tries))
 
         return envelope
 
@@ -587,15 +603,14 @@
     def send(self, raw: bytes) -> RNS.Packet:
         packet = RNS.Packet(self.link, raw, context=RNS.Packet.CHANNEL)
         if self.link.status == RNS.Link.ACTIVE:
             packet.send()
         return packet
 
     def resend(self, packet: RNS.Packet) -> RNS.Packet:
-        RNS.log("Resending packet " + RNS.prettyhexrep(packet.packet_hash), RNS.LOG_DEBUG)
         receipt = packet.resend()
         if not receipt:
             RNS.log("Failed to resend packet", RNS.LOG_ERROR)
         return packet
 
     @property
     def mdu(self):
```

### Comparing `rnspure-0.5.2/RNS/Cryptography/AES.py` & `rnspure-0.5.3/RNS/Cryptography/AES.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/Ed25519.py` & `rnspure-0.5.3/RNS/Cryptography/Ed25519.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/Fernet.py` & `rnspure-0.5.3/RNS/Cryptography/Fernet.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/HKDF.py` & `rnspure-0.5.3/RNS/Cryptography/HKDF.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/HMAC.py` & `rnspure-0.5.3/RNS/Cryptography/HMAC.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/Hashes.py` & `rnspure-0.5.3/RNS/Cryptography/Hashes.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/PKCS7.py` & `rnspure-0.5.3/RNS/Cryptography/PKCS7.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/Provider.py` & `rnspure-0.5.3/RNS/Cryptography/Provider.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/Proxies.py` & `rnspure-0.5.3/RNS/Cryptography/Proxies.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/SHA256.py` & `rnspure-0.5.3/RNS/Cryptography/SHA256.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/SHA512.py` & `rnspure-0.5.3/RNS/Cryptography/SHA512.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/X25519.py` & `rnspure-0.5.3/RNS/Cryptography/X25519.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/__init__.py` & `rnspure-0.5.3/RNS/Cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/aes/aes.py` & `rnspure-0.5.3/RNS/Cryptography/aes/aes.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/aes/utils.py` & `rnspure-0.5.3/RNS/Cryptography/aes/utils.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/pure25519/_ed25519.py` & `rnspure-0.5.3/RNS/Cryptography/pure25519/_ed25519.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/pure25519/basic.py` & `rnspure-0.5.3/RNS/Cryptography/pure25519/basic.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/pure25519/ed25519_oop.py` & `rnspure-0.5.3/RNS/Cryptography/pure25519/ed25519_oop.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Cryptography/pure25519/eddsa.py` & `rnspure-0.5.3/RNS/Cryptography/pure25519/eddsa.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Destination.py` & `rnspure-0.5.3/RNS/Destination.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Identity.py` & `rnspure-0.5.3/RNS/Identity.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/AX25KISSInterface.py` & `rnspure-0.5.3/RNS/Interfaces/AX25KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/Android/KISSInterface.py` & `rnspure-0.5.3/RNS/Interfaces/Android/KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/Android/RNodeInterface.py` & `rnspure-0.5.3/RNS/Interfaces/Android/RNodeInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/Android/SerialInterface.py` & `rnspure-0.5.3/RNS/Interfaces/Android/SerialInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/Android/__init__.py` & `rnspure-0.5.3/RNS/Interfaces/Android/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/AutoInterface.py` & `rnspure-0.5.3/RNS/Interfaces/AutoInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/I2PInterface.py` & `rnspure-0.5.3/RNS/Interfaces/I2PInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/Interface.py` & `rnspure-0.5.3/RNS/Interfaces/Interface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/KISSInterface.py` & `rnspure-0.5.3/RNS/Interfaces/KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/LocalInterface.py` & `rnspure-0.5.3/RNS/Interfaces/LocalInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/PipeInterface.py` & `rnspure-0.5.3/RNS/Interfaces/PipeInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/RNodeInterface.py` & `rnspure-0.5.3/RNS/Interfaces/RNodeInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/SerialInterface.py` & `rnspure-0.5.3/RNS/Interfaces/SerialInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/TCPInterface.py` & `rnspure-0.5.3/RNS/Interfaces/TCPInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/UDPInterface.py` & `rnspure-0.5.3/RNS/Interfaces/UDPInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Interfaces/__init__.py` & `rnspure-0.5.3/RNS/Interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Link.py` & `rnspure-0.5.3/RNS/Link.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Packet.py` & `rnspure-0.5.3/RNS/Packet.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Resource.py` & `rnspure-0.5.3/RNS/Resource.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Reticulum.py` & `rnspure-0.5.3/RNS/Reticulum.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Transport.py` & `rnspure-0.5.3/RNS/Transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,16 @@
                         culled_receipt = Transport.receipts.pop(0)
                         culled_receipt.timeout = -1
                         culled_receipt.check_timeout()
 
                     for receipt in Transport.receipts:
                         receipt.check_timeout()
                         if receipt.status != RNS.PacketReceipt.SENT:
-                            Transport.receipts.remove(receipt)
+                            if receipt in Transport.receipts:
+                                Transport.receipts.remove(receipt)
 
                     Transport.receipts_last_checked = time.time()
 
                 # Process announces needing retransmission
                 if time.time() > Transport.announces_last_checked+Transport.announces_check_interval:
                     for destination_hash in Transport.announce_table:
                         announce_entry = Transport.announce_table[destination_hash]
```

### Comparing `rnspure-0.5.2/RNS/Utilities/__init__.py` & `rnspure-0.5.3/RNS/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Utilities/rncp.py` & `rnspure-0.5.3/RNS/Utilities/rncp.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Utilities/rnid.py` & `rnspure-0.5.3/RNS/Utilities/rnid.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Utilities/rnodeconf.py` & `rnspure-0.5.3/RNS/Utilities/rnodeconf.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Utilities/rnpath.py` & `rnspure-0.5.3/RNS/Utilities/rnpath.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Utilities/rnprobe.py` & `rnspure-0.5.3/RNS/Utilities/rnprobe.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Utilities/rnsd.py` & `rnspure-0.5.3/RNS/Utilities/rnsd.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Utilities/rnstatus.py` & `rnspure-0.5.3/RNS/Utilities/rnstatus.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/Utilities/rnx.py` & `rnspure-0.5.3/RNS/Utilities/rnx.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/__init__.py` & `rnspure-0.5.3/RNS/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/configobj.py` & `rnspure-0.5.3/RNS/vendor/configobj.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/i2plib/__init__.py` & `rnspure-0.5.3/RNS/vendor/i2plib/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/i2plib/aiosam.py` & `rnspure-0.5.3/RNS/vendor/i2plib/aiosam.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/i2plib/exceptions.py` & `rnspure-0.5.3/RNS/vendor/i2plib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/i2plib/sam.py` & `rnspure-0.5.3/RNS/vendor/i2plib/sam.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/i2plib/tunnel.py` & `rnspure-0.5.3/RNS/vendor/i2plib/tunnel.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/i2plib/utils.py` & `rnspure-0.5.3/RNS/vendor/i2plib/utils.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/ifaddr/__init__.py` & `rnspure-0.5.3/RNS/vendor/ifaddr/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/ifaddr/_posix.py` & `rnspure-0.5.3/RNS/vendor/ifaddr/_posix.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/ifaddr/_shared.py` & `rnspure-0.5.3/RNS/vendor/ifaddr/_shared.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/ifaddr/_win32.py` & `rnspure-0.5.3/RNS/vendor/ifaddr/_win32.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/ifaddr/niwrapper.py` & `rnspure-0.5.3/RNS/vendor/ifaddr/niwrapper.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/platformutils.py` & `rnspure-0.5.3/RNS/vendor/platformutils.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/six.py` & `rnspure-0.5.3/RNS/vendor/six.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/RNS/vendor/umsgpack.py` & `rnspure-0.5.3/RNS/vendor/umsgpack.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/rnspure.egg-info/PKG-INFO` & `rnspure-0.5.3/rnspure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rnspure
-Version: 0.5.2
+Version: 0.5.3
 Summary: Self-configuring, encrypted and resilient mesh networking stack for LoRa, packet radio, WiFi and everything in between
 Home-page: https://reticulum.network/
 Author: Mark Qvist
 Author-email: mark@unsigned.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rnspure-0.5.2/rnspure.egg-info/SOURCES.txt` & `rnspure-0.5.3/rnspure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rnspure-0.5.2/setup.py` & `rnspure-0.5.3/setup.py`

 * *Files identical despite different names*

