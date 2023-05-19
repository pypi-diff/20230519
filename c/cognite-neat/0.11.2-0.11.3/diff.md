# Comparing `tmp/cognite_neat-0.11.2.tar.gz` & `tmp/cognite_neat-0.11.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.11.2.tar", max compression
+gzip compressed data, was "cognite_neat-0.11.3.tar", max compression
```

## Comparing `cognite_neat-0.11.2.tar` & `cognite_neat-0.11.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0    11351 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/LICENSE
--rw-r--r--   0        0        0     8748 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/README.md
--rw-r--r--   0        0        0       23 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/__init__.py
--rw-r--r--   0        0        0      616 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2652 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/app.py
--rw-r--r--   0        0        0     1344 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0      408 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/data_classes/__init__.py
--rw-r--r--   0        0        0     4623 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/data_classes/config.py
--rw-r--r--   0        0        0     8132 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/data_classes/rules.py
--rw-r--r--   0        0        0    28433 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/data_classes/transformation_rules.py
--rw-r--r--   0        0        0        0 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     9436 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0      470 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     2250 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/extractors/labels.py
--rw-r--r--   0        0        0    32717 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/extractors/rdf_to_assets.py
--rw-r--r--   0        0        0    16632 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/extractors/rdf_to_relationships.py
--rw-r--r--   0        0        0     6700 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/extractors/rules_to_graphql.py
--rw-r--r--   0        0        0      115 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0    10647 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0      913 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/loader/rules.py
--rw-r--r--   0        0        0        0 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    12025 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0    15303 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/modeler.py
--rw-r--r--   0        0        0      110 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/parser/__init__.py
--rw-r--r--   0        0        0     1727 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/parser/transformation_rules.py
--rw-r--r--   0        0        0       73 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9595 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0    10943 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0     3621 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/utils.py
--rw-r--r--   0        0        0     2558 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      311 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    15521 2023-05-19 07:56:39.496655 cognite_neat-0.11.2/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17630 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0     6183 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     3201 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0      781 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     5186 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0      509 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/examples/config.yaml
--rw-r--r--   0        0        0    79580 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    52178 2023-05-19 07:56:39.500655 cognite_neat-0.11.2/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1155 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1771 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15541 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6763 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0    15552 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/fast_graph/workflow.py
--rw-r--r--   0        0        0     6958 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/fast_graph/workflow.yaml
--rw-r--r--   0        0        0    11477 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4781 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0    13084 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6014 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0        0 2023-05-19 07:56:39.548655 cognite_neat-0.11.2/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 07:56:39.548655 cognite_neat-0.11.2/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1013 2023-05-19 07:56:39.548655 cognite_neat-0.11.2/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    18989 2023-05-19 07:56:39.552655 cognite_neat-0.11.2/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-05-19 07:56:39.552655 cognite_neat-0.11.2/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-05-19 07:56:39.552655 cognite_neat-0.11.2/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4003 2023-05-19 07:56:39.552655 cognite_neat-0.11.2/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css
--rw-r--r--   0        0        0    13320 2023-05-19 07:56:39.504655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css.map
--rw-r--r--   0        0        0  1318896 2023-05-19 07:56:39.512655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js
--rw-r--r--   0        0        0     2667 2023-05-19 07:56:39.512655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.LICENSE.txt
--rw-r--r--   0        0        0  5708777 2023-05-19 07:56:39.544655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.map
--rw-r--r--   0        0        0     2633 2023-05-19 07:56:39.544655 cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-05-19 07:56:39.552655 cognite_neat-0.11.2/cognite/neat/main.py
--rw-r--r--   0        0        0     2005 2023-05-19 07:56:39.908660 cognite_neat-0.11.2/pyproject.toml
--rw-r--r--   0        0        0     9823 1970-01-01 00:00:00.000000 cognite_neat-0.11.2/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/LICENSE
+-rw-r--r--   0        0        0     8748 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/README.md
+-rw-r--r--   0        0        0       23 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/__init__.py
+-rw-r--r--   0        0        0      616 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/constants.py
+-rw-r--r--   0        0        0        0 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/__init__.py
+-rw-r--r--   0        0        0     2652 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/app.py
+-rw-r--r--   0        0        0     1344 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/configuration.py
+-rw-r--r--   0        0        0      408 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/data_classes/__init__.py
+-rw-r--r--   0        0        0     4623 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/data_classes/config.py
+-rw-r--r--   0        0        0     8132 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/data_classes/rules.py
+-rw-r--r--   0        0        0    28433 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/data_classes/transformation_rules.py
+-rw-r--r--   0        0        0        0 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/data_stores/__init__.py
+-rw-r--r--   0        0        0     9436 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0      470 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/extractors/__init__.py
+-rw-r--r--   0        0        0     2250 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/extractors/labels.py
+-rw-r--r--   0        0        0    32700 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/extractors/rdf_to_assets.py
+-rw-r--r--   0        0        0    16632 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/extractors/rdf_to_relationships.py
+-rw-r--r--   0        0        0     6700 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/extractors/rules_to_graphql.py
+-rw-r--r--   0        0        0      115 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/loader/__init__.py
+-rw-r--r--   0        0        0      711 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/loader/config.py
+-rw-r--r--   0        0        0     1210 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/loader/graph.py
+-rw-r--r--   0        0        0    10647 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/loader/graph_store.py
+-rw-r--r--   0        0        0      913 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/loader/rules.py
+-rw-r--r--   0        0        0        0 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/mocks/__init__.py
+-rw-r--r--   0        0        0    12025 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/mocks/graph.py
+-rw-r--r--   0        0        0    15303 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/modeler.py
+-rw-r--r--   0        0        0      110 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/parser/__init__.py
+-rw-r--r--   0        0        0     1727 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/parser/transformation_rules.py
+-rw-r--r--   0        0        0       73 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/query_generator/__init__.py
+-rw-r--r--   0        0        0     9595 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/query_generator/sparql.py
+-rw-r--r--   0        0        0    10943 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/transformer.py
+-rw-r--r--   0        0        0     3621 2023-05-19 09:26:01.304526 cognite_neat-0.11.3/cognite/neat/core/utils.py
+-rw-r--r--   0        0        0     2558 2023-05-19 09:26:01.308526 cognite_neat-0.11.3/cognite/neat/core/validator.py
+-rw-r--r--   0        0        0      311 2023-05-19 09:26:01.308526 cognite_neat-0.11.3/cognite/neat/core/workflow/__init__.py
+-rw-r--r--   0        0        0    15521 2023-05-19 09:26:01.308526 cognite_neat-0.11.3/cognite/neat/core/workflow/base.py
+-rw-r--r--   0        0        0    17630 2023-05-19 09:26:01.308526 cognite_neat-0.11.3/cognite/neat/core/workflow/cdf_store.py
+-rw-r--r--   0        0        0     6183 2023-05-19 09:26:01.308526 cognite_neat-0.11.3/cognite/neat/core/workflow/manager.py
+-rw-r--r--   0        0        0     3201 2023-05-19 09:26:01.308526 cognite_neat-0.11.3/cognite/neat/core/workflow/model.py
+-rw-r--r--   0        0        0      781 2023-05-19 09:26:01.308526 cognite_neat-0.11.3/cognite/neat/core/workflow/tasks.py
+-rw-r--r--   0        0        0     5186 2023-05-19 09:26:01.308526 cognite_neat-0.11.3/cognite/neat/core/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-05-19 09:26:01.308526 cognite_neat-0.11.3/cognite/neat/core/workflow/utils.py
+-rw-r--r--   0        0        0      509 2023-05-19 09:26:01.308526 cognite_neat-0.11.3/cognite/neat/examples/config.yaml
+-rw-r--r--   0        0        0    79580 2023-05-19 09:26:01.308526 cognite_neat-0.11.3/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    52178 2023-05-19 09:26:01.308526 cognite_neat-0.11.3/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1155 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1771 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15541 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6763 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0    15552 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/examples/workflows/fast_graph/workflow.py
+-rw-r--r--   0        0        0     6958 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/examples/workflows/fast_graph/workflow.yaml
+-rw-r--r--   0        0        0    11477 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4781 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0    13084 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6014 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-05-19 09:26:01.356526 cognite_neat-0.11.3/cognite/neat/explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 09:26:01.356526 cognite_neat-0.11.3/cognite/neat/explorer/data_classes/__init__.py
+-rw-r--r--   0        0        0     1013 2023-05-19 09:26:01.356526 cognite_neat-0.11.3/cognite/neat/explorer/data_classes/rest.py
+-rw-r--r--   0        0        0    18989 2023-05-19 09:26:01.356526 cognite_neat-0.11.3/cognite/neat/explorer/explorer.py
+-rw-r--r--   0        0        0        0 2023-05-19 09:26:01.356526 cognite_neat-0.11.3/cognite/neat/explorer/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-05-19 09:26:01.356526 cognite_neat-0.11.3/cognite/neat/explorer/utils/data_mapping.py
+-rw-r--r--   0        0        0     4003 2023-05-19 09:26:01.356526 cognite_neat-0.11.3/cognite/neat/explorer/utils/query_templates.py
+-rw-r--r--   0        0        0       16 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/explorer-ui/index.html
+-rw-r--r--   0        0        0      312 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css
+-rw-r--r--   0        0        0    13320 2023-05-19 09:26:01.312526 cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css.map
+-rw-r--r--   0        0        0  1318896 2023-05-19 09:26:01.320526 cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js
+-rw-r--r--   0        0        0     2667 2023-05-19 09:26:01.320526 cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.LICENSE.txt
+-rw-r--r--   0        0        0  5708777 2023-05-19 09:26:01.348526 cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.map
+-rw-r--r--   0        0        0     2633 2023-05-19 09:26:01.348526 cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      358 2023-05-19 09:26:01.356526 cognite_neat-0.11.3/cognite/neat/main.py
+-rw-r--r--   0        0        0     2005 2023-05-19 09:26:01.700527 cognite_neat-0.11.3/pyproject.toml
+-rw-r--r--   0        0        0     9823 1970-01-01 00:00:00.000000 cognite_neat-0.11.3/PKG-INFO
```

### Comparing `cognite_neat-0.11.2/LICENSE` & `cognite_neat-0.11.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/README.md` & `cognite_neat-0.11.3/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/constants.py` & `cognite_neat-0.11.3/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/app.py` & `cognite_neat-0.11.3/cognite/neat/core/app.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/configuration.py` & `cognite_neat-0.11.3/cognite/neat/core/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/data_classes/config.py` & `cognite_neat-0.11.3/cognite/neat/core/data_classes/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/data_classes/rules.py` & `cognite_neat-0.11.3/cognite/neat/core/data_classes/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/data_classes/transformation_rules.py` & `cognite_neat-0.11.3/cognite/neat/core/data_classes/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.11.3/cognite/neat/core/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/extractors/labels.py` & `cognite_neat-0.11.3/cognite/neat/core/extractors/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/extractors/rdf_to_assets.py` & `cognite_neat-0.11.3/cognite/neat/core/extractors/rdf_to_assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,17 +351,15 @@
     Returns
     -------
     Dict[str, Asset]
         Dictionary of assets with external_id as key
     """
 
     orphanage_asset_external_id = (
-        f"{transformation_rules.metadata.externalIdPrefix}orphanage"
-        if transformation_rules.metadata.externalIdPrefix
-        else "orphanage"
+        f"{transformation_rules.metadata.externalIdPrefix or ''}orphanage-{transformation_rules.metadata.data_set_id}"
     )
 
     graph = graph_store.get_graph()
     # Step 1: Create rdf to asset property mapping
     logging.info("Generating rdf to asset property mapping")
     asset_class_mapping = _define_asset_class_mapping(transformation_rules)
 
@@ -403,15 +401,15 @@
 
                 # class instance is repaired and converted to asset dictionary
                 asset = _class2asset_instance(
                     class_,
                     class_instance,
                     asset_class_mapping[class_],
                     transformation_rules.metadata.data_set_id,
-                    "orphanage" if use_orphanage else None,  # we need only base external id
+                    orphanage_asset_external_id if use_orphanage else None,  # we need only base external id
                     transformation_rules.metadata.externalIdPrefix or None,
                 )
 
                 # adding labels and timestamps
                 asset["labels"] = [asset["metadata"]["type"], "non-historic"]
                 asset["metadata"]["start_time"] = str(datetime.now(timezone.utc))
                 asset["metadata"]["update_time"] = str(datetime.now(timezone.utc))
```

### Comparing `cognite_neat-0.11.2/cognite/neat/core/extractors/rdf_to_relationships.py` & `cognite_neat-0.11.3/cognite/neat/core/extractors/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/extractors/rules_to_graphql.py` & `cognite_neat-0.11.3/cognite/neat/core/extractors/rules_to_graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/loader/config.py` & `cognite_neat-0.11.3/cognite/neat/core/loader/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/loader/graph.py` & `cognite_neat-0.11.3/cognite/neat/core/loader/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.11.3/cognite/neat/core/loader/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/loader/rules.py` & `cognite_neat-0.11.3/cognite/neat/core/loader/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.11.3/cognite/neat/core/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/modeler.py` & `cognite_neat-0.11.3/cognite/neat/core/modeler.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/parser/transformation_rules.py` & `cognite_neat-0.11.3/cognite/neat/core/parser/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.11.3/cognite/neat/core/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/transformer.py` & `cognite_neat-0.11.3/cognite/neat/core/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/utils.py` & `cognite_neat-0.11.3/cognite/neat/core/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/validator.py` & `cognite_neat-0.11.3/cognite/neat/core/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/workflow/base.py` & `cognite_neat-0.11.3/cognite/neat/core/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.11.3/cognite/neat/core/workflow/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.11.3/cognite/neat/core/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/workflow/model.py` & `cognite_neat-0.11.3/cognite/neat/core/workflow/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.11.3/cognite/neat/core/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.11.3/cognite/neat/core/workflow/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.11.3/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.11.3/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.11.3/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.11.3/cognite/neat/examples/workflows/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.11.3/cognite/neat/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.11.3/cognite/neat/examples/workflows/default/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.11.3/cognite/neat/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/examples/workflows/fast_graph/workflow.py` & `cognite_neat-0.11.3/cognite/neat/examples/workflows/fast_graph/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/examples/workflows/fast_graph/workflow.yaml` & `cognite_neat-0.11.3/cognite/neat/examples/workflows/fast_graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.11.3/cognite/neat/examples/workflows/graph_db_import/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.11.3/cognite/neat/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/examples/workflows/sheet2cdf/workflow.py` & `cognite_neat-0.11.3/cognite/neat/examples/workflows/sheet2cdf/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.11.3/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/explorer/data_classes/rest.py` & `cognite_neat-0.11.3/cognite/neat/explorer/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/explorer/explorer.py` & `cognite_neat-0.11.3/cognite/neat/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.11.3/cognite/neat/explorer/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css` & `cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css.map` & `cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js` & `cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.LICENSE.txt` & `cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.map` & `cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.11.3/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.2/pyproject.toml` & `cognite_neat-0.11.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.11.2"
+version = "0.11.3"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 packages = [
```

### Comparing `cognite_neat-0.11.2/PKG-INFO` & `cognite_neat-0.11.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.11.2
+Version: 0.11.3
 Summary: Knowledge graph transformation
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

