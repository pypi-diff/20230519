# Comparing `tmp/cognite_neat-0.11.1.tar.gz` & `tmp/cognite_neat-0.11.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.11.1.tar", max compression
+gzip compressed data, was "cognite_neat-0.11.2.tar", max compression
```

## Comparing `cognite_neat-0.11.1.tar` & `cognite_neat-0.11.2.tar`

### file list

```diff
@@ -1,79 +1,80 @@
--rw-r--r--   0        0        0    11351 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/LICENSE
--rw-r--r--   0        0        0     8748 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/README.md
--rw-r--r--   0        0        0       23 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/__init__.py
--rw-r--r--   0        0        0      532 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2652 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/app.py
--rw-r--r--   0        0        0     1344 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0      408 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/data_classes/__init__.py
--rw-r--r--   0        0        0     4623 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/data_classes/config.py
--rw-r--r--   0        0        0     8132 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/data_classes/rules.py
--rw-r--r--   0        0        0    27182 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/data_classes/transformation_rules.py
--rw-r--r--   0        0        0        0 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     9436 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0      391 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     2250 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/extractors/labels.py
--rw-r--r--   0        0        0    32717 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/extractors/rdf_to_assets.py
--rw-r--r--   0        0        0    16632 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/extractors/rdf_to_relationships.py
--rw-r--r--   0        0        0      115 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0    10574 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0      913 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/loader/rules.py
--rw-r--r--   0        0        0        0 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    12025 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0    15303 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/modeler.py
--rw-r--r--   0        0        0      110 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/parser/__init__.py
--rw-r--r--   0        0        0     1727 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/parser/transformation_rules.py
--rw-r--r--   0        0        0       73 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9595 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0    10943 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0     3621 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/utils.py
--rw-r--r--   0        0        0     2558 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      311 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    15521 2023-05-08 11:27:57.893179 cognite_neat-0.11.1/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17630 2023-05-08 11:27:57.897179 cognite_neat-0.11.1/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0     6183 2023-05-08 11:27:57.897179 cognite_neat-0.11.1/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     3201 2023-05-08 11:27:57.897179 cognite_neat-0.11.1/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0      781 2023-05-08 11:27:57.897179 cognite_neat-0.11.1/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     5186 2023-05-08 11:27:57.897179 cognite_neat-0.11.1/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-05-08 11:27:57.897179 cognite_neat-0.11.1/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0      509 2023-05-08 11:27:57.897179 cognite_neat-0.11.1/cognite/neat/examples/config.yaml
--rw-r--r--   0        0        0    79580 2023-05-08 11:27:57.897179 cognite_neat-0.11.1/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    52178 2023-05-08 11:27:57.897179 cognite_neat-0.11.1/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1155 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1771 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15541 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6763 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0    15552 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/examples/workflows/fast_graph/workflow.py
--rw-r--r--   0        0        0     6959 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/examples/workflows/fast_graph/workflow.yaml
--rw-r--r--   0        0        0    11477 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4781 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0    13084 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6014 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0        0 2023-05-08 11:27:57.937180 cognite_neat-0.11.1/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 11:27:57.937180 cognite_neat-0.11.1/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1013 2023-05-08 11:27:57.937180 cognite_neat-0.11.1/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    18930 2023-05-08 11:27:57.937180 cognite_neat-0.11.1/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-05-08 11:27:57.937180 cognite_neat-0.11.1/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-05-08 11:27:57.937180 cognite_neat-0.11.1/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4003 2023-05-08 11:27:57.937180 cognite_neat-0.11.1/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css
--rw-r--r--   0        0        0    13320 2023-05-08 11:27:57.901179 cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css.map
--rw-r--r--   0        0        0  1318896 2023-05-08 11:27:57.909179 cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js
--rw-r--r--   0        0        0     2667 2023-05-08 11:27:57.909179 cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.LICENSE.txt
--rw-r--r--   0        0        0  5708777 2023-05-08 11:27:57.933180 cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.map
--rw-r--r--   0        0        0     2633 2023-05-08 11:27:57.933180 cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-05-08 11:27:57.937180 cognite_neat-0.11.1/cognite/neat/main.py
--rw-r--r--   0        0        0     1981 2023-05-08 11:27:58.221182 cognite_neat-0.11.1/pyproject.toml
--rw-r--r--   0        0        0     9778 1970-01-01 00:00:00.000000 cognite_neat-0.11.1/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/LICENSE
+-rw-r--r--   0        0        0     8748 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/README.md
+-rw-r--r--   0        0        0       23 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/__init__.py
+-rw-r--r--   0        0        0      616 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/constants.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/__init__.py
+-rw-r--r--   0        0        0     2652 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/app.py
+-rw-r--r--   0        0        0     1344 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/configuration.py
+-rw-r--r--   0        0        0      408 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/data_classes/__init__.py
+-rw-r--r--   0        0        0     4623 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/data_classes/config.py
+-rw-r--r--   0        0        0     8132 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/data_classes/rules.py
+-rw-r--r--   0        0        0    28433 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/data_classes/transformation_rules.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/data_stores/__init__.py
+-rw-r--r--   0        0        0     9436 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0      470 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/extractors/__init__.py
+-rw-r--r--   0        0        0     2250 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/extractors/labels.py
+-rw-r--r--   0        0        0    32717 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/extractors/rdf_to_assets.py
+-rw-r--r--   0        0        0    16632 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/extractors/rdf_to_relationships.py
+-rw-r--r--   0        0        0     6700 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/extractors/rules_to_graphql.py
+-rw-r--r--   0        0        0      115 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/loader/__init__.py
+-rw-r--r--   0        0        0      711 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/loader/config.py
+-rw-r--r--   0        0        0     1210 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/loader/graph.py
+-rw-r--r--   0        0        0    10647 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/loader/graph_store.py
+-rw-r--r--   0        0        0      913 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/loader/rules.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/mocks/__init__.py
+-rw-r--r--   0        0        0    12025 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/mocks/graph.py
+-rw-r--r--   0        0        0    15303 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/modeler.py
+-rw-r--r--   0        0        0      110 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/parser/__init__.py
+-rw-r--r--   0        0        0     1727 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/parser/transformation_rules.py
+-rw-r--r--   0        0        0       73 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/query_generator/__init__.py
+-rw-r--r--   0        0        0     9595 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/query_generator/sparql.py
+-rw-r--r--   0        0        0    10943 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/transformer.py
+-rw-r--r--   0        0        0     3621 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/utils.py
+-rw-r--r--   0        0        0     2558 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/validator.py
+-rw-r--r--   0        0        0      311 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/workflow/__init__.py
+-rw-r--r--   0        0        0    15521 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/workflow/base.py
+-rw-r--r--   0        0        0    17630 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/core/workflow/cdf_store.py
+-rw-r--r--   0        0        0     6183 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/core/workflow/manager.py
+-rw-r--r--   0        0        0     3201 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/core/workflow/model.py
+-rw-r--r--   0        0        0      781 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/core/workflow/tasks.py
+-rw-r--r--   0        0        0     5186 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/core/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/core/workflow/utils.py
+-rw-r--r--   0        0        0      509 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/examples/config.yaml
+-rw-r--r--   0        0        0    79580 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    52178 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1155 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1771 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15541 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6763 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0    15552 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/fast_graph/workflow.py
+-rw-r--r--   0        0        0     6958 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/fast_graph/workflow.yaml
+-rw-r--r--   0        0        0    11477 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4781 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0    13084 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6014 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-05-19 07:56:39.548655 cognite_neat-0.11.2/cognite/neat/explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:56:39.548655 cognite_neat-0.11.2/cognite/neat/explorer/data_classes/__init__.py
+-rw-r--r--   0        0        0     1013 2023-05-19 07:56:39.548655 cognite_neat-0.11.2/cognite/neat/explorer/data_classes/rest.py
+-rw-r--r--   0        0        0    18989 2023-05-19 07:56:39.552655 cognite_neat-0.11.2/cognite/neat/explorer/explorer.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:56:39.552655 cognite_neat-0.11.2/cognite/neat/explorer/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-05-19 07:56:39.552655 cognite_neat-0.11.2/cognite/neat/explorer/utils/data_mapping.py
+-rw-r--r--   0        0        0     4003 2023-05-19 07:56:39.552655 cognite_neat-0.11.2/cognite/neat/explorer/utils/query_templates.py
+-rw-r--r--   0        0        0       16 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/index.html
+-rw-r--r--   0        0        0      312 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css
+-rw-r--r--   0        0        0    13320 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css.map
+-rw-r--r--   0        0        0  1318896 2023-05-19 07:56:39.512655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js
+-rw-r--r--   0        0        0     2667 2023-05-19 07:56:39.512655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.LICENSE.txt
+-rw-r--r--   0        0        0  5708777 2023-05-19 07:56:39.544655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.map
+-rw-r--r--   0        0        0     2633 2023-05-19 07:56:39.544655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      358 2023-05-19 07:56:39.552655 cognite_neat-0.11.2/cognite/neat/main.py
+-rw-r--r--   0        0        0     2005 2023-05-19 07:56:39.908660 cognite_neat-0.11.2/pyproject.toml
+-rw-r--r--   0        0        0     9823 1970-01-01 00:00:00.000000 cognite_neat-0.11.2/PKG-INFO
```

### Comparing `cognite_neat-0.11.1/LICENSE` & `cognite_neat-0.11.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/README.md` & `cognite_neat-0.11.2/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/app.py` & `cognite_neat-0.11.2/cognite/neat/core/app.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/configuration.py` & `cognite_neat-0.11.2/cognite/neat/core/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/data_classes/config.py` & `cognite_neat-0.11.2/cognite/neat/core/data_classes/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/data_classes/rules.py` & `cognite_neat-0.11.2/cognite/neat/core/data_classes/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/data_classes/transformation_rules.py` & `cognite_neat-0.11.2/cognite/neat/core/data_classes/transformation_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,36 +3,35 @@
 import logging
 import math
 import warnings
 from datetime import datetime
 from typing import Dict, List, Optional, Self, Union
 
 import pandas as pd
+from graphql import GraphQLBoolean, GraphQLFloat, GraphQLInt, GraphQLString
 from pydantic import BaseModel, Field, HttpUrl, ValidationError, root_validator, validator
 from rdflib import XSD, Literal, Namespace, URIRef
 
 from cognite.neat.core.configuration import PREFIXES, Tables
 from cognite.neat.core.data_classes.rules import Entity, RuleType, parse_rule
 
 # mapping of XSD types to Python and GraphQL types
 DATA_TYPE_MAPPING = {
-    "boolean": {"python": "bool", "GraphQL": "Boolean"},
-    "float": {"python": "float", "GraphQL": "Float"},
-    "integer": {"python": "int", "GraphQL": "Int"},
-    "nonPositiveInteger": {"python": "int", "GraphQL": "Int"},
-    "nonNegativeInteger": {"python": "int", "GraphQL": "Int"},
-    "negativeInteger": {"python": "int", "GraphQL": "Int"},
-    "long": {"python": "int", "GraphQL": "Int"},
-    "string": {"python": "str", "GraphQL": "String"},
-    "anyURI": {"python": "str", "GraphQL": "String"},
-    "normalizedString": {"python": "str", "GraphQL": "String"},
-    "token": {"python": "str", "GraphQL": "String"},
-    "enumeration": {"python": "list", "GraphQL": "Enum"},
+    "boolean": {"python": "bool", "GraphQL": GraphQLBoolean},
+    "float": {"python": "float", "GraphQL": GraphQLFloat},
+    "integer": {"python": "int", "GraphQL": GraphQLInt},
+    "nonPositiveInteger": {"python": "int", "GraphQL": GraphQLInt},
+    "nonNegativeInteger": {"python": "int", "GraphQL": GraphQLInt},
+    "negativeInteger": {"python": "int", "GraphQL": GraphQLInt},
+    "long": {"python": "int", "GraphQL": GraphQLInt},
+    "string": {"python": "str", "GraphQL": GraphQLString},
+    "anyURI": {"python": "str", "GraphQL": GraphQLString},
+    "normalizedString": {"python": "str", "GraphQL": GraphQLString},
+    "token": {"python": "str", "GraphQL": GraphQLString},
 }
-
 METADATA_VALUE_MAX_LENGTH = 5120
 
 
 class URL(BaseModel):
     url: HttpUrl
 
 
@@ -96,46 +95,48 @@
     resource_type_property: List[str] = Field(alias="Resource Type Property", default=None)
     source_type: str = Field(alias="Relationship Source Type", default="Asset")
     target_type: str = Field(alias="Relationship Target Type", default="Asset")
     label: str = Field(alias="Relationship Label", default=None)
     relationship_external_id_rule: str = Field(alias="Relationship ExternalID Rule", default=None)
 
     # Transformation rule (domain to solution)
-    rule_type: RuleType = Field(alias="Rule Type")
-    rule: str = Field(alias="Rule")
+    rule_type: RuleType = Field(alias="Rule Type", default=None)
+    rule: str = Field(alias="Rule", default=None)
     skip_rule: bool = Field(alias="Skip", default=False)
 
     # Specialization of cdf_resource_type to allow definition of both
     # Asset and Relationship at the same time
     cdf_resource_type: list[str] = Field(alias="Resource Type")
 
     @property
     def is_raw_lookup(self) -> bool:
         return self.rule_type == RuleType.rawlookup
 
-    @validator("rule_type", pre=True)
-    def to_lowercase(cls, value):
-        return value.casefold()
-
     @validator(
         "max_count",
         "min_count",
         "target_type",
         "source_type",
         "label",
         "relationship_external_id_rule",
         "resource_type_property",
         "skip_rule",
+        "rule",
+        "rule_type",
         pre=True,
     )
     def replace_float_nan_with_default(cls, value, field):
         if isinstance(value, float) and math.isnan(value):
             return field.default
         return value
 
+    @validator("rule_type", pre=True)
+    def to_lowercase(cls, value):
+        return value.casefold() if value else value
+
     @validator("skip_rule", pre=True)
     def from_string(cls, value):
         if isinstance(value, str):
             return value.casefold() in {"true", "skip", "yes", "y"}
         return value
 
     @validator("rule")
@@ -167,14 +168,21 @@
     @validator("property_type", pre=True, always=True)
     def set_property_type(cls, value, values):
         if values["expected_value_type"] in DATA_TYPE_MAPPING.keys():
             return "DatatypeProperty"
         else:
             return "ObjectProperty"
 
+    @validator("skip_rule", pre=True, always=True)
+    def no_rule(cls, value, values):
+        if values.get("rule_type") is None:
+            return True
+        else:
+            return value
+
 
 class Metadata(BaseModel):
     prefix: str = Field(alias="shortName")
     namespace: Namespace = None
     version: str
     isCurrentVersion: bool = True
     created: datetime
@@ -412,14 +420,26 @@
             if class_ in class_property_pairs:
                 class_property_pairs[class_] += [property_]
             else:
                 class_property_pairs[class_] = [property_]
 
         return class_property_pairs
 
+    def check_data_model_definitions(self):
+        """Check if data model definitions are valid."""
+        issues = set()
+        for class_, properties in self.get_classes_with_properties().items():
+            analyzed_properties = []
+            for property in properties:
+                if property.property_name not in analyzed_properties:
+                    analyzed_properties.append(property.property_name)
+                else:
+                    issues.add(f"Property {property.property_name} of class {class_} has been defined more than once!")
+        return issues
+
     def reduce_data_model(self, desired_classes: set, skip_validation: bool = False) -> TransformationRules:
         """Reduce the data model to only include desired classes and their properties.
 
         Parameters
         ----------
         desired_classes : set
             Desired classes to include in the reduced data model
@@ -599,14 +619,22 @@
             return RelationshipDefinitions(
                 data_set_id=self.metadata.data_set_id,
                 prefix=self.metadata.prefix,
                 namespace=self.metadata.namespace,
                 relationships={},
             )
 
+    def get_entity_names(self):
+        class_names = set()
+        property_names = set()
+        for class_, properties in self.to_dataframe().items():
+            class_names.add(class_)
+            property_names = property_names.union(set(properties.index))
+        return class_names.union(property_names)
+
 
 class AssetClassMapping(BaseModel):
     external_id: str
     name: str
     parent_external_id: Optional[str]
     description: Optional[str]
     metadata: Optional[dict] = {}
```

### Comparing `cognite_neat-0.11.1/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.11.2/cognite/neat/core/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/extractors/labels.py` & `cognite_neat-0.11.2/cognite/neat/core/extractors/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/extractors/rdf_to_assets.py` & `cognite_neat-0.11.2/cognite/neat/core/extractors/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/extractors/rdf_to_relationships.py` & `cognite_neat-0.11.2/cognite/neat/core/extractors/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/loader/config.py` & `cognite_neat-0.11.2/cognite/neat/core/loader/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/loader/graph.py` & `cognite_neat-0.11.2/cognite/neat/core/loader/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.11.2/cognite/neat/core/loader/graph_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         if self.rdf_store_type in ["", RdfStoreType.MEMORY]:
             logging.info("Initializing graph in memory")
             self.graph = Graph()
         elif self.rdf_store_type == RdfStoreType.OXIGRAPH:
             logging.info("Initializing Oxigraph store")
             # Adding support for both in-memory and file-based storage
             oxstore = None
+            self.internal_storage_dir.mkdir(parents=True, exist_ok=True)
             for i in range(4):
                 try:
                     oxstore = pyoxigraph.Store(
                         path=str(self.internal_storage_dir) if self.internal_storage_dir else None
                     )  # Store (Rust object) accepts only str as path and not Path.
                     break
                 except OSError as e:
```

### Comparing `cognite_neat-0.11.1/cognite/neat/core/loader/rules.py` & `cognite_neat-0.11.2/cognite/neat/core/loader/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.11.2/cognite/neat/core/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/modeler.py` & `cognite_neat-0.11.2/cognite/neat/core/modeler.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/parser/transformation_rules.py` & `cognite_neat-0.11.2/cognite/neat/core/parser/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.11.2/cognite/neat/core/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/transformer.py` & `cognite_neat-0.11.2/cognite/neat/core/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/utils.py` & `cognite_neat-0.11.2/cognite/neat/core/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/validator.py` & `cognite_neat-0.11.2/cognite/neat/core/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/workflow/base.py` & `cognite_neat-0.11.2/cognite/neat/core/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.11.2/cognite/neat/core/workflow/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.11.2/cognite/neat/core/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/workflow/model.py` & `cognite_neat-0.11.2/cognite/neat/core/workflow/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.11.2/cognite/neat/core/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.11.2/cognite/neat/core/workflow/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.11.2/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.11.2/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.11.2/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.11.2/cognite/neat/examples/workflows/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.11.2/cognite/neat/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.11.2/cognite/neat/examples/workflows/default/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.11.2/cognite/neat/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/examples/workflows/fast_graph/workflow.py` & `cognite_neat-0.11.2/cognite/neat/examples/workflows/fast_graph/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/examples/workflows/fast_graph/workflow.yaml` & `cognite_neat-0.11.2/cognite/neat/examples/workflows/fast_graph/workflow.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
     stype: pystep
     transition_to: []
     trigger: false
     ui_config:
         pos_x: 114
         pos_y: 874
 -   description: Upload CDF labels
-    enabled: false
+    enabled: true
     group_id: null
     id: create_cdf_labels
     label: Upload CDF labels
     method: null
     params: {}
     stype: pystep
     transition_to:
```

### Comparing `cognite_neat-0.11.1/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.11.2/cognite/neat/examples/workflows/graph_db_import/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.11.2/cognite/neat/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/examples/workflows/sheet2cdf/workflow.py` & `cognite_neat-0.11.2/cognite/neat/examples/workflows/sheet2cdf/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.11.2/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/explorer/data_classes/rest.py` & `cognite_neat-0.11.2/cognite/neat/explorer/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/explorer/explorer.py` & `cognite_neat-0.11.2/cognite/neat/explorer/explorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,24 +53,25 @@
 logging.info(f" Starting NEAT version {neat.__version__}")
 logging.debug(f" Config: {config.dict(exclude={'cdf_client': {'client_secret': ...}})}")
 
 neat_app = NeatApp(config)
 
 
 @asynccontextmanager
-async def lifespan(app: FastAPI):
+async def lifespan(app_ref: FastAPI):
+    logging.info("Startup FastAPI server")
+    neat_app.set_http_server(app_ref)
+    neat_app.start()
     yield
     logging.info("FastApi shutdown event")
     neat_app.stop()
 
 
 app = FastAPI(title="Neat", lifespan=lifespan)
 
-neat_app.set_http_server(app)
-neat_app.start()
 
 origins = [
     "http://localhost:8000",
     "http://localhost:3000",
 ]
 
 app.add_middleware(
```

### Comparing `cognite_neat-0.11.1/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.11.2/cognite/neat/explorer/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css` & `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css.map` & `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js` & `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.LICENSE.txt` & `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.map` & `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.1/pyproject.toml` & `cognite_neat-0.11.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.11.1"
+version = "0.11.2"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 packages = [
@@ -50,14 +50,15 @@
 prometheus-client = "^0.16.0"
 cognite-sdk = "^6"
 deepdiff = "*"
 fastapi = "^0.95"
 schedule = "^1"
 python-multipart = "^0.0.6"
 oxrdflib = {version = "^0.3.3", extras = ["oxigraph"]}
+graphql-core = "^3.2.3"
 
 [tool.poetry.dev-dependencies]
 twine = "*"
 pytest = "*"
 pytest-cov = "*"
 pre-commit = "*"
 safety = "*"
```

### Comparing `cognite_neat-0.11.1/PKG-INFO` & `cognite_neat-0.11.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.11.1
+Version: 0.11.2
 Summary: Knowledge graph transformation
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML
 Requires-Dist: cognite-sdk (>=6,<7)
 Requires-Dist: deepdiff
 Requires-Dist: fastapi (>=0.95,<0.96)
 Requires-Dist: google-api-python-client
 Requires-Dist: google-auth-oauthlib
+Requires-Dist: graphql-core (>=3.2.3,<4.0.0)
 Requires-Dist: gspread
 Requires-Dist: openpyxl
 Requires-Dist: oxrdflib[oxigraph] (>=0.3.3,<0.4.0)
 Requires-Dist: pandas
 Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
 Requires-Dist: pydantic
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
```

