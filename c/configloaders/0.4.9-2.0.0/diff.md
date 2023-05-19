# Comparing `tmp/configloaders-0.4.9.tar.gz` & `tmp/configloaders-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configloaders-0.4.9.tar", max compression
+gzip compressed data, was "configloaders-2.0.0.tar", max compression
```

## Comparing `configloaders-0.4.9.tar` & `configloaders-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,29 @@
--rw-r--r--   0        0        0      894 2023-03-04 11:36:46.666844 configloaders-0.4.9/configloaders/__init__.py
--rw-r--r--   0        0        0      239 2023-03-04 08:25:37.549047 configloaders-0.4.9/configloaders/__log.py
--rw-r--r--   0        0        0      346 2023-03-04 10:24:14.978237 configloaders-0.4.9/configloaders/__message.py
--rw-r--r--   0        0        0      108 2023-03-04 08:25:37.549047 configloaders-0.4.9/configloaders/__util.py
--rw-r--r--   0        0        0      414 2023-03-04 10:21:46.981627 configloaders-0.4.9/configloaders/_appdir.py
--rw-r--r--   0        0        0     1548 2023-03-04 10:21:44.717686 configloaders-0.4.9/configloaders/_argparse.py
--rw-r--r--   0        0        0     2130 2023-03-06 05:22:38.317047 configloaders-0.4.9/configloaders/_file.py
--rw-r--r--   0        0        0     1660 2023-03-04 10:22:23.833632 configloaders-0.4.9/configloaders/_ini.py
--rw-r--r--   0        0        0      791 2023-03-04 10:22:36.594481 configloaders-0.4.9/configloaders/_json.py
--rw-r--r--   0        0        0     2350 2023-03-04 10:22:44.957101 configloaders-0.4.9/configloaders/_loader.py
--rw-r--r--   0        0        0      657 2023-03-04 10:22:48.613316 configloaders-0.4.9/configloaders/_pickle.py
--rw-r--r--   0        0        0      617 2023-03-04 10:22:51.825227 configloaders-0.4.9/configloaders/_py.py
--rw-r--r--   0        0        0     2213 2023-03-04 10:23:06.930802 configloaders-0.4.9/configloaders/_sqlite.py
--rw-r--r--   0        0        0     1116 2023-03-04 10:23:14.188382 configloaders-0.4.9/configloaders/_textline.py
--rw-r--r--   0        0        0     3605 2023-03-04 14:03:22.044572 configloaders-0.4.9/configloaders/_tkinter.py
--rw-r--r--   0        0        0      631 2023-03-04 10:23:16.858240 configloaders-0.4.9/configloaders/_toml.py
--rw-r--r--   0        0        0     1615 2023-03-04 10:23:24.240476 configloaders-0.4.9/configloaders/_xml.py
--rw-r--r--   0        0        0      640 2023-03-04 10:23:28.058259 configloaders-0.4.9/configloaders/_yaml.py
--rw-r--r--   0        0        0      393 2023-03-06 05:23:54.306779 configloaders-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     1552 2023-03-04 10:15:56.200485 configloaders-0.4.9/README.md
--rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 configloaders-0.4.9/setup.py
--rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 configloaders-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     4330 2023-05-18 02:25:23.404229 configloaders-2.0.0/configloaders/__core.py
+-rw-r--r--   0        0        0      162 2023-05-18 01:08:47.253489 configloaders-2.0.0/configloaders/__init__.py
+-rw-r--r--   0        0        0     1505 2023-05-17 06:42:37.555364 configloaders-2.0.0/configloaders/__main__.py
+-rw-r--r--   0        0        0     4458 2023-05-18 01:03:28.917308 configloaders-2.0.0/configloaders/__type.py
+-rw-r--r--   0        0        0      131 2023-05-15 06:59:20.581187 configloaders-2.0.0/configloaders/providers/__init__.py
+-rw-r--r--   0        0        0      183 2023-05-04 09:13:33.064983 configloaders-2.0.0/configloaders/providers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      380 2023-05-15 07:03:18.799662 configloaders-2.0.0/configloaders/providers/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     1936 2023-05-17 06:57:28.206529 configloaders-2.0.0/configloaders/providers/__pycache__/ini_provider.cpython-37.pyc
+-rw-r--r--   0        0        0      936 2023-05-05 03:13:54.862960 configloaders-2.0.0/configloaders/providers/__pycache__/json_provider.cpython-310.pyc
+-rw-r--r--   0        0        0      843 2023-05-17 06:57:28.216261 configloaders-2.0.0/configloaders/providers/__pycache__/json_provider.cpython-37.pyc
+-rw-r--r--   0        0        0      855 2023-05-17 06:57:28.244261 configloaders-2.0.0/configloaders/providers/__pycache__/pickle_provider.cpython-37.pyc
+-rw-r--r--   0        0        0     1215 2023-05-17 06:57:28.251261 configloaders-2.0.0/configloaders/providers/__pycache__/py_provider.cpython-37.pyc
+-rw-r--r--   0        0        0      843 2023-05-17 06:57:28.255298 configloaders-2.0.0/configloaders/providers/__pycache__/toml_provider.cpython-37.pyc
+-rw-r--r--   0        0        0     1619 2023-05-17 06:57:28.346825 configloaders-2.0.0/configloaders/providers/__pycache__/txt_provider.cpython-37.pyc
+-rw-r--r--   0        0        0     1689 2023-05-17 06:57:28.348830 configloaders-2.0.0/configloaders/providers/__pycache__/xml_provider.cpython-37.pyc
+-rw-r--r--   0        0        0      853 2023-05-17 06:57:28.458830 configloaders-2.0.0/configloaders/providers/__pycache__/yaml_provider.cpython-37.pyc
+-rw-r--r--   0        0        0     1011 2023-05-17 06:42:37.197903 configloaders-2.0.0/configloaders/providers/ini_provider.py
+-rw-r--r--   0        0        0      367 2023-05-17 06:42:37.359904 configloaders-2.0.0/configloaders/providers/json_provider.py
+-rw-r--r--   0        0        0      351 2023-05-17 06:42:37.083912 configloaders-2.0.0/configloaders/providers/pickle_provider.py
+-rw-r--r--   0        0        0      657 2023-05-17 06:42:37.206904 configloaders-2.0.0/configloaders/providers/py_provider.py
+-rw-r--r--   0        0        0      343 2023-05-17 06:42:37.427418 configloaders-2.0.0/configloaders/providers/toml_provider.py
+-rw-r--r--   0        0        0      625 2023-05-17 06:42:37.716516 configloaders-2.0.0/configloaders/providers/txt_provider.py
+-rw-r--r--   0        0        0     1369 2023-05-17 06:42:37.294904 configloaders-2.0.0/configloaders/providers/xml_provider.py
+-rw-r--r--   0        0        0      353 2023-05-17 06:42:37.287127 configloaders-2.0.0/configloaders/providers/yaml_provider.py
+-rw-r--r--   0        0        0     1079 2023-05-18 10:09:54.036619 configloaders-2.0.0/LICENSE
+-rw-r--r--   0        0        0      611 2023-05-18 10:10:47.659824 configloaders-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1756 2023-05-18 10:08:59.013294 configloaders-2.0.0/README.md
+-rw-r--r--   0        0        0     2627 1970-01-01 00:00:00.000000 configloaders-2.0.0/setup.py
+-rw-r--r--   0        0        0     2380 1970-01-01 00:00:00.000000 configloaders-2.0.0/PKG-INFO
```

