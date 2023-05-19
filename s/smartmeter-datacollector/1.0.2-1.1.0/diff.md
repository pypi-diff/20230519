# Comparing `tmp/smartmeter-datacollector-1.0.2.tar.gz` & `tmp/smartmeter-datacollector-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartmeter-datacollector-1.0.2.tar", last modified: Fri Apr  8 06:52:13 2022, max compression
+gzip compressed data, was "smartmeter-datacollector-1.1.0.tar", last modified: Fri May 19 18:23:53 2023, max compression
```

## Comparing `smartmeter-datacollector-1.0.2.tar` & `smartmeter-datacollector-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 06:52:13.618343 smartmeter-datacollector-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)    18391 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    17468 2022-04-08 06:52:13.618343 smartmeter-datacollector-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16501 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 06:52:13.618343 smartmeter-datacollector-1.0.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)      321 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/bin/smartmeter-datacollector
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-08 06:52:13.618343 smartmeter-datacollector-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1992 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 06:52:13.618343 smartmeter-datacollector-1.0.2/smartmeter_datacollector/
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2263 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/collector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1656 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2484 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 06:52:13.618343 smartmeter-datacollector-1.0.2/smartmeter_datacollector/sinks/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/sinks/data_sink.py
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/sinks/logger_sink.py
--rw-r--r--   0 runner    (1001) docker     (121)     6144 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/sinks/mqtt_sink.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 06:52:13.618343 smartmeter-datacollector-1.0.2/smartmeter_datacollector/smartmeter/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/smartmeter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/smartmeter/cosem.py
--rw-r--r--   0 runner    (1001) docker     (121)     5226 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/smartmeter/hdlc_dlms_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4661 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/smartmeter/iskraam550.py
--rw-r--r--   0 runner    (1001) docker     (121)     4502 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/smartmeter/lge450.py
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/smartmeter/meter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4282 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/smartmeter/meter_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/smartmeter/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-04-08 06:50:35.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector/smartmeter/serial_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 06:52:13.618343 smartmeter-datacollector-1.0.2/smartmeter_datacollector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17468 2022-04-08 06:52:13.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-04-08 06:52:13.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-08 06:52:13.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-04-08 06:52:13.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-04-08 06:52:13.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-08 06:52:13.000000 smartmeter-datacollector-1.0.2/smartmeter_datacollector.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:23:53.723106 smartmeter-datacollector-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18391 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-05-19 18:23:53.723106 smartmeter-datacollector-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:23:53.719106 smartmeter-datacollector-1.1.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      321 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/bin/smartmeter-datacollector
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:23:53.723106 smartmeter-datacollector-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:23:53.719106 smartmeter-datacollector-1.1.0/smartmeter_datacollector/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:23:53.719106 smartmeter-datacollector-1.1.0/smartmeter_datacollector/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/sinks/data_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/sinks/logger_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/sinks/mqtt_sink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:23:53.723106 smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/cosem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/hdlc_dlms_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/iskraam550.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/kamstrup_han.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/lge360.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/lge450.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/meter_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/obis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/serial_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:23:53.719106 smartmeter-datacollector-1.1.0/smartmeter_datacollector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-05-19 18:23:53.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-19 18:23:53.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:23:53.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-19 18:23:53.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 18:23:53.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:23:53.000000 smartmeter-datacollector-1.1.0/smartmeter_datacollector.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:23:53.723106 smartmeter-datacollector-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/tests/test_hdlc_dlms_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/tests/test_iskraam550.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/tests/test_lge450.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/tests/test_meter_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/tests/test_mqtt_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-19 18:23:32.000000 smartmeter-datacollector-1.1.0/tests/test_obis.py
```

### Comparing `smartmeter-datacollector-1.0.2/LICENSE` & `smartmeter-datacollector-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.0.2/PKG-INFO` & `smartmeter-datacollector-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: smartmeter-datacollector
-Version: 1.0.2
+Version: 1.1.0
 Summary: Smart Meter Data Collector
 Home-page: https://github.com/scs/smartmeter-datacollector
 Author: Supercomputing Systems AG
 Author-email: info@scs.ch
+Maintainer: Supercomputing Systems AG
+Maintainer-email: info@scs.ch
 License: GPLv2
 Project-URL: Source, https://github.com/scs/smartmeter-datacollector
 Project-URL: Bug Reports, https://github.com/scs/smartmeter-datacollector/issues
 Project-URL: Pull Requests, https://github.com/scs/smartmeter-datacollector/pulls
 Project-URL: SCS, https://www.scs.ch
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Smart Meter Data Collector
 
@@ -33,39 +35,41 @@
 </p>
 
 ---
 
 The `smartmeter-datacollector` tool is a Python3 software which allows you to continuously retrieve data from supported smart meters (listed below).
 The acquired values can be forwarded to one or more data sinks like a MQTT broker or logger.
 
-This tool is an open source software funded by **[EKZ (Elektrizitätswerke des Kantons Zürich)](https://www.ekz.ch)** and developed by **[Supercomputing Systems AG](https://www.scs.ch)**. The goal of this voluntary initiative is to create a tool that can read, decode and decrypt data (if necessary) from the local interface of various smart meters and convert it into human-readable and simple formats. This should eliminate the complexity of decoding DLMS and similar protocols for the user. The user has the data in a format, which he can easily use in various use-cases ranging from simple vizualization (see [Method 1: Raspberry Pi image with demo](#method-1-raspberry-pi-image-with-demo)) to integration into energy management algorithms or into custom home automation software. 
+This tool is an open source software funded by **[EKZ (Elektrizitätswerke des Kantons Zürich)](https://www.ekz.ch)** and developed by **[Supercomputing Systems AG](https://www.scs.ch)**. The goal of this voluntary initiative is to create a tool that can read, decode and decrypt data (if necessary) from the local interface of various smart meters and convert it into human-readable and simple formats. This should eliminate the complexity of decoding DLMS and similar protocols for the user. The user has the data in a format, which he can easily use in various use-cases ranging from simple visualization (see [Method 1: Raspberry Pi image with demo](#method-1-raspberry-pi-image-with-demo)) to integration into energy management algorithms or into custom home automation software. 
 
-The following smart meters are supported:
+The following smart meters are supported (see [Wiki/Home](https://github.com/scs/smartmeter-datacollector/wiki/Home) for detailed information).
 
 * Landis+Gyr E450: \
-  Data pushed by smart meter over CII interface (wired M-Bus). Encoded with HDLC and DLMS/COSEM.
-  * Unencrypted data
-  * Encrypted data
+  Data pushed by smart meter over CII interface (wired M-Bus, HDLC, DLMS/COSEM).
+* Landis+Gyr E360: \
+  Data pushed by smart meter over P1 interface (HDLC, DLMS/COSEM only, no DSMR).
 * Iskraemeco AM550: \
-  Data pushed by smart meter over [P1 interface (DSMR)](https://www.netbeheernederland.nl/_upload/Files/Slimme_meter_15_a727fce1f1.pdf). Encoded with HDLC (IEC 62056-46) and DLMS/COSEM.
-  * Unencrypted data
-  * Encrypted data
+  Data pushed by smart meter over P1 interface (HDLC, DLMS/COSEM only, no DSMR).
+* Kamstrup OMNIPOWER with HAN-NVE: \
+  Data pushed by smart meter over inserted [HAN-NVE module](https://www.kamstrup.com/en-en/electricity-solutions/meters-devices/modules/hannve) (wired M-Bus, HDLC, DLMS/COSEM).
+
+Note: All smart meters integrated so far push binary data encoded with HDLC (IEC 62056-46) and DLMS/COSEM. Both unencrypted and encrypted DLMS messages are accepted by the software.
 
 The following data sinks are implemented:
 * MQTT (v3.1.1):
   * Encryption
     * Unencrypted connection
     * Encrypted connection
       * TLS
       * optional custom CA certificate
   * Authentication
     * Unauthenticated
     * Authenticated with username / password
     * Authenticated with client certificate
-* Logger to STDOUT
+* Logger to `stdout`
 
 `smartmeter-datacollector` is fully configurable through a `.ini` configuration file. The [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-configurator) webinterface can help to create and modify the configuration.
 
 ---
 
 - [Smart Meter Data Collector](#smart-meter-data-collector)
 - [How to install](#how-to-install)
@@ -108,30 +112,15 @@
 * `smartmeter-datacollector-configurator` webinterface
 * demo
   * [mosquiotto](https://mosquitto.org/) as a local MQTT broker to publish the measurements from `smartmeter-datacollector`
   * [Telegraf](https://www.influxdata.com/time-series-platform/telegraf/) to collect measurements published by `smartmeter-datacollector` over MQTT and store them in InfluxDB
   * [InfluxDB](https://www.influxdata.com/) to store the measurements
   * [Grafana](https://grafana.com/) to visualize the measurements
 
-This setup allows a (first time) user to [install](https://www.raspberrypi.org/documentation/computers/getting-started.html#installing-the-operating-system) the image on a Raspberry Pi and immediately get started with `smartmeter-datacollector`. The following steps are required:
-1. Download the Raspberry Pi image from the [latest release](https://github.com/scs/smartmeter-datacollector/releases).
-2. Install the image on a (micro)SD card, e.g. using [Raspberry Pi Imager](https://www.raspberrypi.org/documentation/computers/getting-started.html#using-raspberry-pi-imager).
-3. Prepare the Raspberry Pi.
-   1. Push the (micro)SD card into the proper slot.
-   2. Use an RJ-45 cable (or configure WiFi later) to connect to a network.
-   3. Connect the power cable to the Micro USB port.
-4. Open the `smartmeter-datacollector-configurator` webinterface using `http://<Raspberry Pi IP>:8000/` in your favorite browser.
-   1. Load the pre-defined configuration.
-   2. Adjust the settings of the connected smart meter.
-   3. Deploy the adjusted configuration.
-   4. Restart the `smartmeter-datacollector` service.
-5. Open `Grafana` using `http://<Raspberry Pi IP>:3000/` in your favorite browser.
-6. Observe the measurements from your smart meter while they arrive periodically.
-
-See [Wiki/Demo](https://github.com/scs/smartmeter-datacollector/wiki/Demo-(Raspberry-Pi-Image)) for more details on the provided Raspberry Pi image with the demo.
+See [Wiki/Demo](https://github.com/scs/smartmeter-datacollector/wiki/Demo-(Raspberry-Pi-Image)) for detailed setup instructions.
 
 ## Method 2: Python package
 
 `smartmeter-datacollector` can be installed as a Python3 package either from [PyPi](https://pypi.org/project/smartmeter-datacollector/) or manually using a [released wheel](https://github.com/scs/smartmeter-datacollector/releases).
 
 The Python3 package does not contain any infrastructure to run `smartmeter-datacollector` in the background or to automatically start it during a boot sequence. If such infrastructure is required either see [Method 3: Debian package](#method-3-debian-package) or provide it yourself.
 
@@ -158,15 +147,15 @@
 `smartmeter-datacollector` is also available as a Debian (`.deb`) package from the [releases](https://github.com/scs/smartmeter-datacollector/releases) which installs it system wide. The Debian package includes a systemd service file which enables `smartmeter-datacollector` to automatically start after booting the system.
 
 ### Debian Requirements
 
 * Distribution
   * Debian
 * Release
-  * Buster
+  * Bullseye
 * CPU architecture
   * amd64
   * armhf
 
 ### Installation
 
 Download the Debian package from [releases](https://github.com/scs/smartmeter-datacollector/releases) and install it with
@@ -183,66 +172,17 @@
 
 # How to use
 
 The usage of `smartmeter-datacollector` depends on the installation method. Independent of the installation method a `.ini` configuration file is required to properly run `smartmeter-datacollector`.
 
 ## Configuration
 
-### Specification
-
-The `.ini` configuration file supports the following format
-
-```ini
-[reader0]
-# type of the connected smart meter
-type = lge450
-# serial port to which the smart meter is connected
-port = /dev/ttyUSB0
-# optional encryption key
-key = 
-
-[sink0]
-# type of the sink
-type = mqtt
-# host / IP address of the MQTT broker
-host = localhost
-# port of the MQTT broker
-port = 1883
-# whether to use TLS (Transport Layer Security)
-tls = False
-# optional path to the CA certificate used to validate the MQTT broker's certificate
-ca_file_path = 
-# whether to check the hostname of the MQTT broker against the certificate
-check_hostname = False
-# optional username for authentication with the MQTT broker
-username = 
-# optional password for authentication with the MQTT broker
-password = 
-# optional path to the client certificate for authentication with the MQTT broker
-client_cert_path = 
-# optional path to the private key for the client certificate for authentication with the MQTT broker
-client_key_path = 
-
-[sink1]
-# type of the sink
-type = logger
-# name of the logger
-name = DataLogger
-
-[logging]
-# log level configuration: DEBUG / INFO / WARNING / ERROR
-default = WARNING
-smartmeter = WARNING
-collector = WARNING
-sink = WARNING
-```
-
-There can be multiple `[readerX]` and `[sinkY]` sections for every connected smart meter and / or data sink.
+### Manually create configuration
 
-See [Wiki/Configuration](https://github.com/scs/smartmeter-datacollector/wiki/Configuration) for more details on the available configuration options.
+See [Wiki/Configuration](https://github.com/scs/smartmeter-datacollector/wiki/Configuration#manually-write-configuration) for more details on the available configuration options.
 
 ### smartmeter-datacollector-configurator
 
 To simplify the process of generating a valid `.ini` configuration for `smartmeter-datacollector` the companion [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-configurator) webinterface can be used. It supports
 * a graphical approach to manage the configuration
 * input validation to avoid invalid configurations
 * loading / saving / discarding a configuration
@@ -257,77 +197,56 @@
 ```
 smartmeter-datacollector --config datacollector.ini
 ```
 
 The following command line arguments are supported:
 * `-h, --help`: Shows the help output of `smartmeter-datacollector`.
 * `-c, --config CONFIG`: Path to the `.ini` configuration file.
-* `-s,--saveconfig`: Cteate a default `.ini` configuration file.
+* `-s,--saveconfig`: Create a default `.ini` configuration file.
 * `-d, --dev`: Enable development mode.
 
 ### Configuration
 
 The configuration file can be located anywhere and use any filename. If no `.ini` configuration file is specified a default configuration with the following options is used:
-* Landys+Gir E450 smart meter in unencrypted mode connected to `/dev/ttyUSB0`
+* Landys+Gyr E450 smart meter in unencrypted mode connected to `/dev/ttyUSB0`
 * `LOGGER` sink
 * `MQTT` sink connected to a local broker without encryption or authentication
 
 ## Run as a systemd service
 
-When `smartmeter-datacollector` has been installed as a Debian package it provides a systemd .service file named `python3-smartmeter-datacollector.service`. Therefore the service can be managed using the `systemctl` command:
-
-```
-sudo systemctl start|stop|restart python3-smartmeter-datacollector
-```
-
-Enabling or disabling the service can also be managed using the `systemctl` command:
-
-```
-sudo systemctl enable|disable python3-smartmeter-datacollector
-```
-
-Inspecting the log messages can be done using the `journalctl` command:
+When `smartmeter-datacollector` has been installed as a Debian package it provides a systemd .service file named `python3-smartmeter-datacollector.service`. Therefore the service can be managed using the `systemctl` command. See [Run as a systemd service](https://github.com/scs/smartmeter-datacollector/wiki/How-to-use#run-as-a-systemd-service) for possible commands.
 
-```
-journalctl -u python3-smartmeter-datacollector [-f]
-```
-
-### Configuration
-
-The systemd service expectes the `.ini` configuration to be located at
-`/var/lib/smartmeter-datacollector/datacollector.ini`. This is also the default location used by the [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-configurator) webinterface to load and save the managed configuration.
 
 # How to develop
 
 Help from the community for the `smartmeter-datacollector` project is always welcome. Please follow the next few chapters to setup a working development environment.
 
 ## Development Requirements
 
-* Python >= 3.7
+* Python >= 3.8, <= 3.10
 * [`pipenv`](https://pipenv.pypa.io/en/latest/)
-* Optional software packages (Debian / Ubuntu)
+* Optional software packages (Debian bullseye/ Ubuntu 22.04)
   * python3-all
   * debhelper
   * dh-python
-  * dh-systemd
 
 ## Installation
 
 ### Debian / Ubuntu
 
 To install the listed minimal requirements run the following command:
 
 ```
 sudo apt install git python3 pipenv
 ```
 
 To install the optional requirements also run the following command:
 
 ```
-sudo apt install python3-all debhelper dh-python dh-systemd
+sudo apt install python3-all debhelper dh-python
 ```
 
 ## Checkout the code
 
 Use `git` to clone / checkout `smartmeter-datacollector` from GitHub using
 
 ```
@@ -343,28 +262,26 @@
 ```
 
 This will install all runtime and development dependencies for `smartmeter-datacollector` in a new virtual environment. Now you are ready to start working on `smartmeter-datacollector`.
 
 ## Custom Commands / Workflows
 
 `smartmeter-datacollector` offers a few custom `pipenv run` commands to simplify certain development workflows:
+* `build_check` uses `twine` to check if the built Python package will be accepted by `PiPI`.
+* `build_deb` builds a Debian package for the current development platform.
+* `build_srcdeb` builds a Debian source package which can be used to build a Debian (binary) package for any platform (e.g. using [`pbuilder`](https://pbuilder-docs.readthedocs.io/en/latest/usage.html))
+* `build` builds a Python package which can be uploaded to [`PyPI`](https://pypi.org/project/smartmeter-datacollector/) using `twine`.
+* `debianize` creates a `debian/` directory used to build Debian source / binary packages.
 * `format_check` checks if the code follows the [`autopep8`](https://pypi.org/project/autopep8/) code formatting rules.
 * `format` automatically adjusts the code to follow the `autopep8` code formatting rules.
 * `isort_check` checks if the order of the import statements is correct using [`isort`](https://pycqa.github.io/isort/).
 * `isort` automatically re-orders the import statements using `isort`.
+* `license` makes sure every Python (`*.py`) file contains the proper license header.
 * `lint_check` checks if the code follows the [`pylint`](https://pypi.org/project/pylint/) rules defined in `pyproject.toml`.
 * `lint` automatically adjust the code to follow the `pylint` rules defined in `pyproject.toml`.
-* `license` makes sure every Python (`*.py`) file contains the proper license header.
-* `build` builds a Python package which can be uploaded to [`PyPI`](https://pypi.org/project/smartmeter-datacollector/) using `twine`.
-* `build_check` uses `twine` to check if the built Python package will be accepted by `PiPI`.
 * `setup_check` checks whether the dependencies defined in `Pipfile` / `Pipfile.lock` are in sync with `setup.py`.
 * `setup` synchronizes the dependencies defined in `Pipfile` / `Pipfile.lock` with `setup.py`.
-* `debianize` creates a `debian/` directory used to build Debian source / binary packages.
-* `build_srcdeb` builds a Debian source package which can be used to build a Debian (binary) package for any platform (e.g. using [`pbuilder`](https://pbuilder-docs.readthedocs.io/en/latest/usage.html))
-* `build_deb` builds a Debian package for the current development plattform.
 
-Make sure to run `format_check` / `format`, `isort_check` / `isort`, `lint_check` / `lint`, `license`, `setup_check` / `setup` before commiting changes to the repository to avoid unnecessary development cycles. `smartmeter-datacollector` uses [GitHub Actions](https://github.com/scs/smartmeter-datacollector/actions) to check if these rules apply.
+Make sure to run `format_check` / `format`, `isort_check` / `isort`, `lint_check` / `lint`, `license`, `setup_check` / `setup` before committing changes to the repository to avoid unnecessary development cycles. `smartmeter-datacollector` uses [GitHub Actions](https://github.com/scs/smartmeter-datacollector/actions) to check if these rules apply.
 
 # Acknowledgements
 `smartmeter-datacollector` and its companion project [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-configurator) have been developed by **[Supercomputing Systems AG](https://www.scs.ch)** on behalf of and funded by **[EKZ](https://www.ekz.ch/)**.
-
-
```

#### html2text {}

```diff
@@ -1,48 +1,54 @@
-Metadata-Version: 2.1 Name: smartmeter-datacollector Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: smartmeter-datacollector Version: 1.1.0 Summary:
 Smart Meter Data Collector Home-page: https://github.com/scs/smartmeter-
 datacollector Author: Supercomputing Systems AG Author-email: info@scs.ch
-License: GPLv2 Project-URL: Source, https://github.com/scs/smartmeter-
-datacollector Project-URL: Bug Reports, https://github.com/scs/smartmeter-
-datacollector/issues Project-URL: Pull Requests, https://github.com/scs/
-smartmeter-datacollector/pulls Project-URL: SCS, https://www.scs.ch Platform:
-UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
-License :: OSI Approved :: GNU General Public License v2 (GPLv2) Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Typing :: Typed Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE # Smart Meter
-Data Collector
+Maintainer: Supercomputing Systems AG Maintainer-email: info@scs.ch License:
+GPLv2 Project-URL: Source, https://github.com/scs/smartmeter-datacollector
+Project-URL: Bug Reports, https://github.com/scs/smartmeter-datacollector/
+issues Project-URL: Pull Requests, https://github.com/scs/smartmeter-
+datacollector/pulls Project-URL: SCS, https://www.scs.ch Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: GNU General Public License v2 (GPLv2) Classifier: Programming Language ::
+Python Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Typing :: Typed Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE # Smart Meter Data Collector
    [License:_GPL-2.0-only] [Pull_Requests_Welcome] [Contributions_Welcome]
                  [Python Code Checks] [PyPI_-_Python_Version]
                                 [ekz_logo.png]
 --- The `smartmeter-datacollector` tool is a Python3 software which allows you
 to continuously retrieve data from supported smart meters (listed below). The
 acquired values can be forwarded to one or more data sinks like a MQTT broker
 or logger. This tool is an open source software funded by **[EKZ
 (ElektrizitÃ¤tswerke des Kantons ZÃ¼rich)](https://www.ekz.ch)** and developed
 by **[Supercomputing Systems AG](https://www.scs.ch)**. The goal of this
 voluntary initiative is to create a tool that can read, decode and decrypt data
 (if necessary) from the local interface of various smart meters and convert it
 into human-readable and simple formats. This should eliminate the complexity of
 decoding DLMS and similar protocols for the user. The user has the data in a
 format, which he can easily use in various use-cases ranging from simple
-vizualization (see [Method 1: Raspberry Pi image with demo](#method-1-
+visualization (see [Method 1: Raspberry Pi image with demo](#method-1-
 raspberry-pi-image-with-demo)) to integration into energy management algorithms
 or into custom home automation software. The following smart meters are
-supported: * Landis+Gyr E450: \ Data pushed by smart meter over CII interface
-(wired M-Bus). Encoded with HDLC and DLMS/COSEM. * Unencrypted data * Encrypted
-data * Iskraemeco AM550: \ Data pushed by smart meter over [P1 interface
-(DSMR)](https://www.netbeheernederland.nl/_upload/Files/
-Slimme_meter_15_a727fce1f1.pdf). Encoded with HDLC (IEC 62056-46) and DLMS/
-COSEM. * Unencrypted data * Encrypted data The following data sinks are
+supported (see [Wiki/Home](https://github.com/scs/smartmeter-datacollector/
+wiki/Home) for detailed information). * Landis+Gyr E450: \ Data pushed by smart
+meter over CII interface (wired M-Bus, HDLC, DLMS/COSEM). * Landis+Gyr E360: \
+Data pushed by smart meter over P1 interface (HDLC, DLMS/COSEM only, no DSMR).
+* Iskraemeco AM550: \ Data pushed by smart meter over P1 interface (HDLC, DLMS/
+COSEM only, no DSMR). * Kamstrup OMNIPOWER with HAN-NVE: \ Data pushed by smart
+meter over inserted [HAN-NVE module](https://www.kamstrup.com/en-en/
+electricity-solutions/meters-devices/modules/hannve) (wired M-Bus, HDLC, DLMS/
+COSEM). Note: All smart meters integrated so far push binary data encoded with
+HDLC (IEC 62056-46) and DLMS/COSEM. Both unencrypted and encrypted DLMS
+messages are accepted by the software. The following data sinks are
 implemented: * MQTT (v3.1.1): * Encryption * Unencrypted connection * Encrypted
 connection * TLS * optional custom CA certificate * Authentication *
 Unauthenticated * Authenticated with username / password * Authenticated with
-client certificate * Logger to STDOUT `smartmeter-datacollector` is fully
+client certificate * Logger to `stdout` `smartmeter-datacollector` is fully
 configurable through a `.ini` configuration file. The [`smartmeter-
 datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-
 configurator) webinterface can help to create and modify the configuration. --
 - - [Smart Meter Data Collector](#smart-meter-data-collector) - [How to
 install](#how-to-install) - [Method 1: Raspberry Pi image with demo](#method-1-
 raspberry-pi-image-with-demo) - [Method 2: Python package](#method-2-python-
 package) - [Python Requirements](#python-requirements) - [Installation]
@@ -65,156 +71,116 @@
 (based on Raspberry Pi OS) which contains the following parts: * `smartmeter-
 datacollector` as a systemd service * `smartmeter-datacollector-configurator`
 webinterface * demo * [mosquiotto](https://mosquitto.org/) as a local MQTT
 broker to publish the measurements from `smartmeter-datacollector` * [Telegraf]
 (https://www.influxdata.com/time-series-platform/telegraf/) to collect
 measurements published by `smartmeter-datacollector` over MQTT and store them
 in InfluxDB * [InfluxDB](https://www.influxdata.com/) to store the measurements
-* [Grafana](https://grafana.com/) to visualize the measurements This setup
-allows a (first time) user to [install](https://www.raspberrypi.org/
-documentation/computers/getting-started.html#installing-the-operating-system)
-the image on a Raspberry Pi and immediately get started with `smartmeter-
-datacollector`. The following steps are required: 1. Download the Raspberry Pi
-image from the [latest release](https://github.com/scs/smartmeter-
-datacollector/releases). 2. Install the image on a (micro)SD card, e.g. using
-[Raspberry Pi Imager](https://www.raspberrypi.org/documentation/computers/
-getting-started.html#using-raspberry-pi-imager). 3. Prepare the Raspberry Pi.
-1. Push the (micro)SD card into the proper slot. 2. Use an RJ-45 cable (or
-configure WiFi later) to connect to a network. 3. Connect the power cable to
-the Micro USB port. 4. Open the `smartmeter-datacollector-configurator`
-webinterface using `http://:8000/` in your favorite browser. 1. Load the pre-
-defined configuration. 2. Adjust the settings of the connected smart meter. 3.
-Deploy the adjusted configuration. 4. Restart the `smartmeter-datacollector`
-service. 5. Open `Grafana` using `http://:3000/` in your favorite browser. 6.
-Observe the measurements from your smart meter while they arrive periodically.
-See [Wiki/Demo](https://github.com/scs/smartmeter-datacollector/wiki/Demo-
-(Raspberry-Pi-Image)) for more details on the provided Raspberry Pi image with
-the demo. ## Method 2: Python package `smartmeter-datacollector` can be
-installed as a Python3 package either from [PyPi](https://pypi.org/project/
-smartmeter-datacollector/) or manually using a [released wheel](https://
-github.com/scs/smartmeter-datacollector/releases). The Python3 package does not
-contain any infrastructure to run `smartmeter-datacollector` in the background
-or to automatically start it during a boot sequence. If such infrastructure is
-required either see [Method 3: Debian package](#method-3-debian-package) or
-provide it yourself. ### Python Requirements * Python >= 3.7 (tested with 3.8)
-### Installation Install the package either as global Python package or in a
-virtualenv with ```bash python3 -m pip install smartmeter-datacollector ```
-Similarly the [`smartmeter-datacollector-configurator`](https://github.com/scs/
-smartmeter-datacollector-configurator) webinterface can be installed with
-```bash python3 -m pip install smartmeter-datacollector-configurator ``` ##
-Method 3: Debian package `smartmeter-datacollector` is also available as a
-Debian (`.deb`) package from the [releases](https://github.com/scs/smartmeter-
-datacollector/releases) which installs it system wide. The Debian package
-includes a systemd service file which enables `smartmeter-datacollector` to
-automatically start after booting the system. ### Debian Requirements *
-Distribution * Debian * Release * Buster * CPU architecture * amd64 * armhf ###
-Installation Download the Debian package from [releases](https://github.com/
-scs/smartmeter-datacollector/releases) and install it with ```bash sudo apt
-install ./python3-smartmeter-datacollector_*.deb ``` Similarly the
-[`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-
-datacollector-configurator) webinterface can be installed with a Debian package
-from its [releases](https://github.com/scs/smartmeter-datacollector-
-configurator/releases) with ```bash sudo apt install ./python3-smartmeter-
-datacollector-configurator_*.deb ``` # How to use The usage of `smartmeter-
-datacollector` depends on the installation method. Independent of the
-installation method a `.ini` configuration file is required to properly run
-`smartmeter-datacollector`. ## Configuration ### Specification The `.ini`
-configuration file supports the following format ```ini [reader0] # type of the
-connected smart meter type = lge450 # serial port to which the smart meter is
-connected port = /dev/ttyUSB0 # optional encryption key key = [sink0] # type of
-the sink type = mqtt # host / IP address of the MQTT broker host = localhost #
-port of the MQTT broker port = 1883 # whether to use TLS (Transport Layer
-Security) tls = False # optional path to the CA certificate used to validate
-the MQTT broker's certificate ca_file_path = # whether to check the hostname of
-the MQTT broker against the certificate check_hostname = False # optional
-username for authentication with the MQTT broker username = # optional password
-for authentication with the MQTT broker password = # optional path to the
-client certificate for authentication with the MQTT broker client_cert_path = #
-optional path to the private key for the client certificate for authentication
-with the MQTT broker client_key_path = [sink1] # type of the sink type = logger
-# name of the logger name = DataLogger [logging] # log level configuration:
-DEBUG / INFO / WARNING / ERROR default = WARNING smartmeter = WARNING collector
-= WARNING sink = WARNING ``` There can be multiple `[readerX]` and `[sinkY]`
-sections for every connected smart meter and / or data sink. See [Wiki/
-Configuration](https://github.com/scs/smartmeter-datacollector/wiki/
-Configuration) for more details on the available configuration options. ###
-smartmeter-datacollector-configurator To simplify the process of generating a
-valid `.ini` configuration for `smartmeter-datacollector` the companion
-[`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-
-datacollector-configurator) webinterface can be used. It supports * a graphical
-approach to manage the configuration * input validation to avoid invalid
-configurations * loading / saving / discarding a configuration * restarting
-`smartmeter-datacollector` (only if installed as a Debian package) See [Wiki/
-smartmeter-datacollector-configurator](https://github.com/scs/smartmeter-
-datacollector/wiki/smartmeter-datacollector-configurator) for more details on
-the webinterface and the configuration possibilities. ## Run manually Run
+* [Grafana](https://grafana.com/) to visualize the measurements See [Wiki/Demo]
+(https://github.com/scs/smartmeter-datacollector/wiki/Demo-(Raspberry-Pi-
+Image)) for detailed setup instructions. ## Method 2: Python package
+`smartmeter-datacollector` can be installed as a Python3 package either from
+[PyPi](https://pypi.org/project/smartmeter-datacollector/) or manually using a
+[released wheel](https://github.com/scs/smartmeter-datacollector/releases). The
+Python3 package does not contain any infrastructure to run `smartmeter-
+datacollector` in the background or to automatically start it during a boot
+sequence. If such infrastructure is required either see [Method 3: Debian
+package](#method-3-debian-package) or provide it yourself. ### Python
+Requirements * Python >= 3.7 (tested with 3.8) ### Installation Install the
+package either as global Python package or in a virtualenv with ```bash python3
+-m pip install smartmeter-datacollector ``` Similarly the [`smartmeter-
+datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-
+configurator) webinterface can be installed with ```bash python3 -m pip install
+smartmeter-datacollector-configurator ``` ## Method 3: Debian package
+`smartmeter-datacollector` is also available as a Debian (`.deb`) package from
+the [releases](https://github.com/scs/smartmeter-datacollector/releases) which
+installs it system wide. The Debian package includes a systemd service file
+which enables `smartmeter-datacollector` to automatically start after booting
+the system. ### Debian Requirements * Distribution * Debian * Release *
+Bullseye * CPU architecture * amd64 * armhf ### Installation Download the
+Debian package from [releases](https://github.com/scs/smartmeter-datacollector/
+releases) and install it with ```bash sudo apt install ./python3-smartmeter-
+datacollector_*.deb ``` Similarly the [`smartmeter-datacollector-configurator`]
+(https://github.com/scs/smartmeter-datacollector-configurator) webinterface can
+be installed with a Debian package from its [releases](https://github.com/scs/
+smartmeter-datacollector-configurator/releases) with ```bash sudo apt install
+./python3-smartmeter-datacollector-configurator_*.deb ``` # How to use The
+usage of `smartmeter-datacollector` depends on the installation method.
+Independent of the installation method a `.ini` configuration file is required
+to properly run `smartmeter-datacollector`. ## Configuration ### Manually
+create configuration See [Wiki/Configuration](https://github.com/scs/
+smartmeter-datacollector/wiki/Configuration#manually-write-configuration) for
+more details on the available configuration options. ### smartmeter-
+datacollector-configurator To simplify the process of generating a valid `.ini`
+configuration for `smartmeter-datacollector` the companion [`smartmeter-
+datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-
+configurator) webinterface can be used. It supports * a graphical approach to
+manage the configuration * input validation to avoid invalid configurations *
+loading / saving / discarding a configuration * restarting `smartmeter-
+datacollector` (only if installed as a Debian package) See [Wiki/smartmeter-
+datacollector-configurator](https://github.com/scs/smartmeter-datacollector/
+wiki/smartmeter-datacollector-configurator) for more details on the
+webinterface and the configuration possibilities. ## Run manually Run
 `smartmeter-datacollector` with the following command: ``` smartmeter-
 datacollector --config datacollector.ini ``` The following command line
 arguments are supported: * `-h, --help`: Shows the help output of `smartmeter-
 datacollector`. * `-c, --config CONFIG`: Path to the `.ini` configuration file.
-* `-s,--saveconfig`: Cteate a default `.ini` configuration file. * `-d, --dev`:
+* `-s,--saveconfig`: Create a default `.ini` configuration file. * `-d, --dev`:
 Enable development mode. ### Configuration The configuration file can be
 located anywhere and use any filename. If no `.ini` configuration file is
 specified a default configuration with the following options is used: *
-Landys+Gir E450 smart meter in unencrypted mode connected to `/dev/ttyUSB0` *
+Landys+Gyr E450 smart meter in unencrypted mode connected to `/dev/ttyUSB0` *
 `LOGGER` sink * `MQTT` sink connected to a local broker without encryption or
 authentication ## Run as a systemd service When `smartmeter-datacollector` has
 been installed as a Debian package it provides a systemd .service file named
 `python3-smartmeter-datacollector.service`. Therefore the service can be
-managed using the `systemctl` command: ``` sudo systemctl start|stop|restart
-python3-smartmeter-datacollector ``` Enabling or disabling the service can also
-be managed using the `systemctl` command: ``` sudo systemctl enable|disable
-python3-smartmeter-datacollector ``` Inspecting the log messages can be done
-using the `journalctl` command: ``` journalctl -u python3-smartmeter-
-datacollector [-f] ``` ### Configuration The systemd service expectes the
-`.ini` configuration to be located at `/var/lib/smartmeter-datacollector/
-datacollector.ini`. This is also the default location used by the [`smartmeter-
-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-
-configurator) webinterface to load and save the managed configuration. # How to
-develop Help from the community for the `smartmeter-datacollector` project is
-always welcome. Please follow the next few chapters to setup a working
-development environment. ## Development Requirements * Python >= 3.7 *
-[`pipenv`](https://pipenv.pypa.io/en/latest/) * Optional software packages
-(Debian / Ubuntu) * python3-all * debhelper * dh-python * dh-systemd ##
-Installation ### Debian / Ubuntu To install the listed minimal requirements run
-the following command: ``` sudo apt install git python3 pipenv ``` To install
-the optional requirements also run the following command: ``` sudo apt install
-python3-all debhelper dh-python dh-systemd ``` ## Checkout the code Use `git`
-to clone / checkout `smartmeter-datacollector` from GitHub using ``` git clone
-https://github.com/scs/smartmeter-datacollector.git ``` ## Setup Development
-Environment `smartmeter-datacollector` uses [`pipenv`](https://pipenv.pypa.io/
-en/latest/) to manage its dependencies and setup a virtual environment. Run the
-following command to setup the initial development environment: ``` pipenv
-install --dev ``` This will install all runtime and development dependencies
-for `smartmeter-datacollector` in a new virtual environment. Now you are ready
-to start working on `smartmeter-datacollector`. ## Custom Commands / Workflows
-`smartmeter-datacollector` offers a few custom `pipenv run` commands to
-simplify certain development workflows: * `format_check` checks if the code
-follows the [`autopep8`](https://pypi.org/project/autopep8/) code formatting
-rules. * `format` automatically adjusts the code to follow the `autopep8` code
-formatting rules. * `isort_check` checks if the order of the import statements
-is correct using [`isort`](https://pycqa.github.io/isort/). * `isort`
-automatically re-orders the import statements using `isort`. * `lint_check`
-checks if the code follows the [`pylint`](https://pypi.org/project/pylint/
-) rules defined in `pyproject.toml`. * `lint` automatically adjust the code to
-follow the `pylint` rules defined in `pyproject.toml`. * `license` makes sure
-every Python (`*.py`) file contains the proper license header. * `build` builds
-a Python package which can be uploaded to [`PyPI`](https://pypi.org/project/
-smartmeter-datacollector/) using `twine`. * `build_check` uses `twine` to check
-if the built Python package will be accepted by `PiPI`. * `setup_check` checks
-whether the dependencies defined in `Pipfile` / `Pipfile.lock` are in sync with
-`setup.py`. * `setup` synchronizes the dependencies defined in `Pipfile` /
-`Pipfile.lock` with `setup.py`. * `debianize` creates a `debian/` directory
-used to build Debian source / binary packages. * `build_srcdeb` builds a Debian
+managed using the `systemctl` command. See [Run as a systemd service](https://
+github.com/scs/smartmeter-datacollector/wiki/How-to-use#run-as-a-systemd-
+service) for possible commands. # How to develop Help from the community for
+the `smartmeter-datacollector` project is always welcome. Please follow the
+next few chapters to setup a working development environment. ## Development
+Requirements * Python >= 3.8, <= 3.10 * [`pipenv`](https://pipenv.pypa.io/en/
+latest/) * Optional software packages (Debian bullseye/ Ubuntu 22.04) *
+python3-all * debhelper * dh-python ## Installation ### Debian / Ubuntu To
+install the listed minimal requirements run the following command: ``` sudo apt
+install git python3 pipenv ``` To install the optional requirements also run
+the following command: ``` sudo apt install python3-all debhelper dh-python ```
+## Checkout the code Use `git` to clone / checkout `smartmeter-datacollector`
+from GitHub using ``` git clone https://github.com/scs/smartmeter-
+datacollector.git ``` ## Setup Development Environment `smartmeter-
+datacollector` uses [`pipenv`](https://pipenv.pypa.io/en/latest/) to manage its
+dependencies and setup a virtual environment. Run the following command to
+setup the initial development environment: ``` pipenv install --dev ``` This
+will install all runtime and development dependencies for `smartmeter-
+datacollector` in a new virtual environment. Now you are ready to start working
+on `smartmeter-datacollector`. ## Custom Commands / Workflows `smartmeter-
+datacollector` offers a few custom `pipenv run` commands to simplify certain
+development workflows: * `build_check` uses `twine` to check if the built
+Python package will be accepted by `PiPI`. * `build_deb` builds a Debian
+package for the current development platform. * `build_srcdeb` builds a Debian
 source package which can be used to build a Debian (binary) package for any
 platform (e.g. using [`pbuilder`](https://pbuilder-docs.readthedocs.io/en/
-latest/usage.html)) * `build_deb` builds a Debian package for the current
-development plattform. Make sure to run `format_check` / `format`,
-`isort_check` / `isort`, `lint_check` / `lint`, `license`, `setup_check` /
-`setup` before commiting changes to the repository to avoid unnecessary
-development cycles. `smartmeter-datacollector` uses [GitHub Actions](https://
-github.com/scs/smartmeter-datacollector/actions) to check if these rules apply.
-# Acknowledgements `smartmeter-datacollector` and its companion project
+latest/usage.html)) * `build` builds a Python package which can be uploaded to
+[`PyPI`](https://pypi.org/project/smartmeter-datacollector/) using `twine`. *
+`debianize` creates a `debian/` directory used to build Debian source / binary
+packages. * `format_check` checks if the code follows the [`autopep8`](https://
+pypi.org/project/autopep8/) code formatting rules. * `format` automatically
+adjusts the code to follow the `autopep8` code formatting rules. *
+`isort_check` checks if the order of the import statements is correct using
+[`isort`](https://pycqa.github.io/isort/). * `isort` automatically re-orders
+the import statements using `isort`. * `license` makes sure every Python
+(`*.py`) file contains the proper license header. * `lint_check` checks if the
+code follows the [`pylint`](https://pypi.org/project/pylint/) rules defined in
+`pyproject.toml`. * `lint` automatically adjust the code to follow the `pylint`
+rules defined in `pyproject.toml`. * `setup_check` checks whether the
+dependencies defined in `Pipfile` / `Pipfile.lock` are in sync with `setup.py`.
+* `setup` synchronizes the dependencies defined in `Pipfile` / `Pipfile.lock`
+with `setup.py`. Make sure to run `format_check` / `format`, `isort_check` /
+`isort`, `lint_check` / `lint`, `license`, `setup_check` / `setup` before
+committing changes to the repository to avoid unnecessary development cycles.
+`smartmeter-datacollector` uses [GitHub Actions](https://github.com/scs/
+smartmeter-datacollector/actions) to check if these rules apply. #
+Acknowledgements `smartmeter-datacollector` and its companion project
 [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-
 datacollector-configurator) have been developed by **[Supercomputing Systems
 AG](https://www.scs.ch)** on behalf of and funded by **[EKZ](https://
 www.ekz.ch/)**.
```

### Comparing `smartmeter-datacollector-1.0.2/README.md` & `smartmeter-datacollector-1.1.0/smartmeter_datacollector.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: smartmeter-datacollector
+Version: 1.1.0
+Summary: Smart Meter Data Collector
+Home-page: https://github.com/scs/smartmeter-datacollector
+Author: Supercomputing Systems AG
+Author-email: info@scs.ch
+Maintainer: Supercomputing Systems AG
+Maintainer-email: info@scs.ch
+License: GPLv2
+Project-URL: Source, https://github.com/scs/smartmeter-datacollector
+Project-URL: Bug Reports, https://github.com/scs/smartmeter-datacollector/issues
+Project-URL: Pull Requests, https://github.com/scs/smartmeter-datacollector/pulls
+Project-URL: SCS, https://www.scs.ch
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Smart Meter Data Collector
 
 <p align="center">
     <a href="LICENSE"><img alt="License: GPL-2.0-only" src="https://img.shields.io/badge/license-GPLv2-blue.svg"></a> <a href="https://github.com/scs/smartmeter-datacollector/pulls"><img alt="Pull Requests Welcome" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg"></a> <a href="https://github.com/scs/smartmeter-datacollector/pulls"><img alt="Contributions Welcome" src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg"></a>
     <br />
     <img alt="Python Code Checks" src="https://github.com/scs/smartmeter-datacollector/actions/workflows/python-code-checks.yml/badge.svg?branch=master"> <a href="https://pypi.org/project/smartmeter-datacollector/"><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/smartmeter-datacollector"></a>
     <br />
@@ -9,39 +35,41 @@
 </p>
 
 ---
 
 The `smartmeter-datacollector` tool is a Python3 software which allows you to continuously retrieve data from supported smart meters (listed below).
 The acquired values can be forwarded to one or more data sinks like a MQTT broker or logger.
 
-This tool is an open source software funded by **[EKZ (Elektrizitätswerke des Kantons Zürich)](https://www.ekz.ch)** and developed by **[Supercomputing Systems AG](https://www.scs.ch)**. The goal of this voluntary initiative is to create a tool that can read, decode and decrypt data (if necessary) from the local interface of various smart meters and convert it into human-readable and simple formats. This should eliminate the complexity of decoding DLMS and similar protocols for the user. The user has the data in a format, which he can easily use in various use-cases ranging from simple vizualization (see [Method 1: Raspberry Pi image with demo](#method-1-raspberry-pi-image-with-demo)) to integration into energy management algorithms or into custom home automation software. 
+This tool is an open source software funded by **[EKZ (Elektrizitätswerke des Kantons Zürich)](https://www.ekz.ch)** and developed by **[Supercomputing Systems AG](https://www.scs.ch)**. The goal of this voluntary initiative is to create a tool that can read, decode and decrypt data (if necessary) from the local interface of various smart meters and convert it into human-readable and simple formats. This should eliminate the complexity of decoding DLMS and similar protocols for the user. The user has the data in a format, which he can easily use in various use-cases ranging from simple visualization (see [Method 1: Raspberry Pi image with demo](#method-1-raspberry-pi-image-with-demo)) to integration into energy management algorithms or into custom home automation software. 
 
-The following smart meters are supported:
+The following smart meters are supported (see [Wiki/Home](https://github.com/scs/smartmeter-datacollector/wiki/Home) for detailed information).
 
 * Landis+Gyr E450: \
-  Data pushed by smart meter over CII interface (wired M-Bus). Encoded with HDLC and DLMS/COSEM.
-  * Unencrypted data
-  * Encrypted data
+  Data pushed by smart meter over CII interface (wired M-Bus, HDLC, DLMS/COSEM).
+* Landis+Gyr E360: \
+  Data pushed by smart meter over P1 interface (HDLC, DLMS/COSEM only, no DSMR).
 * Iskraemeco AM550: \
-  Data pushed by smart meter over [P1 interface (DSMR)](https://www.netbeheernederland.nl/_upload/Files/Slimme_meter_15_a727fce1f1.pdf). Encoded with HDLC (IEC 62056-46) and DLMS/COSEM.
-  * Unencrypted data
-  * Encrypted data
+  Data pushed by smart meter over P1 interface (HDLC, DLMS/COSEM only, no DSMR).
+* Kamstrup OMNIPOWER with HAN-NVE: \
+  Data pushed by smart meter over inserted [HAN-NVE module](https://www.kamstrup.com/en-en/electricity-solutions/meters-devices/modules/hannve) (wired M-Bus, HDLC, DLMS/COSEM).
+
+Note: All smart meters integrated so far push binary data encoded with HDLC (IEC 62056-46) and DLMS/COSEM. Both unencrypted and encrypted DLMS messages are accepted by the software.
 
 The following data sinks are implemented:
 * MQTT (v3.1.1):
   * Encryption
     * Unencrypted connection
     * Encrypted connection
       * TLS
       * optional custom CA certificate
   * Authentication
     * Unauthenticated
     * Authenticated with username / password
     * Authenticated with client certificate
-* Logger to STDOUT
+* Logger to `stdout`
 
 `smartmeter-datacollector` is fully configurable through a `.ini` configuration file. The [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-configurator) webinterface can help to create and modify the configuration.
 
 ---
 
 - [Smart Meter Data Collector](#smart-meter-data-collector)
 - [How to install](#how-to-install)
@@ -84,30 +112,15 @@
 * `smartmeter-datacollector-configurator` webinterface
 * demo
   * [mosquiotto](https://mosquitto.org/) as a local MQTT broker to publish the measurements from `smartmeter-datacollector`
   * [Telegraf](https://www.influxdata.com/time-series-platform/telegraf/) to collect measurements published by `smartmeter-datacollector` over MQTT and store them in InfluxDB
   * [InfluxDB](https://www.influxdata.com/) to store the measurements
   * [Grafana](https://grafana.com/) to visualize the measurements
 
-This setup allows a (first time) user to [install](https://www.raspberrypi.org/documentation/computers/getting-started.html#installing-the-operating-system) the image on a Raspberry Pi and immediately get started with `smartmeter-datacollector`. The following steps are required:
-1. Download the Raspberry Pi image from the [latest release](https://github.com/scs/smartmeter-datacollector/releases).
-2. Install the image on a (micro)SD card, e.g. using [Raspberry Pi Imager](https://www.raspberrypi.org/documentation/computers/getting-started.html#using-raspberry-pi-imager).
-3. Prepare the Raspberry Pi.
-   1. Push the (micro)SD card into the proper slot.
-   2. Use an RJ-45 cable (or configure WiFi later) to connect to a network.
-   3. Connect the power cable to the Micro USB port.
-4. Open the `smartmeter-datacollector-configurator` webinterface using `http://<Raspberry Pi IP>:8000/` in your favorite browser.
-   1. Load the pre-defined configuration.
-   2. Adjust the settings of the connected smart meter.
-   3. Deploy the adjusted configuration.
-   4. Restart the `smartmeter-datacollector` service.
-5. Open `Grafana` using `http://<Raspberry Pi IP>:3000/` in your favorite browser.
-6. Observe the measurements from your smart meter while they arrive periodically.
-
-See [Wiki/Demo](https://github.com/scs/smartmeter-datacollector/wiki/Demo-(Raspberry-Pi-Image)) for more details on the provided Raspberry Pi image with the demo.
+See [Wiki/Demo](https://github.com/scs/smartmeter-datacollector/wiki/Demo-(Raspberry-Pi-Image)) for detailed setup instructions.
 
 ## Method 2: Python package
 
 `smartmeter-datacollector` can be installed as a Python3 package either from [PyPi](https://pypi.org/project/smartmeter-datacollector/) or manually using a [released wheel](https://github.com/scs/smartmeter-datacollector/releases).
 
 The Python3 package does not contain any infrastructure to run `smartmeter-datacollector` in the background or to automatically start it during a boot sequence. If such infrastructure is required either see [Method 3: Debian package](#method-3-debian-package) or provide it yourself.
 
@@ -134,15 +147,15 @@
 `smartmeter-datacollector` is also available as a Debian (`.deb`) package from the [releases](https://github.com/scs/smartmeter-datacollector/releases) which installs it system wide. The Debian package includes a systemd service file which enables `smartmeter-datacollector` to automatically start after booting the system.
 
 ### Debian Requirements
 
 * Distribution
   * Debian
 * Release
-  * Buster
+  * Bullseye
 * CPU architecture
   * amd64
   * armhf
 
 ### Installation
 
 Download the Debian package from [releases](https://github.com/scs/smartmeter-datacollector/releases) and install it with
@@ -159,66 +172,17 @@
 
 # How to use
 
 The usage of `smartmeter-datacollector` depends on the installation method. Independent of the installation method a `.ini` configuration file is required to properly run `smartmeter-datacollector`.
 
 ## Configuration
 
-### Specification
-
-The `.ini` configuration file supports the following format
+### Manually create configuration
 
-```ini
-[reader0]
-# type of the connected smart meter
-type = lge450
-# serial port to which the smart meter is connected
-port = /dev/ttyUSB0
-# optional encryption key
-key = 
-
-[sink0]
-# type of the sink
-type = mqtt
-# host / IP address of the MQTT broker
-host = localhost
-# port of the MQTT broker
-port = 1883
-# whether to use TLS (Transport Layer Security)
-tls = False
-# optional path to the CA certificate used to validate the MQTT broker's certificate
-ca_file_path = 
-# whether to check the hostname of the MQTT broker against the certificate
-check_hostname = False
-# optional username for authentication with the MQTT broker
-username = 
-# optional password for authentication with the MQTT broker
-password = 
-# optional path to the client certificate for authentication with the MQTT broker
-client_cert_path = 
-# optional path to the private key for the client certificate for authentication with the MQTT broker
-client_key_path = 
-
-[sink1]
-# type of the sink
-type = logger
-# name of the logger
-name = DataLogger
-
-[logging]
-# log level configuration: DEBUG / INFO / WARNING / ERROR
-default = WARNING
-smartmeter = WARNING
-collector = WARNING
-sink = WARNING
-```
-
-There can be multiple `[readerX]` and `[sinkY]` sections for every connected smart meter and / or data sink.
-
-See [Wiki/Configuration](https://github.com/scs/smartmeter-datacollector/wiki/Configuration) for more details on the available configuration options.
+See [Wiki/Configuration](https://github.com/scs/smartmeter-datacollector/wiki/Configuration#manually-write-configuration) for more details on the available configuration options.
 
 ### smartmeter-datacollector-configurator
 
 To simplify the process of generating a valid `.ini` configuration for `smartmeter-datacollector` the companion [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-configurator) webinterface can be used. It supports
 * a graphical approach to manage the configuration
 * input validation to avoid invalid configurations
 * loading / saving / discarding a configuration
@@ -233,77 +197,56 @@
 ```
 smartmeter-datacollector --config datacollector.ini
 ```
 
 The following command line arguments are supported:
 * `-h, --help`: Shows the help output of `smartmeter-datacollector`.
 * `-c, --config CONFIG`: Path to the `.ini` configuration file.
-* `-s,--saveconfig`: Cteate a default `.ini` configuration file.
+* `-s,--saveconfig`: Create a default `.ini` configuration file.
 * `-d, --dev`: Enable development mode.
 
 ### Configuration
 
 The configuration file can be located anywhere and use any filename. If no `.ini` configuration file is specified a default configuration with the following options is used:
-* Landys+Gir E450 smart meter in unencrypted mode connected to `/dev/ttyUSB0`
+* Landys+Gyr E450 smart meter in unencrypted mode connected to `/dev/ttyUSB0`
 * `LOGGER` sink
 * `MQTT` sink connected to a local broker without encryption or authentication
 
 ## Run as a systemd service
 
-When `smartmeter-datacollector` has been installed as a Debian package it provides a systemd .service file named `python3-smartmeter-datacollector.service`. Therefore the service can be managed using the `systemctl` command:
-
-```
-sudo systemctl start|stop|restart python3-smartmeter-datacollector
-```
-
-Enabling or disabling the service can also be managed using the `systemctl` command:
-
-```
-sudo systemctl enable|disable python3-smartmeter-datacollector
-```
-
-Inspecting the log messages can be done using the `journalctl` command:
+When `smartmeter-datacollector` has been installed as a Debian package it provides a systemd .service file named `python3-smartmeter-datacollector.service`. Therefore the service can be managed using the `systemctl` command. See [Run as a systemd service](https://github.com/scs/smartmeter-datacollector/wiki/How-to-use#run-as-a-systemd-service) for possible commands.
 
-```
-journalctl -u python3-smartmeter-datacollector [-f]
-```
-
-### Configuration
-
-The systemd service expectes the `.ini` configuration to be located at
-`/var/lib/smartmeter-datacollector/datacollector.ini`. This is also the default location used by the [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-configurator) webinterface to load and save the managed configuration.
 
 # How to develop
 
 Help from the community for the `smartmeter-datacollector` project is always welcome. Please follow the next few chapters to setup a working development environment.
 
 ## Development Requirements
 
-* Python >= 3.7
+* Python >= 3.8, <= 3.10
 * [`pipenv`](https://pipenv.pypa.io/en/latest/)
-* Optional software packages (Debian / Ubuntu)
+* Optional software packages (Debian bullseye/ Ubuntu 22.04)
   * python3-all
   * debhelper
   * dh-python
-  * dh-systemd
 
 ## Installation
 
 ### Debian / Ubuntu
 
 To install the listed minimal requirements run the following command:
 
 ```
 sudo apt install git python3 pipenv
 ```
 
 To install the optional requirements also run the following command:
 
 ```
-sudo apt install python3-all debhelper dh-python dh-systemd
+sudo apt install python3-all debhelper dh-python
 ```
 
 ## Checkout the code
 
 Use `git` to clone / checkout `smartmeter-datacollector` from GitHub using
 
 ```
@@ -319,26 +262,26 @@
 ```
 
 This will install all runtime and development dependencies for `smartmeter-datacollector` in a new virtual environment. Now you are ready to start working on `smartmeter-datacollector`.
 
 ## Custom Commands / Workflows
 
 `smartmeter-datacollector` offers a few custom `pipenv run` commands to simplify certain development workflows:
+* `build_check` uses `twine` to check if the built Python package will be accepted by `PiPI`.
+* `build_deb` builds a Debian package for the current development platform.
+* `build_srcdeb` builds a Debian source package which can be used to build a Debian (binary) package for any platform (e.g. using [`pbuilder`](https://pbuilder-docs.readthedocs.io/en/latest/usage.html))
+* `build` builds a Python package which can be uploaded to [`PyPI`](https://pypi.org/project/smartmeter-datacollector/) using `twine`.
+* `debianize` creates a `debian/` directory used to build Debian source / binary packages.
 * `format_check` checks if the code follows the [`autopep8`](https://pypi.org/project/autopep8/) code formatting rules.
 * `format` automatically adjusts the code to follow the `autopep8` code formatting rules.
 * `isort_check` checks if the order of the import statements is correct using [`isort`](https://pycqa.github.io/isort/).
 * `isort` automatically re-orders the import statements using `isort`.
+* `license` makes sure every Python (`*.py`) file contains the proper license header.
 * `lint_check` checks if the code follows the [`pylint`](https://pypi.org/project/pylint/) rules defined in `pyproject.toml`.
 * `lint` automatically adjust the code to follow the `pylint` rules defined in `pyproject.toml`.
-* `license` makes sure every Python (`*.py`) file contains the proper license header.
-* `build` builds a Python package which can be uploaded to [`PyPI`](https://pypi.org/project/smartmeter-datacollector/) using `twine`.
-* `build_check` uses `twine` to check if the built Python package will be accepted by `PiPI`.
 * `setup_check` checks whether the dependencies defined in `Pipfile` / `Pipfile.lock` are in sync with `setup.py`.
 * `setup` synchronizes the dependencies defined in `Pipfile` / `Pipfile.lock` with `setup.py`.
-* `debianize` creates a `debian/` directory used to build Debian source / binary packages.
-* `build_srcdeb` builds a Debian source package which can be used to build a Debian (binary) package for any platform (e.g. using [`pbuilder`](https://pbuilder-docs.readthedocs.io/en/latest/usage.html))
-* `build_deb` builds a Debian package for the current development plattform.
 
-Make sure to run `format_check` / `format`, `isort_check` / `isort`, `lint_check` / `lint`, `license`, `setup_check` / `setup` before commiting changes to the repository to avoid unnecessary development cycles. `smartmeter-datacollector` uses [GitHub Actions](https://github.com/scs/smartmeter-datacollector/actions) to check if these rules apply.
+Make sure to run `format_check` / `format`, `isort_check` / `isort`, `lint_check` / `lint`, `license`, `setup_check` / `setup` before committing changes to the repository to avoid unnecessary development cycles. `smartmeter-datacollector` uses [GitHub Actions](https://github.com/scs/smartmeter-datacollector/actions) to check if these rules apply.
 
 # Acknowledgements
 `smartmeter-datacollector` and its companion project [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-configurator) have been developed by **[Supercomputing Systems AG](https://www.scs.ch)** on behalf of and funded by **[EKZ](https://www.ekz.ch/)**.
```

#### html2text {}

```diff
@@ -1,35 +1,54 @@
-# Smart Meter Data Collector
+Metadata-Version: 2.1 Name: smartmeter-datacollector Version: 1.1.0 Summary:
+Smart Meter Data Collector Home-page: https://github.com/scs/smartmeter-
+datacollector Author: Supercomputing Systems AG Author-email: info@scs.ch
+Maintainer: Supercomputing Systems AG Maintainer-email: info@scs.ch License:
+GPLv2 Project-URL: Source, https://github.com/scs/smartmeter-datacollector
+Project-URL: Bug Reports, https://github.com/scs/smartmeter-datacollector/
+issues Project-URL: Pull Requests, https://github.com/scs/smartmeter-
+datacollector/pulls Project-URL: SCS, https://www.scs.ch Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: GNU General Public License v2 (GPLv2) Classifier: Programming Language ::
+Python Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Typing :: Typed Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE # Smart Meter Data Collector
    [License:_GPL-2.0-only] [Pull_Requests_Welcome] [Contributions_Welcome]
                  [Python Code Checks] [PyPI_-_Python_Version]
                                 [ekz_logo.png]
 --- The `smartmeter-datacollector` tool is a Python3 software which allows you
 to continuously retrieve data from supported smart meters (listed below). The
 acquired values can be forwarded to one or more data sinks like a MQTT broker
 or logger. This tool is an open source software funded by **[EKZ
 (ElektrizitÃ¤tswerke des Kantons ZÃ¼rich)](https://www.ekz.ch)** and developed
 by **[Supercomputing Systems AG](https://www.scs.ch)**. The goal of this
 voluntary initiative is to create a tool that can read, decode and decrypt data
 (if necessary) from the local interface of various smart meters and convert it
 into human-readable and simple formats. This should eliminate the complexity of
 decoding DLMS and similar protocols for the user. The user has the data in a
 format, which he can easily use in various use-cases ranging from simple
-vizualization (see [Method 1: Raspberry Pi image with demo](#method-1-
+visualization (see [Method 1: Raspberry Pi image with demo](#method-1-
 raspberry-pi-image-with-demo)) to integration into energy management algorithms
 or into custom home automation software. The following smart meters are
-supported: * Landis+Gyr E450: \ Data pushed by smart meter over CII interface
-(wired M-Bus). Encoded with HDLC and DLMS/COSEM. * Unencrypted data * Encrypted
-data * Iskraemeco AM550: \ Data pushed by smart meter over [P1 interface
-(DSMR)](https://www.netbeheernederland.nl/_upload/Files/
-Slimme_meter_15_a727fce1f1.pdf). Encoded with HDLC (IEC 62056-46) and DLMS/
-COSEM. * Unencrypted data * Encrypted data The following data sinks are
+supported (see [Wiki/Home](https://github.com/scs/smartmeter-datacollector/
+wiki/Home) for detailed information). * Landis+Gyr E450: \ Data pushed by smart
+meter over CII interface (wired M-Bus, HDLC, DLMS/COSEM). * Landis+Gyr E360: \
+Data pushed by smart meter over P1 interface (HDLC, DLMS/COSEM only, no DSMR).
+* Iskraemeco AM550: \ Data pushed by smart meter over P1 interface (HDLC, DLMS/
+COSEM only, no DSMR). * Kamstrup OMNIPOWER with HAN-NVE: \ Data pushed by smart
+meter over inserted [HAN-NVE module](https://www.kamstrup.com/en-en/
+electricity-solutions/meters-devices/modules/hannve) (wired M-Bus, HDLC, DLMS/
+COSEM). Note: All smart meters integrated so far push binary data encoded with
+HDLC (IEC 62056-46) and DLMS/COSEM. Both unencrypted and encrypted DLMS
+messages are accepted by the software. The following data sinks are
 implemented: * MQTT (v3.1.1): * Encryption * Unencrypted connection * Encrypted
 connection * TLS * optional custom CA certificate * Authentication *
 Unauthenticated * Authenticated with username / password * Authenticated with
-client certificate * Logger to STDOUT `smartmeter-datacollector` is fully
+client certificate * Logger to `stdout` `smartmeter-datacollector` is fully
 configurable through a `.ini` configuration file. The [`smartmeter-
 datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-
 configurator) webinterface can help to create and modify the configuration. --
 - - [Smart Meter Data Collector](#smart-meter-data-collector) - [How to
 install](#how-to-install) - [Method 1: Raspberry Pi image with demo](#method-1-
 raspberry-pi-image-with-demo) - [Method 2: Python package](#method-2-python-
 package) - [Python Requirements](#python-requirements) - [Installation]
@@ -52,156 +71,116 @@
 (based on Raspberry Pi OS) which contains the following parts: * `smartmeter-
 datacollector` as a systemd service * `smartmeter-datacollector-configurator`
 webinterface * demo * [mosquiotto](https://mosquitto.org/) as a local MQTT
 broker to publish the measurements from `smartmeter-datacollector` * [Telegraf]
 (https://www.influxdata.com/time-series-platform/telegraf/) to collect
 measurements published by `smartmeter-datacollector` over MQTT and store them
 in InfluxDB * [InfluxDB](https://www.influxdata.com/) to store the measurements
-* [Grafana](https://grafana.com/) to visualize the measurements This setup
-allows a (first time) user to [install](https://www.raspberrypi.org/
-documentation/computers/getting-started.html#installing-the-operating-system)
-the image on a Raspberry Pi and immediately get started with `smartmeter-
-datacollector`. The following steps are required: 1. Download the Raspberry Pi
-image from the [latest release](https://github.com/scs/smartmeter-
-datacollector/releases). 2. Install the image on a (micro)SD card, e.g. using
-[Raspberry Pi Imager](https://www.raspberrypi.org/documentation/computers/
-getting-started.html#using-raspberry-pi-imager). 3. Prepare the Raspberry Pi.
-1. Push the (micro)SD card into the proper slot. 2. Use an RJ-45 cable (or
-configure WiFi later) to connect to a network. 3. Connect the power cable to
-the Micro USB port. 4. Open the `smartmeter-datacollector-configurator`
-webinterface using `http://:8000/` in your favorite browser. 1. Load the pre-
-defined configuration. 2. Adjust the settings of the connected smart meter. 3.
-Deploy the adjusted configuration. 4. Restart the `smartmeter-datacollector`
-service. 5. Open `Grafana` using `http://:3000/` in your favorite browser. 6.
-Observe the measurements from your smart meter while they arrive periodically.
-See [Wiki/Demo](https://github.com/scs/smartmeter-datacollector/wiki/Demo-
-(Raspberry-Pi-Image)) for more details on the provided Raspberry Pi image with
-the demo. ## Method 2: Python package `smartmeter-datacollector` can be
-installed as a Python3 package either from [PyPi](https://pypi.org/project/
-smartmeter-datacollector/) or manually using a [released wheel](https://
-github.com/scs/smartmeter-datacollector/releases). The Python3 package does not
-contain any infrastructure to run `smartmeter-datacollector` in the background
-or to automatically start it during a boot sequence. If such infrastructure is
-required either see [Method 3: Debian package](#method-3-debian-package) or
-provide it yourself. ### Python Requirements * Python >= 3.7 (tested with 3.8)
-### Installation Install the package either as global Python package or in a
-virtualenv with ```bash python3 -m pip install smartmeter-datacollector ```
-Similarly the [`smartmeter-datacollector-configurator`](https://github.com/scs/
-smartmeter-datacollector-configurator) webinterface can be installed with
-```bash python3 -m pip install smartmeter-datacollector-configurator ``` ##
-Method 3: Debian package `smartmeter-datacollector` is also available as a
-Debian (`.deb`) package from the [releases](https://github.com/scs/smartmeter-
-datacollector/releases) which installs it system wide. The Debian package
-includes a systemd service file which enables `smartmeter-datacollector` to
-automatically start after booting the system. ### Debian Requirements *
-Distribution * Debian * Release * Buster * CPU architecture * amd64 * armhf ###
-Installation Download the Debian package from [releases](https://github.com/
-scs/smartmeter-datacollector/releases) and install it with ```bash sudo apt
-install ./python3-smartmeter-datacollector_*.deb ``` Similarly the
-[`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-
-datacollector-configurator) webinterface can be installed with a Debian package
-from its [releases](https://github.com/scs/smartmeter-datacollector-
-configurator/releases) with ```bash sudo apt install ./python3-smartmeter-
-datacollector-configurator_*.deb ``` # How to use The usage of `smartmeter-
-datacollector` depends on the installation method. Independent of the
-installation method a `.ini` configuration file is required to properly run
-`smartmeter-datacollector`. ## Configuration ### Specification The `.ini`
-configuration file supports the following format ```ini [reader0] # type of the
-connected smart meter type = lge450 # serial port to which the smart meter is
-connected port = /dev/ttyUSB0 # optional encryption key key = [sink0] # type of
-the sink type = mqtt # host / IP address of the MQTT broker host = localhost #
-port of the MQTT broker port = 1883 # whether to use TLS (Transport Layer
-Security) tls = False # optional path to the CA certificate used to validate
-the MQTT broker's certificate ca_file_path = # whether to check the hostname of
-the MQTT broker against the certificate check_hostname = False # optional
-username for authentication with the MQTT broker username = # optional password
-for authentication with the MQTT broker password = # optional path to the
-client certificate for authentication with the MQTT broker client_cert_path = #
-optional path to the private key for the client certificate for authentication
-with the MQTT broker client_key_path = [sink1] # type of the sink type = logger
-# name of the logger name = DataLogger [logging] # log level configuration:
-DEBUG / INFO / WARNING / ERROR default = WARNING smartmeter = WARNING collector
-= WARNING sink = WARNING ``` There can be multiple `[readerX]` and `[sinkY]`
-sections for every connected smart meter and / or data sink. See [Wiki/
-Configuration](https://github.com/scs/smartmeter-datacollector/wiki/
-Configuration) for more details on the available configuration options. ###
-smartmeter-datacollector-configurator To simplify the process of generating a
-valid `.ini` configuration for `smartmeter-datacollector` the companion
-[`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-
-datacollector-configurator) webinterface can be used. It supports * a graphical
-approach to manage the configuration * input validation to avoid invalid
-configurations * loading / saving / discarding a configuration * restarting
-`smartmeter-datacollector` (only if installed as a Debian package) See [Wiki/
-smartmeter-datacollector-configurator](https://github.com/scs/smartmeter-
-datacollector/wiki/smartmeter-datacollector-configurator) for more details on
-the webinterface and the configuration possibilities. ## Run manually Run
+* [Grafana](https://grafana.com/) to visualize the measurements See [Wiki/Demo]
+(https://github.com/scs/smartmeter-datacollector/wiki/Demo-(Raspberry-Pi-
+Image)) for detailed setup instructions. ## Method 2: Python package
+`smartmeter-datacollector` can be installed as a Python3 package either from
+[PyPi](https://pypi.org/project/smartmeter-datacollector/) or manually using a
+[released wheel](https://github.com/scs/smartmeter-datacollector/releases). The
+Python3 package does not contain any infrastructure to run `smartmeter-
+datacollector` in the background or to automatically start it during a boot
+sequence. If such infrastructure is required either see [Method 3: Debian
+package](#method-3-debian-package) or provide it yourself. ### Python
+Requirements * Python >= 3.7 (tested with 3.8) ### Installation Install the
+package either as global Python package or in a virtualenv with ```bash python3
+-m pip install smartmeter-datacollector ``` Similarly the [`smartmeter-
+datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-
+configurator) webinterface can be installed with ```bash python3 -m pip install
+smartmeter-datacollector-configurator ``` ## Method 3: Debian package
+`smartmeter-datacollector` is also available as a Debian (`.deb`) package from
+the [releases](https://github.com/scs/smartmeter-datacollector/releases) which
+installs it system wide. The Debian package includes a systemd service file
+which enables `smartmeter-datacollector` to automatically start after booting
+the system. ### Debian Requirements * Distribution * Debian * Release *
+Bullseye * CPU architecture * amd64 * armhf ### Installation Download the
+Debian package from [releases](https://github.com/scs/smartmeter-datacollector/
+releases) and install it with ```bash sudo apt install ./python3-smartmeter-
+datacollector_*.deb ``` Similarly the [`smartmeter-datacollector-configurator`]
+(https://github.com/scs/smartmeter-datacollector-configurator) webinterface can
+be installed with a Debian package from its [releases](https://github.com/scs/
+smartmeter-datacollector-configurator/releases) with ```bash sudo apt install
+./python3-smartmeter-datacollector-configurator_*.deb ``` # How to use The
+usage of `smartmeter-datacollector` depends on the installation method.
+Independent of the installation method a `.ini` configuration file is required
+to properly run `smartmeter-datacollector`. ## Configuration ### Manually
+create configuration See [Wiki/Configuration](https://github.com/scs/
+smartmeter-datacollector/wiki/Configuration#manually-write-configuration) for
+more details on the available configuration options. ### smartmeter-
+datacollector-configurator To simplify the process of generating a valid `.ini`
+configuration for `smartmeter-datacollector` the companion [`smartmeter-
+datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-
+configurator) webinterface can be used. It supports * a graphical approach to
+manage the configuration * input validation to avoid invalid configurations *
+loading / saving / discarding a configuration * restarting `smartmeter-
+datacollector` (only if installed as a Debian package) See [Wiki/smartmeter-
+datacollector-configurator](https://github.com/scs/smartmeter-datacollector/
+wiki/smartmeter-datacollector-configurator) for more details on the
+webinterface and the configuration possibilities. ## Run manually Run
 `smartmeter-datacollector` with the following command: ``` smartmeter-
 datacollector --config datacollector.ini ``` The following command line
 arguments are supported: * `-h, --help`: Shows the help output of `smartmeter-
 datacollector`. * `-c, --config CONFIG`: Path to the `.ini` configuration file.
-* `-s,--saveconfig`: Cteate a default `.ini` configuration file. * `-d, --dev`:
+* `-s,--saveconfig`: Create a default `.ini` configuration file. * `-d, --dev`:
 Enable development mode. ### Configuration The configuration file can be
 located anywhere and use any filename. If no `.ini` configuration file is
 specified a default configuration with the following options is used: *
-Landys+Gir E450 smart meter in unencrypted mode connected to `/dev/ttyUSB0` *
+Landys+Gyr E450 smart meter in unencrypted mode connected to `/dev/ttyUSB0` *
 `LOGGER` sink * `MQTT` sink connected to a local broker without encryption or
 authentication ## Run as a systemd service When `smartmeter-datacollector` has
 been installed as a Debian package it provides a systemd .service file named
 `python3-smartmeter-datacollector.service`. Therefore the service can be
-managed using the `systemctl` command: ``` sudo systemctl start|stop|restart
-python3-smartmeter-datacollector ``` Enabling or disabling the service can also
-be managed using the `systemctl` command: ``` sudo systemctl enable|disable
-python3-smartmeter-datacollector ``` Inspecting the log messages can be done
-using the `journalctl` command: ``` journalctl -u python3-smartmeter-
-datacollector [-f] ``` ### Configuration The systemd service expectes the
-`.ini` configuration to be located at `/var/lib/smartmeter-datacollector/
-datacollector.ini`. This is also the default location used by the [`smartmeter-
-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-
-configurator) webinterface to load and save the managed configuration. # How to
-develop Help from the community for the `smartmeter-datacollector` project is
-always welcome. Please follow the next few chapters to setup a working
-development environment. ## Development Requirements * Python >= 3.7 *
-[`pipenv`](https://pipenv.pypa.io/en/latest/) * Optional software packages
-(Debian / Ubuntu) * python3-all * debhelper * dh-python * dh-systemd ##
-Installation ### Debian / Ubuntu To install the listed minimal requirements run
-the following command: ``` sudo apt install git python3 pipenv ``` To install
-the optional requirements also run the following command: ``` sudo apt install
-python3-all debhelper dh-python dh-systemd ``` ## Checkout the code Use `git`
-to clone / checkout `smartmeter-datacollector` from GitHub using ``` git clone
-https://github.com/scs/smartmeter-datacollector.git ``` ## Setup Development
-Environment `smartmeter-datacollector` uses [`pipenv`](https://pipenv.pypa.io/
-en/latest/) to manage its dependencies and setup a virtual environment. Run the
-following command to setup the initial development environment: ``` pipenv
-install --dev ``` This will install all runtime and development dependencies
-for `smartmeter-datacollector` in a new virtual environment. Now you are ready
-to start working on `smartmeter-datacollector`. ## Custom Commands / Workflows
-`smartmeter-datacollector` offers a few custom `pipenv run` commands to
-simplify certain development workflows: * `format_check` checks if the code
-follows the [`autopep8`](https://pypi.org/project/autopep8/) code formatting
-rules. * `format` automatically adjusts the code to follow the `autopep8` code
-formatting rules. * `isort_check` checks if the order of the import statements
-is correct using [`isort`](https://pycqa.github.io/isort/). * `isort`
-automatically re-orders the import statements using `isort`. * `lint_check`
-checks if the code follows the [`pylint`](https://pypi.org/project/pylint/
-) rules defined in `pyproject.toml`. * `lint` automatically adjust the code to
-follow the `pylint` rules defined in `pyproject.toml`. * `license` makes sure
-every Python (`*.py`) file contains the proper license header. * `build` builds
-a Python package which can be uploaded to [`PyPI`](https://pypi.org/project/
-smartmeter-datacollector/) using `twine`. * `build_check` uses `twine` to check
-if the built Python package will be accepted by `PiPI`. * `setup_check` checks
-whether the dependencies defined in `Pipfile` / `Pipfile.lock` are in sync with
-`setup.py`. * `setup` synchronizes the dependencies defined in `Pipfile` /
-`Pipfile.lock` with `setup.py`. * `debianize` creates a `debian/` directory
-used to build Debian source / binary packages. * `build_srcdeb` builds a Debian
+managed using the `systemctl` command. See [Run as a systemd service](https://
+github.com/scs/smartmeter-datacollector/wiki/How-to-use#run-as-a-systemd-
+service) for possible commands. # How to develop Help from the community for
+the `smartmeter-datacollector` project is always welcome. Please follow the
+next few chapters to setup a working development environment. ## Development
+Requirements * Python >= 3.8, <= 3.10 * [`pipenv`](https://pipenv.pypa.io/en/
+latest/) * Optional software packages (Debian bullseye/ Ubuntu 22.04) *
+python3-all * debhelper * dh-python ## Installation ### Debian / Ubuntu To
+install the listed minimal requirements run the following command: ``` sudo apt
+install git python3 pipenv ``` To install the optional requirements also run
+the following command: ``` sudo apt install python3-all debhelper dh-python ```
+## Checkout the code Use `git` to clone / checkout `smartmeter-datacollector`
+from GitHub using ``` git clone https://github.com/scs/smartmeter-
+datacollector.git ``` ## Setup Development Environment `smartmeter-
+datacollector` uses [`pipenv`](https://pipenv.pypa.io/en/latest/) to manage its
+dependencies and setup a virtual environment. Run the following command to
+setup the initial development environment: ``` pipenv install --dev ``` This
+will install all runtime and development dependencies for `smartmeter-
+datacollector` in a new virtual environment. Now you are ready to start working
+on `smartmeter-datacollector`. ## Custom Commands / Workflows `smartmeter-
+datacollector` offers a few custom `pipenv run` commands to simplify certain
+development workflows: * `build_check` uses `twine` to check if the built
+Python package will be accepted by `PiPI`. * `build_deb` builds a Debian
+package for the current development platform. * `build_srcdeb` builds a Debian
 source package which can be used to build a Debian (binary) package for any
 platform (e.g. using [`pbuilder`](https://pbuilder-docs.readthedocs.io/en/
-latest/usage.html)) * `build_deb` builds a Debian package for the current
-development plattform. Make sure to run `format_check` / `format`,
-`isort_check` / `isort`, `lint_check` / `lint`, `license`, `setup_check` /
-`setup` before commiting changes to the repository to avoid unnecessary
-development cycles. `smartmeter-datacollector` uses [GitHub Actions](https://
-github.com/scs/smartmeter-datacollector/actions) to check if these rules apply.
-# Acknowledgements `smartmeter-datacollector` and its companion project
+latest/usage.html)) * `build` builds a Python package which can be uploaded to
+[`PyPI`](https://pypi.org/project/smartmeter-datacollector/) using `twine`. *
+`debianize` creates a `debian/` directory used to build Debian source / binary
+packages. * `format_check` checks if the code follows the [`autopep8`](https://
+pypi.org/project/autopep8/) code formatting rules. * `format` automatically
+adjusts the code to follow the `autopep8` code formatting rules. *
+`isort_check` checks if the order of the import statements is correct using
+[`isort`](https://pycqa.github.io/isort/). * `isort` automatically re-orders
+the import statements using `isort`. * `license` makes sure every Python
+(`*.py`) file contains the proper license header. * `lint_check` checks if the
+code follows the [`pylint`](https://pypi.org/project/pylint/) rules defined in
+`pyproject.toml`. * `lint` automatically adjust the code to follow the `pylint`
+rules defined in `pyproject.toml`. * `setup_check` checks whether the
+dependencies defined in `Pipfile` / `Pipfile.lock` are in sync with `setup.py`.
+* `setup` synchronizes the dependencies defined in `Pipfile` / `Pipfile.lock`
+with `setup.py`. Make sure to run `format_check` / `format`, `isort_check` /
+`isort`, `lint_check` / `lint`, `license`, `setup_check` / `setup` before
+committing changes to the repository to avoid unnecessary development cycles.
+`smartmeter-datacollector` uses [GitHub Actions](https://github.com/scs/
+smartmeter-datacollector/actions) to check if these rules apply. #
+Acknowledgements `smartmeter-datacollector` and its companion project
 [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-
 datacollector-configurator) have been developed by **[Supercomputing Systems
 AG](https://www.scs.ch)** on behalf of and funded by **[EKZ](https://
 www.ekz.ch/)**.
```

### Comparing `smartmeter-datacollector-1.0.2/pyproject.toml` & `smartmeter-datacollector-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.0.2/setup.py` & `smartmeter-datacollector-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,33 +29,36 @@
         "Source": "https://github.com/scs/smartmeter-datacollector",
         "Bug Reports": "https://github.com/scs/smartmeter-datacollector/issues",
         "Pull Requests": "https://github.com/scs/smartmeter-datacollector/pulls",
         "SCS": "https://www.scs.ch",
     },
     author="Supercomputing Systems AG",
     author_email="info@scs.ch",
+    maintainer="Supercomputing Systems AG",
+    maintainer_email="info@scs.ch",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Typing :: Typed",
     ],
     license="GPLv2",
     python_requires=">=3.7",
     packages=find_packages(
         exclude=["contrib", "doc", "LICENSES", "scripts", "tests", "tests."]
     ),
     include_package_data=True,
     install_requires=[
-        "aioserial==1.3.0",
-        "asyncio-mqtt==0.10.0",
-        "gurux-dlms==1.0.107",
-        "paho-mqtt==1.5.1",
-        "pyserial==3.5",
+        'aioserial==1.3.1',
+        'asyncio-mqtt==0.16.1',
+        'gurux-dlms==1.0.143',
+        'paho-mqtt==1.6.1',
+        'pyserial==3.5'
     ],
     scripts=["bin/smartmeter-datacollector"],
     zip_safe=True,
     dependency_links=[],
 )
```

### Comparing `smartmeter-datacollector-1.0.2/smartmeter_datacollector/app.py` & `smartmeter-datacollector-1.1.0/smartmeter_datacollector/app.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.0.2/smartmeter_datacollector/collector.py` & `smartmeter-datacollector-1.1.0/smartmeter_datacollector/collector.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.0.2/smartmeter_datacollector/config.py` & `smartmeter-datacollector-1.1.0/smartmeter_datacollector/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     pass
 
 
 DEFAULT_CONFIG = {
     'reader0': {
         'type': "lge450",
         'port': "/dev/ttyUSB0",
+        'baudrate': 2400,
         'key': "",
     },
     'sink0': {
         'type': "logger",
         'name': "DataLogger",
     },
     'sink1': {
```

### Comparing `smartmeter-datacollector-1.0.2/smartmeter_datacollector/factory.py` & `smartmeter-datacollector-1.1.0/smartmeter_datacollector/factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,33 +11,53 @@
 
 from .collector import Collector
 from .config import InvalidConfigError
 from .sinks.data_sink import DataSink
 from .sinks.logger_sink import LoggerSink
 from .sinks.mqtt_sink import MqttConfig, MqttDataSink
 from .smartmeter.iskraam550 import IskraAM550
+from .smartmeter.kamstrup_han import KamstrupHAN
+from .smartmeter.lge360 import LGE360
 from .smartmeter.lge450 import LGE450
 from .smartmeter.meter import Meter, MeterError
 
 
 def build_meters(config: ConfigParser) -> List[Meter]:
     meters = []
     for section_name in filter(lambda sec: sec.startswith("reader"), config.sections()):
         meter_config = config[section_name]
         meter_type = meter_config.get('type')
         try:
             if meter_type == "lge450":
                 meters.append(LGE450(
                     port=meter_config.get('port', "/dev/ttyUSB0"),
-                    decryption_key=meter_config.get('key')
+                    baudrate=meter_config.getint('baudrate', LGE450.BAUDRATE),
+                    decryption_key=meter_config.get('key'),
+                    use_system_time=meter_config.getboolean('systemtime', False)
+                ))
+            elif meter_type == "lge360":
+                meters.append(LGE360(
+                    port=meter_config.get('port', "/dev/ttyUSB0"),
+                    baudrate=meter_config.getint('baudrate', LGE360.BAUDRATE),
+                    decryption_key=meter_config.get('key'),
+                    use_system_time=meter_config.getboolean('systemtime', False)
                 ))
             elif meter_type == "iskraam550":
                 meters.append(IskraAM550(
                     port=meter_config.get('port', "/dev/ttyUSB0"),
-                    decryption_key=meter_config.get('key')
+                    baudrate=meter_config.getint('baudrate', IskraAM550.BAUDRATE),
+                    decryption_key=meter_config.get('key'),
+                    use_system_time=meter_config.getboolean('systemtime', False)
+                ))
+            elif meter_type == "kamstrup_han":
+                meters.append(KamstrupHAN(
+                    port=meter_config.get('port', "/dev/ttyUSB0"),
+                    baudrate=meter_config.getint('baudrate', KamstrupHAN.BAUDRATE),
+                    decryption_key=meter_config.get('key'),
+                    use_system_time=meter_config.getboolean('systemtime', False)
                 ))
             else:
                 raise InvalidConfigError(f"'type' is invalid or missing: {meter_type}")
         except MeterError as ex:
             logging.warning("%s Skipping smart meter.", ex)
             continue
     return meters
```

### Comparing `smartmeter-datacollector-1.0.2/smartmeter_datacollector/sinks/data_sink.py` & `smartmeter-datacollector-1.1.0/smartmeter_datacollector/sinks/data_sink.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.0.2/smartmeter_datacollector/sinks/logger_sink.py` & `smartmeter-datacollector-1.1.0/smartmeter_datacollector/sinks/logger_sink.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.0.2/smartmeter_datacollector/sinks/mqtt_sink.py` & `smartmeter-datacollector-1.1.0/smartmeter_datacollector/sinks/mqtt_sink.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.0.2/smartmeter_datacollector/smartmeter/meter.py` & `smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/meter.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,27 +33,31 @@
         for observer in self._observers:
             observer.notify(data_points)
 
 
 class SerialHdlcDlmsMeter(Meter):
     HDLC_FLAG = b"\x7e"
 
-    def __init__(self, serial_config: SerialConfig, cosem: Cosem, decryption_key: Optional[str] = None) -> None:
+    def __init__(self, serial_config: SerialConfig,
+                 cosem: Cosem,
+                 decryption_key: Optional[str] = None,
+                 use_system_time: bool = False) -> None:
         super().__init__()
-        self._parser = HdlcDlmsParser(cosem, decryption_key)
+        self._parser = HdlcDlmsParser(cosem, decryption_key, use_system_time)
         self._serial = SerialReader(serial_config, self._data_received)
 
     async def start(self) -> None:
         await self._serial.start_and_listen()
 
     def _data_received(self, received_data: bytes) -> None:
         if not received_data:
             return
         if received_data == SerialHdlcDlmsMeter.HDLC_FLAG:
             self._parser.append_to_hdlc_buffer(received_data)
             return
 
         self._parser.append_to_hdlc_buffer(received_data)
         if self._parser.extract_data_from_hdlc_frames():
+            message_time = self._parser.extract_message_time()
             dlms_objects = self._parser.parse_to_dlms_objects()
-            data_points = self._parser.convert_dlms_bundle_to_reader_data(dlms_objects)
+            data_points = self._parser.convert_dlms_bundle_to_reader_data(dlms_objects, message_time)
             self._notify_observers(data_points)
```

### Comparing `smartmeter-datacollector-1.0.2/smartmeter_datacollector/smartmeter/meter_data.py` & `smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/meter_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,19 +52,23 @@
     ANGLE_UI_L2 = MeterDataPointType("ANGLE_UI_L2", "Angle U-I L2", "rad")
     ANGLE_UI_L3 = MeterDataPointType("ANGLE_UI_L3", "Angle U-I L3", "rad")
 
     ACTIVE_ENERGY_P = MeterDataPointType("ACTIVE_ENERGY_P", "Active Energy +", "Wh")
     ACTIVE_ENERGY_P_T1 = MeterDataPointType("ACTIVE_ENERGY_P_T1", "Active Energy + Tariff 1", "Wh")
     ACTIVE_ENERGY_P_T2 = MeterDataPointType("ACTIVE_ENERGY_P_T2", "Active Energy + Tariff 2", "Wh")
     ACTIVE_ENERGY_N = MeterDataPointType("ACTIVE_ENERGY_N", "Active Energy -", "Wh")
-    ACTIVE_ENERGY_N_T1 = MeterDataPointType("ACTIVE_ENERGY_N", "Active Energy - Tariff 1", "Wh")
-    ACTIVE_ENERGY_N_T2 = MeterDataPointType("ACTIVE_ENERGY_N", "Active Energy - Tariff 2", "Wh")
+    ACTIVE_ENERGY_N_T1 = MeterDataPointType("ACTIVE_ENERGY_N_T1", "Active Energy - Tariff 1", "Wh")
+    ACTIVE_ENERGY_N_T2 = MeterDataPointType("ACTIVE_ENERGY_N_T2", "Active Energy - Tariff 2", "Wh")
 
     REACTIVE_ENERGY_P = MeterDataPointType("REACTIVE_ENERGY_P", "Reactive Energy +", "VAh")
+    REACTIVE_ENERGY_P_T1 = MeterDataPointType("REACTIVE_ENERGY_P_T1", "Reactive Energy + Tariff 1", "VAh")
+    REACTIVE_ENERGY_P_T2 = MeterDataPointType("REACTIVE_ENERGY_P_T2", "Reactive Energy + Tariff 2", "VAh")
     REACTIVE_ENERGY_N = MeterDataPointType("REACTIVE_ENERGY_N", "Reactive Energy -", "VAh")
+    REACTIVE_ENERGY_N_T1 = MeterDataPointType("REACTIVE_ENERGY_N_T1", "Reactive Energy - Tariff 1", "VAh")
+    REACTIVE_ENERGY_N_T2 = MeterDataPointType("REACTIVE_ENERGY_N_T2", "Reactive Energy - Tariff 2", "VAh")
 
     REACTIVE_ENERGY_Q1 = MeterDataPointType("REACTIVE_ENERGY_Q1", "Reactive Energy +Ri Q1", "VAh")
     REACTIVE_ENERGY_Q2 = MeterDataPointType("REACTIVE_ENERGY_Q2", "Reactive Energy +Rc Q2", "VAh")
     REACTIVE_ENERGY_Q3 = MeterDataPointType("REACTIVE_ENERGY_Q3", "Reactive Energy -Ri Q3", "VAh")
     REACTIVE_ENERGY_Q4 = MeterDataPointType("REACTIVE_ENERGY_Q4", "Reactive Energy -Rc Q4", "VAh")
 
     POWER_FACTOR = MeterDataPointType("POWER_FACTOR", "Power Factor", "")
```

### Comparing `smartmeter-datacollector-1.0.2/smartmeter_datacollector/smartmeter/reader.py` & `smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/reader.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.0.2/smartmeter_datacollector/smartmeter/serial_reader.py` & `smartmeter-datacollector-1.1.0/smartmeter_datacollector/smartmeter/serial_reader.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.0.2/smartmeter_datacollector.egg-info/PKG-INFO` & `smartmeter-datacollector-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: smartmeter-datacollector
-Version: 1.0.2
-Summary: Smart Meter Data Collector
-Home-page: https://github.com/scs/smartmeter-datacollector
-Author: Supercomputing Systems AG
-Author-email: info@scs.ch
-License: GPLv2
-Project-URL: Source, https://github.com/scs/smartmeter-datacollector
-Project-URL: Bug Reports, https://github.com/scs/smartmeter-datacollector/issues
-Project-URL: Pull Requests, https://github.com/scs/smartmeter-datacollector/pulls
-Project-URL: SCS, https://www.scs.ch
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Smart Meter Data Collector
 
 <p align="center">
     <a href="LICENSE"><img alt="License: GPL-2.0-only" src="https://img.shields.io/badge/license-GPLv2-blue.svg"></a> <a href="https://github.com/scs/smartmeter-datacollector/pulls"><img alt="Pull Requests Welcome" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg"></a> <a href="https://github.com/scs/smartmeter-datacollector/pulls"><img alt="Contributions Welcome" src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg"></a>
     <br />
     <img alt="Python Code Checks" src="https://github.com/scs/smartmeter-datacollector/actions/workflows/python-code-checks.yml/badge.svg?branch=master"> <a href="https://pypi.org/project/smartmeter-datacollector/"><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/smartmeter-datacollector"></a>
     <br />
@@ -33,39 +9,41 @@
 </p>
 
 ---
 
 The `smartmeter-datacollector` tool is a Python3 software which allows you to continuously retrieve data from supported smart meters (listed below).
 The acquired values can be forwarded to one or more data sinks like a MQTT broker or logger.
 
-This tool is an open source software funded by **[EKZ (Elektrizitätswerke des Kantons Zürich)](https://www.ekz.ch)** and developed by **[Supercomputing Systems AG](https://www.scs.ch)**. The goal of this voluntary initiative is to create a tool that can read, decode and decrypt data (if necessary) from the local interface of various smart meters and convert it into human-readable and simple formats. This should eliminate the complexity of decoding DLMS and similar protocols for the user. The user has the data in a format, which he can easily use in various use-cases ranging from simple vizualization (see [Method 1: Raspberry Pi image with demo](#method-1-raspberry-pi-image-with-demo)) to integration into energy management algorithms or into custom home automation software. 
+This tool is an open source software funded by **[EKZ (Elektrizitätswerke des Kantons Zürich)](https://www.ekz.ch)** and developed by **[Supercomputing Systems AG](https://www.scs.ch)**. The goal of this voluntary initiative is to create a tool that can read, decode and decrypt data (if necessary) from the local interface of various smart meters and convert it into human-readable and simple formats. This should eliminate the complexity of decoding DLMS and similar protocols for the user. The user has the data in a format, which he can easily use in various use-cases ranging from simple visualization (see [Method 1: Raspberry Pi image with demo](#method-1-raspberry-pi-image-with-demo)) to integration into energy management algorithms or into custom home automation software. 
 
-The following smart meters are supported:
+The following smart meters are supported (see [Wiki/Home](https://github.com/scs/smartmeter-datacollector/wiki/Home) for detailed information).
 
 * Landis+Gyr E450: \
-  Data pushed by smart meter over CII interface (wired M-Bus). Encoded with HDLC and DLMS/COSEM.
-  * Unencrypted data
-  * Encrypted data
+  Data pushed by smart meter over CII interface (wired M-Bus, HDLC, DLMS/COSEM).
+* Landis+Gyr E360: \
+  Data pushed by smart meter over P1 interface (HDLC, DLMS/COSEM only, no DSMR).
 * Iskraemeco AM550: \
-  Data pushed by smart meter over [P1 interface (DSMR)](https://www.netbeheernederland.nl/_upload/Files/Slimme_meter_15_a727fce1f1.pdf). Encoded with HDLC (IEC 62056-46) and DLMS/COSEM.
-  * Unencrypted data
-  * Encrypted data
+  Data pushed by smart meter over P1 interface (HDLC, DLMS/COSEM only, no DSMR).
+* Kamstrup OMNIPOWER with HAN-NVE: \
+  Data pushed by smart meter over inserted [HAN-NVE module](https://www.kamstrup.com/en-en/electricity-solutions/meters-devices/modules/hannve) (wired M-Bus, HDLC, DLMS/COSEM).
+
+Note: All smart meters integrated so far push binary data encoded with HDLC (IEC 62056-46) and DLMS/COSEM. Both unencrypted and encrypted DLMS messages are accepted by the software.
 
 The following data sinks are implemented:
 * MQTT (v3.1.1):
   * Encryption
     * Unencrypted connection
     * Encrypted connection
       * TLS
       * optional custom CA certificate
   * Authentication
     * Unauthenticated
     * Authenticated with username / password
     * Authenticated with client certificate
-* Logger to STDOUT
+* Logger to `stdout`
 
 `smartmeter-datacollector` is fully configurable through a `.ini` configuration file. The [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-configurator) webinterface can help to create and modify the configuration.
 
 ---
 
 - [Smart Meter Data Collector](#smart-meter-data-collector)
 - [How to install](#how-to-install)
@@ -108,30 +86,15 @@
 * `smartmeter-datacollector-configurator` webinterface
 * demo
   * [mosquiotto](https://mosquitto.org/) as a local MQTT broker to publish the measurements from `smartmeter-datacollector`
   * [Telegraf](https://www.influxdata.com/time-series-platform/telegraf/) to collect measurements published by `smartmeter-datacollector` over MQTT and store them in InfluxDB
   * [InfluxDB](https://www.influxdata.com/) to store the measurements
   * [Grafana](https://grafana.com/) to visualize the measurements
 
-This setup allows a (first time) user to [install](https://www.raspberrypi.org/documentation/computers/getting-started.html#installing-the-operating-system) the image on a Raspberry Pi and immediately get started with `smartmeter-datacollector`. The following steps are required:
-1. Download the Raspberry Pi image from the [latest release](https://github.com/scs/smartmeter-datacollector/releases).
-2. Install the image on a (micro)SD card, e.g. using [Raspberry Pi Imager](https://www.raspberrypi.org/documentation/computers/getting-started.html#using-raspberry-pi-imager).
-3. Prepare the Raspberry Pi.
-   1. Push the (micro)SD card into the proper slot.
-   2. Use an RJ-45 cable (or configure WiFi later) to connect to a network.
-   3. Connect the power cable to the Micro USB port.
-4. Open the `smartmeter-datacollector-configurator` webinterface using `http://<Raspberry Pi IP>:8000/` in your favorite browser.
-   1. Load the pre-defined configuration.
-   2. Adjust the settings of the connected smart meter.
-   3. Deploy the adjusted configuration.
-   4. Restart the `smartmeter-datacollector` service.
-5. Open `Grafana` using `http://<Raspberry Pi IP>:3000/` in your favorite browser.
-6. Observe the measurements from your smart meter while they arrive periodically.
-
-See [Wiki/Demo](https://github.com/scs/smartmeter-datacollector/wiki/Demo-(Raspberry-Pi-Image)) for more details on the provided Raspberry Pi image with the demo.
+See [Wiki/Demo](https://github.com/scs/smartmeter-datacollector/wiki/Demo-(Raspberry-Pi-Image)) for detailed setup instructions.
 
 ## Method 2: Python package
 
 `smartmeter-datacollector` can be installed as a Python3 package either from [PyPi](https://pypi.org/project/smartmeter-datacollector/) or manually using a [released wheel](https://github.com/scs/smartmeter-datacollector/releases).
 
 The Python3 package does not contain any infrastructure to run `smartmeter-datacollector` in the background or to automatically start it during a boot sequence. If such infrastructure is required either see [Method 3: Debian package](#method-3-debian-package) or provide it yourself.
 
@@ -158,15 +121,15 @@
 `smartmeter-datacollector` is also available as a Debian (`.deb`) package from the [releases](https://github.com/scs/smartmeter-datacollector/releases) which installs it system wide. The Debian package includes a systemd service file which enables `smartmeter-datacollector` to automatically start after booting the system.
 
 ### Debian Requirements
 
 * Distribution
   * Debian
 * Release
-  * Buster
+  * Bullseye
 * CPU architecture
   * amd64
   * armhf
 
 ### Installation
 
 Download the Debian package from [releases](https://github.com/scs/smartmeter-datacollector/releases) and install it with
@@ -183,66 +146,17 @@
 
 # How to use
 
 The usage of `smartmeter-datacollector` depends on the installation method. Independent of the installation method a `.ini` configuration file is required to properly run `smartmeter-datacollector`.
 
 ## Configuration
 
-### Specification
-
-The `.ini` configuration file supports the following format
+### Manually create configuration
 
-```ini
-[reader0]
-# type of the connected smart meter
-type = lge450
-# serial port to which the smart meter is connected
-port = /dev/ttyUSB0
-# optional encryption key
-key = 
-
-[sink0]
-# type of the sink
-type = mqtt
-# host / IP address of the MQTT broker
-host = localhost
-# port of the MQTT broker
-port = 1883
-# whether to use TLS (Transport Layer Security)
-tls = False
-# optional path to the CA certificate used to validate the MQTT broker's certificate
-ca_file_path = 
-# whether to check the hostname of the MQTT broker against the certificate
-check_hostname = False
-# optional username for authentication with the MQTT broker
-username = 
-# optional password for authentication with the MQTT broker
-password = 
-# optional path to the client certificate for authentication with the MQTT broker
-client_cert_path = 
-# optional path to the private key for the client certificate for authentication with the MQTT broker
-client_key_path = 
-
-[sink1]
-# type of the sink
-type = logger
-# name of the logger
-name = DataLogger
-
-[logging]
-# log level configuration: DEBUG / INFO / WARNING / ERROR
-default = WARNING
-smartmeter = WARNING
-collector = WARNING
-sink = WARNING
-```
-
-There can be multiple `[readerX]` and `[sinkY]` sections for every connected smart meter and / or data sink.
-
-See [Wiki/Configuration](https://github.com/scs/smartmeter-datacollector/wiki/Configuration) for more details on the available configuration options.
+See [Wiki/Configuration](https://github.com/scs/smartmeter-datacollector/wiki/Configuration#manually-write-configuration) for more details on the available configuration options.
 
 ### smartmeter-datacollector-configurator
 
 To simplify the process of generating a valid `.ini` configuration for `smartmeter-datacollector` the companion [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-configurator) webinterface can be used. It supports
 * a graphical approach to manage the configuration
 * input validation to avoid invalid configurations
 * loading / saving / discarding a configuration
@@ -257,77 +171,56 @@
 ```
 smartmeter-datacollector --config datacollector.ini
 ```
 
 The following command line arguments are supported:
 * `-h, --help`: Shows the help output of `smartmeter-datacollector`.
 * `-c, --config CONFIG`: Path to the `.ini` configuration file.
-* `-s,--saveconfig`: Cteate a default `.ini` configuration file.
+* `-s,--saveconfig`: Create a default `.ini` configuration file.
 * `-d, --dev`: Enable development mode.
 
 ### Configuration
 
 The configuration file can be located anywhere and use any filename. If no `.ini` configuration file is specified a default configuration with the following options is used:
-* Landys+Gir E450 smart meter in unencrypted mode connected to `/dev/ttyUSB0`
+* Landys+Gyr E450 smart meter in unencrypted mode connected to `/dev/ttyUSB0`
 * `LOGGER` sink
 * `MQTT` sink connected to a local broker without encryption or authentication
 
 ## Run as a systemd service
 
-When `smartmeter-datacollector` has been installed as a Debian package it provides a systemd .service file named `python3-smartmeter-datacollector.service`. Therefore the service can be managed using the `systemctl` command:
-
-```
-sudo systemctl start|stop|restart python3-smartmeter-datacollector
-```
-
-Enabling or disabling the service can also be managed using the `systemctl` command:
-
-```
-sudo systemctl enable|disable python3-smartmeter-datacollector
-```
-
-Inspecting the log messages can be done using the `journalctl` command:
-
-```
-journalctl -u python3-smartmeter-datacollector [-f]
-```
-
-### Configuration
+When `smartmeter-datacollector` has been installed as a Debian package it provides a systemd .service file named `python3-smartmeter-datacollector.service`. Therefore the service can be managed using the `systemctl` command. See [Run as a systemd service](https://github.com/scs/smartmeter-datacollector/wiki/How-to-use#run-as-a-systemd-service) for possible commands.
 
-The systemd service expectes the `.ini` configuration to be located at
-`/var/lib/smartmeter-datacollector/datacollector.ini`. This is also the default location used by the [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-configurator) webinterface to load and save the managed configuration.
 
 # How to develop
 
 Help from the community for the `smartmeter-datacollector` project is always welcome. Please follow the next few chapters to setup a working development environment.
 
 ## Development Requirements
 
-* Python >= 3.7
+* Python >= 3.8, <= 3.10
 * [`pipenv`](https://pipenv.pypa.io/en/latest/)
-* Optional software packages (Debian / Ubuntu)
+* Optional software packages (Debian bullseye/ Ubuntu 22.04)
   * python3-all
   * debhelper
   * dh-python
-  * dh-systemd
 
 ## Installation
 
 ### Debian / Ubuntu
 
 To install the listed minimal requirements run the following command:
 
 ```
 sudo apt install git python3 pipenv
 ```
 
 To install the optional requirements also run the following command:
 
 ```
-sudo apt install python3-all debhelper dh-python dh-systemd
+sudo apt install python3-all debhelper dh-python
 ```
 
 ## Checkout the code
 
 Use `git` to clone / checkout `smartmeter-datacollector` from GitHub using
 
 ```
@@ -343,28 +236,26 @@
 ```
 
 This will install all runtime and development dependencies for `smartmeter-datacollector` in a new virtual environment. Now you are ready to start working on `smartmeter-datacollector`.
 
 ## Custom Commands / Workflows
 
 `smartmeter-datacollector` offers a few custom `pipenv run` commands to simplify certain development workflows:
+* `build_check` uses `twine` to check if the built Python package will be accepted by `PiPI`.
+* `build_deb` builds a Debian package for the current development platform.
+* `build_srcdeb` builds a Debian source package which can be used to build a Debian (binary) package for any platform (e.g. using [`pbuilder`](https://pbuilder-docs.readthedocs.io/en/latest/usage.html))
+* `build` builds a Python package which can be uploaded to [`PyPI`](https://pypi.org/project/smartmeter-datacollector/) using `twine`.
+* `debianize` creates a `debian/` directory used to build Debian source / binary packages.
 * `format_check` checks if the code follows the [`autopep8`](https://pypi.org/project/autopep8/) code formatting rules.
 * `format` automatically adjusts the code to follow the `autopep8` code formatting rules.
 * `isort_check` checks if the order of the import statements is correct using [`isort`](https://pycqa.github.io/isort/).
 * `isort` automatically re-orders the import statements using `isort`.
+* `license` makes sure every Python (`*.py`) file contains the proper license header.
 * `lint_check` checks if the code follows the [`pylint`](https://pypi.org/project/pylint/) rules defined in `pyproject.toml`.
 * `lint` automatically adjust the code to follow the `pylint` rules defined in `pyproject.toml`.
-* `license` makes sure every Python (`*.py`) file contains the proper license header.
-* `build` builds a Python package which can be uploaded to [`PyPI`](https://pypi.org/project/smartmeter-datacollector/) using `twine`.
-* `build_check` uses `twine` to check if the built Python package will be accepted by `PiPI`.
 * `setup_check` checks whether the dependencies defined in `Pipfile` / `Pipfile.lock` are in sync with `setup.py`.
 * `setup` synchronizes the dependencies defined in `Pipfile` / `Pipfile.lock` with `setup.py`.
-* `debianize` creates a `debian/` directory used to build Debian source / binary packages.
-* `build_srcdeb` builds a Debian source package which can be used to build a Debian (binary) package for any platform (e.g. using [`pbuilder`](https://pbuilder-docs.readthedocs.io/en/latest/usage.html))
-* `build_deb` builds a Debian package for the current development plattform.
 
-Make sure to run `format_check` / `format`, `isort_check` / `isort`, `lint_check` / `lint`, `license`, `setup_check` / `setup` before commiting changes to the repository to avoid unnecessary development cycles. `smartmeter-datacollector` uses [GitHub Actions](https://github.com/scs/smartmeter-datacollector/actions) to check if these rules apply.
+Make sure to run `format_check` / `format`, `isort_check` / `isort`, `lint_check` / `lint`, `license`, `setup_check` / `setup` before committing changes to the repository to avoid unnecessary development cycles. `smartmeter-datacollector` uses [GitHub Actions](https://github.com/scs/smartmeter-datacollector/actions) to check if these rules apply.
 
 # Acknowledgements
 `smartmeter-datacollector` and its companion project [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-configurator) have been developed by **[Supercomputing Systems AG](https://www.scs.ch)** on behalf of and funded by **[EKZ](https://www.ekz.ch/)**.
-
-
```

#### html2text {}

```diff
@@ -1,48 +1,40 @@
-Metadata-Version: 2.1 Name: smartmeter-datacollector Version: 1.0.2 Summary:
-Smart Meter Data Collector Home-page: https://github.com/scs/smartmeter-
-datacollector Author: Supercomputing Systems AG Author-email: info@scs.ch
-License: GPLv2 Project-URL: Source, https://github.com/scs/smartmeter-
-datacollector Project-URL: Bug Reports, https://github.com/scs/smartmeter-
-datacollector/issues Project-URL: Pull Requests, https://github.com/scs/
-smartmeter-datacollector/pulls Project-URL: SCS, https://www.scs.ch Platform:
-UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
-License :: OSI Approved :: GNU General Public License v2 (GPLv2) Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Typing :: Typed Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE # Smart Meter
-Data Collector
+# Smart Meter Data Collector
    [License:_GPL-2.0-only] [Pull_Requests_Welcome] [Contributions_Welcome]
                  [Python Code Checks] [PyPI_-_Python_Version]
                                 [ekz_logo.png]
 --- The `smartmeter-datacollector` tool is a Python3 software which allows you
 to continuously retrieve data from supported smart meters (listed below). The
 acquired values can be forwarded to one or more data sinks like a MQTT broker
 or logger. This tool is an open source software funded by **[EKZ
 (ElektrizitÃ¤tswerke des Kantons ZÃ¼rich)](https://www.ekz.ch)** and developed
 by **[Supercomputing Systems AG](https://www.scs.ch)**. The goal of this
 voluntary initiative is to create a tool that can read, decode and decrypt data
 (if necessary) from the local interface of various smart meters and convert it
 into human-readable and simple formats. This should eliminate the complexity of
 decoding DLMS and similar protocols for the user. The user has the data in a
 format, which he can easily use in various use-cases ranging from simple
-vizualization (see [Method 1: Raspberry Pi image with demo](#method-1-
+visualization (see [Method 1: Raspberry Pi image with demo](#method-1-
 raspberry-pi-image-with-demo)) to integration into energy management algorithms
 or into custom home automation software. The following smart meters are
-supported: * Landis+Gyr E450: \ Data pushed by smart meter over CII interface
-(wired M-Bus). Encoded with HDLC and DLMS/COSEM. * Unencrypted data * Encrypted
-data * Iskraemeco AM550: \ Data pushed by smart meter over [P1 interface
-(DSMR)](https://www.netbeheernederland.nl/_upload/Files/
-Slimme_meter_15_a727fce1f1.pdf). Encoded with HDLC (IEC 62056-46) and DLMS/
-COSEM. * Unencrypted data * Encrypted data The following data sinks are
+supported (see [Wiki/Home](https://github.com/scs/smartmeter-datacollector/
+wiki/Home) for detailed information). * Landis+Gyr E450: \ Data pushed by smart
+meter over CII interface (wired M-Bus, HDLC, DLMS/COSEM). * Landis+Gyr E360: \
+Data pushed by smart meter over P1 interface (HDLC, DLMS/COSEM only, no DSMR).
+* Iskraemeco AM550: \ Data pushed by smart meter over P1 interface (HDLC, DLMS/
+COSEM only, no DSMR). * Kamstrup OMNIPOWER with HAN-NVE: \ Data pushed by smart
+meter over inserted [HAN-NVE module](https://www.kamstrup.com/en-en/
+electricity-solutions/meters-devices/modules/hannve) (wired M-Bus, HDLC, DLMS/
+COSEM). Note: All smart meters integrated so far push binary data encoded with
+HDLC (IEC 62056-46) and DLMS/COSEM. Both unencrypted and encrypted DLMS
+messages are accepted by the software. The following data sinks are
 implemented: * MQTT (v3.1.1): * Encryption * Unencrypted connection * Encrypted
 connection * TLS * optional custom CA certificate * Authentication *
 Unauthenticated * Authenticated with username / password * Authenticated with
-client certificate * Logger to STDOUT `smartmeter-datacollector` is fully
+client certificate * Logger to `stdout` `smartmeter-datacollector` is fully
 configurable through a `.ini` configuration file. The [`smartmeter-
 datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-
 configurator) webinterface can help to create and modify the configuration. --
 - - [Smart Meter Data Collector](#smart-meter-data-collector) - [How to
 install](#how-to-install) - [Method 1: Raspberry Pi image with demo](#method-1-
 raspberry-pi-image-with-demo) - [Method 2: Python package](#method-2-python-
 package) - [Python Requirements](#python-requirements) - [Installation]
@@ -65,156 +57,116 @@
 (based on Raspberry Pi OS) which contains the following parts: * `smartmeter-
 datacollector` as a systemd service * `smartmeter-datacollector-configurator`
 webinterface * demo * [mosquiotto](https://mosquitto.org/) as a local MQTT
 broker to publish the measurements from `smartmeter-datacollector` * [Telegraf]
 (https://www.influxdata.com/time-series-platform/telegraf/) to collect
 measurements published by `smartmeter-datacollector` over MQTT and store them
 in InfluxDB * [InfluxDB](https://www.influxdata.com/) to store the measurements
-* [Grafana](https://grafana.com/) to visualize the measurements This setup
-allows a (first time) user to [install](https://www.raspberrypi.org/
-documentation/computers/getting-started.html#installing-the-operating-system)
-the image on a Raspberry Pi and immediately get started with `smartmeter-
-datacollector`. The following steps are required: 1. Download the Raspberry Pi
-image from the [latest release](https://github.com/scs/smartmeter-
-datacollector/releases). 2. Install the image on a (micro)SD card, e.g. using
-[Raspberry Pi Imager](https://www.raspberrypi.org/documentation/computers/
-getting-started.html#using-raspberry-pi-imager). 3. Prepare the Raspberry Pi.
-1. Push the (micro)SD card into the proper slot. 2. Use an RJ-45 cable (or
-configure WiFi later) to connect to a network. 3. Connect the power cable to
-the Micro USB port. 4. Open the `smartmeter-datacollector-configurator`
-webinterface using `http://:8000/` in your favorite browser. 1. Load the pre-
-defined configuration. 2. Adjust the settings of the connected smart meter. 3.
-Deploy the adjusted configuration. 4. Restart the `smartmeter-datacollector`
-service. 5. Open `Grafana` using `http://:3000/` in your favorite browser. 6.
-Observe the measurements from your smart meter while they arrive periodically.
-See [Wiki/Demo](https://github.com/scs/smartmeter-datacollector/wiki/Demo-
-(Raspberry-Pi-Image)) for more details on the provided Raspberry Pi image with
-the demo. ## Method 2: Python package `smartmeter-datacollector` can be
-installed as a Python3 package either from [PyPi](https://pypi.org/project/
-smartmeter-datacollector/) or manually using a [released wheel](https://
-github.com/scs/smartmeter-datacollector/releases). The Python3 package does not
-contain any infrastructure to run `smartmeter-datacollector` in the background
-or to automatically start it during a boot sequence. If such infrastructure is
-required either see [Method 3: Debian package](#method-3-debian-package) or
-provide it yourself. ### Python Requirements * Python >= 3.7 (tested with 3.8)
-### Installation Install the package either as global Python package or in a
-virtualenv with ```bash python3 -m pip install smartmeter-datacollector ```
-Similarly the [`smartmeter-datacollector-configurator`](https://github.com/scs/
-smartmeter-datacollector-configurator) webinterface can be installed with
-```bash python3 -m pip install smartmeter-datacollector-configurator ``` ##
-Method 3: Debian package `smartmeter-datacollector` is also available as a
-Debian (`.deb`) package from the [releases](https://github.com/scs/smartmeter-
-datacollector/releases) which installs it system wide. The Debian package
-includes a systemd service file which enables `smartmeter-datacollector` to
-automatically start after booting the system. ### Debian Requirements *
-Distribution * Debian * Release * Buster * CPU architecture * amd64 * armhf ###
-Installation Download the Debian package from [releases](https://github.com/
-scs/smartmeter-datacollector/releases) and install it with ```bash sudo apt
-install ./python3-smartmeter-datacollector_*.deb ``` Similarly the
-[`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-
-datacollector-configurator) webinterface can be installed with a Debian package
-from its [releases](https://github.com/scs/smartmeter-datacollector-
-configurator/releases) with ```bash sudo apt install ./python3-smartmeter-
-datacollector-configurator_*.deb ``` # How to use The usage of `smartmeter-
-datacollector` depends on the installation method. Independent of the
-installation method a `.ini` configuration file is required to properly run
-`smartmeter-datacollector`. ## Configuration ### Specification The `.ini`
-configuration file supports the following format ```ini [reader0] # type of the
-connected smart meter type = lge450 # serial port to which the smart meter is
-connected port = /dev/ttyUSB0 # optional encryption key key = [sink0] # type of
-the sink type = mqtt # host / IP address of the MQTT broker host = localhost #
-port of the MQTT broker port = 1883 # whether to use TLS (Transport Layer
-Security) tls = False # optional path to the CA certificate used to validate
-the MQTT broker's certificate ca_file_path = # whether to check the hostname of
-the MQTT broker against the certificate check_hostname = False # optional
-username for authentication with the MQTT broker username = # optional password
-for authentication with the MQTT broker password = # optional path to the
-client certificate for authentication with the MQTT broker client_cert_path = #
-optional path to the private key for the client certificate for authentication
-with the MQTT broker client_key_path = [sink1] # type of the sink type = logger
-# name of the logger name = DataLogger [logging] # log level configuration:
-DEBUG / INFO / WARNING / ERROR default = WARNING smartmeter = WARNING collector
-= WARNING sink = WARNING ``` There can be multiple `[readerX]` and `[sinkY]`
-sections for every connected smart meter and / or data sink. See [Wiki/
-Configuration](https://github.com/scs/smartmeter-datacollector/wiki/
-Configuration) for more details on the available configuration options. ###
-smartmeter-datacollector-configurator To simplify the process of generating a
-valid `.ini` configuration for `smartmeter-datacollector` the companion
-[`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-
-datacollector-configurator) webinterface can be used. It supports * a graphical
-approach to manage the configuration * input validation to avoid invalid
-configurations * loading / saving / discarding a configuration * restarting
-`smartmeter-datacollector` (only if installed as a Debian package) See [Wiki/
-smartmeter-datacollector-configurator](https://github.com/scs/smartmeter-
-datacollector/wiki/smartmeter-datacollector-configurator) for more details on
-the webinterface and the configuration possibilities. ## Run manually Run
+* [Grafana](https://grafana.com/) to visualize the measurements See [Wiki/Demo]
+(https://github.com/scs/smartmeter-datacollector/wiki/Demo-(Raspberry-Pi-
+Image)) for detailed setup instructions. ## Method 2: Python package
+`smartmeter-datacollector` can be installed as a Python3 package either from
+[PyPi](https://pypi.org/project/smartmeter-datacollector/) or manually using a
+[released wheel](https://github.com/scs/smartmeter-datacollector/releases). The
+Python3 package does not contain any infrastructure to run `smartmeter-
+datacollector` in the background or to automatically start it during a boot
+sequence. If such infrastructure is required either see [Method 3: Debian
+package](#method-3-debian-package) or provide it yourself. ### Python
+Requirements * Python >= 3.7 (tested with 3.8) ### Installation Install the
+package either as global Python package or in a virtualenv with ```bash python3
+-m pip install smartmeter-datacollector ``` Similarly the [`smartmeter-
+datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-
+configurator) webinterface can be installed with ```bash python3 -m pip install
+smartmeter-datacollector-configurator ``` ## Method 3: Debian package
+`smartmeter-datacollector` is also available as a Debian (`.deb`) package from
+the [releases](https://github.com/scs/smartmeter-datacollector/releases) which
+installs it system wide. The Debian package includes a systemd service file
+which enables `smartmeter-datacollector` to automatically start after booting
+the system. ### Debian Requirements * Distribution * Debian * Release *
+Bullseye * CPU architecture * amd64 * armhf ### Installation Download the
+Debian package from [releases](https://github.com/scs/smartmeter-datacollector/
+releases) and install it with ```bash sudo apt install ./python3-smartmeter-
+datacollector_*.deb ``` Similarly the [`smartmeter-datacollector-configurator`]
+(https://github.com/scs/smartmeter-datacollector-configurator) webinterface can
+be installed with a Debian package from its [releases](https://github.com/scs/
+smartmeter-datacollector-configurator/releases) with ```bash sudo apt install
+./python3-smartmeter-datacollector-configurator_*.deb ``` # How to use The
+usage of `smartmeter-datacollector` depends on the installation method.
+Independent of the installation method a `.ini` configuration file is required
+to properly run `smartmeter-datacollector`. ## Configuration ### Manually
+create configuration See [Wiki/Configuration](https://github.com/scs/
+smartmeter-datacollector/wiki/Configuration#manually-write-configuration) for
+more details on the available configuration options. ### smartmeter-
+datacollector-configurator To simplify the process of generating a valid `.ini`
+configuration for `smartmeter-datacollector` the companion [`smartmeter-
+datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-
+configurator) webinterface can be used. It supports * a graphical approach to
+manage the configuration * input validation to avoid invalid configurations *
+loading / saving / discarding a configuration * restarting `smartmeter-
+datacollector` (only if installed as a Debian package) See [Wiki/smartmeter-
+datacollector-configurator](https://github.com/scs/smartmeter-datacollector/
+wiki/smartmeter-datacollector-configurator) for more details on the
+webinterface and the configuration possibilities. ## Run manually Run
 `smartmeter-datacollector` with the following command: ``` smartmeter-
 datacollector --config datacollector.ini ``` The following command line
 arguments are supported: * `-h, --help`: Shows the help output of `smartmeter-
 datacollector`. * `-c, --config CONFIG`: Path to the `.ini` configuration file.
-* `-s,--saveconfig`: Cteate a default `.ini` configuration file. * `-d, --dev`:
+* `-s,--saveconfig`: Create a default `.ini` configuration file. * `-d, --dev`:
 Enable development mode. ### Configuration The configuration file can be
 located anywhere and use any filename. If no `.ini` configuration file is
 specified a default configuration with the following options is used: *
-Landys+Gir E450 smart meter in unencrypted mode connected to `/dev/ttyUSB0` *
+Landys+Gyr E450 smart meter in unencrypted mode connected to `/dev/ttyUSB0` *
 `LOGGER` sink * `MQTT` sink connected to a local broker without encryption or
 authentication ## Run as a systemd service When `smartmeter-datacollector` has
 been installed as a Debian package it provides a systemd .service file named
 `python3-smartmeter-datacollector.service`. Therefore the service can be
-managed using the `systemctl` command: ``` sudo systemctl start|stop|restart
-python3-smartmeter-datacollector ``` Enabling or disabling the service can also
-be managed using the `systemctl` command: ``` sudo systemctl enable|disable
-python3-smartmeter-datacollector ``` Inspecting the log messages can be done
-using the `journalctl` command: ``` journalctl -u python3-smartmeter-
-datacollector [-f] ``` ### Configuration The systemd service expectes the
-`.ini` configuration to be located at `/var/lib/smartmeter-datacollector/
-datacollector.ini`. This is also the default location used by the [`smartmeter-
-datacollector-configurator`](https://github.com/scs/smartmeter-datacollector-
-configurator) webinterface to load and save the managed configuration. # How to
-develop Help from the community for the `smartmeter-datacollector` project is
-always welcome. Please follow the next few chapters to setup a working
-development environment. ## Development Requirements * Python >= 3.7 *
-[`pipenv`](https://pipenv.pypa.io/en/latest/) * Optional software packages
-(Debian / Ubuntu) * python3-all * debhelper * dh-python * dh-systemd ##
-Installation ### Debian / Ubuntu To install the listed minimal requirements run
-the following command: ``` sudo apt install git python3 pipenv ``` To install
-the optional requirements also run the following command: ``` sudo apt install
-python3-all debhelper dh-python dh-systemd ``` ## Checkout the code Use `git`
-to clone / checkout `smartmeter-datacollector` from GitHub using ``` git clone
-https://github.com/scs/smartmeter-datacollector.git ``` ## Setup Development
-Environment `smartmeter-datacollector` uses [`pipenv`](https://pipenv.pypa.io/
-en/latest/) to manage its dependencies and setup a virtual environment. Run the
-following command to setup the initial development environment: ``` pipenv
-install --dev ``` This will install all runtime and development dependencies
-for `smartmeter-datacollector` in a new virtual environment. Now you are ready
-to start working on `smartmeter-datacollector`. ## Custom Commands / Workflows
-`smartmeter-datacollector` offers a few custom `pipenv run` commands to
-simplify certain development workflows: * `format_check` checks if the code
-follows the [`autopep8`](https://pypi.org/project/autopep8/) code formatting
-rules. * `format` automatically adjusts the code to follow the `autopep8` code
-formatting rules. * `isort_check` checks if the order of the import statements
-is correct using [`isort`](https://pycqa.github.io/isort/). * `isort`
-automatically re-orders the import statements using `isort`. * `lint_check`
-checks if the code follows the [`pylint`](https://pypi.org/project/pylint/
-) rules defined in `pyproject.toml`. * `lint` automatically adjust the code to
-follow the `pylint` rules defined in `pyproject.toml`. * `license` makes sure
-every Python (`*.py`) file contains the proper license header. * `build` builds
-a Python package which can be uploaded to [`PyPI`](https://pypi.org/project/
-smartmeter-datacollector/) using `twine`. * `build_check` uses `twine` to check
-if the built Python package will be accepted by `PiPI`. * `setup_check` checks
-whether the dependencies defined in `Pipfile` / `Pipfile.lock` are in sync with
-`setup.py`. * `setup` synchronizes the dependencies defined in `Pipfile` /
-`Pipfile.lock` with `setup.py`. * `debianize` creates a `debian/` directory
-used to build Debian source / binary packages. * `build_srcdeb` builds a Debian
+managed using the `systemctl` command. See [Run as a systemd service](https://
+github.com/scs/smartmeter-datacollector/wiki/How-to-use#run-as-a-systemd-
+service) for possible commands. # How to develop Help from the community for
+the `smartmeter-datacollector` project is always welcome. Please follow the
+next few chapters to setup a working development environment. ## Development
+Requirements * Python >= 3.8, <= 3.10 * [`pipenv`](https://pipenv.pypa.io/en/
+latest/) * Optional software packages (Debian bullseye/ Ubuntu 22.04) *
+python3-all * debhelper * dh-python ## Installation ### Debian / Ubuntu To
+install the listed minimal requirements run the following command: ``` sudo apt
+install git python3 pipenv ``` To install the optional requirements also run
+the following command: ``` sudo apt install python3-all debhelper dh-python ```
+## Checkout the code Use `git` to clone / checkout `smartmeter-datacollector`
+from GitHub using ``` git clone https://github.com/scs/smartmeter-
+datacollector.git ``` ## Setup Development Environment `smartmeter-
+datacollector` uses [`pipenv`](https://pipenv.pypa.io/en/latest/) to manage its
+dependencies and setup a virtual environment. Run the following command to
+setup the initial development environment: ``` pipenv install --dev ``` This
+will install all runtime and development dependencies for `smartmeter-
+datacollector` in a new virtual environment. Now you are ready to start working
+on `smartmeter-datacollector`. ## Custom Commands / Workflows `smartmeter-
+datacollector` offers a few custom `pipenv run` commands to simplify certain
+development workflows: * `build_check` uses `twine` to check if the built
+Python package will be accepted by `PiPI`. * `build_deb` builds a Debian
+package for the current development platform. * `build_srcdeb` builds a Debian
 source package which can be used to build a Debian (binary) package for any
 platform (e.g. using [`pbuilder`](https://pbuilder-docs.readthedocs.io/en/
-latest/usage.html)) * `build_deb` builds a Debian package for the current
-development plattform. Make sure to run `format_check` / `format`,
-`isort_check` / `isort`, `lint_check` / `lint`, `license`, `setup_check` /
-`setup` before commiting changes to the repository to avoid unnecessary
-development cycles. `smartmeter-datacollector` uses [GitHub Actions](https://
-github.com/scs/smartmeter-datacollector/actions) to check if these rules apply.
-# Acknowledgements `smartmeter-datacollector` and its companion project
+latest/usage.html)) * `build` builds a Python package which can be uploaded to
+[`PyPI`](https://pypi.org/project/smartmeter-datacollector/) using `twine`. *
+`debianize` creates a `debian/` directory used to build Debian source / binary
+packages. * `format_check` checks if the code follows the [`autopep8`](https://
+pypi.org/project/autopep8/) code formatting rules. * `format` automatically
+adjusts the code to follow the `autopep8` code formatting rules. *
+`isort_check` checks if the order of the import statements is correct using
+[`isort`](https://pycqa.github.io/isort/). * `isort` automatically re-orders
+the import statements using `isort`. * `license` makes sure every Python
+(`*.py`) file contains the proper license header. * `lint_check` checks if the
+code follows the [`pylint`](https://pypi.org/project/pylint/) rules defined in
+`pyproject.toml`. * `lint` automatically adjust the code to follow the `pylint`
+rules defined in `pyproject.toml`. * `setup_check` checks whether the
+dependencies defined in `Pipfile` / `Pipfile.lock` are in sync with `setup.py`.
+* `setup` synchronizes the dependencies defined in `Pipfile` / `Pipfile.lock`
+with `setup.py`. Make sure to run `format_check` / `format`, `isort_check` /
+`isort`, `lint_check` / `lint`, `license`, `setup_check` / `setup` before
+committing changes to the repository to avoid unnecessary development cycles.
+`smartmeter-datacollector` uses [GitHub Actions](https://github.com/scs/
+smartmeter-datacollector/actions) to check if these rules apply. #
+Acknowledgements `smartmeter-datacollector` and its companion project
 [`smartmeter-datacollector-configurator`](https://github.com/scs/smartmeter-
 datacollector-configurator) have been developed by **[Supercomputing Systems
 AG](https://www.scs.ch)** on behalf of and funded by **[EKZ](https://
 www.ekz.ch/)**.
```

