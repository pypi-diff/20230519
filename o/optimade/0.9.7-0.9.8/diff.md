# Comparing `tmp/optimade-0.9.7.tar.gz` & `tmp/optimade-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/optimade-0.9.7.tar", last modified: Sun Jun 28 17:21:00 2020, max compression
+gzip compressed data, was "dist/optimade-0.9.8.tar", last modified: Fri Jul  3 08:41:57 2020, max compression
```

## Comparing `optimade-0.9.7.tar` & `optimade-0.9.8.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (116)      228 2020-06-28 17:12:17.000000 optimade-0.9.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     5835 2020-06-28 17:21:00.000000 optimade-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4388 2020-06-28 17:12:17.000000 optimade-0.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/
--rw-r--r--   0 runner    (1001) docker     (116)       53 2020-06-28 17:20:57.000000 optimade-0.9.7/optimade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/adapters/
--rw-r--r--   0 runner    (1001) docker     (116)      244 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4807 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (116)      111 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/adapters/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/adapters/references/
--rw-r--r--   0 runner    (1001) docker     (116)      314 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/adapters/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/adapters/structures/
--rw-r--r--   0 runner    (1001) docker     (116)      814 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/adapters/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2495 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/adapters/structures/aiida.py
--rw-r--r--   0 runner    (1001) docker     (116)     2049 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/adapters/structures/ase.py
--rw-r--r--   0 runner    (1001) docker     (116)     4741 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/adapters/structures/cif.py
--rw-r--r--   0 runner    (1001) docker     (116)     1321 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/adapters/structures/jarvis.py
--rw-r--r--   0 runner    (1001) docker     (116)     9062 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/adapters/structures/proteindatabank.py
--rw-r--r--   0 runner    (1001) docker     (116)     3088 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/adapters/structures/pymatgen.py
--rw-r--r--   0 runner    (1001) docker     (116)     7519 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/adapters/structures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/filterparser/
--rw-r--r--   0 runner    (1001) docker     (116)       90 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/filterparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1488 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/filterparser/lark_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/filtertransformers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/filtertransformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5900 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/filtertransformers/debug.py
--rw-r--r--   0 runner    (1001) docker     (116)     2969 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/filtertransformers/django.py
--rw-r--r--   0 runner    (1001) docker     (116)     9824 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/filtertransformers/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (116)     1159 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/filtertransformers/json.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    17415 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/filtertransformers/mongo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/grammar/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1412 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/grammar/v0.10.0.elastic.lark
--rw-r--r--   0 runner    (1001) docker     (116)     2829 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/grammar/v0.10.0.lark
--rw-r--r--   0 runner    (1001) docker     (116)     3116 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/grammar/v0.10.1.lark
--rw-r--r--   0 runner    (1001) docker     (116)      699 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/grammar/v0.9.5.lark
--rw-r--r--   0 runner    (1001) docker     (116)      762 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/grammar/v0.9.6.lark
--rw-r--r--   0 runner    (1001) docker     (116)      754 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/grammar/v0.9.7.lark
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/models/
--rw-r--r--   0 runner    (1001) docker     (116)      812 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4000 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/models/baseinfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     7010 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/models/entries.py
--rw-r--r--   0 runner    (1001) docker     (116)     1850 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/models/index_metadb.py
--rw-r--r--   0 runner    (1001) docker     (116)    10375 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/models/jsonapi.py
--rw-r--r--   0 runner    (1001) docker     (116)     3555 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/models/links.py
--rw-r--r--   0 runner    (1001) docker     (116)    11170 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/models/optimade_json.py
--rw-r--r--   0 runner    (1001) docker     (116)     6378 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/models/references.py
--rw-r--r--   0 runner    (1001) docker     (116)     3371 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/models/responses.py
--rw-r--r--   0 runner    (1001) docker     (116)    49547 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/models/structures.py
--rw-r--r--   0 runner    (1001) docker     (116)     3264 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/server/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5065 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/config.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/server/data/
--rw-r--r--   0 runner    (1001) docker     (116)      512 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5614 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/data/providers.json
--rw-r--r--   0 runner    (1001) docker     (116)      313 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/data/test_links.json
--rw-r--r--   0 runner    (1001) docker     (116)     1338 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/data/test_references.json
--rw-r--r--   0 runner    (1001) docker     (116)    65399 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/data/test_structures.json
--rw-r--r--   0 runner    (1001) docker     (116)     5248 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/data/test_structures_v0.9.7.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/server/entry_collections/
--rw-r--r--   0 runner    (1001) docker     (116)      184 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/entry_collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2052 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/entry_collections/entry_collections.py
--rw-r--r--   0 runner    (1001) docker     (116)     6235 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/entry_collections/mongo.py
--rw-r--r--   0 runner    (1001) docker     (116)     3921 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (116)      378 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)      399 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/index_links.json
--rw-r--r--   0 runner    (1001) docker     (116)     4109 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     3383 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/main_index.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/server/mappers/
--rw-r--r--   0 runner    (1001) docker     (116)      350 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5361 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/mappers/entries.py
--rw-r--r--   0 runner    (1001) docker     (116)      533 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/mappers/links.py
--rw-r--r--   0 runner    (1001) docker     (116)      146 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/mappers/references.py
--rw-r--r--   0 runner    (1001) docker     (116)      340 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/mappers/structures.py
--rw-r--r--   0 runner    (1001) docker     (116)     1128 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/middleware.py
--rw-r--r--   0 runner    (1001) docker     (116)     9954 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/query_params.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/server/routers/
--rw-r--r--   0 runner    (1001) docker     (116)      230 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1775 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/routers/index_info.py
--rw-r--r--   0 runner    (1001) docker     (116)     2954 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/routers/info.py
--rw-r--r--   0 runner    (1001) docker     (116)     1230 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/routers/landing.py
--rw-r--r--   0 runner    (1001) docker     (116)      956 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/routers/links.py
--rw-r--r--   0 runner    (1001) docker     (116)     1610 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/routers/references.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/server/routers/static/
--rw-r--r--   0 runner    (1001) docker     (116)     2543 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/routers/static/landing_page.html
--rw-r--r--   0 runner    (1001) docker     (116)     1609 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/routers/structures.py
--rw-r--r--   0 runner    (1001) docker     (116)    11750 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/server/routers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/validator/
--rw-r--r--   0 runner    (1001) docker     (116)     3143 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/validator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade/validator/data/
--rw-r--r--   0 runner    (1001) docker     (116)     1459 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/validator/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1605 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/validator/data/filters.txt
--rw-r--r--   0 runner    (1001) docker     (116)      814 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/validator/data/optional_filters.txt
--rw-r--r--   0 runner    (1001) docker     (116)    24040 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/validator/validator.py
--rw-r--r--   0 runner    (1001) docker     (116)     1417 2020-06-28 17:12:17.000000 optimade-0.9.7/optimade/validator/validator_model_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5835 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2925 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       68 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1726 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-06-28 17:21:00.000000 optimade-0.9.7/optimade.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      121 2020-06-28 17:21:00.000000 optimade-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     3399 2020-06-28 17:12:17.000000 optimade-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (116)      228 2020-07-03 08:33:26.000000 optimade-0.9.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     5835 2020-07-03 08:41:57.000000 optimade-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4388 2020-07-03 08:33:26.000000 optimade-0.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/
+-rw-r--r--   0 runner    (1001) docker     (116)       48 2020-07-03 08:41:53.000000 optimade-0.9.8/optimade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/adapters/
+-rw-r--r--   0 runner    (1001) docker     (116)      244 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4807 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (116)      111 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/adapters/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/adapters/references/
+-rw-r--r--   0 runner    (1001) docker     (116)      314 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/adapters/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/adapters/structures/
+-rw-r--r--   0 runner    (1001) docker     (116)      814 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/adapters/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2495 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/adapters/structures/aiida.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2049 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/adapters/structures/ase.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4741 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/adapters/structures/cif.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1321 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/adapters/structures/jarvis.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9062 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/adapters/structures/proteindatabank.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3088 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/adapters/structures/pymatgen.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7519 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/adapters/structures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/filterparser/
+-rw-r--r--   0 runner    (1001) docker     (116)       90 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/filterparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1488 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/filterparser/lark_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/filtertransformers/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/filtertransformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5900 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/filtertransformers/debug.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2969 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/filtertransformers/django.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9824 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/filtertransformers/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1159 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/filtertransformers/json.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    17415 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/filtertransformers/mongo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/grammar/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1412 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/grammar/v0.10.0.elastic.lark
+-rw-r--r--   0 runner    (1001) docker     (116)     2829 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/grammar/v0.10.0.lark
+-rw-r--r--   0 runner    (1001) docker     (116)     3116 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/grammar/v0.10.1.lark
+-rw-r--r--   0 runner    (1001) docker     (116)      699 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/grammar/v0.9.5.lark
+-rw-r--r--   0 runner    (1001) docker     (116)      762 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/grammar/v0.9.6.lark
+-rw-r--r--   0 runner    (1001) docker     (116)      754 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/grammar/v0.9.7.lark
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/models/
+-rw-r--r--   0 runner    (1001) docker     (116)      812 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4140 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/models/baseinfo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7162 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/models/entries.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1850 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/models/index_metadb.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10375 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/models/jsonapi.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3555 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12666 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/models/optimade_json.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6378 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/models/references.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3360 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/models/responses.py
+-rw-r--r--   0 runner    (1001) docker     (116)    49547 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/models/structures.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3264 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/server/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5494 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/config.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/server/data/
+-rw-r--r--   0 runner    (1001) docker     (116)      512 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5614 2020-07-03 08:33:28.000000 optimade-0.9.8/optimade/server/data/providers.json
+-rw-r--r--   0 runner    (1001) docker     (116)      313 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/data/test_links.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1338 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/data/test_references.json
+-rw-r--r--   0 runner    (1001) docker     (116)    65399 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/data/test_structures.json
+-rw-r--r--   0 runner    (1001) docker     (116)     5248 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/data/test_structures_v0.9.7.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/server/entry_collections/
+-rw-r--r--   0 runner    (1001) docker     (116)      184 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/entry_collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2052 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/entry_collections/entry_collections.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6235 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/entry_collections/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3921 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (116)      378 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)      399 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/index_links.json
+-rw-r--r--   0 runner    (1001) docker     (116)     3917 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/main.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3658 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/main_index.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/server/mappers/
+-rw-r--r--   0 runner    (1001) docker     (116)      350 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5361 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/mappers/entries.py
+-rw-r--r--   0 runner    (1001) docker     (116)      533 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/mappers/links.py
+-rw-r--r--   0 runner    (1001) docker     (116)      146 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/mappers/references.py
+-rw-r--r--   0 runner    (1001) docker     (116)      340 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/mappers/structures.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1128 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9954 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/query_params.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/server/routers/
+-rw-r--r--   0 runner    (1001) docker     (116)      230 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1907 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/routers/index_info.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2954 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/routers/info.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1366 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/routers/landing.py
+-rw-r--r--   0 runner    (1001) docker     (116)      956 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/routers/links.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1610 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/routers/references.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/server/routers/static/
+-rw-r--r--   0 runner    (1001) docker     (116)     2593 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/routers/static/landing_page.html
+-rw-r--r--   0 runner    (1001) docker     (116)     1609 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/routers/structures.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11750 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/routers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      579 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/server/routers/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/validator/
+-rw-r--r--   0 runner    (1001) docker     (116)     3143 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/validator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade/validator/data/
+-rw-r--r--   0 runner    (1001) docker     (116)     1459 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/validator/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1605 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/validator/data/filters.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      814 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/validator/data/optional_filters.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    24040 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/validator/validator.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1417 2020-07-03 08:33:26.000000 optimade-0.9.8/optimade/validator/validator_model_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     5835 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2961 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       68 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1726 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2020-07-03 08:41:57.000000 optimade-0.9.8/optimade.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      121 2020-07-03 08:41:57.000000 optimade-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     3399 2020-07-03 08:33:26.000000 optimade-0.9.8/setup.py
```

### Comparing `optimade-0.9.7/PKG-INFO` & `optimade-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimade
-Version: 0.9.7
+Version: 0.9.8
 Summary: Tools for implementing and consuming OPTIMADE APIs.
 Home-page: https://github.com/Materials-Consortia/optimade-python-tools
 Author: OPTIMADE Development Team
 Author-email: dev@optimade.org
 License: MIT
 Description: # OPTIMADE Python tools
```

### Comparing `optimade-0.9.7/README.md` & `optimade-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/adapters/base.py` & `optimade-0.9.8/optimade/adapters/base.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/adapters/structures/__init__.py` & `optimade-0.9.8/optimade/adapters/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/adapters/structures/aiida.py` & `optimade-0.9.8/optimade/adapters/structures/aiida.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/adapters/structures/ase.py` & `optimade-0.9.8/optimade/adapters/structures/ase.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/adapters/structures/cif.py` & `optimade-0.9.8/optimade/adapters/structures/cif.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/adapters/structures/jarvis.py` & `optimade-0.9.8/optimade/adapters/structures/jarvis.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/adapters/structures/proteindatabank.py` & `optimade-0.9.8/optimade/adapters/structures/proteindatabank.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/adapters/structures/pymatgen.py` & `optimade-0.9.8/optimade/adapters/structures/pymatgen.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/adapters/structures/utils.py` & `optimade-0.9.8/optimade/adapters/structures/utils.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/filterparser/lark_parser.py` & `optimade-0.9.8/optimade/filterparser/lark_parser.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/filtertransformers/debug.py` & `optimade-0.9.8/optimade/filtertransformers/debug.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/filtertransformers/django.py` & `optimade-0.9.8/optimade/filtertransformers/django.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/filtertransformers/elasticsearch.py` & `optimade-0.9.8/optimade/filtertransformers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/filtertransformers/json.py` & `optimade-0.9.8/optimade/filtertransformers/json.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/filtertransformers/mongo.py` & `optimade-0.9.8/optimade/filtertransformers/mongo.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/grammar/v0.10.0.elastic.lark` & `optimade-0.9.8/optimade/grammar/v0.10.0.elastic.lark`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/grammar/v0.10.0.lark` & `optimade-0.9.8/optimade/grammar/v0.10.0.lark`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/grammar/v0.10.1.lark` & `optimade-0.9.8/optimade/grammar/v0.10.1.lark`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/grammar/v0.9.5.lark` & `optimade-0.9.8/optimade/grammar/v0.9.5.lark`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/grammar/v0.9.6.lark` & `optimade-0.9.8/optimade/grammar/v0.9.6.lark`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/grammar/v0.9.7.lark` & `optimade-0.9.8/optimade/grammar/v0.9.7.lark`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/models/__init__.py` & `optimade-0.9.8/optimade/models/__init__.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/models/baseinfo.py` & `optimade-0.9.8/optimade/models/baseinfo.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,16 +18,17 @@
         ...,
         description="A string specifying a versioned base URL that MUST adhere to the rules in section Base URL",
         pattern=r".+/v[0-1](\.[0-9]+)*/?$",
     )
 
     version: SemanticVersion = Field(
         ...,
-        description="A string containing the full version number of the API served at that versioned base URL. "
-        "The version number string MUST NOT be prefixed by, e.g., 'v'.",
+        description="""A string containing the full version number of the API served at that versioned base URL.
+The version number string MUST NOT be prefixed by, e.g., 'v'.
+Examples: `1.0.0`, `1.0.0-rc.2`.""",
     )
 
     @validator("url")
     def url_must_be_versioned_base_url(cls, v):
         """The URL must be a valid versioned Base URL"""
         if not re.match(r".+/v[0-1](\.[0-9]+)*/?$", v):
             raise ValueError(f"url MUST be a versioned base URL. It is: {v}")
@@ -55,15 +56,18 @@
         return values
 
 
 class BaseInfoAttributes(BaseModel):
     """Attributes for Base URL Info endpoint"""
 
     api_version: SemanticVersion = Field(
-        ..., description="Presently used version of the OPTIMADE API"
+        ...,
+        description="""Presently used full version of the OPTIMADE API.
+The version number string MUST NOT be prefixed by, e.g., "v".
+Examples: `1.0.0`, `1.0.0-rc.2`.""",
     )
     available_api_versions: List[AvailableApiVersion] = Field(
         ...,
         description="A list of dictionaries of available API versions at other base URLs",
     )
     formats: List[str] = Field(
         default=["json"], description="List of available output formats."
```

### Comparing `optimade-0.9.7/optimade/models/entries.py` & `optimade-0.9.8/optimade/models/entries.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
     description: str = Field(
         ..., description="A human-readable description of the entry property"
     )
 
     unit: Optional[str] = Field(
         None,
         description="""The physical unit of the entry property.
+This MUST be a valid representation of units according to version 2.1 of [The Unified Code for Units of Measure](https://unitsofmeasure.org/ucum.html).
 It is RECOMMENDED that non-standard (non-SI) units are described in the description for the property.""",
     )
 
     sortable: Optional[bool] = Field(
         None,
         description="""Defines whether the entry property can be used for sorting with the "sort" parameter.
 If the entry listing endpoint supports sorting, this key MUST be present for sortable properties with value `true`.""",
```

### Comparing `optimade-0.9.7/optimade/models/index_metadb.py` & `optimade-0.9.8/optimade/models/index_metadb.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/models/jsonapi.py` & `optimade-0.9.8/optimade/models/jsonapi.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/models/links.py` & `optimade-0.9.8/optimade/models/links.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/models/optimade_json.py` & `optimade-0.9.8/optimade/models/optimade_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -155,46 +155,42 @@
 
 
 class ResponseMetaQuery(BaseModel):
     """ Information on the query that was requested. """
 
     representation: str = Field(
         ...,
-        description="a string with the part of the URL that follows the base URL. Example: '/structures?'",
+        description="""A string with the part of the URL following the versioned or unversioned base URL that serves the API.
+Query parameters that have not been used in processing the request MAY be omitted.
+In particular, if no query parameters have been involved in processing the request, the query part of the URL MAY be excluded.
+Example: `/structures?filter=nelements=2`""",
     )
 
 
 class Provider(BaseModel):
     """Information on the database provider of the implementation."""
 
     name: str = Field(..., description="a short name for the database provider")
 
     description: str = Field(
         ..., description="a longer description of the database provider"
     )
 
     prefix: str = Field(
-        ..., description="database-provider-specific prefix as found in " "Appendix 1."
+        ...,
+        description="database-provider-specific prefix as found in section Database-Provider-Specific Namespace Prefixes.",
     )
 
     homepage: Optional[Union[AnyHttpUrl, jsonapi.Link]] = Field(
         None,
         description="a [JSON API links object](http://jsonapi.org/format/1.0#document-links) "
         "pointing to homepage of the database provider, either "
         "directly as a string, or as a link object.",
     )
 
-    index_base_url: Optional[Union[AnyHttpUrl, jsonapi.Link]] = Field(
-        None,
-        description="a [JSON API links object](http://jsonapi.org/format/1.0#document-links) "
-        "pointing to the base URL for the `index` meta-database as "
-        "specified in Appendix 1, either directly as a string, or "
-        "as a link object.",
-    )
-
 
 class ImplementationMaintainer(BaseModel):
     """Details about the maintainer of the implementation"""
 
     email: EmailStr = Field(..., description="the maintainer's email address")
 
 
@@ -203,17 +199,22 @@
 
     name: Optional[str] = Field(None, description="name of the implementation")
 
     version: Optional[str] = Field(
         None, description="version string of the current implementation"
     )
 
-    source_url: Optional[AnyUrl] = Field(
+    homepage: Optional[Union[AnyHttpUrl, jsonapi.Link]] = Field(
+        None,
+        description="A [JSON API links object](http://jsonapi.org/format/1.0/#document-links) pointing to the homepage of the implementation.",
+    )
+
+    source_url: Optional[Union[AnyUrl, jsonapi.Link]] = Field(
         None,
-        description="URL of the implementation source, either downloadable archive or version control system",
+        description="A [JSON API links object](http://jsonapi.org/format/1.0/#document-links) pointing to the implementation source, either downloadable archive or version control system.",
     )
 
     maintainer: Optional[ImplementationMaintainer] = Field(
         None,
         description="A dictionary providing details about the maintainer of the implementation.",
     )
 
@@ -230,37 +231,51 @@
     """
 
     query: ResponseMetaQuery = Field(
         ..., description="Information on the Query that was requested"
     )
 
     api_version: SemanticVersion = Field(
-        ..., description="A string containing the version of the API implementation.",
+        ...,
+        description="""Presently used full version of the OPTIMADE API.
+The version number string MUST NOT be prefixed by, e.g., "v".
+Examples: `1.0.0`, `1.0.0-rc.2`.""",
     )
 
-    time_stamp: datetime = Field(
+    more_data_available: bool = Field(
         ...,
+        description="`false` if the response contains all data for the request (e.g., a request issued to a single entry endpoint, or a `filter` query at the last page of a paginated response) and `true` if the response is incomplete in the sense that multiple objects match the request, and not all of them have been included in the response (e.g., a query with multiple pages that is not at the last page).",
+    )
+
+    # start of "SHOULD" fields for meta response
+    optimade_schema: Optional[Union[AnyHttpUrl, jsonapi.Link]] = Field(
+        None,
+        alias="schema",
+        description="""A [JSON API links object](http://jsonapi.org/format/1.0/#document-links) that points to a schema for the response.
+If it is a string, or a dictionary containing no `meta` field, the provided URL MUST point at an [OpenAPI](https://swagger.io/specification/) schema.
+It is possible that future versions of this specification allows for alternative schema types.
+Hence, if the `meta` field of the JSON API links object is provided and contains a field `schema_type` that is not equal to the string `OpenAPI` the client MUST not handle failures to parse the schema or to validate the response against the schema as errors.""",
+    )
+
+    time_stamp: Optional[datetime] = Field(
+        None,
         description="A timestamp containing the date and time at which the query was executed.",
     )
 
-    data_returned: int = Field(
-        ...,
+    data_returned: Optional[int] = Field(
+        None,
         description="An integer containing the total number of data resource objects returned for the current `filter` query, independent of pagination.",
         ge=0,
     )
 
-    more_data_available: bool = Field(
-        ...,
-        description="`false` if all data resource objects for this `filter` query have been returned in the response or if it is the last page of a paginated response, and `true` otherwise.",
-    )
-
-    provider: Provider = Field(
-        ..., description="information on the database provider of the implementation."
+    provider: Optional[Provider] = Field(
+        None, description="information on the database provider of the implementation."
     )
 
+    # start of "MAY" fields for meta response
     data_available: Optional[int] = Field(
         None,
         description="An integer containing the total number of data resource objects available in the database for the endpoint.",
     )
 
     last_id: Optional[str] = Field(
         None, description="a string containing the last ID returned"
@@ -284,16 +299,16 @@
         uniqueItems=True,
     )
 
 
 class Success(jsonapi.Response):
     """errors are not allowed"""
 
-    meta: Optional[ResponseMeta] = Field(
-        None, description="A meta object containing non-standard information"
+    meta: ResponseMeta = Field(
+        ..., description="A meta object containing non-standard information"
     )
 
     @root_validator(pre=True)
     def either_data_meta_or_errors_must_be_set(cls, values):
         """Overwriting the existing validation function, since 'errors' MUST NOT be set"""
         required_fields = ("data", "meta")
         if not any(values.get(field) for field in required_fields):
```

### Comparing `optimade-0.9.7/optimade/models/references.py` & `optimade-0.9.8/optimade/models/references.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/models/responses.py` & `optimade-0.9.8/optimade/models/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     "ReferenceResponseMany",
 )
 
 
 class ErrorResponse(Response):
     """errors MUST be present and data MUST be skipped"""
 
-    meta: Optional[ResponseMeta] = Field(
-        None, description="A meta object containing non-standard information"
+    meta: ResponseMeta = Field(
+        ..., description="A meta object containing non-standard information"
     )
     errors: List[OptimadeError] = Field(
         ...,
         description="A list of OPTIMADE-specific JSON API error objects, where the field detail MUST be present.",
         uniqueItems=True,
     )
```

### Comparing `optimade-0.9.7/optimade/models/structures.py` & `optimade-0.9.8/optimade/models/structures.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/models/utils.py` & `optimade-0.9.8/optimade/models/utils.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/config.py` & `optimade-0.9.8/optimade/server/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 from pathlib import Path
 
-from pydantic import BaseSettings, Field, root_validator
+from pydantic import (  # pylint: disable=no-name-in-module
+    BaseSettings,
+    Field,
+    root_validator,
+    AnyHttpUrl,
+    validator,
+)
 
 from optimade import __version__
 from optimade.models import Implementation, Provider
 
 
 DEFAULT_CONFIG_FILE_PATH = str(Path.home().joinpath(".optimade.json"))
 logger = logging.getLogger("optimade")
@@ -69,21 +75,24 @@
             name="Optimade Python Tools",
             version=__version__,
             source_url="https://github.com/Materials-Consortia/optimade-python-tools",
             maintainer={"email": "dev@optimade.org"},
         ),
         description="Introspective information about this OPTIMADE implementation",
     )
+    index_base_url: Optional[AnyHttpUrl] = Field(
+        None,
+        description="An optional link to the base URL for the index meta-database of the provider.",
+    )
     provider: Provider = Field(
         Provider(
             prefix="exmpl",
             name="Example provider",
             description="Provider used for examples, not to be assigned to a real database",
             homepage="https://example.com",
-            index_base_url="http://localhost:5001",
         ),
         description="General information about the provider of this OPTIMADE implementation",
     )
     provider_fields: Dict[
         Literal["links", "references", "structures"], List[str]
     ] = Field(
         {},
@@ -106,14 +115,21 @@
     )
 
     index_links_path: Path = Field(
         Path(__file__).parent.joinpath("index_links.json"),
         description="Absolute path to a JSON file containing the MongoDB collection of /links resources for the index meta-database",
     )
 
+    @validator("implementation", pre=True)
+    def set_implementation_version(cls, v):
+        """Set defaults and modify by passed value(s)"""
+        res = {"version": __version__}
+        res.update(v)
+        return res
+
     @root_validator(pre=True)
     def load_default_settings(cls, values):  # pylint: disable=no-self-argument
         """
         Loads settings from a root file if available and uses that as defaults in
         place of built in defaults
         """
         config_file_path = Path(values.get("config_file", DEFAULT_CONFIG_FILE_PATH))
```

### Comparing `optimade-0.9.7/optimade/server/data/__init__.py` & `optimade-0.9.8/optimade/server/data/__init__.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/data/providers.json` & `optimade-0.9.8/optimade/server/data/providers.json`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/data/test_references.json` & `optimade-0.9.8/optimade/server/data/test_references.json`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/data/test_structures.json` & `optimade-0.9.8/optimade/server/data/test_structures.json`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/data/test_structures_v0.9.7.json` & `optimade-0.9.8/optimade/server/data/test_structures_v0.9.7.json`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/entry_collections/entry_collections.py` & `optimade-0.9.8/optimade/server/entry_collections/entry_collections.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/entry_collections/mongo.py` & `optimade-0.9.8/optimade/server/entry_collections/mongo.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/exception_handlers.py` & `optimade-0.9.8/optimade/server/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/main.py` & `optimade-0.9.8/optimade/server/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from optimade import __api_version__, __version__
 import optimade.server.exception_handlers as exc_handlers
 
 from .entry_collections import MongoCollection
 from .config import CONFIG
 from .middleware import EnsureQueryParamIntegrity
-from .routers import info, links, references, structures, landing
+from .routers import info, links, references, structures, landing, versions
 from .routers.utils import get_providers, BASE_URL_PREFIXES
 
 
 if CONFIG.debug:  # pragma: no cover
     print("DEBUG MODE")
 
 
@@ -66,39 +66,36 @@
     RequestValidationError, exc_handlers.request_validation_exception_handler
 )
 app.add_exception_handler(ValidationError, exc_handlers.validation_exception_handler)
 app.add_exception_handler(VisitError, exc_handlers.grammar_not_implemented_handler)
 app.add_exception_handler(NotImplementedError, exc_handlers.not_implemented_handler)
 app.add_exception_handler(Exception, exc_handlers.general_exception_handler)
 
+# Add various endpoints to unversioned URL
+for endpoint in (info, links, references, structures, landing, versions):
+    app.include_router(endpoint.router)
 
-# Add various endpoints to `/vMAJOR`
-app.include_router(info.router, prefix=BASE_URL_PREFIXES["major"])
-app.include_router(links.router, prefix=BASE_URL_PREFIXES["major"])
-app.include_router(references.router, prefix=BASE_URL_PREFIXES["major"])
-app.include_router(structures.router, prefix=BASE_URL_PREFIXES["major"])
 
-
-# Add the router for the landing page for all prefixes
-app.include_router(landing.router)
-app.include_router(landing.router, prefix=BASE_URL_PREFIXES["major"])
+def add_major_version_base_url(app: FastAPI):
+    """ Add mandatory vMajor endpoints, i.e. all except versions. """
+    for endpoint in (info, links, references, structures, landing):
+        app.include_router(endpoint.router, prefix=BASE_URL_PREFIXES["major"])
 
 
 def add_optional_versioned_base_urls(app: FastAPI):
     """Add the following OPTIONAL prefixes/base URLs to server:
     ```
         /vMajor.Minor
         /vMajor.Minor.Patch
     ```
     """
     for version in ("minor", "patch"):
-        app.include_router(info.router, prefix=BASE_URL_PREFIXES[version])
-        app.include_router(links.router, prefix=BASE_URL_PREFIXES[version])
-        app.include_router(references.router, prefix=BASE_URL_PREFIXES[version])
-        app.include_router(structures.router, prefix=BASE_URL_PREFIXES[version])
-        app.include_router(landing.router, prefix=BASE_URL_PREFIXES[version])
+        for endpoint in (info, links, references, structures, landing):
+            app.include_router(endpoint.router, prefix=BASE_URL_PREFIXES[version])
 
 
 @app.on_event("startup")
 async def startup_event():
+    # Add API endpoints for MANDATORY base URL `/vMAJOR`
+    add_major_version_base_url(app)
     # Add API endpoints for OPTIONAL base URLs `/vMAJOR.MINOR` and `/vMAJOR.MINOR.PATCH`
     add_optional_versioned_base_urls(app)
```

### Comparing `optimade-0.9.7/optimade/server/main_index.py` & `optimade-0.9.8/optimade/server/main_index.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from fastapi.middleware.cors import CORSMiddleware
 
 from optimade import __api_version__, __version__
 import optimade.server.exception_handlers as exc_handlers
 
 from .config import CONFIG
 from .middleware import EnsureQueryParamIntegrity
-from .routers import index_info, links
+from .routers import index_info, links, versions
 from .routers.utils import BASE_URL_PREFIXES
 
 
 if CONFIG.debug:  # pragma: no cover
     print("DEBUG MODE")
 
 
@@ -69,17 +69,23 @@
     RequestValidationError, exc_handlers.request_validation_exception_handler
 )
 app.add_exception_handler(ValidationError, exc_handlers.validation_exception_handler)
 app.add_exception_handler(VisitError, exc_handlers.grammar_not_implemented_handler)
 app.add_exception_handler(Exception, exc_handlers.general_exception_handler)
 
 
-# Add various endpoints to `/vMAJOR`
-app.include_router(index_info.router, prefix=BASE_URL_PREFIXES["major"])
-app.include_router(links.router, prefix=BASE_URL_PREFIXES["major"])
+# Add all endpoints to unversioned URL
+for endpoint in (index_info, links, versions):
+    app.include_router(endpoint.router)
+
+
+def add_major_version_base_url(app: FastAPI):
+    """ Add mandatory endpoints to `/vMAJOR` base URL. """
+    for endpoint in (index_info, links):
+        app.include_router(links.router, prefix=BASE_URL_PREFIXES["major"])
 
 
 def add_optional_versioned_base_urls(app: FastAPI):
     """Add the following OPTIONAL prefixes/base URLs to server:
     ```
         /vMajor.Minor
         /vMajor.Minor.Patch
@@ -88,9 +94,11 @@
     for version in ("minor", "patch"):
         app.include_router(index_info.router, prefix=BASE_URL_PREFIXES[version])
         app.include_router(links.router, prefix=BASE_URL_PREFIXES[version])
 
 
 @app.on_event("startup")
 async def startup_event():
+    # Add API endpoints for MANDATORY base URL `/vMAJOR`
+    add_major_version_base_url(app)
     # Add API endpoints for OPTIONAL base URLs `/vMAJOR.MINOR` and `/vMAJOR.MINOR.PATCH`
     add_optional_versioned_base_urls(app)
```

### Comparing `optimade-0.9.7/optimade/server/mappers/entries.py` & `optimade-0.9.8/optimade/server/mappers/entries.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/mappers/links.py` & `optimade-0.9.8/optimade/server/mappers/links.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/middleware.py` & `optimade-0.9.8/optimade/server/middleware.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/query_params.py` & `optimade-0.9.8/optimade/server/query_params.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/routers/index_info.py` & `optimade-0.9.8/optimade/server/routers/index_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import urllib
 from typing import Union
 
 from fastapi import APIRouter, Request
 
 from optimade import __api_version__
 
 from optimade.models import (
@@ -11,37 +12,41 @@
     IndexInfoResource,
     IndexRelationship,
     RelatedLinksResource,
 )
 
 from optimade.server.config import CONFIG
 
-from .utils import meta_values
+from optimade.server.routers.utils import meta_values, get_base_url
 
 
 router = APIRouter(redirect_slashes=True)
 
 
 @router.get(
     "/info",
     response_model=Union[IndexInfoResponse, ErrorResponse],
     response_model_exclude_unset=True,
     tags=["Info"],
 )
 def get_info(request: Request):
+
+    parse_result = urllib.parse.urlparse(str(request.url))
+    base_url = get_base_url(parse_result)
+
     return IndexInfoResponse(
         meta=meta_values(str(request.url), 1, 1, more_data_available=False),
         data=IndexInfoResource(
             id=IndexInfoResource.schema()["properties"]["id"]["const"],
             type=IndexInfoResource.schema()["properties"]["type"]["const"],
             attributes=IndexInfoAttributes(
                 api_version=f"{__api_version__}",
                 available_api_versions=[
                     {
-                        "url": f"{CONFIG.provider.index_base_url}/v{__api_version__.split('.')[0]}/",
+                        "url": f"{base_url}/v{__api_version__.split('.')[0]}/",
                         "version": f"{__api_version__}",
                     }
                 ],
                 formats=["json"],
                 available_endpoints=["info", "links"],
                 entry_types_by_format={"json": []},
                 is_index=True,
```

### Comparing `optimade-0.9.7/optimade/server/routers/info.py` & `optimade-0.9.8/optimade/server/routers/info.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/routers/landing.py` & `optimade-0.9.8/optimade/server/routers/landing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """ OPTIMADE landing page, rendered as a Jinja2 template. """
 
 from pathlib import Path
 from fastapi.templating import Jinja2Templates
 from starlette.routing import Router, Route
 from optimade import __api_version__
 
-from . import ENTRY_COLLECTIONS
-from .utils import meta_values
+from optimade.server.routers import ENTRY_COLLECTIONS
+from optimade.server.routers.utils import meta_values
+from optimade.server.config import CONFIG
 
 template_dir = Path(__file__).parent.joinpath("static").resolve()
 TEMPLATES = Jinja2Templates(directory=[template_dir])
 
 
 async def landing(request):
     """ Show a human-readable landing page when the base URL is accessed. """
@@ -27,14 +28,15 @@
     context = {
         "request": request,
         "request_url": request.url,
         "api_version": __api_version__,
         "implementation": meta.implementation,
         "versioned_url": versioned_url,
         "provider": meta.provider,
+        "index_base_url": CONFIG.index_base_url,
         "endpoints": list(ENTRY_COLLECTIONS.keys()) + ["info"],
     }
 
     return TEMPLATES.TemplateResponse("landing_page.html", context)
 
 
 router = Router(routes=[Route("/", endpoint=landing)])
```

### Comparing `optimade-0.9.7/optimade/server/routers/links.py` & `optimade-0.9.8/optimade/server/routers/links.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/routers/references.py` & `optimade-0.9.8/optimade/server/routers/references.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/routers/static/landing_page.html` & `optimade-0.9.8/optimade/server/routers/static/landing_page.html`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,18 @@
         <p><a href={{ implementation.source_url }}>{{ implementation.source_url }}</a></p>
         <h3>Available endpoints:</h3>
         <ul>
         {% for endpoint in endpoints %}
         {{ '<li><a href="{}{}">{}{}</a></li>'.format(versioned_url, endpoint, versioned_url, endpoint) | safe }}
         {% endfor %}
         </ul>
-        <h3>Index base URL:</h3>
-        <p><a href={{ provider.index_base_url }}>{{ provider.index_base_url }}</a></p>
+        {% if index_base_url != None %}
+            <h3>Index base URL:</h3>
+            <p><a href={{ index_base_url }}>{{ index_base_url }}</a></p>
+        {% endif %}
     </body>
     <footer>
         <div class="footer_text">
             <ul style="list-style-type: none; margin: 0; padding:0; overflow: hidden">
                 <li style="padding-top: 5px;">Compliant with the <i class="fa fa-github"></i> <a href="https://github.com/Materials-Consortia/OPTIMADE">OPTIMADE specification</a>.</li>
                 <li style="padding-top: 5px;">Powered by <i class="fa fa-github"></i> <a href="https://www.github.com/Materials-Consortia/optimade-python-tools">Materials-Consortia/optimade-python-tools</a></li>
             </ul>
```

#### html2text {}

```diff
@@ -19,11 +19,13 @@
 Version: {{ implementation.version }}
 source_url }}>{{ implementation.source_url }}
 **** Available endpoints: ****
     * {% for endpoint in endpoints %} {{ '
     * {}{}
     * '.format(versioned_url, endpoint, versioned_url, endpoint) | safe }} {%
       endfor %}
+{% if index_base_url != None %}
 **** Index base URL: ****
-index_base_url }}>{{ provider.index_base_url }}
+}>{{ index_base_url }}
+{% endif %}
     * Compliant with the  OPTIMADE_specification.
     * Powered by  Materials-Consortia/optimade-python-tools
```

### Comparing `optimade-0.9.7/optimade/server/routers/structures.py` & `optimade-0.9.8/optimade/server/routers/structures.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/server/routers/utils.py` & `optimade-0.9.8/optimade/server/routers/utils.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/validator/__init__.py` & `optimade-0.9.8/optimade/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/validator/data/__init__.py` & `optimade-0.9.8/optimade/validator/data/__init__.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/validator/data/filters.txt` & `optimade-0.9.8/optimade/validator/data/filters.txt`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/validator/data/optional_filters.txt` & `optimade-0.9.8/optimade/validator/data/optional_filters.txt`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/validator/validator.py` & `optimade-0.9.8/optimade/validator/validator.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade/validator/validator_model_patches.py` & `optimade-0.9.8/optimade/validator/validator_model_patches.py`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/optimade.egg-info/PKG-INFO` & `optimade-0.9.8/optimade.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimade
-Version: 0.9.7
+Version: 0.9.8
 Summary: Tools for implementing and consuming OPTIMADE APIs.
 Home-page: https://github.com/Materials-Consortia/optimade-python-tools
 Author: OPTIMADE Development Team
 Author-email: dev@optimade.org
 License: MIT
 Description: # OPTIMADE Python tools
```

### Comparing `optimade-0.9.7/optimade.egg-info/SOURCES.txt` & `optimade-0.9.8/optimade.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 optimade/server/routers/index_info.py
 optimade/server/routers/info.py
 optimade/server/routers/landing.py
 optimade/server/routers/links.py
 optimade/server/routers/references.py
 optimade/server/routers/structures.py
 optimade/server/routers/utils.py
+optimade/server/routers/versions.py
 optimade/server/routers/static/landing_page.html
 optimade/validator/__init__.py
 optimade/validator/validator.py
 optimade/validator/validator_model_patches.py
 optimade/validator/data/__init__.py
 optimade/validator/data/filters.txt
 optimade/validator/data/optional_filters.txt
```

### Comparing `optimade-0.9.7/optimade.egg-info/requires.txt` & `optimade-0.9.8/optimade.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `optimade-0.9.7/setup.py` & `optimade-0.9.8/setup.py`

 * *Files identical despite different names*

