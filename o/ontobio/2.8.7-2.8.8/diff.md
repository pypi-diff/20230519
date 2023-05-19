# Comparing `tmp/ontobio-2.8.7.tar.gz` & `tmp/ontobio-2.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontobio-2.8.7.tar", last modified: Tue May 16 18:16:48 2023, max compression
+gzip compressed data, was "ontobio-2.8.8.tar", last modified: Fri May 19 18:08:01 2023, max compression
```

## Comparing `ontobio-2.8.7.tar` & `ontobio-2.8.8.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.938502 ontobio-2.8.7/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1547 2023-02-15 19:42:46.000000 ontobio-2.8.7/LICENSE
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)       28 2023-02-15 19:42:46.000000 ontobio-2.8.7/MANIFEST.in
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1691 2023-05-16 18:16:48.938502 ontobio-2.8.7/PKG-INFO
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      970 2023-02-15 19:42:46.000000 ontobio-2.8.7/README.rst
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.898502 ontobio-2.8.7/bin/
--rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)      171 2023-02-15 19:42:46.000000 ontobio-2.8.7/bin/clear-cache.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6455 2023-02-15 19:42:46.000000 ontobio-2.8.7/bin/materialize.py
--rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)     7499 2023-02-15 19:42:46.000000 ontobio-2.8.7/bin/ogr.py
--rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)    20798 2023-02-15 19:42:46.000000 ontobio-2.8.7/bin/ontobio-assoc.py
--rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)     7331 2023-02-15 19:42:46.000000 ontobio-2.8.7/bin/ontobio-lexmap.py
--rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)     9695 2023-02-15 19:42:46.000000 ontobio-2.8.7/bin/ontobio-parse-assocs.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1778 2023-02-15 19:42:46.000000 ontobio-2.8.7/bin/rdfgen.py
--rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)    31600 2023-02-15 19:42:46.000000 ontobio-2.8.7/bin/validate.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.898502 ontobio-2.8.7/ontobio/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1697 2023-05-16 18:13:26.000000 ontobio-2.8.7/ontobio/__init__.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.908502 ontobio-2.8.7/ontobio/analysis/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/analysis/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      457 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/analysis/semsim.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6821 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/assoc_factory.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3665 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/assoc_schema.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    17363 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/assocmodel.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2114 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/cgraph.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7379 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/config.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1084 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/config.yaml
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3867 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/ecomap.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.908502 ontobio-2.8.7/ontobio/golr/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/golr/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3013 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/golr/beacon_query.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    10470 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/golr/golr_associations.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        1 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/golr/golr_entities.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2174 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/golr/golr_matrix.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    68763 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/golr/golr_query.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1450 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/golr/golr_sim.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4799 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/golr/golr_stats.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.908502 ontobio-2.8.7/ontobio/io/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      228 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/io/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    40092 2023-05-12 00:17:37.000000 ontobio-2.8.7/ontobio/io/assocparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6271 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/io/assocwriter.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    18018 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/io/differ.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    13053 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/io/entityparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2902 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/io/entitywriter.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6868 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/io/gaference.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1544 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/io/gafgpibridge.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    24503 2023-04-25 22:08:05.000000 ontobio-2.8.7/ontobio/io/gafparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    23204 2023-04-25 22:08:05.000000 ontobio-2.8.7/ontobio/io/gpadparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6903 2023-04-19 18:09:14.000000 ontobio-2.8.7/ontobio/io/hpoaparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12899 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/io/ontol_renderers.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1633 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/io/parsereport.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    42833 2023-05-16 18:04:14.000000 ontobio-2.8.7/ontobio/io/qc.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    35539 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/lexmap.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.908502 ontobio-2.8.7/ontobio/model/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1527 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/model/GolrResults.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      972 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/model/OBOGraph.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/model/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    27873 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/model/association.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3211 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/model/bbop_graph.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3589 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/model/biomodel.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5399 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/model/collections.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.908502 ontobio-2.8.7/ontobio/model/mme/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/model/mme/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1928 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/model/mme/request.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      607 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/model/mme/response.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1227 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/model/nlp.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2252 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/model/similarity.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.908502 ontobio-2.8.7/ontobio/neo/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/neo/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8261 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/neo/scigraph_ontology.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12801 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/obograph_util.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    37123 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/ontol.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6351 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/ontol_factory.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.918502 ontobio-2.8.7/ontobio/rdfgen/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/rdfgen/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12608 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/rdfgen/assoc_rdfgen.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.918502 ontobio-2.8.7/ontobio/rdfgen/gocamgen/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/rdfgen/gocamgen/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     9655 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/rdfgen/gocamgen/collapsed_assoc.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      489 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/rdfgen/gocamgen/errors.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3330 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/rdfgen/gocamgen/filter_rule.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    13135 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/rdfgen/gocamgen/gocam_builder.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    56549 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/rdfgen/gocamgen/gocamgen.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4947 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/rdfgen/gocamgen/rdflib_sparql_wrapper.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8070 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/rdfgen/gocamgen/subgraphs.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7567 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/rdfgen/gocamgen/triple_pattern_finder.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6653 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/rdfgen/gocamgen/utils.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8382 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/rdfgen/relations.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.918502 ontobio-2.8.7/ontobio/sim/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sim/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6273 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sim/annotation_scorer.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.918502 ontobio-2.8.7/ontobio/sim/api/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sim/api/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2397 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sim/api/interfaces.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    17404 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sim/api/owlsim2.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2163 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sim/api/owlsim3.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7262 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sim/api/semsearch.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2918 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sim/mme.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7583 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sim/phenosim_engine.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1290 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sim/sim_engine.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2961 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/slimmer.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.918502 ontobio-2.8.7/ontobio/sparql/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sparql/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2261 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sparql/rdf2nx.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1531 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sparql/rdflib_bridge.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4073 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sparql/skos.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12491 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sparql/sparql_go.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    11088 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sparql/sparql_ontol_utils.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8756 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sparql/sparql_ontology.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4673 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sparql/wikidata.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5814 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/sparql/wikidata_ontology.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1642 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/tsv_expander.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.918502 ontobio-2.8.7/ontobio/util/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/util/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      516 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/util/curie_map.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2826 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/util/go_utils.py
--rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)      736 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/util/obog2cg.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    18224 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/util/scigraph_util.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      903 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/util/user_agent.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.918502 ontobio-2.8.7/ontobio/validation/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/validation/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5693 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/validation/metadata.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    10167 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/validation/rules.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1322 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/validation/tools.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.918502 ontobio-2.8.7/ontobio/vocabulary/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/vocabulary/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      239 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/vocabulary/categories.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1226 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/vocabulary/relations.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      955 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/vocabulary/similarity.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      823 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/vocabulary/upper.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      310 2023-02-15 19:42:46.000000 ontobio-2.8.7/ontobio/xref_util.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.908502 ontobio-2.8.7/ontobio.egg-info/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1691 2023-05-16 18:16:48.000000 ontobio-2.8.7/ontobio.egg-info/PKG-INFO
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4357 2023-05-16 18:16:48.000000 ontobio-2.8.7/ontobio.egg-info/SOURCES.txt
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        1 2023-05-16 18:16:48.000000 ontobio-2.8.7/ontobio.egg-info/dependency_links.txt
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      471 2023-05-16 18:16:48.000000 ontobio-2.8.7/ontobio.egg-info/requires.txt
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)       14 2023-05-16 18:16:48.000000 ontobio-2.8.7/ontobio.egg-info/top_level.txt
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)       80 2023-05-16 18:16:48.938502 ontobio-2.8.7/setup.cfg
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2370 2023-02-15 19:42:46.000000 ontobio-2.8.7/setup.py
-drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-16 18:16:48.938502 ontobio-2.8.7/tests/
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/__init__.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      510 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_alt_id.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12770 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_assoc_writer.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3528 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_assocfactory.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3636 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_assocmodel.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      775 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_bgiparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5151 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_collections.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      915 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_config.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      736 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_ecomap.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1478 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_enrich.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1756 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_evidence_table.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      719 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_expand_tsv.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5319 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_gaference.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    26453 2023-05-12 00:17:37.000000 ontobio-2.8.7/tests/test_gafparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4929 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_goassociation_model.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5645 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_gocamgen.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5578 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_golr_associations.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1536 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_golr_map2slim.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      983 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_golr_query.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2234 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_golr_search.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    10349 2023-04-25 22:08:05.000000 ontobio-2.8.7/tests/test_gpad_parser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      761 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_gpad_writer.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_gpaddiffer.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1043 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_gpiparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      963 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_gpiwriter.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2199 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_hpoaparser.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1043 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_lexmap.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    11952 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_lexmap_local.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8184 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_local_json.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1159 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_local_ttl.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1912 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_map2slim.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      695 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_mutable.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1706 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_ontol.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3967 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_owlsim2_int.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4535 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_parse_ids.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      664 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_parse_taxon.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5390 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_phenosim_engine.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)    32563 2023-05-16 18:04:14.000000 ontobio-2.8.7/tests/test_qc.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4310 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_rdfgen.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      450 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_relations.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3363 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_remote_scigraph.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5059 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_remote_sparql.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1846 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_semsearch.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      550 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_skos_local.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1281 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_sparql_connection.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3463 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_validation_rules.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1301 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_wd.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1610 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_wd_ontol.py
--rw-r--r--   0 muruganu  (1000) muruganu  (1000)      351 2023-02-15 19:42:46.000000 ontobio-2.8.7/tests/test_write_obo.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.421720 ontobio-2.8.8/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1547 2023-02-15 19:42:46.000000 ontobio-2.8.8/LICENSE
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)       28 2023-02-15 19:42:46.000000 ontobio-2.8.8/MANIFEST.in
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1691 2023-05-19 18:08:01.421720 ontobio-2.8.8/PKG-INFO
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      970 2023-02-15 19:42:46.000000 ontobio-2.8.8/README.rst
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.381720 ontobio-2.8.8/bin/
+-rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)      171 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/clear-cache.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6455 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/materialize.py
+-rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)     7499 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/ogr.py
+-rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)    20798 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/ontobio-assoc.py
+-rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)     7331 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/ontobio-lexmap.py
+-rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)     9695 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/ontobio-parse-assocs.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1778 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/rdfgen.py
+-rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)    31600 2023-02-15 19:42:46.000000 ontobio-2.8.8/bin/validate.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.381720 ontobio-2.8.8/ontobio/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1697 2023-05-19 18:06:42.000000 ontobio-2.8.8/ontobio/__init__.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.381720 ontobio-2.8.8/ontobio/analysis/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/analysis/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      457 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/analysis/semsim.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6821 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/assoc_factory.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3665 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/assoc_schema.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    17363 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/assocmodel.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2114 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/cgraph.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7379 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/config.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1084 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/config.yaml
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3867 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/ecomap.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.391720 ontobio-2.8.8/ontobio/golr/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3013 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/beacon_query.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    10470 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/golr_associations.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        1 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/golr_entities.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2174 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/golr_matrix.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    68763 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/golr_query.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1450 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/golr_sim.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4799 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/golr/golr_stats.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.391720 ontobio-2.8.8/ontobio/io/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      228 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    40092 2023-05-12 00:17:37.000000 ontobio-2.8.8/ontobio/io/assocparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6271 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/assocwriter.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    18018 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/differ.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    13053 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/entityparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2902 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/entitywriter.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6868 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/gaference.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1544 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/gafgpibridge.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    24503 2023-04-25 22:08:05.000000 ontobio-2.8.8/ontobio/io/gafparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    23204 2023-04-25 22:08:05.000000 ontobio-2.8.8/ontobio/io/gpadparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6903 2023-04-19 18:09:14.000000 ontobio-2.8.8/ontobio/io/hpoaparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12899 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/ontol_renderers.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1633 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/io/parsereport.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    43181 2023-05-19 18:03:52.000000 ontobio-2.8.8/ontobio/io/qc.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    35539 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/lexmap.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.391720 ontobio-2.8.8/ontobio/model/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1527 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/GolrResults.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      972 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/OBOGraph.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    27873 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/association.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3211 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/bbop_graph.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3589 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/biomodel.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5399 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/collections.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.391720 ontobio-2.8.8/ontobio/model/mme/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/mme/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1928 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/mme/request.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      607 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/mme/response.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1227 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/nlp.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2252 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/model/similarity.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.391720 ontobio-2.8.8/ontobio/neo/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/neo/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8261 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/neo/scigraph_ontology.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12801 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/obograph_util.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    37123 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/ontol.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6351 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/ontol_factory.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.391720 ontobio-2.8.8/ontobio/rdfgen/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12608 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/assoc_rdfgen.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.401720 ontobio-2.8.8/ontobio/rdfgen/gocamgen/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     9655 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/collapsed_assoc.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      489 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/errors.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3330 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/filter_rule.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    13135 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/gocam_builder.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    56549 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/gocamgen.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4947 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/rdflib_sparql_wrapper.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8070 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/subgraphs.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7567 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/triple_pattern_finder.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6653 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/gocamgen/utils.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8382 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/rdfgen/relations.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.401720 ontobio-2.8.8/ontobio/sim/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     6273 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/annotation_scorer.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.401720 ontobio-2.8.8/ontobio/sim/api/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/api/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2397 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/api/interfaces.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    17404 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/api/owlsim2.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2163 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/api/owlsim3.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7262 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/api/semsearch.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2918 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/mme.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     7583 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/phenosim_engine.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1290 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sim/sim_engine.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2961 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/slimmer.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.401720 ontobio-2.8.8/ontobio/sparql/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2261 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/rdf2nx.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1531 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/rdflib_bridge.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4073 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/skos.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12491 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/sparql_go.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    11088 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/sparql_ontol_utils.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8756 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/sparql_ontology.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4673 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/wikidata.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5814 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/sparql/wikidata_ontology.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1642 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/tsv_expander.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.401720 ontobio-2.8.8/ontobio/util/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/util/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      516 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/util/curie_map.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2826 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/util/go_utils.py
+-rwxr-xr-x   0 muruganu  (1000) muruganu  (1000)      736 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/util/obog2cg.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    18224 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/util/scigraph_util.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      903 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/util/user_agent.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.401720 ontobio-2.8.8/ontobio/validation/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/validation/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5693 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/validation/metadata.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    10167 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/validation/rules.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1322 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/validation/tools.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.401720 ontobio-2.8.8/ontobio/vocabulary/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/vocabulary/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      239 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/vocabulary/categories.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1226 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/vocabulary/relations.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      955 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/vocabulary/similarity.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      823 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/vocabulary/upper.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      310 2023-02-15 19:42:46.000000 ontobio-2.8.8/ontobio/xref_util.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.381720 ontobio-2.8.8/ontobio.egg-info/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1691 2023-05-19 18:08:01.000000 ontobio-2.8.8/ontobio.egg-info/PKG-INFO
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4357 2023-05-19 18:08:01.000000 ontobio-2.8.8/ontobio.egg-info/SOURCES.txt
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        1 2023-05-19 18:08:01.000000 ontobio-2.8.8/ontobio.egg-info/dependency_links.txt
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      471 2023-05-19 18:08:01.000000 ontobio-2.8.8/ontobio.egg-info/requires.txt
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)       14 2023-05-19 18:08:01.000000 ontobio-2.8.8/ontobio.egg-info/top_level.txt
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)       80 2023-05-19 18:08:01.421720 ontobio-2.8.8/setup.cfg
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2370 2023-02-15 19:42:46.000000 ontobio-2.8.8/setup.py
+drwxr-xr-x   0 muruganu  (1000) muruganu  (1000)        0 2023-05-19 18:08:01.421720 ontobio-2.8.8/tests/
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/__init__.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      510 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_alt_id.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    12770 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_assoc_writer.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3528 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_assocfactory.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3636 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_assocmodel.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      775 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_bgiparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5151 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_collections.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      915 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_config.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      736 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_ecomap.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1478 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_enrich.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1756 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_evidence_table.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      719 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_expand_tsv.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5319 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_gaference.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    26453 2023-05-12 00:17:37.000000 ontobio-2.8.8/tests/test_gafparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4929 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_goassociation_model.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5645 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_gocamgen.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5578 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_golr_associations.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1536 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_golr_map2slim.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      983 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_golr_query.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2234 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_golr_search.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    10349 2023-04-25 22:08:05.000000 ontobio-2.8.8/tests/test_gpad_parser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      761 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_gpad_writer.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)        0 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_gpaddiffer.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1043 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_gpiparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      963 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_gpiwriter.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     2199 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_hpoaparser.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1043 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_lexmap.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    11952 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_lexmap_local.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     8184 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_local_json.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1159 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_local_ttl.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1912 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_map2slim.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      695 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_mutable.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1706 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_ontol.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3967 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_owlsim2_int.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4535 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_parse_ids.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      664 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_parse_taxon.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5390 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_phenosim_engine.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)    33092 2023-05-19 18:03:52.000000 ontobio-2.8.8/tests/test_qc.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     4310 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_rdfgen.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      450 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_relations.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3363 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_remote_scigraph.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     5059 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_remote_sparql.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1846 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_semsearch.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      550 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_skos_local.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1281 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_sparql_connection.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     3463 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_validation_rules.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1301 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_wd.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)     1610 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_wd_ontol.py
+-rw-r--r--   0 muruganu  (1000) muruganu  (1000)      351 2023-02-15 19:42:46.000000 ontobio-2.8.8/tests/test_write_obo.py
```

### Comparing `ontobio-2.8.7/LICENSE` & `ontobio-2.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/PKG-INFO` & `ontobio-2.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontobio
-Version: 2.8.7
+Version: 2.8.8
 Summary: Library for working with OBO Library Ontologies and associations
 Home-page: https://github.com/biolink/ontobio
 Author: Chris Mungall
 Author-email: cmungall@gmail.com
 License: BSD
 Keywords: ontology graph obo owl sparql networkx network
 Platform: UNKNOWN
```

### Comparing `ontobio-2.8.7/README.rst` & `ontobio-2.8.8/README.rst`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/bin/materialize.py` & `ontobio-2.8.8/bin/materialize.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/bin/ogr.py` & `ontobio-2.8.8/bin/ogr.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/bin/ontobio-assoc.py` & `ontobio-2.8.8/bin/ontobio-assoc.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/bin/ontobio-lexmap.py` & `ontobio-2.8.8/bin/ontobio-lexmap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/bin/ontobio-parse-assocs.py` & `ontobio-2.8.8/bin/ontobio-parse-assocs.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/bin/rdfgen.py` & `ontobio-2.8.8/bin/rdfgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/bin/validate.py` & `ontobio-2.8.8/bin/validate.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/__init__.py` & `ontobio-2.8.8/ontobio/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import absolute_import
 
-__version__ = '2.8.7'
+__version__ = '2.8.8'
 
 
 from .ontol_factory import OntologyFactory
 from .ontol import Ontology, Synonym, TextDefinition
 from .assoc_factory import AssociationSetFactory
 from .io.ontol_renderers import GraphRenderer
```

### Comparing `ontobio-2.8.7/ontobio/assoc_factory.py` & `ontobio-2.8.8/ontobio/assoc_factory.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/assoc_schema.py` & `ontobio-2.8.8/ontobio/assoc_schema.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/assocmodel.py` & `ontobio-2.8.8/ontobio/assocmodel.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/cgraph.py` & `ontobio-2.8.8/ontobio/cgraph.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/config.py` & `ontobio-2.8.8/ontobio/config.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/config.yaml` & `ontobio-2.8.8/ontobio/config.yaml`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/ecomap.py` & `ontobio-2.8.8/ontobio/ecomap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/golr/beacon_query.py` & `ontobio-2.8.8/ontobio/golr/beacon_query.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/golr/golr_associations.py` & `ontobio-2.8.8/ontobio/golr/golr_associations.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/golr/golr_matrix.py` & `ontobio-2.8.8/ontobio/golr/golr_matrix.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/golr/golr_query.py` & `ontobio-2.8.8/ontobio/golr/golr_query.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/golr/golr_sim.py` & `ontobio-2.8.8/ontobio/golr/golr_sim.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/golr/golr_stats.py` & `ontobio-2.8.8/ontobio/golr/golr_stats.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/io/assocparser.py` & `ontobio-2.8.8/ontobio/io/assocparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/io/assocwriter.py` & `ontobio-2.8.8/ontobio/io/assocwriter.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/io/differ.py` & `ontobio-2.8.8/ontobio/io/differ.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/io/entityparser.py` & `ontobio-2.8.8/ontobio/io/entityparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/io/entitywriter.py` & `ontobio-2.8.8/ontobio/io/entitywriter.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/io/gaference.py` & `ontobio-2.8.8/ontobio/io/gaference.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/io/gafgpibridge.py` & `ontobio-2.8.8/ontobio/io/gafgpibridge.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/io/gafparser.py` & `ontobio-2.8.8/ontobio/io/gafparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/io/gpadparser.py` & `ontobio-2.8.8/ontobio/io/gpadparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/io/hpoaparser.py` & `ontobio-2.8.8/ontobio/io/hpoaparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/io/ontol_renderers.py` & `ontobio-2.8.8/ontobio/io/ontol_renderers.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/io/parsereport.py` & `ontobio-2.8.8/ontobio/io/parsereport.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/io/qc.py` & `ontobio-2.8.8/ontobio/io/qc.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,16 +191,20 @@
     def __init__(self):
         super().__init__("GORULE:0000006", "IEP and HEP usage is restricted to terms from the Biological Process ontology", FailMode.HARD)
 
     def test(self, annotation: association.GoAssociation, config: assocparser.AssocParserConfig, group=None) -> TestResult:
         if config.ontology is None:
             return self._result(True)
 
-        go_namespace = [predval for predval in config.ontology.get_graph().nodes.get(str(annotation.object.id), {}).get("meta", {}).get("basicPropertyValues", []) if predval["pred"]=="OIO:hasOBONamespace"]
         evidence = str(annotation.evidence.type)
+        assigned_by = annotation.provided_by
+        #Annotations with code IEP and HEP assigned by GOC are not restricted to Biological Process terms
+        if evidence in [iep_eco, hep_eco] and assigned_by == "GOC":
+            return self._result(True)
+        go_namespace = [predval for predval in config.ontology.get_graph().nodes.get(str(annotation.object.id), {}).get("meta", {}).get("basicPropertyValues", []) if predval["pred"]=="OIO:hasOBONamespace"]
         fails = evidence in [iep_eco, hep_eco] and "biological_process" not in [o["val"] for o in go_namespace]
         return self._result(not fails)
 
 
 class GoRule07(GoRule):
 
     def __init__(self):
@@ -521,14 +525,17 @@
             closure = gafparser.protein_complex_sublcass_closure(ontology)
             self.protein_containing_complex_descendents = closure
 
         return {} if self.protein_containing_complex_descendents is None else self.protein_containing_complex_descendents    
 
     def test(self, annotation: association.GoAssociation, config: assocparser.AssocParserConfig, group=None) -> TestResult:
         # An implementation note: This is done by testing if the DB (column 1) is ComplexPortal or DB Object type (column 12) is protein_complex
+        if config.ontology is None:
+            return self._result(True)
+                
         db = annotation.subject.id.namespace
         objecttype = annotation.subject.type
         goterm = str(annotation.object.id)
         namespace = config.ontology.obo_namespace(goterm)      
  
         if namespace == "cellular_component" and goterm in self.make_protein_complex_descendents_if_not_present(config.ontology):
             for ot in objecttype:
```

### Comparing `ontobio-2.8.7/ontobio/lexmap.py` & `ontobio-2.8.8/ontobio/lexmap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/model/GolrResults.py` & `ontobio-2.8.8/ontobio/model/GolrResults.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/model/OBOGraph.py` & `ontobio-2.8.8/ontobio/model/OBOGraph.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/model/association.py` & `ontobio-2.8.8/ontobio/model/association.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/model/bbop_graph.py` & `ontobio-2.8.8/ontobio/model/bbop_graph.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/model/biomodel.py` & `ontobio-2.8.8/ontobio/model/biomodel.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/model/collections.py` & `ontobio-2.8.8/ontobio/model/collections.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/model/mme/request.py` & `ontobio-2.8.8/ontobio/model/mme/request.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/model/mme/response.py` & `ontobio-2.8.8/ontobio/model/mme/response.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/model/nlp.py` & `ontobio-2.8.8/ontobio/model/nlp.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/model/similarity.py` & `ontobio-2.8.8/ontobio/model/similarity.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/neo/scigraph_ontology.py` & `ontobio-2.8.8/ontobio/neo/scigraph_ontology.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/obograph_util.py` & `ontobio-2.8.8/ontobio/obograph_util.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/ontol.py` & `ontobio-2.8.8/ontobio/ontol.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/ontol_factory.py` & `ontobio-2.8.8/ontobio/ontol_factory.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/rdfgen/assoc_rdfgen.py` & `ontobio-2.8.8/ontobio/rdfgen/assoc_rdfgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/rdfgen/gocamgen/collapsed_assoc.py` & `ontobio-2.8.8/ontobio/rdfgen/gocamgen/collapsed_assoc.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/rdfgen/gocamgen/filter_rule.py` & `ontobio-2.8.8/ontobio/rdfgen/gocamgen/filter_rule.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/rdfgen/gocamgen/gocam_builder.py` & `ontobio-2.8.8/ontobio/rdfgen/gocamgen/gocam_builder.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/rdfgen/gocamgen/gocamgen.py` & `ontobio-2.8.8/ontobio/rdfgen/gocamgen/gocamgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/rdfgen/gocamgen/rdflib_sparql_wrapper.py` & `ontobio-2.8.8/ontobio/rdfgen/gocamgen/rdflib_sparql_wrapper.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/rdfgen/gocamgen/subgraphs.py` & `ontobio-2.8.8/ontobio/rdfgen/gocamgen/subgraphs.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/rdfgen/gocamgen/triple_pattern_finder.py` & `ontobio-2.8.8/ontobio/rdfgen/gocamgen/triple_pattern_finder.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/rdfgen/gocamgen/utils.py` & `ontobio-2.8.8/ontobio/rdfgen/gocamgen/utils.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/rdfgen/relations.py` & `ontobio-2.8.8/ontobio/rdfgen/relations.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sim/annotation_scorer.py` & `ontobio-2.8.8/ontobio/sim/annotation_scorer.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sim/api/interfaces.py` & `ontobio-2.8.8/ontobio/sim/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sim/api/owlsim2.py` & `ontobio-2.8.8/ontobio/sim/api/owlsim2.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sim/api/owlsim3.py` & `ontobio-2.8.8/ontobio/sim/api/owlsim3.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sim/api/semsearch.py` & `ontobio-2.8.8/ontobio/sim/api/semsearch.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sim/mme.py` & `ontobio-2.8.8/ontobio/sim/mme.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sim/phenosim_engine.py` & `ontobio-2.8.8/ontobio/sim/phenosim_engine.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sim/sim_engine.py` & `ontobio-2.8.8/ontobio/sim/sim_engine.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/slimmer.py` & `ontobio-2.8.8/ontobio/slimmer.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sparql/rdf2nx.py` & `ontobio-2.8.8/ontobio/sparql/rdf2nx.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sparql/rdflib_bridge.py` & `ontobio-2.8.8/ontobio/sparql/rdflib_bridge.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sparql/skos.py` & `ontobio-2.8.8/ontobio/sparql/skos.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sparql/sparql_go.py` & `ontobio-2.8.8/ontobio/sparql/sparql_go.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sparql/sparql_ontol_utils.py` & `ontobio-2.8.8/ontobio/sparql/sparql_ontol_utils.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sparql/sparql_ontology.py` & `ontobio-2.8.8/ontobio/sparql/sparql_ontology.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sparql/wikidata.py` & `ontobio-2.8.8/ontobio/sparql/wikidata.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/sparql/wikidata_ontology.py` & `ontobio-2.8.8/ontobio/sparql/wikidata_ontology.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/tsv_expander.py` & `ontobio-2.8.8/ontobio/tsv_expander.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/util/curie_map.py` & `ontobio-2.8.8/ontobio/util/curie_map.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/util/go_utils.py` & `ontobio-2.8.8/ontobio/util/go_utils.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/util/obog2cg.py` & `ontobio-2.8.8/ontobio/util/obog2cg.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/util/scigraph_util.py` & `ontobio-2.8.8/ontobio/util/scigraph_util.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/util/user_agent.py` & `ontobio-2.8.8/ontobio/util/user_agent.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/validation/metadata.py` & `ontobio-2.8.8/ontobio/validation/metadata.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/validation/rules.py` & `ontobio-2.8.8/ontobio/validation/rules.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/validation/tools.py` & `ontobio-2.8.8/ontobio/validation/tools.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/vocabulary/relations.py` & `ontobio-2.8.8/ontobio/vocabulary/relations.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/vocabulary/similarity.py` & `ontobio-2.8.8/ontobio/vocabulary/similarity.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio/vocabulary/upper.py` & `ontobio-2.8.8/ontobio/vocabulary/upper.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/ontobio.egg-info/PKG-INFO` & `ontobio-2.8.8/ontobio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontobio
-Version: 2.8.7
+Version: 2.8.8
 Summary: Library for working with OBO Library Ontologies and associations
 Home-page: https://github.com/biolink/ontobio
 Author: Chris Mungall
 Author-email: cmungall@gmail.com
 License: BSD
 Keywords: ontology graph obo owl sparql networkx network
 Platform: UNKNOWN
```

### Comparing `ontobio-2.8.7/ontobio.egg-info/SOURCES.txt` & `ontobio-2.8.8/ontobio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/setup.py` & `ontobio-2.8.8/setup.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_assoc_writer.py` & `ontobio-2.8.8/tests/test_assoc_writer.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_assocfactory.py` & `ontobio-2.8.8/tests/test_assocfactory.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_assocmodel.py` & `ontobio-2.8.8/tests/test_assocmodel.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_bgiparser.py` & `ontobio-2.8.8/tests/test_bgiparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_collections.py` & `ontobio-2.8.8/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_config.py` & `ontobio-2.8.8/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_ecomap.py` & `ontobio-2.8.8/tests/test_ecomap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_enrich.py` & `ontobio-2.8.8/tests/test_enrich.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_evidence_table.py` & `ontobio-2.8.8/tests/test_evidence_table.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_expand_tsv.py` & `ontobio-2.8.8/tests/test_expand_tsv.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_gaference.py` & `ontobio-2.8.8/tests/test_gaference.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_gafparser.py` & `ontobio-2.8.8/tests/test_gafparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_goassociation_model.py` & `ontobio-2.8.8/tests/test_goassociation_model.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_gocamgen.py` & `ontobio-2.8.8/tests/test_gocamgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_golr_associations.py` & `ontobio-2.8.8/tests/test_golr_associations.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_golr_map2slim.py` & `ontobio-2.8.8/tests/test_golr_map2slim.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_golr_query.py` & `ontobio-2.8.8/tests/test_golr_query.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_golr_search.py` & `ontobio-2.8.8/tests/test_golr_search.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_gpad_parser.py` & `ontobio-2.8.8/tests/test_gpad_parser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_gpad_writer.py` & `ontobio-2.8.8/tests/test_gpad_writer.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_gpiparser.py` & `ontobio-2.8.8/tests/test_gpiparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_gpiwriter.py` & `ontobio-2.8.8/tests/test_gpiwriter.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_hpoaparser.py` & `ontobio-2.8.8/tests/test_hpoaparser.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_lexmap.py` & `ontobio-2.8.8/tests/test_lexmap.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_lexmap_local.py` & `ontobio-2.8.8/tests/test_lexmap_local.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_local_json.py` & `ontobio-2.8.8/tests/test_local_json.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_local_ttl.py` & `ontobio-2.8.8/tests/test_local_ttl.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_map2slim.py` & `ontobio-2.8.8/tests/test_map2slim.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_mutable.py` & `ontobio-2.8.8/tests/test_mutable.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_ontol.py` & `ontobio-2.8.8/tests/test_ontol.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_owlsim2_int.py` & `ontobio-2.8.8/tests/test_owlsim2_int.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_parse_ids.py` & `ontobio-2.8.8/tests/test_parse_ids.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_parse_taxon.py` & `ontobio-2.8.8/tests/test_parse_taxon.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_phenosim_engine.py` & `ontobio-2.8.8/tests/test_phenosim_engine.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_qc.py` & `ontobio-2.8.8/tests/test_qc.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from ontobio import ontol, ontol_factory, ecomap
 
 import copy
 
 ontology = ontol_factory.OntologyFactory().create("tests/resources/goslim_generic.json")
 ecomapping = ecomap.EcoMap()
 iea_eco = ecomapping.coderef_to_ecoclass("IEA")
+hep_eco = ecomapping.coderef_to_ecoclass("HEP")
 ic_eco = ecomapping.coderef_to_ecoclass("IC")
 ikr_eco = ecomapping.coderef_to_ecoclass("IKR")
 iba_eco = ecomapping.coderef_to_ecoclass("IBA")
 iso_eco = ecomapping.coderef_to_ecoclass("ISO")
 
 
 def make_annotation(db="blah",
@@ -100,15 +101,26 @@
     assoc.object.id = Curie.from_str("GO:0008150")
     test_result = qc.GoRule06().test(assoc, all_rules_config(ontology=ontology))
     assert test_result.result_type == qc.ResultType.PASS
 
     assoc.evidence.type = Curie.from_str(iea_eco)
     test_result = qc.GoRule06().test(assoc, all_rules_config(ontology=ontology))
     assert test_result.result_type == qc.ResultType.PASS
+    
+    assoc.evidence.type = Curie.from_str(hep_eco)
+    assoc.provided_by = "GOC"
+    assoc.aspect = "F"
+    assoc.object.id = Curie.from_str("GO:0003674");    
+    test_result = qc.GoRule06().test(assoc, all_rules_config(ontology=ontology))
+    assert test_result.result_type == qc.ResultType.PASS    
 
+    assoc.provided_by = "WB"  
+    test_result = qc.GoRule06().test(assoc, all_rules_config(ontology=ontology))
+    assert test_result.result_type == qc.ResultType.ERROR
+    
 def test_go_rule_07():
 
     assoc = make_annotation(goid="GO:0003824", evidence="IPI").associations[0]
 
     test_result = qc.GoRule07().test(assoc, all_rules_config(ontology=ontology))
     assert test_result.result_type == qc.ResultType.WARNING
```

### Comparing `ontobio-2.8.7/tests/test_rdfgen.py` & `ontobio-2.8.8/tests/test_rdfgen.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_remote_scigraph.py` & `ontobio-2.8.8/tests/test_remote_scigraph.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_remote_sparql.py` & `ontobio-2.8.8/tests/test_remote_sparql.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_semsearch.py` & `ontobio-2.8.8/tests/test_semsearch.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_skos_local.py` & `ontobio-2.8.8/tests/test_skos_local.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_sparql_connection.py` & `ontobio-2.8.8/tests/test_sparql_connection.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_validation_rules.py` & `ontobio-2.8.8/tests/test_validation_rules.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_wd.py` & `ontobio-2.8.8/tests/test_wd.py`

 * *Files identical despite different names*

### Comparing `ontobio-2.8.7/tests/test_wd_ontol.py` & `ontobio-2.8.8/tests/test_wd_ontol.py`

 * *Files identical despite different names*

