# Comparing `tmp/llpy-helper-lib-0.2.1.tar.gz` & `tmp/llpy-helper-lib-2.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llpy-helper-lib-0.2.1.tar", last modified: Sat Apr 22 10:17:22 2023, max compression
+gzip compressed data, was "llpy-helper-lib-2.13.1.tar", last modified: Fri May 19 11:05:26 2023, max compression
```

## Comparing `llpy-helper-lib-0.2.1.tar` & `llpy-helper-lib-2.13.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
--rw-r--r--   0        0        0     1077 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/LICENSE
--rw-r--r--   0        0        0     1047 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/README.md
--rw-r--r--   0        0        0     4863 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/__init__.py
--rw-r--r--   0        0        0       48 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/directionangle/__init__.py
--rw-r--r--   0        0        0      813 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/directionangle/__init__.pyi
--rw-r--r--   0        0        0      338 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/enumdefine/__init__.pyi
--rw-r--r--   0        0        0       32 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/format/__init__.py
--rw-r--r--   0        0        0     1758 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/format/__init__.pyi
--rw-r--r--   0        0        0       68 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/pos/__init__.py
--rw-r--r--   0        0        0     1230 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/pos/__init__.pyi
--rw-r--r--   0        0        0      444 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/types.py
--rw-r--r--   0        0        0       59 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/block/__init__.py
--rw-r--r--   0        0        0     4230 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/block/__init__.pyi
--rw-r--r--   0        0        0       83 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/block/entity/__init__.py
--rw-r--r--   0        0        0     1039 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/block/entity/__init__.pyi
--rw-r--r--   0        0        0       67 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/__init__.py
--rw-r--r--   0        0        0     7199 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/__init__.pyi
--rw-r--r--   0        0        0      156 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/enums/__init__.py
--rw-r--r--   0        0        0     4983 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/enums/__init__.pyi
--rw-r--r--   0        0        0       91 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/origin/__init__.py
--rw-r--r--   0        0        0      873 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/origin/__init__.pyi
--rw-r--r--   0        0        0       91 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/output/__init__.py
--rw-r--r--   0        0        0     1754 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/output/__init__.pyi
--rw-r--r--   0        0        0     3381 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/types.py
--rw-r--r--   0        0        0       46 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/config/ini/__init__.py
--rw-r--r--   0        0        0     5673 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/config/ini/__init__.pyi
--rw-r--r--   0        0        0       48 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/config/json/__init__.py
--rw-r--r--   0        0        0     3738 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/config/json/__init__.pyi
--rw-r--r--   0        0        0      221 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/config/types.py
--rw-r--r--   0        0        0       75 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/container/__init__.py
--rw-r--r--   0        0        0     3611 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/container/__init__.pyi
--rw-r--r--   0        0        0       28 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/data/__init__.py
--rw-r--r--   0        0        0     4357 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/data/__init__.pyi
--rw-r--r--   0        0        0      330 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/data/types.py
--rw-r--r--   0        0        0       38 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/db/dbsession/__init__.py
--rw-r--r--   0        0        0     2243 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/db/dbsession/__init__.pyi
--rw-r--r--   0        0        0       32 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/db/dbstmt/__init__.py
--rw-r--r--   0        0        0     4663 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/db/dbstmt/__init__.pyi
--rw-r--r--   0        0        0       40 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/db/kvdb/__init__.py
--rw-r--r--   0        0        0     1657 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/db/kvdb/__init__.pyi
--rw-r--r--   0        0        0      570 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/db/types.py
--rw-r--r--   0        0        0       63 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/entity/__init__.py
--rw-r--r--   0        0        0    15776 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/entity/__init__.pyi
--rw-r--r--   0        0        0       93 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/entity/damagecause/__init__.py
--rw-r--r--   0        0        0     3678 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/entity/damagecause/__init__.pyi
--rw-r--r--   0        0        0     1962 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/entity/types.py
--rw-r--r--   0        0        0       28 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/file/__init__.py
--rw-r--r--   0        0        0    12487 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/file/__init__.pyi
--rw-r--r--   0        0        0      208 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/file/types.py
--rw-r--r--   0        0        0       79 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/form/custom/__init__.py
--rw-r--r--   0        0        0     3106 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/form/custom/__init__.pyi
--rw-r--r--   0        0        0       79 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/form/simple/__init__.py
--rw-r--r--   0        0        0     1263 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/form/simple/__init__.pyi
--rw-r--r--   0        0        0       28 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/i18n/__init__.py
--rw-r--r--   0        0        0     3434 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/i18n/__init__.pyi
--rw-r--r--   0        0        0       43 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/i18n/types.py
--rw-r--r--   0        0        0       55 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/item/__init__.py
--rw-r--r--   0        0        0     5079 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/item/__init__.pyi
--rw-r--r--   0        0        0       24 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/ll/__init__.py
--rw-r--r--   0        0        0     7505 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/ll/__init__.pyi
--rw-r--r--   0        0        0      612 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/ll/types.py
--rw-r--r--   0        0        0       34 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/ll/version/__init__.py
--rw-r--r--   0        0        0      471 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/ll/version/__init__.pyi
--rw-r--r--   0        0        0       32 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/logger/__init__.py
--rw-r--r--   0        0        0     3440 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/logger/__init__.pyi
--rw-r--r--   0        0        0      431 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/logger/types.py
--rw-r--r--   0        0        0       24 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/mc/__init__.py
--rw-r--r--   0        0        0    82826 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/mc/__init__.pyi
--rw-r--r--   0        0        0     1930 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/mc/types.py
--rw-r--r--   0        0        0       30 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/money/__init__.py
--rw-r--r--   0        0        0     2537 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/money/__init__.pyi
--rw-r--r--   0        0        0      468 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/money/types.py
--rw-r--r--   0        0        0       42 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/enum/__init__.py
--rw-r--r--   0        0        0     1047 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/enum/__init__.pyi
--rw-r--r--   0        0        0       48 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/function/__init__.py
--rw-r--r--   0        0        0     2598 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/function/__init__.pyi
--rw-r--r--   0        0        0       46 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/globalpointer/__init__.py
--rw-r--r--   0        0        0      861 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/globalpointer/__init__.pyi
--rw-r--r--   0        0        0       40 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/hook/__init__.py
--rw-r--r--   0        0        0      700 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/hook/__init__.pyi
--rw-r--r--   0        0        0       42 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/patch/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/patch/__init__.pyi
--rw-r--r--   0        0        0       46 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/pointer/__init__.py
--rw-r--r--   0        0        0     4298 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/pointer/__init__.pyi
--rw-r--r--   0        0        0       50 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/stdstring/__init__.py
--rw-r--r--   0        0        0     1693 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/stdstring/__init__.pyi
--rw-r--r--   0        0        0      953 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/types.py
--rw-r--r--   0        0        0      324 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/base/__init__.py
--rw-r--r--   0        0        0     2021 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/base/__init__.pyi
--rw-r--r--   0        0        0       42 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/compound/__init__.py
--rw-r--r--   0        0        0     7453 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/compound/__init__.pyi
--rw-r--r--   0        0        0       34 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/list/__init__.py
--rw-r--r--   0        0        0     6992 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/list/__init__.pyi
--rw-r--r--   0        0        0       26 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/static/__init__.py
--rw-r--r--   0        0        0     2382 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/static/__init__.pyi
--rw-r--r--   0        0        0     1181 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/types.py
--rw-r--r--   0        0        0       34 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/__init__.py
--rw-r--r--   0        0        0     3497 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/__init__.pyi
--rw-r--r--   0        0        0       42 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/httprequest/__init__.py
--rw-r--r--   0        0        0     1289 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/httprequest/__init__.pyi
--rw-r--r--   0        0        0       44 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/httpresponse/__init__.py
--rw-r--r--   0        0        0     1291 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/httpresponse/__init__.pyi
--rw-r--r--   0        0        0       40 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/httpserver/__init__.py
--rw-r--r--   0        0        0     7655 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/httpserver/__init__.pyi
--rw-r--r--   0        0        0      833 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/types.py
--rw-r--r--   0        0        0       36 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/wsclient/__init__.py
--rw-r--r--   0        0        0     4258 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/wsclient/__init__.pyi
--rw-r--r--   0        0        0       75 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/objective/__init__.py
--rw-r--r--   0        0        0     3364 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/objective/__init__.pyi
--rw-r--r--   0        0        0      211 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/objective/types.py
--rw-r--r--   0        0        0      108 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/packet/__init__.py
--rw-r--r--   0        0        0     5149 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/packet/__init__.pyi
--rw-r--r--   0        0        0       46 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/particle/color/__init__.py
--rw-r--r--   0        0        0     1724 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/particle/color/__init__.pyi
--rw-r--r--   0        0        0       38 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/particle/direction/__init__.py
--rw-r--r--   0        0        0      703 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/particle/direction/__init__.pyi
--rw-r--r--   0        0        0       50 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/particle/spawner/__init__.py
--rw-r--r--   0        0        0     5726 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/particle/spawner/__init__.pyi
--rw-r--r--   0        0        0     1745 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/particle/types.py
--rw-r--r--   0        0        0       40 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/permission/__init__.py
--rw-r--r--   0        0        0     4827 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/permission/__init__.pyi
--rw-r--r--   0        0        0       28 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/permission/role/__init__.py
--rw-r--r--   0        0        0     5082 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/permission/role/__init__.pyi
--rw-r--r--   0        0        0      253 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/permission/types.py
--rw-r--r--   0        0        0       63 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/player/__init__.py
--rw-r--r--   0        0        0    45602 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/player/__init__.pyi
--rw-r--r--   0        0        0       63 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/player/device/__init__.py
--rw-r--r--   0        0        0     2342 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/player/device/__init__.pyi
--rw-r--r--   0        0        0     2684 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/player/types.py
--rw-r--r--   0        0        0       32 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/system/__init__.py
--rw-r--r--   0        0        0     2434 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/system/__init__.pyi
--rw-r--r--   0        0        0      380 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/system/types.py
--rw-r--r--   0        0        0      256 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/functions/__init__.py
--rw-r--r--   0        0        0     2738 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/functions/__init__.pyi
--rw-r--r--   0        0        0      304 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/functions/types.py
--rw-r--r--   0        0        0    15844 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/types.py
--rw-r--r--   0        0        0     1101 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 llpy-helper-lib-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-19 11:05:14.432544 llpy-helper-lib-2.13.1/LICENSE
+-rw-r--r--   0        0        0     1385 2023-05-19 11:05:14.432544 llpy-helper-lib-2.13.1/README.md
+-rw-r--r--   0        0        0     4863 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/base/directionangle/__init__.py
+-rw-r--r--   0        0        0      813 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/base/directionangle/__init__.pyi
+-rw-r--r--   0        0        0      338 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/base/enumdefine/__init__.pyi
+-rw-r--r--   0        0        0       32 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/base/format/__init__.py
+-rw-r--r--   0        0        0     1758 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/base/format/__init__.pyi
+-rw-r--r--   0        0        0       68 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/base/pos/__init__.py
+-rw-r--r--   0        0        0     1230 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/base/pos/__init__.pyi
+-rw-r--r--   0        0        0     2329 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/base/types.py
+-rw-r--r--   0        0        0       59 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/block/__init__.py
+-rw-r--r--   0        0        0     4230 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/block/__init__.pyi
+-rw-r--r--   0        0        0       83 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/block/entity/__init__.py
+-rw-r--r--   0        0        0     1039 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/block/entity/__init__.pyi
+-rw-r--r--   0        0        0       67 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/command/__init__.py
+-rw-r--r--   0        0        0     7199 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/command/__init__.pyi
+-rw-r--r--   0        0        0      156 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/command/enums/__init__.py
+-rw-r--r--   0        0        0     4983 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/command/enums/__init__.pyi
+-rw-r--r--   0        0        0       91 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/command/origin/__init__.py
+-rw-r--r--   0        0        0      873 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/command/origin/__init__.pyi
+-rw-r--r--   0        0        0       91 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/command/output/__init__.py
+-rw-r--r--   0        0        0     1754 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/command/output/__init__.pyi
+-rw-r--r--   0        0        0     3381 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/command/types.py
+-rw-r--r--   0        0        0       46 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/config/ini/__init__.py
+-rw-r--r--   0        0        0     5673 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/config/ini/__init__.pyi
+-rw-r--r--   0        0        0       48 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/config/json/__init__.py
+-rw-r--r--   0        0        0     3738 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/config/json/__init__.pyi
+-rw-r--r--   0        0        0      221 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/config/types.py
+-rw-r--r--   0        0        0       75 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/container/__init__.py
+-rw-r--r--   0        0        0     3611 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/container/__init__.pyi
+-rw-r--r--   0        0        0       28 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/data/__init__.py
+-rw-r--r--   0        0        0     4357 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/data/__init__.pyi
+-rw-r--r--   0        0        0      330 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/data/types.py
+-rw-r--r--   0        0        0       38 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/db/dbsession/__init__.py
+-rw-r--r--   0        0        0     2243 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/db/dbsession/__init__.pyi
+-rw-r--r--   0        0        0       32 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/db/dbstmt/__init__.py
+-rw-r--r--   0        0        0     4663 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/db/dbstmt/__init__.pyi
+-rw-r--r--   0        0        0       40 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/db/kvdb/__init__.py
+-rw-r--r--   0        0        0     1657 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/db/kvdb/__init__.pyi
+-rw-r--r--   0        0        0      570 2023-05-19 11:05:14.436544 llpy-helper-lib-2.13.1/llpy/classes/db/types.py
+-rw-r--r--   0        0        0       63 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/entity/__init__.py
+-rw-r--r--   0        0        0    16604 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/entity/__init__.pyi
+-rw-r--r--   0        0        0       93 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/entity/damagecause/__init__.py
+-rw-r--r--   0        0        0     3678 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/entity/damagecause/__init__.pyi
+-rw-r--r--   0        0        0     1962 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/entity/types.py
+-rw-r--r--   0        0        0       28 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/file/__init__.py
+-rw-r--r--   0        0        0    12487 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/file/__init__.pyi
+-rw-r--r--   0        0        0      208 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/file/types.py
+-rw-r--r--   0        0        0       79 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/form/custom/__init__.py
+-rw-r--r--   0        0        0     3106 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/form/custom/__init__.pyi
+-rw-r--r--   0        0        0       79 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/form/simple/__init__.py
+-rw-r--r--   0        0        0     1263 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/form/simple/__init__.pyi
+-rw-r--r--   0        0        0       28 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/i18n/__init__.py
+-rw-r--r--   0        0        0     3434 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/i18n/__init__.pyi
+-rw-r--r--   0        0        0       43 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/i18n/types.py
+-rw-r--r--   0        0        0       55 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/item/__init__.py
+-rw-r--r--   0        0        0     5079 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/item/__init__.pyi
+-rw-r--r--   0        0        0       24 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/ll/__init__.py
+-rw-r--r--   0        0        0     7505 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/ll/__init__.pyi
+-rw-r--r--   0        0        0      612 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/ll/types.py
+-rw-r--r--   0        0        0       34 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/ll/version/__init__.py
+-rw-r--r--   0        0        0      471 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/ll/version/__init__.pyi
+-rw-r--r--   0        0        0       32 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/logger/__init__.py
+-rw-r--r--   0        0        0     3440 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/logger/__init__.pyi
+-rw-r--r--   0        0        0      431 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/logger/types.py
+-rw-r--r--   0        0        0       24 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/mc/__init__.py
+-rw-r--r--   0        0        0    83694 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/mc/__init__.pyi
+-rw-r--r--   0        0        0     1930 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/mc/types.py
+-rw-r--r--   0        0        0       30 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/money/__init__.py
+-rw-r--r--   0        0        0     2537 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/money/__init__.pyi
+-rw-r--r--   0        0        0      468 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/money/types.py
+-rw-r--r--   0        0        0       42 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/enum/__init__.py
+-rw-r--r--   0        0        0     1047 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/enum/__init__.pyi
+-rw-r--r--   0        0        0       48 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/function/__init__.py
+-rw-r--r--   0        0        0     2598 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/function/__init__.pyi
+-rw-r--r--   0        0        0       46 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/globalpointer/__init__.py
+-rw-r--r--   0        0        0      861 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/globalpointer/__init__.pyi
+-rw-r--r--   0        0        0       40 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/hook/__init__.py
+-rw-r--r--   0        0        0      700 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/hook/__init__.pyi
+-rw-r--r--   0        0        0       42 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/patch/__init__.py
+-rw-r--r--   0        0        0     1112 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/patch/__init__.pyi
+-rw-r--r--   0        0        0       46 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/pointer/__init__.py
+-rw-r--r--   0        0        0     4298 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/pointer/__init__.pyi
+-rw-r--r--   0        0        0       50 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/stdstring/__init__.py
+-rw-r--r--   0        0        0     1693 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/stdstring/__init__.pyi
+-rw-r--r--   0        0        0      953 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/native/types.py
+-rw-r--r--   0        0        0      324 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/nbt/base/__init__.py
+-rw-r--r--   0        0        0     2021 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/nbt/base/__init__.pyi
+-rw-r--r--   0        0        0       42 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/nbt/compound/__init__.py
+-rw-r--r--   0        0        0     7453 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/nbt/compound/__init__.pyi
+-rw-r--r--   0        0        0       34 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/nbt/list/__init__.py
+-rw-r--r--   0        0        0     6992 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/nbt/list/__init__.pyi
+-rw-r--r--   0        0        0       26 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/nbt/static/__init__.py
+-rw-r--r--   0        0        0     2382 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/nbt/static/__init__.pyi
+-rw-r--r--   0        0        0     1181 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/nbt/types.py
+-rw-r--r--   0        0        0       34 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/network/__init__.py
+-rw-r--r--   0        0        0     3497 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/network/__init__.pyi
+-rw-r--r--   0        0        0       42 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/network/httprequest/__init__.py
+-rw-r--r--   0        0        0     1289 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/network/httprequest/__init__.pyi
+-rw-r--r--   0        0        0       44 2023-05-19 11:05:14.440544 llpy-helper-lib-2.13.1/llpy/classes/network/httpresponse/__init__.py
+-rw-r--r--   0        0        0     1291 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/network/httpresponse/__init__.pyi
+-rw-r--r--   0        0        0       40 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/network/httpserver/__init__.py
+-rw-r--r--   0        0        0     7655 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/network/httpserver/__init__.pyi
+-rw-r--r--   0        0        0      833 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/network/types.py
+-rw-r--r--   0        0        0       36 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/network/wsclient/__init__.py
+-rw-r--r--   0        0        0     4258 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/network/wsclient/__init__.pyi
+-rw-r--r--   0        0        0       75 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/objective/__init__.py
+-rw-r--r--   0        0        0     3364 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/objective/__init__.pyi
+-rw-r--r--   0        0        0      211 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/objective/types.py
+-rw-r--r--   0        0        0      108 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/packet/__init__.py
+-rw-r--r--   0        0        0     5149 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/packet/__init__.pyi
+-rw-r--r--   0        0        0       46 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/particle/color/__init__.py
+-rw-r--r--   0        0        0     1724 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/particle/color/__init__.pyi
+-rw-r--r--   0        0        0       38 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/particle/direction/__init__.py
+-rw-r--r--   0        0        0      703 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/particle/direction/__init__.pyi
+-rw-r--r--   0        0        0       50 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/particle/spawner/__init__.py
+-rw-r--r--   0        0        0     5726 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/particle/spawner/__init__.pyi
+-rw-r--r--   0        0        0     1745 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/particle/types.py
+-rw-r--r--   0        0        0       40 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/permission/__init__.py
+-rw-r--r--   0        0        0     4827 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/permission/__init__.pyi
+-rw-r--r--   0        0        0       28 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/permission/role/__init__.py
+-rw-r--r--   0        0        0     5082 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/permission/role/__init__.pyi
+-rw-r--r--   0        0        0      253 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/permission/types.py
+-rw-r--r--   0        0        0       63 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/player/__init__.py
+-rw-r--r--   0        0        0    45635 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/player/__init__.pyi
+-rw-r--r--   0        0        0       63 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/player/device/__init__.py
+-rw-r--r--   0        0        0     2342 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/player/device/__init__.pyi
+-rw-r--r--   0        0        0     2684 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/player/types.py
+-rw-r--r--   0        0        0       32 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/system/__init__.py
+-rw-r--r--   0        0        0     2434 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/system/__init__.pyi
+-rw-r--r--   0        0        0      380 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/classes/system/types.py
+-rw-r--r--   0        0        0      256 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/functions/__init__.py
+-rw-r--r--   0        0        0     2738 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/functions/__init__.pyi
+-rw-r--r--   0        0        0      304 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/functions/types.py
+-rw-r--r--   0        0        0    15901 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/llpy/types.py
+-rw-r--r--   0        0        0     1102 2023-05-19 11:05:14.444544 llpy-helper-lib-2.13.1/pyproject.toml
+-rw-r--r--   0        0        0     1642 1970-01-01 00:00:00.000000 llpy-helper-lib-2.13.1/PKG-INFO
```

### Comparing `llpy-helper-lib-0.2.1/LICENSE` & `llpy-helper-lib-2.13.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/README.md` & `llpy-helper-lib-2.13.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: llpy-helper-lib
+Version: 2.13.1
+Summary: A typing & util lib for LLSE Python runtime
+License: MIT
+Author-email: student_2333 <lgc2333@126.com>
+Requires-Python: >=3.10
+Provides-Extra: dev
+Description-Content-Type: text/markdown
+
 <!-- markdownlint-disable MD033 MD036 -->
 
 # LLSE-Python Helper Lib
 
 [![wakatime](https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/dcd72d53-ac99-4567-a96a-e3de0d0b6836.svg)](https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/dcd72d53-ac99-4567-a96a-e3de0d0b6836)
 
 A typing & util lib for LLSE Python runtime
@@ -28,13 +38,21 @@
 
 ## Usage / 用法
 
 **[example.py](./example.py)**
 
 ## Update Log / 更新日志
 
+### 2.13.1
+
+- Synchronized this library version number with the LL version, also synchronized this library content with LL version 2.13.1  
+  补全库版本与 LL 版本同步，且补全库内容与 LL 2.13.1 版本同步
+- Fixed a mistake in the game mode type (`T_GameMode`)  
+  修复 游戏模式类型 (`T_GameMode`) 中的错误
+
 ### 0.2.0
 
 - Removed module `llpy.utils`  
   删除了 `llpy.utils` 模块
 - Added things from `BaseLib.py`  
   添加了来自 `BaseLib.py` 的东西
+
```

### Comparing `llpy-helper-lib-0.2.1/llpy/__init__.py` & `llpy-helper-lib-2.13.1/llpy/__init__.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/base/directionangle/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/base/directionangle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/base/format/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/base/format/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/base/pos/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/base/pos/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/block/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/block/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/block/entity/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/block/entity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/command/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/command/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/command/enums/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/command/enums/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/command/origin/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/command/origin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/command/output/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/command/output/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/command/types.py` & `llpy-helper-lib-2.13.1/llpy/classes/command/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/config/ini/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/config/ini/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/config/json/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/config/json/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/container/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/container/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/data/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/db/dbsession/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/db/dbsession/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/db/dbstmt/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/db/dbstmt/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/db/kvdb/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/db/kvdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/db/types.py` & `llpy-helper-lib-2.13.1/llpy/classes/db/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/entity/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/entity/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     LLSE_Block,
     LLSE_Container,
     LLSE_Item,
     LLSE_Player,
     NativePointer,
     NbtCompound,
 )
-from llpy.types import T_DamageCause, T_DimID, T_Number, T_PosType
+from llpy.types import T_DamageCause, T_DimID, T_EffectID, T_Number, T_PosType
 
 class LLSE_Entity:
     """实体对象"""
 
     def __init__(self) -> NoReturn: ...
     @property
     def name(self) -> str:
@@ -600,19 +600,55 @@
     def getBiomeName(self) -> str:
         """
         获取实体所在群系名称
 
         Returns:
             群系名称
         """
+    def getAllEffects(self) -> list[T_EffectID]:
+        """
+        获取实体全部药水效果
+
+        Returns:
+            实体所有的药水效果 ID
+        """
+    def addEffect(
+        self,
+        effect_id: T_EffectID,
+        tick: int,
+        level: int,
+        show_particles: bool,
+    ) -> bool:
+        """
+        为实体添加一个药水效果
+
+        Args:
+            id: 药水效果的 ID
+            tick: 持续时间
+            level: 等级
+            show_particles: 是否显示粒子
+
+        Returns:
+            操作是否成功
+        """
+    def removeEffect(self, effect_id: int) -> bool:
+        """
+        为实体移除一个药水效果
+
+        Args:
+            effect_id: 药水效果的 ID
+
+        Returns:
+            操作是否成功
+        """
     def quickEvalMolangScript(self, exp: str) -> float:
         """
         快速执行 Molang 表达式
 
-        关于Molang的详细使用方法，请参考 [MOLANG 文档 bedrock.dev](https://bedrock.dev/zh/docs/stable/Molang)
+        关于 Molang 的详细使用方法，请参考 [MOLANG 文档 bedrock.dev](https://bedrock.dev/zh/docs/stable/Molang)
 
         Args:
             exp: Molang 表达式
 
         Returns:
             表达式执行结果
         """
```

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/entity/damagecause/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/entity/damagecause/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/entity/types.py` & `llpy-helper-lib-2.13.1/llpy/classes/entity/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/file/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/file/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/form/custom/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/form/custom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/form/simple/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/form/simple/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/i18n/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/i18n/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/item/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/item/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/ll/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/ll/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/ll/types.py` & `llpy-helper-lib-2.13.1/llpy/classes/ll/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/logger/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/logger/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/mc/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/mc/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -990,14 +990,42 @@
 
         Returns:
             是否成功监听事件
         """
     @overload
     @staticmethod
     def listen(
+        event: Literal["onPlayerPullFishingHook"],
+        callback: Callable[
+            [LLSE_Player, LLSE_Entity, LLSE_Item | None],
+            Literal[False] | Any,
+        ],
+    ) -> bool:
+        """
+        注册监听器
+
+        玩家使用钓鱼竿钓起实体 监听
+
+        拦截事件：函数返回 `False`
+
+        Callback Args:
+            player (LLSE_Player): 使用钓鱼竿的玩家对象
+            entity (LLSE_Entity): 钓起的实体（鱼钩拉起任意实体都会触发该事件，不一定是物品实体）
+            item (LLSE_Item | None): 钓起的物品对象（如果钓到的不是物品则返回 `None`）
+
+        Args:
+            event: 要监听的事件名
+            callback: 注册的监听函数
+
+        Returns:
+            是否成功监听事件
+        """
+    @overload
+    @staticmethod
+    def listen(
         event: Literal["onMobDie"],
         callback: Callable[
             [LLSE_Entity, LLSE_Entity | None, T_DamageCause],
             Literal[False] | Any,
         ],
     ) -> bool:
         """
```

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/mc/types.py` & `llpy-helper-lib-2.13.1/llpy/classes/mc/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/money/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/money/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/native/enum/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/native/enum/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/native/function/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/native/function/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/native/globalpointer/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/native/globalpointer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/native/hook/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/native/hook/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/native/patch/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/native/patch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/native/pointer/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/native/pointer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/native/stdstring/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/native/stdstring/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/native/types.py` & `llpy-helper-lib-2.13.1/llpy/classes/native/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/nbt/base/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/nbt/base/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/nbt/compound/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/nbt/compound/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/nbt/list/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/nbt/list/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/nbt/static/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/nbt/static/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/nbt/types.py` & `llpy-helper-lib-2.13.1/llpy/classes/nbt/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/network/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/network/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/network/httprequest/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/network/httprequest/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/network/httpresponse/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/network/httpresponse/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/network/httpserver/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/network/httpserver/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/network/types.py` & `llpy-helper-lib-2.13.1/llpy/classes/network/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/network/wsclient/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/network/wsclient/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/objective/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/objective/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/packet/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/packet/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/particle/color/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/particle/color/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/particle/direction/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/particle/direction/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/particle/spawner/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/particle/spawner/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/particle/types.py` & `llpy-helper-lib-2.13.1/llpy/classes/particle/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/permission/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/permission/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/permission/role/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/permission/role/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/player/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/player/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     LLSE_Entity,
     LLSE_Item,
     LLSE_Packet,
     LLSE_SimpleForm,
     NativePointer,
     NbtCompound,
 )
-from llpy.types import T_DimID, T_MoneyHistory, T_Number, T_PosType
+from llpy.types import T_DimID, T_EffectID, T_MoneyHistory, T_Number, T_PosType
 
 from .types import (
     T_BossEventColor,
     T_CustomFormCallback,
     T_GameMode,
     T_ModalFormCallback,
     T_NavigatePath,
@@ -1101,34 +1101,34 @@
     def getBiomeName(self) -> str:
         """
         获取玩家所在群系名称
 
         Returns:
             群系名称
         """
-    def getAllEffects(self) -> list[int] | None:
+    def getAllEffects(self) -> list[T_EffectID] | None:
         """
         获取玩家身上的状态效果
 
         Returns:
             状态效果 ID 列表。如果玩家身上没有状态效果则返回 `None`
         """
-    def addEffect(self, effect_id: int, tick: int, level: int) -> bool:
+    def addEffect(self, effect_id: T_EffectID, tick: int, level: int) -> bool:
         """
         给玩家添加状态效果
 
         Args:
             effect_id: 状态效果数字 ID
             tick: 持续的 `Ticks`
             level: 效果等级
 
         Returns:
             是否成功添加效果
         """
-    def removeEffect(self, effect_id: int) -> bool:
+    def removeEffect(self, effect_id: T_EffectID) -> bool:
         """
         移除玩家的状态效果
 
         Args:
             effect_id: 状态效果数字 ID
 
         Returns:
```

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/player/device/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/player/device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/player/types.py` & `llpy-helper-lib-2.13.1/llpy/classes/player/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 """
 操作权限等级
 
 - 0. 普通成员
 - 1. OP
 - 4. 控制台
 """
-T_GameMode = Literal[0, 1, 2, 3]
+T_GameMode = Literal[0, 1, 2, 6]
 """
 游戏模式
 
 - 0. 生存
 - 1. 创造
 - 2. 冒险
-- 3. 旁观
+- 6. 旁观
 """
 T_TextPacketType = Literal[0, 1, 4, 5, 9]
 """
 `LLSE_Player.tell()` 发送的文本消息类型
 
 - 0. 普通消息 (`Raw`)
 - 1. 聊天消息 (`Chat`)
```

### Comparing `llpy-helper-lib-0.2.1/llpy/classes/system/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/classes/system/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/functions/__init__.pyi` & `llpy-helper-lib-2.13.1/llpy/functions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.1/llpy/types.py` & `llpy-helper-lib-2.13.1/llpy/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .classes.base.types import T_BasicFacing as T_BasicFacing
 from .classes.base.types import T_DimID as T_DimID
 from .classes.base.types import T_DimIDNether as T_DimIDNether
 from .classes.base.types import T_DimIDOverWorld as T_DimIDOverWorld
 from .classes.base.types import T_DimIDTheEnd as T_DimIDTheEnd
+from .classes.base.types import T_EffectID as T_EffectID
 from .classes.base.types import T_Number as T_Number
 from .classes.base.types import T_PosType as T_PosType
 from .classes.command.types import T_CommandCallback as T_CommandCallback
 from .classes.command.types import T_CommandCallbackResult as T_CommandCallbackResult
 from .classes.command.types import T_OriginType as T_OriginType
 from .classes.command.types import T_OriginTypeActor as T_OriginTypeActor
 from .classes.command.types import T_OriginTypeActorServer as T_OriginTypeActorServer
```

### Comparing `llpy-helper-lib-0.2.1/pyproject.toml` & `llpy-helper-lib-2.13.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 "example.py" = [
     "F403",
     "F405",
 ]
 
 [project]
 name = "llpy-helper-lib"
-version = "0.2.1"
+version = "2.13.1"
 description = "A typing & util lib for LLSE Python runtime"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
 ]
```

