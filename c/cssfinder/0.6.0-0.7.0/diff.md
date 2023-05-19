# Comparing `tmp/cssfinder-0.6.0.tar.gz` & `tmp/cssfinder-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cssfinder-0.6.0.tar", max compression
+gzip compressed data, was "cssfinder-0.7.0.tar", max compression
```

## Comparing `cssfinder-0.6.0.tar` & `cssfinder-0.7.0.tar`

### file list

```diff
@@ -1,85 +1,86 @@
--rw-r--r--   0        0        0     1069 2023-04-27 23:10:30.086484 cssfinder-0.6.0/LICENSE.md
--rw-r--r--   0        0        0    11275 2023-04-27 23:10:30.086484 cssfinder-0.6.0/README.md
--rw-r--r--   0        0        0     1417 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/__init__.py
--rw-r--r--   0        0        0     1280 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/__main__.py
--rw-r--r--   0        0        0     1224 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/algorithm/__init__.py
--rw-r--r--   0        0        0     1308 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/algorithm/backend/__init__.py
--rw-r--r--   0        0        0     3951 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/algorithm/backend/base.py
--rw-r--r--   0        0        0     6456 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/algorithm/backend/loader.py
--rw-r--r--   0        0        0     6934 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/algorithm/gilbert.py
--rw-r--r--   0        0        0     6166 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/algorithm/mode_util.py
--rw-r--r--   0        0        0     9651 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/api.py
--rw-r--r--   0        0        0     1676 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/base_model.py
--rw-r--r--   0        0        0    18270 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/cli.py
--rw-r--r--   0        0        0     3875 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/constants.py
--rw-r--r--   0        0        0     4915 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/crossplatform.py
--rw-r--r--   0        0        0    23376 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/cssfproject.py
--rw-r--r--   0        0        0     2169 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/enums.py
--rw-r--r--   0        0        0       10 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/.gitignore
--rw-r--r--   0        0        0     1192 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/5qubits_json/5qubits_in.mtx
--rw-r--r--   0        0        0     1819 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/5qubits_json/cssfproject.json
--rw-r--r--   0        0        0     1192 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/5qubits_py/5qubits_in.mtx
--rw-r--r--   0        0        0     2667 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/5qubits_py/cssfproject.py
--rw-r--r--   0        0        0     1036 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/GHZ3_in.mtx
--rw-r--r--   0        0        0     2101 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/cssfproject.json
--rw-r--r--   0        0        0      175 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_0_0.mtx
--rw-r--r--   0        0        0      175 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_0_1.mtx
--rw-r--r--   0        0        0      175 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_0.mtx
--rw-r--r--   0        0        0     1762 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_1.mtx
--rw-r--r--   0        0        0      166 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_2.mtx
--rw-r--r--   0        0        0     1762 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_3.mtx
--rw-r--r--   0        0        0      183 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_4.mtx
--rw-r--r--   0        0        0     1762 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_5.mtx
--rw-r--r--   0        0        0      166 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_6.mtx
--rw-r--r--   0        0        0     1762 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_7.mtx
--rw-r--r--   0        0        0     3638 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ4_json/GHZ4_in.mtx
--rw-r--r--   0        0        0     1174 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/GHZ4_json/cssfproject.json
--rw-r--r--   0        0        0     2593 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/SBiPa_json/cssfproject.json
--rw-r--r--   0        0        0     1270 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/SBiPa_json/projection.mtx
--rw-r--r--   0        0        0     1270 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/SBiPa_json/state.mtx
--rw-r--r--   0        0        0     5139 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/__init__.py
--rw-r--r--   0        0        0     1192 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/benchmark_32x32/5qubits_in.mtx
--rw-r--r--   0        0        0     2957 2023-04-27 23:10:30.086484 cssfinder-0.6.0/cssfinder/examples/benchmark_32x32/cssfproject.py
--rw-r--r--   0        0        0    54182 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/10_in.mtx
--rw-r--r--   0        0        0     3693 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/cssfproject.py
--rw-r--r--   0        0        0     4265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_0.mtx
--rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_1.mtx
--rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_2.mtx
--rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_3.mtx
--rw-r--r--   0        0        0     4297 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_4.mtx
--rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_5.mtx
--rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_6.mtx
--rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_7.mtx
--rw-r--r--   0        0        0     4265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_0.mtx
--rw-r--r--   0        0        0   106596 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_1.mtx
--rw-r--r--   0        0        0   106596 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_2.mtx
--rw-r--r--   0        0        0   106596 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_3.mtx
--rw-r--r--   0        0        0     4281 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_4.mtx
--rw-r--r--   0        0        0   106596 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_5.mtx
--rw-r--r--   0        0        0   106596 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_6.mtx
--rw-r--r--   0        0        0   106596 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_7.mtx
--rw-r--r--   0        0        0     4265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_0.mtx
--rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_1.mtx
--rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_2.mtx
--rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_3.mtx
--rw-r--r--   0        0        0     4297 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_4.mtx
--rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_5.mtx
--rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_6.mtx
--rw-r--r--   0        0        0   108265 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_7.mtx
--rw-r--r--   0        0        0    14212 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/interactive.py
--rw-r--r--   0        0        0     1227 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/io/__init__.py
--rw-r--r--   0        0        0     6003 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/io/gilbert_io.py
--rw-r--r--   0        0        0     4182 2023-04-27 23:10:30.090484 cssfinder-0.6.0/cssfinder/io/matrix.py
--rwxr-xr-x   0        0        0    12147 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/log.py
--rw-r--r--   0        0        0     1547 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/__init__.py
--rw-r--r--   0        0        0     1291 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/archive.py
--rw-r--r--   0        0        0     2200 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/html.py
--rw-r--r--   0        0        0     4292 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/manager.py
--rw-r--r--   0        0        0     9217 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/math.py
--rw-r--r--   0        0        0     2937 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/pdf.py
--rw-r--r--   0        0        0     8295 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/plotting.py
--rw-r--r--   0        0        0     4619 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/renderer.py
--rw-r--r--   0        0        0     1203 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/reports/txt.py
--rw-r--r--   0        0        0     3947 2023-04-27 23:10:30.094484 cssfinder-0.6.0/cssfinder/templates/report.html.jinja2
--rw-r--r--   0        0        0    17232 2023-04-27 23:10:30.098484 cssfinder-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    12779 1970-01-01 00:00:00.000000 cssfinder-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-19 13:27:27.719206 cssfinder-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0    14948 2023-05-19 13:27:27.719206 cssfinder-0.7.0/README.md
+-rw-r--r--   0        0        0     1417 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/__init__.py
+-rw-r--r--   0        0        0     1280 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/__main__.py
+-rw-r--r--   0        0        0     1224 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/algorithm/__init__.py
+-rw-r--r--   0        0        0     1308 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/algorithm/backend/__init__.py
+-rw-r--r--   0        0        0     3951 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/algorithm/backend/base.py
+-rw-r--r--   0        0        0     6456 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/algorithm/backend/loader.py
+-rw-r--r--   0        0        0     6934 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/algorithm/gilbert.py
+-rw-r--r--   0        0        0     6857 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/algorithm/mode_util.py
+-rw-r--r--   0        0        0    10007 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/api.py
+-rw-r--r--   0        0        0     1676 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/base_model.py
+-rw-r--r--   0        0        0    21413 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/cli.py
+-rw-r--r--   0        0        0     3875 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/constants.py
+-rw-r--r--   0        0        0     4915 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/crossplatform.py
+-rw-r--r--   0        0        0    23376 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/cssfproject.py
+-rw-r--r--   0        0        0     2169 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/enums.py
+-rw-r--r--   0        0        0       10 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/.gitignore
+-rw-r--r--   0        0        0     1192 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/5qubits_json/5qubits_in.mtx
+-rw-r--r--   0        0        0     1819 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/5qubits_json/cssfproject.json
+-rw-r--r--   0        0        0     1192 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/5qubits_py/5qubits_in.mtx
+-rw-r--r--   0        0        0     2667 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/5qubits_py/cssfproject.py
+-rw-r--r--   0        0        0     1036 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/GHZ3_in.mtx
+-rw-r--r--   0        0        0     2874 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/cssfproject.json
+-rw-r--r--   0        0        0      175 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_0_0.mtx
+-rw-r--r--   0        0        0      175 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_0_1.mtx
+-rw-r--r--   0        0        0      175 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_0.mtx
+-rw-r--r--   0        0        0     1762 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_1.mtx
+-rw-r--r--   0        0        0      166 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_2.mtx
+-rw-r--r--   0        0        0     1762 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_3.mtx
+-rw-r--r--   0        0        0      183 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_4.mtx
+-rw-r--r--   0        0        0     1762 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_5.mtx
+-rw-r--r--   0        0        0      166 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_6.mtx
+-rw-r--r--   0        0        0     1762 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_7.mtx
+-rw-r--r--   0        0        0     3638 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ4_json/GHZ4_in.mtx
+-rw-r--r--   0        0        0     1174 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/GHZ4_json/cssfproject.json
+-rw-r--r--   0        0        0     2593 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/SBiPa_json/cssfproject.json
+-rw-r--r--   0        0        0     1270 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/SBiPa_json/projection.mtx
+-rw-r--r--   0        0        0     1270 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/SBiPa_json/state.mtx
+-rw-r--r--   0        0        0     5139 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/__init__.py
+-rw-r--r--   0        0        0     1192 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/benchmark_32x32/5qubits_in.mtx
+-rw-r--r--   0        0        0     2957 2023-05-19 13:27:27.719206 cssfinder-0.7.0/cssfinder/examples/benchmark_32x32/cssfproject.py
+-rw-r--r--   0        0        0    54182 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/10_in.mtx
+-rw-r--r--   0        0        0     3693 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/cssfproject.py
+-rw-r--r--   0        0        0     4265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_0.mtx
+-rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_1.mtx
+-rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_2.mtx
+-rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_3.mtx
+-rw-r--r--   0        0        0     4297 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_4.mtx
+-rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_5.mtx
+-rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_6.mtx
+-rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_7.mtx
+-rw-r--r--   0        0        0     4265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_0.mtx
+-rw-r--r--   0        0        0   106596 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_1.mtx
+-rw-r--r--   0        0        0   106596 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_2.mtx
+-rw-r--r--   0        0        0   106596 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_3.mtx
+-rw-r--r--   0        0        0     4281 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_4.mtx
+-rw-r--r--   0        0        0   106596 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_5.mtx
+-rw-r--r--   0        0        0   106596 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_6.mtx
+-rw-r--r--   0        0        0   106596 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_7.mtx
+-rw-r--r--   0        0        0     4265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_0.mtx
+-rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_1.mtx
+-rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_2.mtx
+-rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_3.mtx
+-rw-r--r--   0        0        0     4297 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_4.mtx
+-rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_5.mtx
+-rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_6.mtx
+-rw-r--r--   0        0        0   108265 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_7.mtx
+-rw-r--r--   0        0        0    14212 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/interactive.py
+-rw-r--r--   0        0        0     1227 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/io/__init__.py
+-rw-r--r--   0        0        0     6003 2023-05-19 13:27:27.723206 cssfinder-0.7.0/cssfinder/io/gilbert_io.py
+-rw-r--r--   0        0        0     4182 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/io/matrix.py
+-rwxr-xr-x   0        0        0    12147 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/log.py
+-rw-r--r--   0        0        0     1666 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/__init__.py
+-rw-r--r--   0        0        0     1291 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/archive.py
+-rw-r--r--   0        0        0     2200 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/html.py
+-rw-r--r--   0        0        0     1845 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/json.py
+-rw-r--r--   0        0        0     4292 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/manager.py
+-rw-r--r--   0        0        0     9298 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/math.py
+-rw-r--r--   0        0        0     2937 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/pdf.py
+-rw-r--r--   0        0        0     8299 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/plotting.py
+-rw-r--r--   0        0        0     4889 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/renderer.py
+-rw-r--r--   0        0        0     1203 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/reports/txt.py
+-rw-r--r--   0        0        0     3947 2023-05-19 13:27:27.727206 cssfinder-0.7.0/cssfinder/templates/report.html.jinja2
+-rw-r--r--   0        0        0    17232 2023-05-19 13:27:27.731206 cssfinder-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    16452 1970-01-01 00:00:00.000000 cssfinder-0.7.0/PKG-INFO
```

### Comparing `cssfinder-0.6.0/LICENSE.md` & `cssfinder-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/__init__.py` & `cssfinder-0.7.0/cssfinder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 """CSSFinder (Closest Separable State Finder) is a package containing implementation of
 Gilbert algorithm for finding an upper bound on the Hilbert-Schmidt distance between a
 given state and the set of separable states.
 """
 
 from __future__ import annotations
 
-__version__ = "0.6.0"
+__version__ = "0.7.0"
```

### Comparing `cssfinder-0.6.0/cssfinder/__main__.py` & `cssfinder-0.7.0/cssfinder/__main__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/algorithm/__init__.py` & `cssfinder-0.7.0/cssfinder/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/algorithm/backend/__init__.py` & `cssfinder-0.7.0/cssfinder/algorithm/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/algorithm/backend/base.py` & `cssfinder-0.7.0/cssfinder/algorithm/backend/base.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/algorithm/backend/loader.py` & `cssfinder-0.7.0/cssfinder/algorithm/backend/loader.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/algorithm/gilbert.py` & `cssfinder-0.7.0/cssfinder/algorithm/gilbert.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/algorithm/mode_util.py` & `cssfinder-0.7.0/cssfinder/algorithm/mode_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,14 +86,17 @@
         """
         if mode == AlgoMode.FSnQd:
             return FSnQdUtil()
 
         if mode == AlgoMode.SBiPa:
             return SBiPaUtil()
 
+        if mode == AlgoMode.G3PaE3qD:
+            return G3PaE3qDUtil()
+
         msg = f"Unsupported mode {mode.name}"
         raise NotImplementedError(msg)
 
     def get_dimensions(self, state: npt.NDArray[np.complex128]) -> Dimensions:
         """Detect both system depth and system quantity.
 
         Parameters
@@ -108,15 +111,23 @@
 
         Raises
         ------
         ValueError
             When depth and quantity can't be determined.
 
         """
-        return self.detect_depth_and_quantity(len(state))
+        dim = self.detect_depth_and_quantity(len(state))
+
+        logging.debug(
+            "Deduced quantity %r and depth %r when given total size %r",
+            dim.depth,
+            dim.quantity,
+            len(state),
+        )
+        return dim
 
     @abstractmethod
     def detect_depth_and_quantity(self, total: int) -> Dimensions:
         """Detect both system depth and system quantity.
 
         Parameters
         ----------
@@ -162,20 +173,14 @@
             When depth and quantity can't be determined.
 
         """
         for depth in PRIMES:
             quantity = int(math.log(total, depth))
 
             if quantity == int(quantity):
-                logging.debug(
-                    "Deduced quantity %r and depth %r when given total size %r",
-                    depth,
-                    quantity,
-                    total,
-                )
                 return Dimensions(depth, quantity)
 
         reason = "prime number range exceeded"
         raise UndefinedSystemSizeError(reason)
 
 
 class SBiPaUtil(ModeUtil):
@@ -209,24 +214,51 @@
 
         if total_sqrt == floored_total_sqrt:
             return Dimensions(floored_total_sqrt, floored_total_sqrt)
 
         for depth in PRIMES:
             if total % depth == 0:
                 quantity = int(total / depth)
-                logging.debug(
-                    "Deduced quantity %r and depth %r when given total size %r",
-                    depth,
-                    quantity,
-                    total,
-                )
                 return Dimensions(depth, quantity)
 
         reason = "prime number range exceeded"
         raise UndefinedSystemSizeError(reason)
 
 
 class UndefinedSystemSizeError(ValueError):
     """Raised when it is not possible to determine system dimensions."""
 
     def __init__(self, reason: str) -> None:
         super().__init__(f"Couldn't determine size of system: {reason}.")
+
+
+class G3PaE3qDUtil(ModeUtil):
+    """G3PaE3q specific implementation of utilities eg.
+
+    shape deduction.
+
+    """
+
+    def detect_depth_and_quantity(self, total: int) -> Dimensions:
+        """Detect both system depth and system quantity.
+
+        Parameters
+        ----------
+        total : int
+            Dimension along one of axes. Matrix is expected to be square.
+
+        Returns
+        -------
+        Dimensions
+            System dimensions within dedicated container.
+
+        Raises
+        ------
+        ValueError
+            When depth and quantity can't be determined.
+
+        """
+        if round(total ** (1.0 / 3), 3) == round(total ** (1.0 / 3), 0):
+            return Dimensions(depth=int(total ** (1.0 / 3)), quantity=3)
+
+        reason = "prime number range exceeded"
+        raise UndefinedSystemSizeError(reason)
```

### Comparing `cssfinder-0.6.0/cssfinder/api.py` & `cssfinder-0.7.0/cssfinder/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 """Module contains high level API of cssfinder."""
 
 from __future__ import annotations
 
 import logging
 import os
+import traceback
 from concurrent.futures import ProcessPoolExecutor
 from dataclasses import dataclass
 from itertools import repeat
 from typing import TYPE_CHECKING, Iterable
 
 import psutil
 
@@ -112,15 +113,28 @@
 
     is_debug: bool
 
 
 def run_task(task: Task, options: TaskOptions) -> None:
     """Run task until completed."""
     try:
-        set_priority(os.getpid(), Priority.REALTIME, IoPriority.HIGH)
+        return _run_task(task, options)
+    except Exception as e:
+        logging.critical(
+            "Task %r failed due to exception:\n%s",
+            task.task_name,
+            str.join("", traceback.format_exception(type(e), e, e.__traceback__)),
+        )
+        raise
+
+
+def _run_task(task: Task, options: TaskOptions) -> None:
+    """Run task until completed."""
+    try:
+        set_priority(os.getpid(), Priority.ABOVE_NORMAL, IoPriority.HIGH)
     except (OSError, psutil.AccessDenied):
         logging.warning(
             "Failed to elevate process priority. It can negatively affect program "
             "performance if there are more programs running in background. "
             "To allow automated priority elevation run this program as super user. "
             "You can change priority manually for process PID %r.",
             os.getpid(),
@@ -282,25 +296,22 @@
 
 def create_report(
     project: CSSFProject, task: str, reports: list[ReportType]
 ) -> Iterable[Report]:
     """Create report for task selected by pattern from project object."""
     tasks = project.select_tasks([task])
 
-    if len(tasks) > 1:
-        matched_tasks_names = [t.task_name for t in tasks]
-        message = (
-            f"Pattern {task!r} matches more than one task ({len(tasks)}): "
-            f"{matched_tasks_names!r}"
-        )
-        raise AmbiguousTaskKeyError(message)
+    for task_object in tasks:
+        logging.info("Creating summary for task %s", task_object.task_name)
 
-    task_object, *_ = tasks
+        manager = ReportManager(project, task_object)
+        prepared_manager = manager.prepare()
 
-    manager = ReportManager(project, task_object)
-    prepared_manager = manager.prepare()
-    for report_type in reports:
-        yield prepared_manager.request_report(report_type)
+        for report_type in reports:
+            logging.info(
+                "Report for task %s of type %s", task_object.task_name, report_type.name
+            )
+            yield prepared_manager.request_report(report_type)
 
 
 class AmbiguousTaskKeyError(KeyError):
     """Raised during report creation when name pattern selects more than one task."""
```

### Comparing `cssfinder-0.6.0/cssfinder/base_model.py` & `cssfinder-0.7.0/cssfinder/base_model.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/cli.py` & `cssfinder-0.7.0/cssfinder/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 from typing import TYPE_CHECKING, Callable, Optional
 
 import click
 import pendulum
 import rich
 
 import cssfinder
+from cssfinder.api import create_report_from
 from cssfinder.log import enable_performance_logging
+from cssfinder.reports.renderer import ReportType
 
 if TYPE_CHECKING:
     from cssfinder import examples
 
 VERBOSITY_INFO: int = 2
 
 
@@ -87,37 +89,87 @@
  ██║     ╚════██║╚════██║██╔══╝  ██║██║╚██╗██║██║  ██║██╔══╝  ██╔══██╗
  ╚██████╗███████║███████║██║     ██║██║ ╚████║██████╔╝███████╗██║  ██║
   ╚═════╝╚══════╝╚══════╝╚═╝     ╚═╝╚═╝  ╚═══╝╚═════╝ ╚══════╝╚═╝  ╚═╝
 """,
         )
 
 
-def _is_path_needed_for_subcommand(
-    ctx: click.Context, param: click.Option, value: Optional[str]  # noqa: ARG001
-) -> str | None:
-    if ctx.invoked_subcommand in ["task"] and not value:
-        msg = "The path parameter is required for this subcommand."
-        raise click.BadParameter(msg)
-    return value
+@main.command(name="show-command-tree")
+@click.pass_context
+def tree(ctx: click.Context) -> None:
+    """Show the command tree of your CLI."""
+    root_cmd = _build_command_tree(ctx.find_root().command)
+    _print_tree(root_cmd)
 
 
-@main.group("project")
-@click.pass_context
-@click.option(
-    "--path",
-    "-p",
-    type=click.Path(exists=True, file_okay=True, dir_okay=True),
-    callback=_is_path_needed_for_subcommand,
-)
-def _project(ctx: click.Context, path: str) -> None:
-    """Group of commands for interaction with projects."""
-    ctx.obj.project_path = path
+class _CommandWrapper:
+    """Command tree printing based on `https://github.com/whwright/click-command-
+    tree`.
+    """
+
+    def __init__(
+        self,
+        command: Optional[click.Command] = None,
+        _children: Optional[list[click.Command]] = None,
+    ) -> None:
+        self.command = command
+        self.children: list[_CommandWrapper] = []
+
+    @property
+    def name(self) -> str:
+        assert self.command is not None
+        assert self.command.name is not None
+        return self.command.name
+
+    def __repr__(self) -> str:
+        return f"{{_CommandWrapper {self.name}}}"
+
+
+def _build_command_tree(click_command: click.Command) -> _CommandWrapper:
+    wrapper = _CommandWrapper(click_command)
+
+    if isinstance(click_command, click.core.Group):
+        for _, cmd in click_command.commands.items():
+            if not getattr(cmd, "hidden", False):
+                wrapper.children.append(_build_command_tree(cmd))
+
+    return wrapper
+
+
+def _print_tree(
+    command: _CommandWrapper,
+    depth: int = 0,
+    *,
+    is_last_item: bool = False,
+    is_last_parent: bool = False,
+) -> None:
+    if depth == 0:
+        prefix = ""
+        tree_item = ""
+    else:
+        prefix = "    " if is_last_parent else "│   "
+        tree_item = "└── " if is_last_item else "├── "
 
+    doc = command.command.__doc__
+    first_line = " - " + doc.split("\n")[0] if doc else ""
 
-@_project.command("new")
+    line = f"{prefix * (depth - 1) + tree_item + command.name:<30}{first_line}"
+
+    click.echo(line)
+
+    for i, child in enumerate(sorted(command.children, key=lambda x: x.name)):
+        _print_tree(
+            child,
+            depth=(depth + 1),
+            is_last_item=(i == (len(command.children) - 1)),
+            is_last_parent=is_last_item,
+        )
+
+
+@main.command("create-new-project")
 @click.option("--author", default=None, help="Author metadata field value.")
 @click.option("--email", default=None, help="Email metadata field value.")
 @click.option("--name", default=None, help="Name metadata field value.")
 @click.option("--description", default=None, help="Description metadata field value.")
 @click.option("--project-version", default=None, help="Version metadata field value.")
 def _project_new(
     author: Optional[str],
@@ -128,25 +180,63 @@
 ) -> None:
     """Create new project."""
     from cssfinder.interactive import create_new_project
 
     create_new_project(author, email, name, description, project_version)
 
 
-@_project.group("task")
-def _task() -> None:
-    """Group of commands to operate on tasks."""
+@main.group("project")
+@click.pass_context
+def _project(ctx: click.Context) -> None:
+    """Group of commands for interaction with projects."""
+    ctx.obj.project_path = Path.cwd().as_posix()
+
+
+@_project.command("inspect")
+@click.pass_obj
+def _inspect(ctx: Ctx) -> None:
+    """Load and display project."""
+    from cssfinder.cssfproject import CSSFProject
+
+    if ctx.project_path is None:
+        reason = "ctx.project_path shall not be None."
+        raise RuntimeError(reason)
+
+    project = CSSFProject.load_project(ctx.project_path)
+    rich.print_json(project.json(indent=4))
+
+
+@_project.command("inspect-output")
+@click.argument("task_pattern")
+@click.pass_obj
+def _inspect_output(ctx: Ctx, task_pattern: str) -> None:
+    """Load and display project."""
+    import json
+
+    from cssfinder.cssfproject import CSSFProject
+
+    if ctx.project_path is None:
+        reason = "ctx.project_path shall not be None."
+        raise RuntimeError(reason)
 
+    project = CSSFProject.load_project(ctx.project_path)
+    tasks = project.select_tasks([task_pattern])
+    for i, task in enumerate(tasks):
+        corrections = json.loads(
+            task.output_corrections_file.read_text(encoding="utf-8")
+        )
+        print("First correction: ", corrections[0])
+        print("Middle correction:", corrections[len(corrections) // 2 - 1])
+        print("Last correction:  ", corrections[-1])
 
-@_task.group("add")
-def _add() -> None:
-    """Command for adding new tasks."""
+        if i < (len(tasks) - 1):
+            print("-" * 70)
 
 
-@_add.command("gilbert")
+@_project.command("add-gilbert-task")
 @click.pass_obj
 @click.option("--name", default=None, help="Name for the task.")
 @click.option("--mode", default=None, help="Algorithm mode.")
 @click.option(
     "--backend-name",
     default=None,
     help="Name of backend. Use `cssfinder backend list` to show installed backends.",
@@ -196,15 +286,15 @@
     help="List of lists of files containing symmetries matrices as valid JSON literal.",
 )
 @click.option(
     "--projection",
     default=None,
     help="Path to file containing projection matrix.",
 )
-def _gilbert(  # noqa: PLR0913
+def _add_gilbert_task(  # noqa: PLR0913
     ctx: Ctx,
     name: Optional[str],
     mode: Optional[str],
     backend_name: Optional[str],
     precision: Optional[str],
     state: Optional[str],
     depth: Optional[str],
@@ -248,15 +338,15 @@
             symmetries or "[]",
             projection,
             derive,
         ),
     )
 
 
-@_task.command("run")
+@_project.command("run-tasks")
 @click.option(
     "--match",
     "-m",
     "match_",
     multiple=True,
     help="Use to specify names of tasks to run. When omitted, all tasks are executed.",
 )
@@ -272,15 +362,15 @@
     "-p",
     type=int,
     default=-1,
     help="Limit maximal number of tasks executed in parallel. Note that this never "
     "changes execution scheme, thus code won't be executed in main thread.",
 )
 @click.pass_obj
-def _run(
+def _run_tasks(
     ctx: Ctx, match_: list[str] | None, *, force_sequential: bool, max_parallel: int
 ) -> None:
     """Run tasks from the project."""
     from cssfinder.algorithm.gilbert import SaveCorrectionsHookError, SaveStateHookError
     from cssfinder.api import run_project_from
     from cssfinder.cssfproject import (
         InvalidCSSFProjectContentError,
@@ -323,15 +413,15 @@
 
     except SaveCorrectionsHookError:
         _log_exit(304_000)
 
     raise SystemExit(0)
 
 
-@_task.command("report")
+@_project.command("create-task-report")
 @click.argument(
     "task",
 )
 @click.option(
     "--html",
     "--no-html",
     is_flag=True,
@@ -342,23 +432,32 @@
     "--pdf",
     "--no-pdf",
     is_flag=True,
     default=False,
     help="Include PDF report.",
 )
 @click.option(
+    "--json",
+    "--no-json",
+    is_flag=True,
+    default=False,
+    help="Include JSON report.",
+)
+@click.option(
     "--open",
     "--no-open",
     "open_",
     is_flag=True,
     default=False,
     help="Automatically open report in web browser.",
 )
 @click.pass_obj
-def _task_report(ctx: Ctx, task: str, *, html: bool, pdf: bool, open_: bool) -> None:
+def _create_task_report(
+    ctx: Ctx, task: str, *, html: bool, pdf: bool, json: bool, open_: bool
+) -> None:
     """Create short report for task.
 
     TASK - name pattern matching exactly one task, for which report should be created.
 
     """
     from cssfinder.api import AmbiguousTaskKeyError, create_report_from
     from cssfinder.reports.renderer import ReportType
@@ -369,14 +468,17 @@
 
     if html:
         include_report_types.append(ReportType.HTML)
 
     if pdf:
         include_report_types.append(ReportType.PDF)
 
+    if json:
+        include_report_types.append(ReportType.JSON)
+
     if len(include_report_types) == 0:
         logging.critical(
             "No report type was selected therefore nothing will be calculated, exiting."
         )
         raise SystemExit(0)
 
     try:
@@ -388,38 +490,48 @@
 
     except AmbiguousTaskKeyError as exc:
         logging.critical(exc.args[0])
         raise SystemExit(304_00) from exc
 
 
 def _log_exit(code: int) -> None:
-    logging.exception("Exit with code code.")
+    logging.exception("Exit with code %d.", code)
     raise SystemExit(code)
 
 
-@main.group("backend")
-def _backend() -> None:
-    """Group of commands for inspecting available backends."""
+@_project.command("create-json-summary")
+@click.argument("task_pattern")
+@click.pass_obj
+def _create_json_summary(ctx: Ctx, task_pattern: str) -> None:
+    """Load and display project."""
+    import json
+
+    assert ctx.project_path is not None
+    output = []
 
+    for report in create_report_from(
+        ctx.project_path, task=task_pattern, reports=[ReportType.JSON]
+    ):
+        content = json.loads(report.content)
+        output.append(content)
 
-@_backend.command("list")
-def _backend_list() -> None:
+    dest = Path(ctx.project_path) / "output" / "summary.json"
+    dest.write_text(json.dumps(output, indent=4))
+
+
+@main.command("list-backends")
+def _list_backends() -> None:
     """List available backends."""
     from cssfinder.algorithm.backend.loader import Loader
 
     rich.get_console().print(Loader.new().get_rich_table())
 
 
-@main.group("examples")
-def _examples() -> None:
-    """Group of commands for accessing bundled examples."""
-
-
-@_examples.command("list")
-def _examples_list() -> None:
+@main.command("list-examples")
+def _list_examples() -> None:
     """Show list of all available example projects."""
     from cssfinder import examples
 
     console = rich.get_console()
     table = examples.Example.get_info_table()
     console.print()
     console.print(table)
@@ -439,27 +551,17 @@
             raise click.BadParameter(msg)
 
         return value
 
     return _
 
 
-@_examples.command("clone")
-@click.option(
-    "--sha",
-    default=None,
-    help="SHA of example. Mutually exclusive with `--name`.",
-    expose_value=True,
-)
-@click.option(
-    "--name",
-    default=None,
-    help="Name of example. Mutually exclusive with `--sha`.",
-    expose_value=True,
-    callback=validate_mutually_exclusive("name", "sha"),
+@main.command("clone-example")
+@click.argument(
+    "sha_or_name",
 )
 @click.option(
     "-o",
     "--out",
     default=None,
     help="Path to destination directory, where project folder should be placed.",
 )
@@ -481,30 +583,34 @@
     "-e",
     "--explorer",
     "do_open_explorer",
     is_flag=True,
     help="When set, automatically open new explorer window in example directory.",
 )
 def _examples_clone(
-    sha: Optional[str],
-    name: Optional[str],
+    sha_or_name: str,
     out: Optional[str],
     *,
     force_overwrite: bool,
     do_open_terminal: bool,
     do_open_explorer: bool,
 ) -> None:
-    """Clone one of examples to specific location."""
+    """Clone one of examples to specific location.
+
+    SHA_OR_NAME - or name of example. to select by sha, use 'sha:000000', otherwise this
+                    parameter will be considered a example name.
+
+    """
     from cssfinder.crossplatform import open_file_explorer, open_terminal
     from cssfinder.cssfproject import ProjectFileNotFoundError
     from cssfinder.enums import ExitCode
 
     destination = Path.cwd() if out is None else Path(out).expanduser().resolve()
 
-    example = _select_example(sha, name)
+    example = _select_example(sha_or_name)
     try:
         project = example.get_project()
     except ProjectFileNotFoundError as exc:
         logging.debug(traceback.format_exc())
         logging.critical(
             "Sorry but example is broken. (%s)", exc.__class__.__qualname__
         )
@@ -516,14 +622,15 @@
     )
 
     destination_project_folder = _get_validated_destination(
         destination, example, force_overwrite=force_overwrite
     )
     try:
         example.clone(destination)
+        rich.print(f"Cloned example to {destination.as_posix()!r}")
 
     except FileNotFoundError as exc:
         logging.critical(str(exc))
         raise SystemExit(ExitCode.PROJECT_NOT_FOUND) from exc
 
     if do_open_explorer:
         open_file_explorer(destination_project_folder)
@@ -556,30 +663,27 @@
                 example.folder_name,
             )
             raise SystemExit(ExitCode.EXAMPLE_DESTINATION_ALREADY_EXISTS)
 
     return destination_project_folder
 
 
-def _select_example(sha: Optional[str], name: Optional[str]) -> examples.Example:
+def _select_example(sha_or_name: str) -> examples.Example:
     from cssfinder import examples
     from cssfinder.enums import ExitCode
 
-    if name is not None:
+    if sha_or_name.startswith("sha:"):
+        sha_or_name = sha_or_name[4:]
         try:
-            example = examples.Example.select_by_name(name)
+            example = examples.Example.select_by_sha256(sha_or_name)
         except examples.ExampleNotFoundError as exc:
             logging.critical("%s", exc)
-            raise SystemExit(ExitCode.EXAMPLE_WITH_NAME_NOT_FOUND) from exc
+            raise SystemExit(ExitCode.EXAMPLE_WITH_SHA_NOT_FOUND) from exc
 
-    elif sha is not None:
+    else:
         try:
-            example = examples.Example.select_by_sha256(sha)
+            example = examples.Example.select_by_name(sha_or_name)
         except examples.ExampleNotFoundError as exc:
             logging.critical("%s", exc)
-            raise SystemExit(ExitCode.EXAMPLE_WITH_SHA_NOT_FOUND) from exc
-
-    else:
-        logging.critical("Neither `--name` not `--sha` given, no example was selected.")
-        raise SystemExit(ExitCode.EXAMPLE_SHA_NOR_NAME_GIVEN)
+            raise SystemExit(ExitCode.EXAMPLE_WITH_NAME_NOT_FOUND) from exc
 
     return example
```

### Comparing `cssfinder-0.6.0/cssfinder/constants.py` & `cssfinder-0.7.0/cssfinder/constants.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/crossplatform.py` & `cssfinder-0.7.0/cssfinder/crossplatform.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/cssfproject.py` & `cssfinder-0.7.0/cssfinder/cssfproject.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/enums.py` & `cssfinder-0.7.0/cssfinder/enums.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/5qubits_json/5qubits_in.mtx` & `cssfinder-0.7.0/cssfinder/examples/5qubits_json/5qubits_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/5qubits_json/cssfproject.json` & `cssfinder-0.7.0/cssfinder/examples/5qubits_json/cssfproject.json`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/5qubits_py/5qubits_in.mtx` & `cssfinder-0.7.0/cssfinder/examples/5qubits_py/5qubits_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/5qubits_py/cssfproject.py` & `cssfinder-0.7.0/cssfinder/examples/5qubits_py/cssfproject.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/GHZ3_json/GHZ3_in.mtx` & `cssfinder-0.7.0/cssfinder/examples/GHZ3_json/GHZ3_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/GHZ3_json/cssfproject.json` & `cssfinder-0.7.0/cssfinder/examples/GHZ3_json/cssfproject.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'tasks'": "{'test_g3pae3qd': OrderedDict([('gilbert', OrderedDict([('mode', 'G3PaE3qD'), "*

 * *            "('backend', OrderedDict([('name', 'numpy'), ('precision', 'single')])), ('runtime', "*

 * *            "OrderedDict([('visibility', 0.4), ('max_epochs', 1000), ('iters_per_epoch', 1000), "*

 * *            "('max_corrections', 1000)])), ('state', OrderedDict([('file', "*

 * *            "'{project.project_directory}/GHZ3_in.mtx'), ('depth', None), ('quantity', None)])), "*

 * *            "('resources', OrderedDict([('symm […]*

```diff
@@ -41,11 +41,35 @@
                 },
                 "state": {
                     "depth": null,
                     "file": "{project.project_directory}/GHZ3_in.mtx",
                     "quantity": null
                 }
             }
+        },
+        "test_g3pae3qd": {
+            "gilbert": {
+                "backend": {
+                    "name": "numpy",
+                    "precision": "single"
+                },
+                "mode": "G3PaE3qD",
+                "resources": {
+                    "projection": null,
+                    "symmetries": null
+                },
+                "runtime": {
+                    "iters_per_epoch": 1000,
+                    "max_corrections": 1000,
+                    "max_epochs": 1000,
+                    "visibility": 0.4
+                },
+                "state": {
+                    "depth": null,
+                    "file": "{project.project_directory}/GHZ3_in.mtx",
+                    "quantity": null
+                }
+            }
         }
     },
     "version": "1.0.0"
 }
```

### Comparing `cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_1.mtx` & `cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_1.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_3.mtx` & `cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_3.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_5.mtx` & `cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_5.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_7.mtx` & `cssfinder-0.7.0/cssfinder/examples/GHZ3_json/symmetries/GHZ3_sym_1_7.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/GHZ4_json/GHZ4_in.mtx` & `cssfinder-0.7.0/cssfinder/examples/GHZ4_json/GHZ4_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/GHZ4_json/cssfproject.json` & `cssfinder-0.7.0/cssfinder/examples/GHZ4_json/cssfproject.json`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/SBiPa_json/cssfproject.json` & `cssfinder-0.7.0/cssfinder/examples/SBiPa_json/cssfproject.json`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/SBiPa_json/projection.mtx` & `cssfinder-0.7.0/cssfinder/examples/SBiPa_json/projection.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/SBiPa_json/state.mtx` & `cssfinder-0.7.0/cssfinder/examples/SBiPa_json/state.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/__init__.py` & `cssfinder-0.7.0/cssfinder/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_32x32/5qubits_in.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_32x32/5qubits_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_32x32/cssfproject.py` & `cssfinder-0.7.0/cssfinder/examples/benchmark_32x32/cssfproject.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/10_in.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/10_in.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/cssfproject.py` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/cssfproject.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_0.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_0.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_1.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_1.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_2.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_2.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_3.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_3.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_4.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_4.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_5.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_5.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_6.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_6.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_7.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_0_7.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_0.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_0.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_1.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_1.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_2.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_2.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_3.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_3.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_4.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_4.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_5.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_5.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_6.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_6.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_7.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_1_7.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_0.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_0.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_1.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_1.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_2.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_2.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_3.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_3.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_4.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_4.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_5.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_5.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_6.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_6.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_7.mtx` & `cssfinder-0.7.0/cssfinder/examples/benchmark_64x64/symmetries/sym_sym_2_7.mtx`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/interactive.py` & `cssfinder-0.7.0/cssfinder/interactive.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/io/__init__.py` & `cssfinder-0.7.0/cssfinder/io/__init__.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/io/gilbert_io.py` & `cssfinder-0.7.0/cssfinder/io/gilbert_io.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/io/matrix.py` & `cssfinder-0.7.0/cssfinder/io/matrix.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/log.py` & `cssfinder-0.7.0/cssfinder/log.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/reports/__init__.py` & `cssfinder-0.7.0/cssfinder/reports/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,13 +20,15 @@
 
 
 """Report generation tools."""
 
 from __future__ import annotations
 
 from cssfinder.reports.html import HTMLRenderer
+from cssfinder.reports.json import JSONRenderer
 from cssfinder.reports.manager import PreparedReportManager
 from cssfinder.reports.pdf import PDFRenderer
 from cssfinder.reports.renderer import ReportType
 
 PreparedReportManager.register_renderer(HTMLRenderer, ReportType.HTML)
 PreparedReportManager.register_renderer(PDFRenderer, ReportType.PDF)
+PreparedReportManager.register_renderer(JSONRenderer, ReportType.JSON)
```

### Comparing `cssfinder-0.6.0/cssfinder/reports/archive.py` & `cssfinder-0.7.0/cssfinder/reports/archive.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/reports/html.py` & `cssfinder-0.7.0/cssfinder/reports/html.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/reports/manager.py` & `cssfinder-0.7.0/cssfinder/reports/manager.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/reports/math.py` & `cssfinder-0.7.0/cssfinder/reports/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     get_correction(x: npt.NDArray[np.float64]) -> np.float64:
         Returns the correction values for a given input array `x`.
     find(data: npt.NDArray[np.float64]) -> 'SlopeProperties':
         Finds the slope properties for a given dataset `data`.
 
     """
 
+    correction_count: int
     optimum: np.float64
     r_value: np.float64
     aa1: np.float64
     bb1: np.float64
 
     def get_correction_count(self, x: np.float64) -> np.float64:
         """Return the correction values for a given input array `x`.
@@ -104,22 +105,23 @@
             of the input data.
 
         """
         iteration_index: npt.NDArray[np.float64] = data[:, 0]
         correction_index: npt.NDArray[np.float64] = data[:, 1]
         correction_value: npt.NDArray[np.float64] = data[int(2 * len(data) / 3) :, 2]
 
+        correction_count = len(data)
         optimum = find_correction_optimum(data[:, 2])
 
         r_value = R(correction_value, optimum)
 
         aa1 = trend(iteration_index, correction_index)
         bb1 = np.exp(offset(iteration_index, correction_index))
 
-        return cls(optimum, r_value, aa1, bb1)
+        return cls(correction_count, optimum, r_value, aa1, bb1)
 
     def save_to(self, dest: Path) -> None:
         """Save properties to file."""
         with dest.open("w", encoding="utf-8") as file:
             json.dump(asdict(self), file)
```

### Comparing `cssfinder-0.6.0/cssfinder/reports/pdf.py` & `cssfinder-0.7.0/cssfinder/reports/pdf.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/reports/plotting.py` & `cssfinder-0.7.0/cssfinder/reports/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,17 +139,17 @@
         axes.plot(
             self.corrections[["index"]],
             1 / (self.corrections[["value"]] - self.slope_props.optimum),
         )
         axes.grid(visible=True)
 
         axes.set_xlabel("Correction index")
-        axes.set_ylabel("Correction offsetted inverse value")
+        axes.set_ylabel("Inverse correction value with offset")
 
-        axes.set_title("Distance offsetted inverse decay")
+        axes.set_title("Inverse distance decay with offset")
 
         return Plot(axes)
 
     def plot_iteration(self, axes: Optional[plt.Axes] = None) -> Plot:
         """Create a plot of iteration linear corrections.
 
         Returns
```

### Comparing `cssfinder-0.6.0/cssfinder/reports/renderer.py` & `cssfinder-0.7.0/cssfinder/reports/renderer.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 class ReportType(Enum):
     """Possible report types."""
 
     HTML = "html"
     PDF = "pdf"
     ARCHIVE = "zip"
     TXT = "txt"
+    JSON = "json"
 
     def get_file_name(self) -> str:
         """Return default file name for specific type of report."""
         return f"report.{self.value}"
 
 
 class Renderer(ABC):
@@ -96,16 +97,20 @@
         )
 
     @property
     def math_props(self) -> OrderedDict:
         """Return mathematical properties."""
         return OrderedDict(
             {
+                "Correction count": f"{self.props.correction_count}",
                 "Hilbert-Schmidt distance": f"{self.props.optimum:.3f}",
                 "Sample correlation coefficient": f"{self.props.r_value:.3f}",
+                "Offset (optimum)": f"{self.props.optimum:.3f}",
+                "Trend (aa1)": f"{self.props.aa1:.3f}",
+                "Exp Offset (bb1)": f"{self.props.bb1:.3f}",
             }
         )
 
 
 @dataclass
 class Report:
     """Container for rendered report."""
```

### Comparing `cssfinder-0.6.0/cssfinder/reports/txt.py` & `cssfinder-0.7.0/cssfinder/reports/txt.py`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/cssfinder/templates/report.html.jinja2` & `cssfinder-0.7.0/cssfinder/templates/report.html.jinja2`

 * *Files identical despite different names*

### Comparing `cssfinder-0.6.0/pyproject.toml` & `cssfinder-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry] # ANCHOR: tool.poetry
 name = "cssfinder"
-version = "0.6.0"
+version = "0.7.0"
 description = "Tool for Hilbert-Schmidt distance calculation with Gilbert algorithm."
 authors = [
     "Krzysztof Wiśniewski <argmaster.world@gmail.com>",
     "Marcin Wieśniak <marcin.wiesniak@ug.edu.pl>",
 ]
 repository = "https://github.com/argmaster/CSSFinder"
 readme = "README.md"
@@ -22,16 +22,16 @@
 jsonref = "^1.1.0"
 matplotlib = "^3.7.0"
 pandas = "^1.5.3"
 weasyprint = "^58.1"
 psutil = "^5.9.4"
 pytermgui = "^7.3.0"
 jinja2 = "^3.1.2"
-cssfinder-backend-numpy = { version = ">=0.3.0", optional = true }
-cssfinder-backend-rust = { version = ">=0.1.0", optional = true }
+cssfinder-backend-numpy = { version = ">=0.5.0", optional = true }
+cssfinder-backend-rust = { version = ">=0.1.1", optional = true }
 filelock = "^3.12.0"
 
 [tool.poetry.group.dev.dependencies] # ANCHOR: tool.poetry.dev-dependencies
 black = ">=22.12,<24.0"
 isort = "^5.11.4"
 docformatter = { extras = ["tomli"], version = "==1.5.1" }
 pytest = "^7.2.0"
@@ -43,15 +43,15 @@
 typing-extensions = "^4.4.0"
 snakeviz = "^2.1.1"
 poethepoet = ">=0.18.1,<0.20.0"
 poetry = "^1.3.2"
 jinja2 = "^3.1.2"
 ruff = ">=0.0.254"
 ipykernel = "^6.21.3"
-cssfinder-backend-numpy = ">=0.3.0"
+cssfinder-backend-numpy = ">=0.5.0"
 
 [tool.poetry.extras]
 backend-numpy = ["cssfinder-backend-numpy"]
 backend-rust = ["cssfinder-backend-rust"]
 
 [tool.poetry.scripts]
 cssfinder = "cssfinder.cli:main"
```

### Comparing `cssfinder-0.6.0/PKG-INFO` & `cssfinder-0.7.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,44 @@
-Metadata-Version: 2.1
-Name: cssfinder
-Version: 0.6.0
-Summary: Tool for Hilbert-Schmidt distance calculation with Gilbert algorithm.
-Home-page: https://github.com/argmaster/CSSFinder
-Author: Krzysztof Wiśniewski
-Author-email: argmaster.world@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: backend-numpy
-Provides-Extra: backend-rust
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: cssfinder-backend-numpy (>=0.3.0) ; extra == "backend-numpy"
-Requires-Dist: cssfinder-backend-rust (>=0.1.0) ; extra == "backend-rust"
-Requires-Dist: filelock (>=3.12.0,<4.0.0)
-Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: jsonref (>=1.1.0,<2.0.0)
-Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
-Requires-Dist: numba (>=0.56.4,<0.57.0)
-Requires-Dist: numpy (>=1.23.0,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: pendulum (>=2.1.2,<3.0.0)
-Requires-Dist: psutil (>=5.9.4,<6.0.0)
-Requires-Dist: pydantic[email] (>=1.10.5,<2.0.0)
-Requires-Dist: pytermgui (>=7.3.0,<8.0.0)
-Requires-Dist: rich (>=13.3.1,<14.0.0)
-Requires-Dist: scipy (>=1.9.3,<2.0.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
-Requires-Dist: weasyprint (>=58.1,<59.0)
-Project-URL: Repository, https://github.com/argmaster/CSSFinder
-Description-Content-Type: text/markdown
+# CSSFinder - Closest Separable State Finder
 
-# CSSFinder
+CSSFinder is a software designed to find the closest separable state (CSS) for
+a given quantum state. This helps in quantifying entanglement and classifying
+quantum states as entangled or separable.
+
+This software has been designed in a modular way. This is manifested by the
+separation of the main part, which contains the user interface and modularity
+support elements, from the algorithm implementation. The main part was written
+in Python and uses the mechanisms of Python modules. Since it is possible to
+craft shared libraries in such a way that Python imports them as native modules
+any compiled language can be used to create highly optimized implementations of
+desired algorithms. Such implementations are called backends and they use
+minimalistic interface to interact with main part of the program.
+
+In parallel with the development of this main part, two implementations of the
+algorithm were created:
+
+- `cssfinder_backend_numpy` - based on Python NumPy library implementing highly
+  optimized multidimensional arrays and linear algebra.
+- `cssfinder_backend_rust` - based on Rust ndarray crate which is an equivalent
+  of NumPy from Rust language world.
 
-Closest separable state finder.
+Development of those two implementations allowed us to better understand limits
+of what can and what can not become faster.
 
 ## Installing
 
 To install CSSFinder from PyPI, use `pip` in terminal:
 
 ```
 pip install cssfinder
 ```
 
-Because CSSFinder is a modular tool, you will have to also install a `backend`
-package, which contains concrete implementation of algorithms. Simples way is
-to just install `numpy` or `rust` extras set:
+You will have to also install a `backend` package, which contains concrete
+implementation of algorithms. Simples way is to just install `numpy` or `rust`
+extras set:
 
 ```
 pip install cssfinder[numpy]
 ```
 
 ```
 pip install cssfinder[rust]
@@ -129,14 +115,90 @@
 seconds and few minutes, depending on your hardware.
 
 Result of calculations can be inspected in `output/` directory in project
 folder (`5qubits_json/`).
 
 ![image](https://user-images.githubusercontent.com/56170852/233218942-ac47a923-21f7-4b3a-af02-7a7961360abc.png)
 
+## Workflow
+
+In CSSFinder, computations are described in special `cssfproject.*` files
+within dedicated directories. Such directory with all files within it is called
+a `project`. Project must contain either `cssfproject.json` or `cssfproject.py`
+files which describe what should be done. `Json` file is purely declarative,
+but with `$ref` support, while python scripts (`cssfproject.py`) allow for
+dynamic creation of tasks. Tasks are smallest possible unit of work which can
+be scheduled for execution by CSSFinder. They can be automatically executed in
+parallel with automatic queues to speed up calculations.
+
+### Project with static (json) project
+
+During this tutorial it is preferable to create an empty directory and do
+everything from now on within this directory. Let's call this directory
+`tutorial1` and we will create it in home directory (`~`).
+
+```
+~/tutorial1/
+```
+
+Start by creating new directory, `project1`, in there. This directory will
+contain all project files needed for calculations.
+
+Fastest way to start with CSSFinder is to use static `json` files, therefore
+this is what we are going to use now.
+
+Create `cssfproject.json` file in `~/tutorial1/project1` directory.
+
+We will use our example `state.mtx` file, but you can use Your own real data.
+
+Create `state.mtx` file within `~/tutorial1/project1` directory and fill it
+with following data:
+
+```
+%%MatrixMarket matrix array real symmetric
+%Created with the Wolfram Language : www.wolfram.com
+8 8
+   2.5000000000000000E-01
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+  -2.5000000000000000E-01
+   0.0000000000000000E+00
+  -2.5000000000000000E-01
+  -2.5000000000000000E-01
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   2.5000000000000000E-01
+   0.0000000000000000E+00
+   2.5000000000000000E-01
+   2.5000000000000000E-01
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+   2.5000000000000000E-01
+   2.5000000000000000E-01
+   0.0000000000000000E+00
+   2.5000000000000000E-01
+   0.0000000000000000E+00
+   0.0000000000000000E+00
+```
+
 ## Development
 
 This project uses `Python` programming language and requires at least python
 `3.8` for development and distribution. Development dependencies
 [`poetry`](https://pypi.org/project/poetry/) for managing dependencies and
 distribution building. It is necessary to perform any operations in development
 environment.
@@ -187,35 +249,35 @@
 
 ```
 poe build
 ```
 
 ![poe_build](https://user-images.githubusercontent.com/56170852/223251363-61fc4d00-68ad-429c-9fbb-8ab7f4712451.png)
 
-This will create `dist/` directory with `cssfinder-0.6.0` or alike inside.
+This will create `dist/` directory with `cssfinder-0.7.0` or alike inside.
 
 Wheel file can be installed with
 
 ```
-pip install ./dist/cssfinder-0.6.0
+pip install ./dist/cssfinder-0.7.0
 ```
 
 What you expect is
 
 ```
-Successfully installed cssfinder-0.6.0
+Successfully installed cssfinder-0.7.0
 ```
 
 or rather something like
 
 ```
-Successfully installed click-8.1.3 contourpy-1.0.7 cssfinder-0.6.0 cycler-0.11.0 dnspython-2.3.0 email-validator-1.3.1 fonttools-4.39.0 idna-3.4 jsonref-1.1.0 kiwisolver-1.4.4 llvmlite-0.39.1 markdown-it-py-2.2.0 matplotlib-3.7.1 mdurl-0.1.2 numba-0.56.4 numpy-1.23.5 packaging-23.0 pandas-1.5.3 pendulum-2.1.2 pillow-9.4.0 pydantic-1.10.5 pygments-2.14.0 pyparsing-3.0.9 python-dateutil-2.8.2 pytz-2022.7.1 pytzdata-2020.1 rich-13.3.2 scipy-1.10.1 six-1.16.0 typing-extensions-4.5.0
+Successfully installed click-8.1.3 contourpy-1.0.7 cssfinder-0.7.0 cycler-0.11.0 dnspython-2.3.0 email-validator-1.3.1 fonttools-4.39.0 idna-3.4 jsonref-1.1.0 kiwisolver-1.4.4 llvmlite-0.39.1 markdown-it-py-2.2.0 matplotlib-3.7.1 mdurl-0.1.2 numba-0.56.4 numpy-1.23.5 packaging-23.0 pandas-1.5.3 pendulum-2.1.2 pillow-9.4.0 pydantic-1.10.5 pygments-2.14.0 pyparsing-3.0.9 python-dateutil-2.8.2 pytz-2022.7.1 pytzdata-2020.1 rich-13.3.2 scipy-1.10.1 six-1.16.0 typing-extensions-4.5.0
 ```
 
-But `cssfinder-0.6.0` should be included in this list.
+But `cssfinder-0.7.0` should be included in this list.
 
 ## Code quality
 
 To ensure that all code follow same style guidelines and code quality rules,
 multiple static analysis tools are used. For simplicity, all of them are
 configured as `pre-commit` ([learn about pre-commit](https://pre-commit.com/))
 hooks. Most of them however are listed as development dependencies.
@@ -367,8 +429,7 @@
 ##### Options
 
 - `--html`, `--no-html`: include or exclude an HTML report in the generated
   report.
 - `--pdf`, `--no-pdf`: include or exclude a PDF report in the generated report.
 
 - `--open`, `--no-open`: automatically open report in web browser.
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

