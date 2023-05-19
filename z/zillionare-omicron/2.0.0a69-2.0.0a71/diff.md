# Comparing `tmp/zillionare_omicron-2.0.0a69.tar.gz` & `tmp/zillionare_omicron-2.0.0a71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillionare_omicron-2.0.0a69.tar", max compression
+gzip compressed data, was "zillionare_omicron-2.0.0a71.tar", max compression
```

## Comparing `zillionare_omicron-2.0.0a69.tar` & `zillionare_omicron-2.0.0a71.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0      112 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a69/AUTHORS.md
--rw-r--r--   0        0        0     1726 2023-05-09 07:42:36.089641 zillionare_omicron-2.0.0a69/HISTORY.md
--rw-r--r--   0        0        0     1068 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a69/LICENSE
--rw-r--r--   0        0        0     1331 2023-05-07 03:30:41.208098 zillionare_omicron-2.0.0a69/README.md
--rw-r--r--   0        0        0   503846 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/_static/Omicron_Windows10.docx
--rw-r--r--   0        0        0     5620 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a69/docs/_static/jetbrains-variant-3.svg
--rw-r--r--   0        0        0       84 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/dal/flux.md
--rw-r--r--   0        0        0      110 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/dal/influxclient.md
--rw-r--r--   0        0        0      189 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/dal/serialize.md
--rw-r--r--   0        0        0     5772 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/metrics.md
--rw-r--r--   0        0        0      203 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/omicron.md
--rw-r--r--   0        0        0       73 2023-05-08 07:55:54.700078 zillionare_omicron-2.0.0a69/docs/api/plotting/candlestick.md
--rw-r--r--   0        0        0       69 2023-05-08 07:55:45.740005 zillionare_omicron-2.0.0a69/docs/api/plotting/metrics.md
--rw-r--r--   0        0        0       68 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/security.md
--rw-r--r--   0        0        0       65 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/stock.md
--rw-r--r--   0        0        0       21 2023-05-07 03:32:19.736871 zillionare_omicron-2.0.0a69/docs/api/strategy.md
--rw-r--r--   0        0        0       58 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/talib.md
--rw-r--r--   0        0        0       57 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/api/timeframe.md
--rw-r--r--   0        0        0       66 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a69/docs/api/triggers.md
--rw-r--r--   0        0        0      907 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a69/docs/css/extra.css
--rw-r--r--   0        0        0     1778 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/developer.md
--rw-r--r--   0        0        0       43 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a69/docs/history.md
--rw-r--r--   0        0        0       42 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a69/docs/index.md
--rw-r--r--   0        0        0     1820 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/installation.md
--rw-r--r--   0        0        0     9823 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/docs/usage.md
--rw-r--r--   0        0        0      920 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/omicron/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a69/omicron/config/__init__.py
--rw-r--r--   0        0        0    56389 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/config/calendar.json
--rw-r--r--   0        0        0      441 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/config/defaults.yaml
--rw-r--r--   0        0        0      378 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/config/dev.yaml
--rw-r--r--   0        0        0     1334 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/config/schema.py
--rw-r--r--   0        0        0      816 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a69/omicron/config/sql/v0.6.sql
--rw-r--r--   0        0        0     2785 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/config/sql/v1.0.sql
--rw-r--r--   0        0        0       46 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a69/omicron/core/__init__.py
--rw-r--r--   0        0        0      140 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/core/constants.py
--rw-r--r--   0        0        0     1095 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/core/errors.py
--rw-r--r--   0        0        0       46 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/core/events.py
--rw-r--r--   0        0        0     6517 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/core/triggers.py
--rw-r--r--   0        0        0       71 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/dal/__init__.py
--rw-r--r--   0        0        0     3215 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/dal/cache.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/dal/influx/__init__.py
--rw-r--r--   0        0        0      370 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/dal/influx/errors.py
--rw-r--r--   0        0        0      996 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a69/omicron/dal/influx/escape.py
--rw-r--r--   0        0        0    19097 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a69/omicron/dal/influx/flux.py
--rw-r--r--   0        0        0    16805 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a69/omicron/dal/influx/influxclient.py
--rw-r--r--   0        0        0    27708 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a69/omicron/dal/influx/serialize.py
--rw-r--r--   0        0        0       78 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a69/omicron/extensions/__init__.py
--rw-r--r--   0        0        0      656 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a69/omicron/extensions/decimals.py
--rw-r--r--   0        0        0    15929 2023-05-01 02:32:25.512887 zillionare_omicron-2.0.0a69/omicron/extensions/np.py
--rw-r--r--   0        0        0      492 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a69/omicron/models/__init__.py
--rw-r--r--   0        0        0     7867 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a69/omicron/models/board.py
--rw-r--r--   0        0        0    26127 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/models/security.py
--rw-r--r--   0        0        0    53741 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/models/stock.py
--rw-r--r--   0        0        0    41959 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/models/timeframe.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/notify/__init__.py
--rw-r--r--   0        0        0     5472 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/notify/dingtalk.py
--rw-r--r--   0        0        0     6006 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/notify/mail.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/notify/tts.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/plotting/__init__.py
--rw-r--r--   0        0        0    16523 2023-05-08 08:53:56.981283 zillionare_omicron-2.0.0a69/omicron/plotting/candlestick.py
--rw-r--r--   0        0        0     8474 2023-05-08 08:53:20.740774 zillionare_omicron-2.0.0a69/omicron/plotting/metrics.py
--rw-r--r--   0        0        0        0 2023-05-07 01:07:54.376952 zillionare_omicron-2.0.0a69/omicron/strategy/__init__.py
--rw-r--r--   0        0        0     9053 2023-05-09 07:41:37.353693 zillionare_omicron-2.0.0a69/omicron/strategy/base.py
--rw-r--r--   0        0        0     1099 2023-05-07 02:09:33.855184 zillionare_omicron-2.0.0a69/omicron/strategy/sma.py
--rw-r--r--   0        0        0      114 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a69/omicron/talib/__init__.py
--rw-r--r--   0        0        0     9958 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a69/omicron/talib/core.py
--rw-r--r--   0        0        0    23141 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a69/omicron/talib/morph.py
--rwxr-xr-x   0        0        0     3391 2023-05-09 07:42:01.057668 zillionare_omicron-2.0.0a69/pyproject.toml
--rw-r--r--   0        0        0     5556 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a69/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a69/tests/core/__init__.py
--rw-r--r--   0        0        0      297 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a69/tests/core/test_errors.py
--rw-r--r--   0        0        0     3615 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a69/tests/core/test_triggers.py
--rw-r--r--   0        0        0     1024 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/core/test_types.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/dal/__init__.py
--rw-r--r--   0        0        0      622 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/dal/influx/__init__.py
--rw-r--r--   0        0        0     1177 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/dal/influx/test_escape.py
--rw-r--r--   0        0        0     8531 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/dal/influx/test_flux.py
--rw-r--r--   0        0        0    14284 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/dal/influx/test_influxclient.py
--rw-r--r--   0        0        0    15710 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/dal/influx/test_serialize.py
--rw-r--r--   0        0        0     1253 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.15m.csv
--rw-r--r--   0        0        0      118 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.1M.csv
--rw-r--r--   0        0        0      188 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.1d.csv
--rw-r--r--   0        0        0    22206 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.1m.csv
--rw-r--r--   0        0        0      115 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.1w.csv
--rw-r--r--   0        0        0      654 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.30m.csv
--rw-r--r--   0        0        0     3633 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.5m.csv
--rw-r--r--   0        0        0      352 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.60m.csv
--rw-r--r--   0        0        0  1059606 2023-05-07 02:32:26.029160 zillionare_omicron-2.0.0a69/tests/data/000001.XSHG.1m.csv
--rw-r--r--   0        0        0     8089 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.1d.csv
--rw-r--r--   0        0        0    22419 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.1m.csv
--rw-r--r--   0        0        0     7166 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.1w.csv
--rw-r--r--   0        0        0     8096 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.30m.csv
--rw-r--r--   0        0        0     7585 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.1d.csv
--rw-r--r--   0        0        0    20344 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.1m.csv
--rw-r--r--   0        0        0     6443 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.1w.csv
--rw-r--r--   0        0        0     7688 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.30m.csv
--rw-r--r--   0        0        0     4206 2023-05-07 02:31:54.553073 zillionare_omicron-2.0.0a69/tests/data/600000.XSHG.1d.csv
--rw-r--r--   0        0        0     1145 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/README.md
--rw-r--r--   0        0        0     2191 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a69/tests/data/bars_1d.pkl
--rw-r--r--   0        0        0   408697 2023-01-24 12:41:24.943079 zillionare_omicron-2.0.0a69/tests/data/bars_1m.pkl
--rw-r--r--   0        0        0      713 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/data/limits.csv
--rw-r--r--   0        0        0   164066 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/data/stock_bars_flux_query.txt
--rw-r--r--   0        0        0     6315 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/data/test.jpg
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/extensions/__init__.py
--rw-r--r--   0        0        0      594 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/extensions/test_decimals.py
--rw-r--r--   0        0        0     9864 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/extensions/test_np.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/models/__init__.py
--rw-r--r--   0        0        0     6802 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/models/test_board.py
--rw-r--r--   0        0        0    11161 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a69/tests/models/test_security.py
--rw-r--r--   0        0        0    68822 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/models/test_stock.py
--rw-r--r--   0        0        0    36351 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/models/test_timeframe.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/notify/__init__.py
--rw-r--r--   0        0        0      823 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/notify/test_dingtalk.py
--rw-r--r--   0        0        0     2686 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/notify/test_mail.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/performance/influx/__init__.py
--rw-r--r--   0        0        0     3317 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/performance/influx/end2end.py
--rw-r--r--   0        0        0     4197 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/performance/influx/serialize.py
--rw-r--r--   0        0        0      294 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/performance/readme.md
--rw-r--r--   0        0        0      406 2023-01-19 03:32:37.466696 zillionare_omicron-2.0.0a69/tests/pyrightconfig.json
--rw-r--r--   0        0        0        0 2023-05-07 02:10:22.915444 zillionare_omicron-2.0.0a69/tests/strategy/__init__.py
--rw-r--r--   0        0        0     1517 2023-05-07 03:14:15.795948 zillionare_omicron-2.0.0a69/tests/strategy/test_strategy.py
--rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/talib/__init__.py
--rw-r--r--   0        0        0     2917 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/talib/test_core.py
--rw-r--r--   0        0        0    37991 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a69/tests/talib/test_morph.py
--rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 zillionare_omicron-2.0.0a69/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-01-24 12:41:24.903079 zillionare_omicron-2.0.0a71/AUTHORS.md
+-rw-r--r--   0        0        0     1726 2023-05-09 07:42:36.089641 zillionare_omicron-2.0.0a71/HISTORY.md
+-rw-r--r--   0        0        0     1068 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a71/LICENSE
+-rw-r--r--   0        0        0     1331 2023-05-07 03:30:41.208098 zillionare_omicron-2.0.0a71/README.md
+-rw-r--r--   0        0        0   503846 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/docs/_static/Omicron_Windows10.docx
+-rw-r--r--   0        0        0     5620 2023-01-19 03:32:37.450696 zillionare_omicron-2.0.0a71/docs/_static/jetbrains-variant-3.svg
+-rw-r--r--   0        0        0       84 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/docs/api/dal/flux.md
+-rw-r--r--   0        0        0      110 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/docs/api/dal/influxclient.md
+-rw-r--r--   0        0        0      189 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/docs/api/dal/serialize.md
+-rw-r--r--   0        0        0     5772 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/docs/api/metrics.md
+-rw-r--r--   0        0        0      203 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/docs/api/omicron.md
+-rw-r--r--   0        0        0       73 2023-05-08 07:55:54.700078 zillionare_omicron-2.0.0a71/docs/api/plotting/candlestick.md
+-rw-r--r--   0        0        0       69 2023-05-08 07:55:45.740005 zillionare_omicron-2.0.0a71/docs/api/plotting/metrics.md
+-rw-r--r--   0        0        0       68 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/docs/api/security.md
+-rw-r--r--   0        0        0       65 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/docs/api/stock.md
+-rw-r--r--   0        0        0       21 2023-05-07 03:32:19.736871 zillionare_omicron-2.0.0a71/docs/api/strategy.md
+-rw-r--r--   0        0        0       58 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/docs/api/talib.md
+-rw-r--r--   0        0        0       57 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/docs/api/timeframe.md
+-rw-r--r--   0        0        0       66 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a71/docs/api/triggers.md
+-rw-r--r--   0        0        0      907 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a71/docs/css/extra.css
+-rw-r--r--   0        0        0     1778 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/docs/developer.md
+-rw-r--r--   0        0        0       43 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a71/docs/history.md
+-rw-r--r--   0        0        0       42 2023-01-19 03:32:37.454697 zillionare_omicron-2.0.0a71/docs/index.md
+-rw-r--r--   0        0        0     1820 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/docs/installation.md
+-rw-r--r--   0        0        0     9823 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/docs/usage.md
+-rw-r--r--   0        0        0      920 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/omicron/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.911079 zillionare_omicron-2.0.0a71/omicron/config/__init__.py
+-rw-r--r--   0        0        0    56389 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a71/omicron/config/calendar.json
+-rw-r--r--   0        0        0      441 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a71/omicron/config/defaults.yaml
+-rw-r--r--   0        0        0      378 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a71/omicron/config/dev.yaml
+-rw-r--r--   0        0        0     1334 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a71/omicron/config/schema.py
+-rw-r--r--   0        0        0      816 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a71/omicron/config/sql/v0.6.sql
+-rw-r--r--   0        0        0     2785 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a71/omicron/config/sql/v1.0.sql
+-rw-r--r--   0        0        0       46 2023-01-19 03:32:37.458696 zillionare_omicron-2.0.0a71/omicron/core/__init__.py
+-rw-r--r--   0        0        0      140 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a71/omicron/core/constants.py
+-rw-r--r--   0        0        0     1095 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a71/omicron/core/errors.py
+-rw-r--r--   0        0        0       46 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a71/omicron/core/events.py
+-rw-r--r--   0        0        0     6517 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a71/omicron/core/triggers.py
+-rw-r--r--   0        0        0       71 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a71/omicron/dal/__init__.py
+-rw-r--r--   0        0        0     3215 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a71/omicron/dal/cache.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a71/omicron/dal/influx/__init__.py
+-rw-r--r--   0        0        0      370 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a71/omicron/dal/influx/errors.py
+-rw-r--r--   0        0        0      996 2023-01-24 12:41:24.915079 zillionare_omicron-2.0.0a71/omicron/dal/influx/escape.py
+-rw-r--r--   0        0        0    19097 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a71/omicron/dal/influx/flux.py
+-rw-r--r--   0        0        0    16805 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a71/omicron/dal/influx/influxclient.py
+-rw-r--r--   0        0        0    27708 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a71/omicron/dal/influx/serialize.py
+-rw-r--r--   0        0        0       78 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a71/omicron/extensions/__init__.py
+-rw-r--r--   0        0        0      656 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a71/omicron/extensions/decimals.py
+-rw-r--r--   0        0        0    15929 2023-05-01 02:32:25.512887 zillionare_omicron-2.0.0a71/omicron/extensions/np.py
+-rw-r--r--   0        0        0      492 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a71/omicron/models/__init__.py
+-rw-r--r--   0        0        0     7867 2023-01-24 12:41:24.919079 zillionare_omicron-2.0.0a71/omicron/models/board.py
+-rw-r--r--   0        0        0    26127 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a71/omicron/models/security.py
+-rw-r--r--   0        0        0    53741 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a71/omicron/models/stock.py
+-rw-r--r--   0        0        0    41959 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a71/omicron/models/timeframe.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a71/omicron/notify/__init__.py
+-rw-r--r--   0        0        0     5472 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a71/omicron/notify/dingtalk.py
+-rw-r--r--   0        0        0     6006 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a71/omicron/notify/mail.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a71/omicron/notify/tts.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a71/omicron/plotting/__init__.py
+-rw-r--r--   0        0        0    16941 2023-05-09 12:33:23.495223 zillionare_omicron-2.0.0a71/omicron/plotting/candlestick.py
+-rw-r--r--   0        0        0     9469 2023-05-19 14:47:28.042965 zillionare_omicron-2.0.0a71/omicron/plotting/metrics.py
+-rw-r--r--   0        0        0        0 2023-05-07 01:07:54.376952 zillionare_omicron-2.0.0a71/omicron/strategy/__init__.py
+-rw-r--r--   0        0        0     9141 2023-05-15 09:03:58.321265 zillionare_omicron-2.0.0a71/omicron/strategy/base.py
+-rw-r--r--   0        0        0     1099 2023-05-07 02:09:33.855184 zillionare_omicron-2.0.0a71/omicron/strategy/sma.py
+-rw-r--r--   0        0        0      114 2023-01-24 12:41:24.923079 zillionare_omicron-2.0.0a71/omicron/talib/__init__.py
+-rw-r--r--   0        0        0     9958 2023-01-24 12:41:24.927079 zillionare_omicron-2.0.0a71/omicron/talib/core.py
+-rw-r--r--   0        0        0    23170 2023-05-09 09:20:57.088066 zillionare_omicron-2.0.0a71/omicron/talib/morph.py
+-rwxr-xr-x   0        0        0     3391 2023-05-19 14:49:05.979491 zillionare_omicron-2.0.0a71/pyproject.toml
+-rw-r--r--   0        0        0     5556 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a71/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a71/tests/core/__init__.py
+-rw-r--r--   0        0        0      297 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a71/tests/core/test_errors.py
+-rw-r--r--   0        0        0     3615 2023-01-24 12:41:24.931079 zillionare_omicron-2.0.0a71/tests/core/test_triggers.py
+-rw-r--r--   0        0        0     1024 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/core/test_types.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/dal/__init__.py
+-rw-r--r--   0        0        0      622 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/dal/influx/__init__.py
+-rw-r--r--   0        0        0     1177 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/dal/influx/test_escape.py
+-rw-r--r--   0        0        0     8531 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/dal/influx/test_flux.py
+-rw-r--r--   0        0        0    14284 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/dal/influx/test_influxclient.py
+-rw-r--r--   0        0        0    15710 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/dal/influx/test_serialize.py
+-rw-r--r--   0        0        0     1253 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/data/000001.XSHE.15m.csv
+-rw-r--r--   0        0        0      118 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/data/000001.XSHE.1M.csv
+-rw-r--r--   0        0        0      188 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/data/000001.XSHE.1d.csv
+-rw-r--r--   0        0        0    22206 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/data/000001.XSHE.1m.csv
+-rw-r--r--   0        0        0      115 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/data/000001.XSHE.1w.csv
+-rw-r--r--   0        0        0      654 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/data/000001.XSHE.30m.csv
+-rw-r--r--   0        0        0     3633 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/data/000001.XSHE.5m.csv
+-rw-r--r--   0        0        0      352 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/data/000001.XSHE.60m.csv
+-rw-r--r--   0        0        0  1059606 2023-05-07 02:32:26.029160 zillionare_omicron-2.0.0a71/tests/data/000001.XSHG.1m.csv
+-rw-r--r--   0        0        0     8089 2023-01-24 12:41:24.935079 zillionare_omicron-2.0.0a71/tests/data/000002.XSHE.1d.csv
+-rw-r--r--   0        0        0    22419 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a71/tests/data/000002.XSHE.1m.csv
+-rw-r--r--   0        0        0     7166 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a71/tests/data/000002.XSHE.1w.csv
+-rw-r--r--   0        0        0     8096 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a71/tests/data/000002.XSHE.30m.csv
+-rw-r--r--   0        0        0     7585 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a71/tests/data/000004.XSHE.1d.csv
+-rw-r--r--   0        0        0    20344 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a71/tests/data/000004.XSHE.1m.csv
+-rw-r--r--   0        0        0     6443 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a71/tests/data/000004.XSHE.1w.csv
+-rw-r--r--   0        0        0     7688 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a71/tests/data/000004.XSHE.30m.csv
+-rw-r--r--   0        0        0     4206 2023-05-07 02:31:54.553073 zillionare_omicron-2.0.0a71/tests/data/600000.XSHG.1d.csv
+-rw-r--r--   0        0        0     1145 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a71/tests/data/README.md
+-rw-r--r--   0        0        0     2191 2023-01-24 12:41:24.939079 zillionare_omicron-2.0.0a71/tests/data/bars_1d.pkl
+-rw-r--r--   0        0        0   408697 2023-01-24 12:41:24.943079 zillionare_omicron-2.0.0a71/tests/data/bars_1m.pkl
+-rw-r--r--   0        0        0      713 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a71/tests/data/limits.csv
+-rw-r--r--   0        0        0   164066 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a71/tests/data/stock_bars_flux_query.txt
+-rw-r--r--   0        0        0     6315 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a71/tests/data/test.jpg
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a71/tests/extensions/__init__.py
+-rw-r--r--   0        0        0      594 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a71/tests/extensions/test_decimals.py
+-rw-r--r--   0        0        0     9864 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a71/tests/extensions/test_np.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a71/tests/models/__init__.py
+-rw-r--r--   0        0        0     6802 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a71/tests/models/test_board.py
+-rw-r--r--   0        0        0    11161 2023-01-24 12:41:24.947079 zillionare_omicron-2.0.0a71/tests/models/test_security.py
+-rw-r--r--   0        0        0    68822 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a71/tests/models/test_stock.py
+-rw-r--r--   0        0        0    36351 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a71/tests/models/test_timeframe.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a71/tests/notify/__init__.py
+-rw-r--r--   0        0        0      823 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a71/tests/notify/test_dingtalk.py
+-rw-r--r--   0        0        0     2686 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a71/tests/notify/test_mail.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a71/tests/performance/influx/__init__.py
+-rw-r--r--   0        0        0     3317 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a71/tests/performance/influx/end2end.py
+-rw-r--r--   0        0        0     4197 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a71/tests/performance/influx/serialize.py
+-rw-r--r--   0        0        0      294 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a71/tests/performance/readme.md
+-rw-r--r--   0        0        0      406 2023-01-19 03:32:37.466696 zillionare_omicron-2.0.0a71/tests/pyrightconfig.json
+-rw-r--r--   0        0        0        0 2023-05-07 02:10:22.915444 zillionare_omicron-2.0.0a71/tests/strategy/__init__.py
+-rw-r--r--   0        0        0     1517 2023-05-07 03:14:15.795948 zillionare_omicron-2.0.0a71/tests/strategy/test_strategy.py
+-rw-r--r--   0        0        0        0 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a71/tests/talib/__init__.py
+-rw-r--r--   0        0        0     2917 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a71/tests/talib/test_core.py
+-rw-r--r--   0        0        0    37991 2023-01-24 12:41:24.951079 zillionare_omicron-2.0.0a71/tests/talib/test_morph.py
+-rw-r--r--   0        0        0     4334 1970-01-01 00:00:00.000000 zillionare_omicron-2.0.0a71/PKG-INFO
```

### Comparing `zillionare_omicron-2.0.0a69/HISTORY.md` & `zillionare_omicron-2.0.0a71/HISTORY.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/LICENSE` & `zillionare_omicron-2.0.0a71/LICENSE`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/README.md` & `zillionare_omicron-2.0.0a71/README.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/docs/_static/Omicron_Windows10.docx` & `zillionare_omicron-2.0.0a71/docs/_static/Omicron_Windows10.docx`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/docs/_static/jetbrains-variant-3.svg` & `zillionare_omicron-2.0.0a71/docs/_static/jetbrains-variant-3.svg`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/docs/api/metrics.md` & `zillionare_omicron-2.0.0a71/docs/api/metrics.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/docs/css/extra.css` & `zillionare_omicron-2.0.0a71/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/docs/developer.md` & `zillionare_omicron-2.0.0a71/docs/developer.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/docs/installation.md` & `zillionare_omicron-2.0.0a71/docs/installation.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/docs/usage.md` & `zillionare_omicron-2.0.0a71/docs/usage.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/__init__.py` & `zillionare_omicron-2.0.0a71/omicron/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/config/calendar.json` & `zillionare_omicron-2.0.0a71/omicron/config/calendar.json`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/config/schema.py` & `zillionare_omicron-2.0.0a71/omicron/config/schema.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/config/sql/v0.6.sql` & `zillionare_omicron-2.0.0a71/omicron/config/sql/v0.6.sql`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/config/sql/v1.0.sql` & `zillionare_omicron-2.0.0a71/omicron/config/sql/v1.0.sql`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/core/errors.py` & `zillionare_omicron-2.0.0a71/omicron/core/errors.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/core/triggers.py` & `zillionare_omicron-2.0.0a71/omicron/core/triggers.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/dal/cache.py` & `zillionare_omicron-2.0.0a71/omicron/dal/cache.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/dal/influx/escape.py` & `zillionare_omicron-2.0.0a71/omicron/dal/influx/escape.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/dal/influx/flux.py` & `zillionare_omicron-2.0.0a71/omicron/dal/influx/flux.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/dal/influx/influxclient.py` & `zillionare_omicron-2.0.0a71/omicron/dal/influx/influxclient.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/dal/influx/serialize.py` & `zillionare_omicron-2.0.0a71/omicron/dal/influx/serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/extensions/decimals.py` & `zillionare_omicron-2.0.0a71/omicron/extensions/decimals.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/extensions/np.py` & `zillionare_omicron-2.0.0a71/omicron/extensions/np.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/models/board.py` & `zillionare_omicron-2.0.0a71/omicron/models/board.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/models/security.py` & `zillionare_omicron-2.0.0a71/omicron/models/security.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/models/stock.py` & `zillionare_omicron-2.0.0a71/omicron/models/stock.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/models/timeframe.py` & `zillionare_omicron-2.0.0a71/omicron/models/timeframe.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/notify/dingtalk.py` & `zillionare_omicron-2.0.0a71/omicron/notify/dingtalk.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/notify/mail.py` & `zillionare_omicron-2.0.0a71/omicron/notify/mail.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/plotting/candlestick.py` & `zillionare_omicron-2.0.0a71/omicron/plotting/candlestick.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 cs.mark_bbox()
 cs.plot()
 ```
 ![](https://images.jieyu.ai/images/2023/05/20230508164848.png)
 
 """
 from collections import defaultdict
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 import arrow
 import numpy as np
 import plotly.graph_objects as go
 import talib
 from numpy._typing import NDArray
 from plotly.subplots import make_subplots
@@ -396,15 +396,17 @@
             name="backtest",
             hovertext=hover,
             textfont=labels_color,
         )
 
         self.main_traces["bs"] = trace
 
-    def mark_peaks_and_valleys(self, up_thres: float = None, down_thres: float = None):
+    def mark_peaks_and_valleys(
+        self, up_thres: Optional[float] = None, down_thres: Optional[float] = None
+    ):
         """在K线图上标注峰谷点
 
         Args:
             up_thres : 用来检测峰谷时使用的阈值，参见[omicron.talib.morph.peaks_and_valleys][]
             down_thres : 用来检测峰谷时使用的阈值，参见[omicron.talib.morph.peaks_and_valleys][]
 
         """
@@ -482,46 +484,59 @@
             trace = go.Bar(
                 x=self.ticks,
                 y=self.bars["volume"],
                 showlegend=False,
                 marker={"color": colors},
             )
         elif indicator == "rsi":
-            rsi = talib.RSI(self.bars["close"].astype(np.float64))
+            rsi = talib.RSI(self.bars["close"].astype(np.float64))  # type: ignore
             trace = go.Scatter(x=self.ticks, y=rsi, showlegend=False)
         elif indicator == "bbands":
             self._remove_ma()
             for name, ind in zip(
                 ["bbands-high", "bbands-mean", "bbands-low"],
-                talib.BBANDS(self.bars["close"].astype(np.float64)),
+                talib.BBANDS(self.bars["close"].astype(np.float64)),  # type: ignore
             ):
                 trace = go.Scatter(x=self.ticks, y=ind, showlegend=True, name=name)
                 self.main_traces[name] = trace
 
             return
         else:
             raise ValueError(f"{indicator} not supported")
 
         self.ind_traces[indicator] = trace
 
-    def add_marks(self, x: List[int]):
+    def add_marks(
+        self,
+        x: List[int],
+        y: List[float],
+        name: str,
+        marker: str = "cross",
+        color: Optional[str] = None,
+    ):
         """向k线图中增加标记点"""
         trace = go.Scatter(
             x=self.ticks[x],
-            y=self.bars["high"][x] * 1.02,
+            y=y,
             mode="markers",
-            marker_symbol="cross",
+            marker_symbol=marker,
+            marker_color=color,
+            name=name,
         )
-        self.main_traces["marks"] = trace
+        self.main_traces[name] = trace
 
     def plot(self):
         """绘制图表"""
         fig = self.figure
+        ymin = np.min(self.bars["low"])
+        ymax = np.max(self.bars["high"])
 
+        ylim = [ymin * 0.95, ymax * 1.05]
+        fig.update_layout(yaxis=dict(range=ylim))
         fig.show()
 
 
 def plot_candlestick(
-    bars: np.ndarray, ma_groups: List[int], title: str = None, **kwargs
+    bars: np.ndarray, ma_groups: List[int], title: Optional[str] = None, **kwargs
 ):
     cs = Candlestick(bars, ma_groups, title=title)
     cs.plot()
```

### Comparing `zillionare_omicron-2.0.0a69/omicron/plotting/metrics.py` & `zillionare_omicron-2.0.0a71/omicron/plotting/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ![](https://images.jieyu.ai/images/2023/05/20230508160012.png)
 
 """
 import datetime
 import logging
 from collections import defaultdict
 from copy import deepcopy
-from typing import List, Union
+from typing import List, Optional, Union
 
 import arrow
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 from coretypes import BarsArray, Frame, FrameType
 from numpy.typing import NDArray
@@ -32,15 +32,17 @@
 from omicron.models.security import Security
 from omicron.models.stock import Stock
 
 logger = logging.getLogger(__name__)
 
 
 class MetricsGraph:
-    def __init__(self, bills: dict, metrics: dict):
+    def __init__(
+        self, bills: dict, metrics: dict, baseline_code: Optional[str] = "399300.XSHE"
+    ):
         self.metrics = metrics
         self.trades = bills["trades"]
         self.positions = bills["positions"]
         self.start = arrow.get(bills["assets"][0][0]).date()
         self.end = arrow.get(bills["assets"][-1][0]).date()
 
         self.frames = [
@@ -52,14 +54,16 @@
         self.ticks = self._format_tick(self.frames)
 
         self.assets = pd.DataFrame(bills["assets"], columns=["frame", "assets"])[
             "assets"
         ].to_numpy()
         self.nv = self.assets / self.assets[0]
 
+        self.baseline_code = baseline_code or "399300.XSHE"
+
     def _fill_missing_prices(self, bars: BarsArray, frames: Union[List, NDArray]):
         """将bars中缺失值采用其前值替换
 
         当baseline为个股时，可能存在停牌的情况，这样导致由此计算的参考收益无法与回测的资产收益对齐，因此需要进行调整。
 
         出于这个目的，本函数只返回处理后的收盘价。
 
@@ -128,22 +132,20 @@
             "annual_return": "{:.2%}",
             "volatility": "{:.2%}",
             "sortino": "{:.2f}",
             "calmar": "{:.2f}",
         }
 
         metrics = deepcopy(self.metrics)
-        baseline = metrics["baseline"]
+        baseline = metrics["baseline"] or {}
         del metrics["baseline"]
 
-        if "code" in baseline:
-            baseline_name = await Security.alias(baseline["code"])
-            del baseline["code"]
-        else:
-            baseline_name = "基准"
+        baseline_name = (
+            await Security.alias(self.baseline_code) if self.baseline_code else "基准"
+        )
 
         metrics_formatted = []
         for k in metric_names.keys():
             if metrics.get(k):
                 metrics_formatted.append(metric_formatter[k].format(metrics.get(k)))
             else:
                 metrics_formatted.append("-")
@@ -155,30 +157,27 @@
             else:
                 baseline_formatted.append("-")
 
         return go.Table(
             header=dict(values=["指标名", "策略", baseline_name]),
             cells=dict(
                 values=[
-                    [metric_names[k] for k in metrics],
+                    [v for _,v in metric_names.items()],
                     metrics_formatted,
                     baseline_formatted,
                 ],
                 font_size=10,
             ),
         )
 
     async def _trade_info_trace(self):
         """构建hover text 序列"""
-        X = []
-        Y = []
-        data = []
-
         # convert trades into hover_info
-        merged = defaultdict(list)
+        buys = defaultdict(list)
+        sells = defaultdict(list)
         for _, trade in self.trades.items():
             trade_date = arrow.get(trade["time"]).date()
 
             ipos = self._frame2pos.get(trade_date)
             if ipos is None:
                 logger.warning(
                     "date  %s in trade record not in backtest range", trade_date
@@ -188,32 +187,64 @@
             name = await Security.alias(trade["security"])
             price = trade["price"]
             side = trade["order_side"]
             filled = trade["filled"]
 
             trade_text = f"{side}:{name} {filled/100:.0f}手 价格:{price:.02f} 成交额{filled * price/10000:.1f}万"
 
-            merged[trade_date].append(trade_text)
+            if side == "卖出":
+                sells[trade_date].append(trade_text)
+            elif side in ("买入", "分红配股"):
+                buys[trade_date].append(trade_text)
+
+        X_buy, Y_buy, data_buy = [], [], []
+        X_sell, Y_sell, data_sell = [], [], []
+
+        for dt, text in buys.items():
+            ipos = self._frame2pos.get(dt)
+            Y_buy.append(self.nv[ipos])
+            X_buy.append(self._format_tick(dt))
+
+            asset = self.assets[ipos]
+            hover = f"资产:{asset/10000:.1f}万<br>{'<br>'.join(text)}"
+            data_buy.append(hover)
 
-        for dt, text in merged.items():
+        trace_buy = go.Scatter(
+            x=X_buy,
+            y=Y_buy,
+            mode="markers",
+            text=data_buy,
+            name="买入成交",
+            marker = dict(color='red', symbol='triangle-up'),
+        )
+
+        for dt, text in sells.items():
             ipos = self._frame2pos.get(dt)
-            Y.append(self.nv[ipos])
-            X.append(self._format_tick(dt))
+            Y_sell.append(self.nv[ipos])
+            X_sell.append(self._format_tick(dt))
 
             asset = self.assets[ipos]
             hover = f"资产:{asset/10000:.1f}万<br>{'<br>'.join(text)}"
-            data.append(hover)
+            data_sell.append(hover)
+
+        trace_sell = go.Scatter(
+            x=X_sell,
+            y=Y_sell,
+            mode="markers",
+            text=data_sell,
+            name="卖出成交",
+            marker = dict(color='green', symbol='triangle-down'),
+        )
 
-        trace = go.Scatter(x=X, y=Y, mode="markers", text=data, name="交易详情")
-        return trace
+        return trace_buy, trace_sell
 
-    async def plot(self, baseline_code: str = "399300.XSHE"):
+    async def plot(self):
         """绘制资产曲线及回测指标图"""
         n = len(self.assets)
-        bars = await Stock.get_bars(baseline_code, n, FrameType.DAY, self.end)
+        bars = await Stock.get_bars(self.baseline_code, n, FrameType.DAY, self.end)
 
         baseline_prices = self._fill_missing_prices(bars, self.frames)
         baseline_prices /= baseline_prices[0]
 
         fig = make_subplots(
             rows=1,
             cols=2,
@@ -239,13 +270,13 @@
         fig.add_trace(baseline_trace, row=1, col=1)
 
         nv_trace = go.Scatter(
             y=self.nv, x=self.ticks, mode="lines", name="策略净值", showlegend=True
         )
         fig.add_trace(nv_trace, row=1, col=1)
 
-        trade_info_trace = await self._trade_info_trace()
-        fig.add_trace(trade_info_trace, row=1, col=1)
+        for trace in await self._trade_info_trace():
+            fig.add_trace(trace, row=1, col=1)
 
         fig.update_xaxes(type="category", tickangle=45, nticks=len(self.ticks) // 5)
         fig.update_layout(margin=dict(l=20, r=20, t=50, b=50), width=1040, height=435)
         fig.show()
```

### Comparing `zillionare_omicron-2.0.0a69/omicron/strategy/base.py` & `zillionare_omicron-2.0.0a71/omicron/strategy/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,22 +125,21 @@
         self.metrics = self.broker.metrics(baseline=self._baseline)
 
     @property
     def cash(self):
         """返回当前可用现金"""
         return self.broker.available_money
 
-    @property
-    def positions(self):
+    def positions(self, dt: Optional[datetime.date] = None):
         """返回当前持仓"""
-        return self.broker.positions
+        return self.broker.positions(dt)
 
-    def available_shares(self, sec: str):
+    def available_shares(self, sec: str, dt: Optional[Frame] = None):
         """返回给定股票当前可售股数。"""
-        return self.broker.available_shares(sec)
+        return self.broker.available_shares(sec, dt)
 
     async def buy(
         self,
         sec: str,
         price: Optional[float] = None,
         vol: Optional[int] = None,
         money: Optional[float] = None,
@@ -222,9 +221,9 @@
         """
         raise NotImplementedError
 
     async def plot_metrics(self):
         if self.bills is None or self.metrics is None:
             raise ValueError("Please run `start_backtest` first.")
 
-        mg = MetricsGraph(self.bills, self.metrics)
+        mg = MetricsGraph(self.bills, self.metrics, baseline_code=self._baseline)
         await mg.plot()
```

### Comparing `zillionare_omicron-2.0.0a69/omicron/strategy/sma.py` & `zillionare_omicron-2.0.0a71/omicron/strategy/sma.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/talib/core.py` & `zillionare_omicron-2.0.0a71/omicron/talib/core.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/omicron/talib/morph.py` & `zillionare_omicron-2.0.0a71/omicron/talib/morph.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,17 @@
 class BreakoutFlag(IntEnum):
     UP = 1
     DOWN = -1
     NONE = 0
 
 
 def peaks_and_valleys(
-    ts: np.ndarray, up_thresh: float = None, down_thresh: float = None
+    ts: np.ndarray,
+    up_thresh: Optional[float] = None,
+    down_thresh: Optional[float] = None,
 ) -> np.ndarray:
     """寻找ts中的波峰和波谷，返回数组指示在该位置上是否为波峰或波谷。如果为1，则为波峰；如果为-1，则为波谷。
 
     本函数直接使用了zigzag中的peak_valley_pivots. 有很多方法可以实现本功能，比如scipy.signals.find_peaks_cwt, peak_valley_pivots等。本函数更适合金融时间序列，并且使用了cython加速。
 
     Args:
         ts (np.ndarray): 时间序列
```

### Comparing `zillionare_omicron-2.0.0a69/pyproject.toml` & `zillionare_omicron-2.0.0a71/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.poetry.dev-dependencies]
 [tool.poetry]
 name = "zillionare-omicron"
 packages = [
     {include = "omicron"}
 ]
-version = "2.0.0a69"
+version = "2.0.0a71"
 description = "Core Library for Zillionare"
 authors = ["jieyu <code@jieyu.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://zillionare-omicron.readthedocs.io"
 repository = "https://github.com/zillionare/omicron"
 documentation = "https://zillionare-omicron.readthedocs.io"
```

### Comparing `zillionare_omicron-2.0.0a69/tests/__init__.py` & `zillionare_omicron-2.0.0a71/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/core/test_triggers.py` & `zillionare_omicron-2.0.0a71/tests/core/test_triggers.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/core/test_types.py` & `zillionare_omicron-2.0.0a71/tests/core/test_types.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/dal/influx/__init__.py` & `zillionare_omicron-2.0.0a71/tests/dal/influx/__init__.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/dal/influx/test_escape.py` & `zillionare_omicron-2.0.0a71/tests/dal/influx/test_escape.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/dal/influx/test_flux.py` & `zillionare_omicron-2.0.0a71/tests/dal/influx/test_flux.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/dal/influx/test_influxclient.py` & `zillionare_omicron-2.0.0a71/tests/dal/influx/test_influxclient.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/dal/influx/test_serialize.py` & `zillionare_omicron-2.0.0a71/tests/dal/influx/test_serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.15m.csv` & `zillionare_omicron-2.0.0a71/tests/data/000001.XSHE.15m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.1m.csv` & `zillionare_omicron-2.0.0a71/tests/data/000001.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.30m.csv` & `zillionare_omicron-2.0.0a71/tests/data/000001.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/000001.XSHE.5m.csv` & `zillionare_omicron-2.0.0a71/tests/data/000001.XSHE.5m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/000001.XSHG.1m.csv` & `zillionare_omicron-2.0.0a71/tests/data/000001.XSHG.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.1d.csv` & `zillionare_omicron-2.0.0a71/tests/data/000002.XSHE.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.1m.csv` & `zillionare_omicron-2.0.0a71/tests/data/000002.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.1w.csv` & `zillionare_omicron-2.0.0a71/tests/data/000002.XSHE.1w.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/000002.XSHE.30m.csv` & `zillionare_omicron-2.0.0a71/tests/data/000002.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.1d.csv` & `zillionare_omicron-2.0.0a71/tests/data/000004.XSHE.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.1m.csv` & `zillionare_omicron-2.0.0a71/tests/data/000004.XSHE.1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.1w.csv` & `zillionare_omicron-2.0.0a71/tests/data/000004.XSHE.1w.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/000004.XSHE.30m.csv` & `zillionare_omicron-2.0.0a71/tests/data/000004.XSHE.30m.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/600000.XSHG.1d.csv` & `zillionare_omicron-2.0.0a71/tests/data/600000.XSHG.1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/README.md` & `zillionare_omicron-2.0.0a71/tests/data/README.md`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/bars_1d.pkl` & `zillionare_omicron-2.0.0a71/tests/data/bars_1d.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/bars_1m.pkl` & `zillionare_omicron-2.0.0a71/tests/data/bars_1m.pkl`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/limits.csv` & `zillionare_omicron-2.0.0a71/tests/data/limits.csv`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/stock_bars_flux_query.txt` & `zillionare_omicron-2.0.0a71/tests/data/stock_bars_flux_query.txt`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/data/test.jpg` & `zillionare_omicron-2.0.0a71/tests/data/test.jpg`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/extensions/test_decimals.py` & `zillionare_omicron-2.0.0a71/tests/extensions/test_decimals.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/extensions/test_np.py` & `zillionare_omicron-2.0.0a71/tests/extensions/test_np.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/models/test_board.py` & `zillionare_omicron-2.0.0a71/tests/models/test_board.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/models/test_security.py` & `zillionare_omicron-2.0.0a71/tests/models/test_security.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/models/test_stock.py` & `zillionare_omicron-2.0.0a71/tests/models/test_stock.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/models/test_timeframe.py` & `zillionare_omicron-2.0.0a71/tests/models/test_timeframe.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/notify/test_dingtalk.py` & `zillionare_omicron-2.0.0a71/tests/notify/test_dingtalk.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/notify/test_mail.py` & `zillionare_omicron-2.0.0a71/tests/notify/test_mail.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/performance/influx/end2end.py` & `zillionare_omicron-2.0.0a71/tests/performance/influx/end2end.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/performance/influx/serialize.py` & `zillionare_omicron-2.0.0a71/tests/performance/influx/serialize.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/strategy/test_strategy.py` & `zillionare_omicron-2.0.0a71/tests/strategy/test_strategy.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/talib/test_core.py` & `zillionare_omicron-2.0.0a71/tests/talib/test_core.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/tests/talib/test_morph.py` & `zillionare_omicron-2.0.0a71/tests/talib/test_morph.py`

 * *Files identical despite different names*

### Comparing `zillionare_omicron-2.0.0a69/PKG-INFO` & `zillionare_omicron-2.0.0a71/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zillionare-omicron
-Version: 2.0.0a69
+Version: 2.0.0a71
 Summary: Core Library for Zillionare
 Home-page: https://zillionare-omicron.readthedocs.io
 License: MIT
 Keywords: AI,quant,trade,stock
 Author: jieyu
 Author-email: code@jieyu.ai
 Requires-Python: >=3.8,<3.9
```

