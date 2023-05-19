# Comparing `tmp/oaklib-0.5.6.tar.gz` & `tmp/oaklib-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaklib-0.5.6.tar", max compression
+gzip compressed data, was "oaklib-0.5.7.tar", max compression
```

## Comparing `oaklib-0.5.6.tar` & `oaklib-0.5.7.tar`

### file list

```diff
@@ -1,269 +1,274 @@
--rw-r--r--   0        0        0    11357 2023-05-15 15:52:40.563784 oaklib-0.5.6/LICENSE
--rw-r--r--   0        0        0     7241 2023-05-15 15:52:40.563784 oaklib-0.5.6/README.md
--rw-r--r--   0        0        0     1883 2023-05-15 15:53:30.576518 oaklib-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      271 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/__init__.py
--rw-r--r--   0        0        0   193630 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/cli.py
--rw-r--r--   0        0        0       64 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/__init__.py
--rw-r--r--   0        0        0      372 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/go-human-input-spec.yaml
--rw-r--r--   0        0        0      162 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/go-pombase-input-spec.yaml
--rw-r--r--   0        0        0      109 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/hpoa-g2p-input-spec.yaml
--rw-r--r--   0        0        0      106 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/hpoa-input-spec.yaml
--rw-r--r--   0        0        0     1903 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
--rw-r--r--   0        0        0      562 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/mondo-g2d-input-spec.yaml
--rw-r--r--   0        0        0      109 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/mondo-gencc-input-spec.yaml
--rw-r--r--   0        0        0      118 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
--rw-r--r--   0        0        0     4537 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/obograph-style.json
--rw-r--r--   0        0        0      256 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/omo-to-skos.sssom.tsv
--rw-r--r--   0        0        0      131 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/value-set-expander.conf.yaml
--rw-r--r--   0        0        0      128 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/constants.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/converters/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/converters/data_model_converter.py
--rw-r--r--   0        0        0     2561 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/converters/logical_definition_flattener.py
--rw-r--r--   0        0        0     2371 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/converters/obo_graph_to_cx_converter.py
--rw-r--r--   0        0        0    12159 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/converters/obo_graph_to_fhir_converter.py
--rw-r--r--   0        0        0     5713 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/converters/obo_graph_to_obo_format_converter.py
--rw-r--r--   0        0        0     5793 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
--rw-r--r--   0        0        0       60 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/__init__.py
--rw-r--r--   0        0        0     4034 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/association.owl.ttl
--rw-r--r--   0        0        0    36266 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/association.py
--rw-r--r--   0        0        0    11740 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/association.yaml
--rw-r--r--   0        0        0     6165 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/class_enrichment.owl.ttl
--rw-r--r--   0        0        0    13328 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/class_enrichment.py
--rw-r--r--   0        0        0     3192 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/class_enrichment.yaml
--rw-r--r--   0        0        0    19083 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
--rw-r--r--   0        0        0    24246 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/cross_ontology_diff.py
--rw-r--r--   0        0        0    10687 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/cross_ontology_diff.yaml
--rw-r--r--   0        0        0    29418 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/cx.py
--rw-r--r--   0        0        0     6314 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/cx.yaml
--rw-r--r--   0        0        0    15826 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/fhir.owl.ttl
--rw-r--r--   0        0        0    35744 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/fhir.py
--rw-r--r--   0        0        0     5064 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/fhir.yaml
--rw-r--r--   0        0        0    14564 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/input_specification.py
--rw-r--r--   0        0        0     3560 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/input_specification.yaml
--rw-r--r--   0        0        0    15768 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/item_list.py
--rw-r--r--   0        0        0     6339 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/item_list.yaml
--rw-r--r--   0        0        0     8984 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/lexical_index.owl.ttl
--rw-r--r--   0        0        0    17256 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/lexical_index.py
--rw-r--r--   0        0        0     6429 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/lexical_index.schema.json
--rw-r--r--   0        0        0     4016 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/lexical_index.yaml
--rw-r--r--   0        0        0    26434 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/mapping_cluster_datamodel.py
--rw-r--r--   0        0        0     7317 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
--rw-r--r--   0        0        0   226115 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
--rw-r--r--   0        0        0    32727 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.py
--rw-r--r--   0        0        0    12889 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
--rw-r--r--   0        0        0     3607 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.yaml
--rw-r--r--   0        0        0    25354 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/obograph.owl.ttl
--rw-r--r--   0        0        0    46876 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/obograph.py
--rw-r--r--   0        0        0    22375 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/obograph.schema.json
--rw-r--r--   0        0        0    18191 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/obograph.yaml
--rw-r--r--   0        0        0    59793 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.owl.ttl
--rw-r--r--   0        0        0   117175 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.py
--rw-r--r--   0        0        0    95288 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.schema.json
--rw-r--r--   0        0        0    30433 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.yaml
--rw-r--r--   0        0        0    14759 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/oxo.owl.ttl
--rw-r--r--   0        0        0    21914 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/oxo.py
--rw-r--r--   0        0        0     4392 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/oxo.yaml
--rw-r--r--   0        0        0     3240 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/search.py
--rw-r--r--   0        0        0    16948 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/search_datamodel.owl.ttl
--rw-r--r--   0        0        0    25145 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/search_datamodel.py
--rw-r--r--   0        0        0     6683 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/search_datamodel.yaml
--rw-r--r--   0        0        0      287 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/settings.py
--rw-r--r--   0        0        0    12767 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/similarity.owl.ttl
--rw-r--r--   0        0        0    22226 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/similarity.py
--rw-r--r--   0        0        0     5511 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/similarity.yaml
--rw-r--r--   0        0        0    31217 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
--rw-r--r--   0        0        0    50743 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.py
--rw-r--r--   0        0        0    21176 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
--rw-r--r--   0        0        0    16246 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.yaml
--rw-r--r--   0        0        0     9909 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/taxon_constraints.owl.ttl
--rw-r--r--   0        0        0    18430 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/taxon_constraints.py
--rw-r--r--   0        0        0     5879 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/taxon_constraints.yaml
--rw-r--r--   0        0        0    11599 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/text_annotator.owl.ttl
--rw-r--r--   0        0        0    20418 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/text_annotator.py
--rw-r--r--   0        0        0     2464 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/text_annotator.schema.json
--rw-r--r--   0        0        0     4219 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/text_annotator.yaml
--rw-r--r--   0        0        0    13670 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.owl.ttl
--rw-r--r--   0        0        0    25351 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.py
--rw-r--r--   0        0        0    10783 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.schema.json
--rw-r--r--   0        0        0     7510 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.yaml
--rw-r--r--   0        0        0     6640 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/value_set_configuration.owl.ttl
--rw-r--r--   0        0        0     8458 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/value_set_configuration.py
--rw-r--r--   0        0        0     2276 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/value_set_configuration.yaml
--rw-r--r--   0        0        0     5614 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/vocabulary.py
--rw-r--r--   0        0        0     5623 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/implementations/aggregator/__init__.py
--rw-r--r--   0        0        0     5996 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/implementations/aggregator/aggregator_implementation.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/implementations/amigo/__init__.py
--rw-r--r--   0        0        0     4563 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/implementations/amigo/amigo_implementation.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/cx/__init__.py
--rw-r--r--   0        0        0     1985 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/cx/cx_implementation.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/eutils/__init__.py
--rw-r--r--   0        0        0     2179 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/eutils/eutils_implementation.py
--rw-r--r--   0        0        0     1053 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/eutils/pubmed_implementation.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/fhir/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/funowl/__init__.py
--rw-r--r--   0        0        0     8473 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/funowl/funowl_implementation.py
--rw-r--r--   0        0        0     2313 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/gilda.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/kgx/__init__.py
--rw-r--r--   0        0        0    30434 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/kgx/kgx_implementation.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/neo4j/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/obograph/__init__.py
--rw-r--r--   0        0        0    16240 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/obograph/obograph_implementation.py
--rw-r--r--   0        0        0      267 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ols/__init__.py
--rw-r--r--   0        0        0      132 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ols/constants.py
--rw-r--r--   0        0        0     7942 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ols/ols_implementation.py
--rw-r--r--   0        0        0      686 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ols/oxo_utils.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontobee/__init__.py
--rw-r--r--   0        0        0     2532 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontobee/ontobee_implementation.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontoportal/__init__.py
--rw-r--r--   0        0        0      382 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontoportal/agroportal_implementation.py
--rw-r--r--   0        0        0     1238 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontoportal/bioportal_implementation.py
--rw-r--r--   0        0        0      378 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
--rw-r--r--   0        0        0      378 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontoportal/matportal_implementation.py
--rw-r--r--   0        0        0    12106 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/owlery/__init__.py
--rw-r--r--   0        0        0      427 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/owlery/owlery_implementation.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/pronto/__init__.py
--rw-r--r--   0        0        0    35620 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/pronto/pronto_implementation.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/robot/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/scigraph/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/semsimian/__init__.py
--rw-r--r--   0        0        0    14075 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/semsimian/semsimian_implementation.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/simpleobo/__init__.py
--rw-r--r--   0        0        0    34382 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
--rw-r--r--   0        0        0    21451 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/simpleobo/simple_obo_parser.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/skos/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/solor/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/solr/__init__.py
--rw-r--r--   0        0        0       96 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sparql/__init__.py
--rw-r--r--   0        0        0    36699 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
--rw-r--r--   0        0        0      885 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sparql/lov_implementation.py
--rw-r--r--   0        0        0     1721 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
--rw-r--r--   0        0        0     2658 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sparql/sparql_implementation.py
--rw-r--r--   0        0        0     2326 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sparql/sparql_query.py
--rw-r--r--   0        0        0       96 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sqldb/__init__.py
--rw-r--r--   0        0        0   106362 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sqldb/sql_implementation.py
--rw-r--r--   0        0        0     1903 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sqldb/sqlite_utils.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/tccm/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/translator/__init__.py
--rw-r--r--   0        0        0     3283 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/translator/translator_implementation.py
--rw-r--r--   0        0        0      108 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ubergraph/__init__.py
--rw-r--r--   0        0        0    19393 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/umls/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/uniprot/__init__.py
--rw-r--r--   0        0        0     9603 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/uniprot/uniprot_implementation.py
--rw-r--r--   0        0        0       96 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/wikidata/__init__.py
--rw-r--r--   0        0        0    17121 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/wikidata/wikidata_implementation.py
--rw-r--r--   0        0        0      913 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/interfaces/__init__.py
--rw-r--r--   0        0        0    20557 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/interfaces/association_provider_interface.py
--rw-r--r--   0        0        0    50981 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/interfaces/basic_ontology_interface.py
--rw-r--r--   0        0        0     8830 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/interfaces/class_enrichment_calculation_interface.py
--rw-r--r--   0        0        0    11720 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/interfaces/differ_interface.py
--rw-r--r--   0        0        0     2649 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/interfaces/dumper_interface.py
--rw-r--r--   0        0        0      977 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/embedding_provider_interface.py
--rw-r--r--   0        0        0    13681 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/mapping_provider_interface.py
--rw-r--r--   0        0        0     3262 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/merge_interface.py
--rw-r--r--   0        0        0     3103 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/metadata_interface.py
--rw-r--r--   0        0        0    18964 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/obograph_interface.py
--rw-r--r--   0        0        0     1003 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/obolegacy_interface.py
--rw-r--r--   0        0        0      784 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/ontology_interface.py
--rw-r--r--   0        0        0    10988 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/owl_interface.py
--rw-r--r--   0        0        0     8236 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/patcher_interface.py
--rw-r--r--   0        0        0     1955 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/rdf_interface.py
--rw-r--r--   0        0        0     2459 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/relation_graph_interface.py
--rw-r--r--   0        0        0     2638 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/search_interface.py
--rw-r--r--   0        0        0    12778 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/semsim_interface.py
--rw-r--r--   0        0        0     1063 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/skos_interface.py
--rw-r--r--   0        0        0     2112 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/subsetter_interface.py
--rw-r--r--   0        0        0    10140 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/summary_statistics_interface.py
--rw-r--r--   0        0        0    18296 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/taxon_constraint_interface.py
--rw-r--r--   0        0        0     7511 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/text_annotator_interface.py
--rw-r--r--   0        0        0     3033 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/validator_interface.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/__init__.py
--rw-r--r--   0        0        0     2087 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/heatmap_writer.py
--rw-r--r--   0        0        0     1698 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/html_writer.py
--rw-r--r--   0        0        0     1379 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/obograph_writer.py
--rw-r--r--   0        0        0     3444 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/rollup_report_writer.py
--rw-r--r--   0        0        0      739 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_axiom_writer.py
--rw-r--r--   0        0        0     7906 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_csv_writer.py
--rw-r--r--   0        0        0     1284 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_fhir_writer.py
--rw-r--r--   0        0        0     2524 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_info_writer.py
--rw-r--r--   0        0        0     1231 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_json_lines_writer.py
--rw-r--r--   0        0        0     1806 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_json_writer.py
--rw-r--r--   0        0        0      741 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_kgcl_writer.py
--rw-r--r--   0        0        0     2088 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_markdown_writer.py
--rw-r--r--   0        0        0     1152 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_nl_writer.py
--rw-r--r--   0        0        0     1117 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_obo_json_writer.py
--rw-r--r--   0        0        0     3496 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_obo_writer.py
--rw-r--r--   0        0        0     1270 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_owl_functional_writer.py
--rw-r--r--   0        0        0     2244 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_rdf_writer.py
--rw-r--r--   0        0        0     5129 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_writer.py
--rw-r--r--   0        0        0     1318 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_yaml_writer.py
--rw-r--r--   0        0        0      113 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/mappers/__init__.py
--rw-r--r--   0        0        0     3717 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/mappers/base_mapper.py
--rw-r--r--   0        0        0     1849 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/mappers/ontology_metadata_mapper.py
--rw-r--r--   0        0        0     2179 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/__init__.py
--rw-r--r--   0        0        0     1524 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/association_parser.py
--rw-r--r--   0        0        0      522 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/association_parser_factory.py
--rw-r--r--   0        0        0     4731 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/boomer_parser.py
--rw-r--r--   0        0        0     2208 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/gaf_association_parser.py
--rw-r--r--   0        0        0     1090 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/gencc_association_parser.py
--rw-r--r--   0        0        0     1130 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/hpoa_association_parser.py
--rw-r--r--   0        0        0      602 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/hpoa_g2p_association_parser.py
--rw-r--r--   0        0        0      653 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/kgx_association_parser.py
--rw-r--r--   0        0        0     1666 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/mim2gene_association_parser.py
--rw-r--r--   0        0        0      525 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/pairwise_association_parser.py
--rw-r--r--   0        0        0     1432 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/parser_base.py
--rw-r--r--   0        0        0      707 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/phaf_association_parser.py
--rw-r--r--   0        0        0     8084 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/xaf_association_parser.py
--rw-r--r--   0        0        0     2210 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/resource.py
--rw-r--r--   0        0        0    14739 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/selector.py
--rw-r--r--   0        0        0      177 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/types.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/__init__.py
--rw-r--r--   0        0        0     1613 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/apikey_manager.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/associations/__init__.py
--rw-r--r--   0        0        0    13441 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/associations/association_differ.py
--rw-r--r--   0        0        0     3419 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/associations/association_index.py
--rw-r--r--   0        0        0     1540 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/basic_utils.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/graph/__init__.py
--rw-r--r--   0        0        0     2490 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/graph/networkx_bridge.py
--rw-r--r--   0        0        0     2918 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/graph/relationship_walker.py
--rw-r--r--   0        0        0      993 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/identifier_utils.py
--rw-r--r--   0        0        0      999 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/iterator_utils.py
--rw-r--r--   0        0        0     3345 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/kgcl_utilities.py
--rw-r--r--   0        0        0      850 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/label_utilities.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/lexical/__init__.py
--rw-r--r--   0        0        0    19516 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/lexical/lexical_indexer.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/mapping/__init__.py
--rw-r--r--   0        0        0    14467 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/mapping/boomer_utils.py
--rw-r--r--   0        0        0    15328 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/mapping/cross_ontology_diffs.py
--rw-r--r--   0        0        0      751 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/mapping/mapping_propagator.py
--rw-r--r--   0        0        0     2270 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/mapping/mapping_validation.py
--rw-r--r--   0        0        0     2694 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/mapping/sssom_utils.py
--rw-r--r--   0        0        0      684 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/ner_utilities.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/nlp/__init__.py
--rw-r--r--   0        0        0     3358 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/nlp/natual_language_generation.py
--rw-r--r--   0        0        0      136 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/oboformat_utils.py
--rw-r--r--   0        0        0    22274 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/obograph_utils.py
--rw-r--r--   0        0        0     2275 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/ontology_builder.py
--rw-r--r--   0        0        0      379 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/rate_limiter.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/reasoning/__init__.py
--rw-r--r--   0        0        0      569 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/reasoning/relation_graph.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/semsim/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/semsim/similarity_utils.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/stats/__init__.py
--rw-r--r--   0        0        0     1511 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/stats/hypergeometric.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/subsets/__init__.py
--rw-r--r--   0        0        0     2819 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/subsets/slimmer_utils.py
--rw-r--r--   0        0        0     4701 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/subsets/subset_analysis.py
--rw-r--r--   0        0        0    11592 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/subsets/value_set_expander.py
--rw-r--r--   0        0        0    13212 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/table_filler.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/taxon/__init__.py
--rw-r--r--   0        0        0     1743 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/taxon/taxon_constraint_utils.py
--rw-r--r--   0        0        0        0 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/validation/__init__.py
--rw-r--r--   0        0        0    10097 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/validation/definition_ontology_rule.py
--rw-r--r--   0        0        0     7492 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/validation/disjointness_rule.py
--rw-r--r--   0        0        0     1729 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/validation/lint_utils.py
--rw-r--r--   0        0        0     1402 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/validation/ontology_rule.py
--rw-r--r--   0        0        0     1313 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/validation/rule_runner.py
--rw-r--r--   0        0        0     8867 1970-01-01 00:00:00.000000 oaklib-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-19 00:06:17.004512 oaklib-0.5.7/LICENSE
+-rw-r--r--   0        0        0     7241 2023-05-19 00:06:17.004512 oaklib-0.5.7/README.md
+-rw-r--r--   0        0        0     1880 2023-05-19 00:07:13.982994 oaklib-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0      271 2023-05-19 00:06:17.148518 oaklib-0.5.7/src/oaklib/__init__.py
+-rw-r--r--   0        0        0   194032 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/cli.py
+-rw-r--r--   0        0        0       64 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/__init__.py
+-rw-r--r--   0        0        0      372 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/go-human-input-spec.yaml
+-rw-r--r--   0        0        0      162 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/go-pombase-input-spec.yaml
+-rw-r--r--   0        0        0      109 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/hpoa-g2p-input-spec.yaml
+-rw-r--r--   0        0        0      106 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/hpoa-input-spec.yaml
+-rw-r--r--   0        0        0     1903 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
+-rw-r--r--   0        0        0      562 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/mondo-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      109 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/mondo-gencc-input-spec.yaml
+-rw-r--r--   0        0        0      118 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
+-rw-r--r--   0        0        0     4537 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/obograph-style.json
+-rw-r--r--   0        0        0      256 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/omo-to-skos.sssom.tsv
+-rw-r--r--   0        0        0      131 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/value-set-expander.conf.yaml
+-rw-r--r--   0        0        0      128 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/constants.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/converters/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/converters/data_model_converter.py
+-rw-r--r--   0        0        0     2561 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/converters/logical_definition_flattener.py
+-rw-r--r--   0        0        0     2371 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/converters/obo_graph_to_cx_converter.py
+-rw-r--r--   0        0        0    12159 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/converters/obo_graph_to_fhir_converter.py
+-rw-r--r--   0        0        0     5713 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/converters/obo_graph_to_obo_format_converter.py
+-rw-r--r--   0        0        0     5789 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
+-rw-r--r--   0        0        0       60 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/__init__.py
+-rw-r--r--   0        0        0     4034 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/association.owl.ttl
+-rw-r--r--   0        0        0    36266 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/association.py
+-rw-r--r--   0        0        0    11740 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/association.yaml
+-rw-r--r--   0        0        0     6165 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/class_enrichment.owl.ttl
+-rw-r--r--   0        0        0    13328 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/class_enrichment.py
+-rw-r--r--   0        0        0     3192 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/class_enrichment.yaml
+-rw-r--r--   0        0        0    19083 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
+-rw-r--r--   0        0        0    24246 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/cross_ontology_diff.py
+-rw-r--r--   0        0        0    10687 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/cross_ontology_diff.yaml
+-rw-r--r--   0        0        0    29418 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/cx.py
+-rw-r--r--   0        0        0     6314 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/cx.yaml
+-rw-r--r--   0        0        0    15826 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/fhir.owl.ttl
+-rw-r--r--   0        0        0    35744 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/fhir.py
+-rw-r--r--   0        0        0     5064 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/fhir.yaml
+-rw-r--r--   0        0        0    14564 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/input_specification.py
+-rw-r--r--   0        0        0     3560 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/input_specification.yaml
+-rw-r--r--   0        0        0    15768 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/item_list.py
+-rw-r--r--   0        0        0     6339 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/item_list.yaml
+-rw-r--r--   0        0        0     8984 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/lexical_index.owl.ttl
+-rw-r--r--   0        0        0    17256 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/lexical_index.py
+-rw-r--r--   0        0        0     6429 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/lexical_index.schema.json
+-rw-r--r--   0        0        0     4016 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/lexical_index.yaml
+-rw-r--r--   0        0        0    26434 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/mapping_cluster_datamodel.py
+-rw-r--r--   0        0        0     7317 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
+-rw-r--r--   0        0        0   226115 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
+-rw-r--r--   0        0        0    32727 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.py
+-rw-r--r--   0        0        0    12889 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
+-rw-r--r--   0        0        0     3607 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.yaml
+-rw-r--r--   0        0        0    25354 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/obograph.owl.ttl
+-rw-r--r--   0        0        0    46876 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/obograph.py
+-rw-r--r--   0        0        0    22375 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/obograph.schema.json
+-rw-r--r--   0        0        0    18191 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/obograph.yaml
+-rw-r--r--   0        0        0    59793 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.owl.ttl
+-rw-r--r--   0        0        0   117175 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.py
+-rw-r--r--   0        0        0    95288 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.schema.json
+-rw-r--r--   0        0        0    30433 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.yaml
+-rw-r--r--   0        0        0    14759 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/oxo.owl.ttl
+-rw-r--r--   0        0        0    21914 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/oxo.py
+-rw-r--r--   0        0        0     4392 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/oxo.yaml
+-rw-r--r--   0        0        0     3240 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/search.py
+-rw-r--r--   0        0        0    16948 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/search_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25145 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/search_datamodel.py
+-rw-r--r--   0        0        0     6683 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/search_datamodel.yaml
+-rw-r--r--   0        0        0      287 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/settings.py
+-rw-r--r--   0        0        0    12767 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/similarity.owl.ttl
+-rw-r--r--   0        0        0    22226 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/similarity.py
+-rw-r--r--   0        0        0     5511 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/similarity.yaml
+-rw-r--r--   0        0        0    31217 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
+-rw-r--r--   0        0        0    50743 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.py
+-rw-r--r--   0        0        0    21176 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
+-rw-r--r--   0        0        0    16246 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.yaml
+-rw-r--r--   0        0        0     9909 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/taxon_constraints.owl.ttl
+-rw-r--r--   0        0        0    18430 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/taxon_constraints.py
+-rw-r--r--   0        0        0     5879 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/taxon_constraints.yaml
+-rw-r--r--   0        0        0    11599 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/text_annotator.owl.ttl
+-rw-r--r--   0        0        0    20418 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/text_annotator.py
+-rw-r--r--   0        0        0     2464 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/text_annotator.schema.json
+-rw-r--r--   0        0        0     4219 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/text_annotator.yaml
+-rw-r--r--   0        0        0    13670 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25351 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.py
+-rw-r--r--   0        0        0    10783 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.schema.json
+-rw-r--r--   0        0        0     7510 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.yaml
+-rw-r--r--   0        0        0     6640 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/value_set_configuration.owl.ttl
+-rw-r--r--   0        0        0     8458 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/value_set_configuration.py
+-rw-r--r--   0        0        0     2276 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/value_set_configuration.yaml
+-rw-r--r--   0        0        0     5614 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/vocabulary.py
+-rw-r--r--   0        0        0     5849 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/implementations/aggregator/__init__.py
+-rw-r--r--   0        0        0     5996 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/implementations/aggregator/aggregator_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/agrkb/__init__.py
+-rw-r--r--   0        0        0     8126 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/agrkb/agrkb_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/amigo/__init__.py
+-rw-r--r--   0        0        0     4601 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/amigo/amigo_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/cx/__init__.py
+-rw-r--r--   0        0        0     1985 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/cx/cx_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/eutils/__init__.py
+-rw-r--r--   0        0        0     2179 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/eutils/eutils_implementation.py
+-rw-r--r--   0        0        0     1053 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/eutils/pubmed_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/fhir/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/funowl/__init__.py
+-rw-r--r--   0        0        0     8473 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/funowl/funowl_implementation.py
+-rw-r--r--   0        0        0     2313 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/gilda.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/kgx/__init__.py
+-rw-r--r--   0        0        0    30434 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/kgx/kgx_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/monarch/__init__.py
+-rw-r--r--   0        0        0     7009 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/monarch/monarch_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/neo4j/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/obograph/__init__.py
+-rw-r--r--   0        0        0    16240 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/obograph/obograph_implementation.py
+-rw-r--r--   0        0        0      267 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ols/__init__.py
+-rw-r--r--   0        0        0      132 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ols/constants.py
+-rw-r--r--   0        0        0     7942 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ols/ols_implementation.py
+-rw-r--r--   0        0        0      686 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ols/oxo_utils.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontobee/__init__.py
+-rw-r--r--   0        0        0     2532 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontobee/ontobee_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontoportal/__init__.py
+-rw-r--r--   0        0        0      382 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontoportal/agroportal_implementation.py
+-rw-r--r--   0        0        0     1238 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontoportal/bioportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontoportal/matportal_implementation.py
+-rw-r--r--   0        0        0    12106 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/owlery/__init__.py
+-rw-r--r--   0        0        0      427 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/owlery/owlery_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/pronto/__init__.py
+-rw-r--r--   0        0        0    35620 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/pronto/pronto_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/robot/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/scigraph/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/semsimian/__init__.py
+-rw-r--r--   0        0        0      246 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/semsimian/profiler.py
+-rw-r--r--   0        0        0     4110 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/semsimian/semsimian_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/simpleobo/__init__.py
+-rw-r--r--   0        0        0    34382 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
+-rw-r--r--   0        0        0    21451 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/simpleobo/simple_obo_parser.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/skos/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/solor/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/solr/__init__.py
+-rw-r--r--   0        0        0       96 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sparql/__init__.py
+-rw-r--r--   0        0        0    36699 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
+-rw-r--r--   0        0        0      885 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sparql/lov_implementation.py
+-rw-r--r--   0        0        0     1721 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
+-rw-r--r--   0        0        0     2658 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sparql/sparql_implementation.py
+-rw-r--r--   0        0        0     2326 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sparql/sparql_query.py
+-rw-r--r--   0        0        0       96 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sqldb/__init__.py
+-rw-r--r--   0        0        0   106362 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sqldb/sql_implementation.py
+-rw-r--r--   0        0        0     1903 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sqldb/sqlite_utils.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/tccm/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/translator/__init__.py
+-rw-r--r--   0        0        0     3283 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/translator/translator_implementation.py
+-rw-r--r--   0        0        0      108 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ubergraph/__init__.py
+-rw-r--r--   0        0        0    19393 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/umls/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/uniprot/__init__.py
+-rw-r--r--   0        0        0     9603 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/implementations/uniprot/uniprot_implementation.py
+-rw-r--r--   0        0        0       96 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/implementations/wikidata/__init__.py
+-rw-r--r--   0        0        0    17121 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/implementations/wikidata/wikidata_implementation.py
+-rw-r--r--   0        0        0      913 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/__init__.py
+-rw-r--r--   0        0        0    20557 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/association_provider_interface.py
+-rw-r--r--   0        0        0    50981 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/basic_ontology_interface.py
+-rw-r--r--   0        0        0     8830 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/class_enrichment_calculation_interface.py
+-rw-r--r--   0        0        0    11720 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/differ_interface.py
+-rw-r--r--   0        0        0     2649 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/dumper_interface.py
+-rw-r--r--   0        0        0      977 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/embedding_provider_interface.py
+-rw-r--r--   0        0        0    13681 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/mapping_provider_interface.py
+-rw-r--r--   0        0        0     3262 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/merge_interface.py
+-rw-r--r--   0        0        0     3103 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/metadata_interface.py
+-rw-r--r--   0        0        0    18964 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/obograph_interface.py
+-rw-r--r--   0        0        0     1003 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/obolegacy_interface.py
+-rw-r--r--   0        0        0      784 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/ontology_interface.py
+-rw-r--r--   0        0        0    10988 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/owl_interface.py
+-rw-r--r--   0        0        0     8236 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/patcher_interface.py
+-rw-r--r--   0        0        0     1955 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/rdf_interface.py
+-rw-r--r--   0        0        0     2459 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/relation_graph_interface.py
+-rw-r--r--   0        0        0     3759 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/search_interface.py
+-rw-r--r--   0        0        0    12778 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/semsim_interface.py
+-rw-r--r--   0        0        0     1063 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/skos_interface.py
+-rw-r--r--   0        0        0     2112 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/subsetter_interface.py
+-rw-r--r--   0        0        0    10140 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/summary_statistics_interface.py
+-rw-r--r--   0        0        0    18296 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/taxon_constraint_interface.py
+-rw-r--r--   0        0        0     7511 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/text_annotator_interface.py
+-rw-r--r--   0        0        0     3033 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/validator_interface.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/__init__.py
+-rw-r--r--   0        0        0     2087 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/heatmap_writer.py
+-rw-r--r--   0        0        0     1698 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/html_writer.py
+-rw-r--r--   0        0        0     1379 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/obograph_writer.py
+-rw-r--r--   0        0        0     3444 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/rollup_report_writer.py
+-rw-r--r--   0        0        0      739 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_axiom_writer.py
+-rw-r--r--   0        0        0     7906 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_csv_writer.py
+-rw-r--r--   0        0        0     1284 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_fhir_writer.py
+-rw-r--r--   0        0        0     2524 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_info_writer.py
+-rw-r--r--   0        0        0     1231 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_json_lines_writer.py
+-rw-r--r--   0        0        0     1806 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_json_writer.py
+-rw-r--r--   0        0        0      741 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_kgcl_writer.py
+-rw-r--r--   0        0        0     2088 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_markdown_writer.py
+-rw-r--r--   0        0        0     1152 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_nl_writer.py
+-rw-r--r--   0        0        0     1117 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_obo_json_writer.py
+-rw-r--r--   0        0        0     3496 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_obo_writer.py
+-rw-r--r--   0        0        0     1270 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_owl_functional_writer.py
+-rw-r--r--   0        0        0     2244 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_rdf_writer.py
+-rw-r--r--   0        0        0     5129 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_writer.py
+-rw-r--r--   0        0        0     1318 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_yaml_writer.py
+-rw-r--r--   0        0        0      113 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/mappers/__init__.py
+-rw-r--r--   0        0        0     3717 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/mappers/base_mapper.py
+-rw-r--r--   0        0        0     1849 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/mappers/ontology_metadata_mapper.py
+-rw-r--r--   0        0        0     2179 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/__init__.py
+-rw-r--r--   0        0        0     1524 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/association_parser.py
+-rw-r--r--   0        0        0      522 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/association_parser_factory.py
+-rw-r--r--   0        0        0     4731 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/boomer_parser.py
+-rw-r--r--   0        0        0     2208 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/gaf_association_parser.py
+-rw-r--r--   0        0        0     1090 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/gencc_association_parser.py
+-rw-r--r--   0        0        0     1130 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/hpoa_association_parser.py
+-rw-r--r--   0        0        0      602 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/hpoa_g2p_association_parser.py
+-rw-r--r--   0        0        0      653 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/kgx_association_parser.py
+-rw-r--r--   0        0        0     1666 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/mim2gene_association_parser.py
+-rw-r--r--   0        0        0      525 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/pairwise_association_parser.py
+-rw-r--r--   0        0        0     1432 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/parser_base.py
+-rw-r--r--   0        0        0      707 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/phaf_association_parser.py
+-rw-r--r--   0        0        0     8084 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/xaf_association_parser.py
+-rw-r--r--   0        0        0     2210 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/resource.py
+-rw-r--r--   0        0        0    14702 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/selector.py
+-rw-r--r--   0        0        0      177 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/types.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/__init__.py
+-rw-r--r--   0        0        0     1613 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/apikey_manager.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/associations/__init__.py
+-rw-r--r--   0        0        0    13441 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/associations/association_differ.py
+-rw-r--r--   0        0        0     3419 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/associations/association_index.py
+-rw-r--r--   0        0        0     1540 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/basic_utils.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/graph/__init__.py
+-rw-r--r--   0        0        0     2490 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/graph/networkx_bridge.py
+-rw-r--r--   0        0        0     2918 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/graph/relationship_walker.py
+-rw-r--r--   0        0        0      993 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/identifier_utils.py
+-rw-r--r--   0        0        0      999 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/iterator_utils.py
+-rw-r--r--   0        0        0     3345 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/kgcl_utilities.py
+-rw-r--r--   0        0        0      850 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/label_utilities.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/lexical/__init__.py
+-rw-r--r--   0        0        0    19516 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/lexical/lexical_indexer.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/mapping/__init__.py
+-rw-r--r--   0        0        0    14467 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/mapping/boomer_utils.py
+-rw-r--r--   0        0        0    15328 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/mapping/cross_ontology_diffs.py
+-rw-r--r--   0        0        0      751 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/mapping/mapping_propagator.py
+-rw-r--r--   0        0        0     2270 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/mapping/mapping_validation.py
+-rw-r--r--   0        0        0     2694 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/mapping/sssom_utils.py
+-rw-r--r--   0        0        0      684 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/ner_utilities.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/nlp/__init__.py
+-rw-r--r--   0        0        0     3358 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/nlp/natual_language_generation.py
+-rw-r--r--   0        0        0      136 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/oboformat_utils.py
+-rw-r--r--   0        0        0    22646 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/obograph_utils.py
+-rw-r--r--   0        0        0     2275 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/ontology_builder.py
+-rw-r--r--   0        0        0      379 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/rate_limiter.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/reasoning/__init__.py
+-rw-r--r--   0        0        0      569 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/reasoning/relation_graph.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/semsim/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/semsim/similarity_utils.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/stats/__init__.py
+-rw-r--r--   0        0        0     1511 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/stats/hypergeometric.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/subsets/__init__.py
+-rw-r--r--   0        0        0     2819 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/subsets/slimmer_utils.py
+-rw-r--r--   0        0        0     4701 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/subsets/subset_analysis.py
+-rw-r--r--   0        0        0    11592 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/subsets/value_set_expander.py
+-rw-r--r--   0        0        0    13212 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/table_filler.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/taxon/__init__.py
+-rw-r--r--   0        0        0     1743 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/taxon/taxon_constraint_utils.py
+-rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/validation/__init__.py
+-rw-r--r--   0        0        0    10097 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/validation/definition_ontology_rule.py
+-rw-r--r--   0        0        0     7492 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/validation/disjointness_rule.py
+-rw-r--r--   0        0        0     1729 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/validation/lint_utils.py
+-rw-r--r--   0        0        0     1402 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/validation/ontology_rule.py
+-rw-r--r--   0        0        0     1313 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/validation/rule_runner.py
+-rw-r--r--   0        0        0     8866 1970-01-01 00:00:00.000000 oaklib-0.5.7/PKG-INFO
```

### Comparing `oaklib-0.5.6/LICENSE` & `oaklib-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/README.md` & `oaklib-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/pyproject.toml` & `oaklib-0.5.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "oaklib"
-version = "v0.5.6"
+version = "v0.5.7"
 description = "Ontology Access Kit: Python library for common ontology operations over a variety of backends"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
 curies = ">=0.4.0"
 pronto = ">=2.5.0"
 SPARQLWrapper = "*"
 SQLAlchemy = ">=1.4.32"
-linkml-runtime = ">=1.2.15"
+linkml-runtime = ">=1.5.3"
 networkx = ">=2.7.1"
 sssom-schema = ">=0.11.0"
 sssom = ">=0.3.26"
 ratelimit = ">=2.2.1"
 appdirs = ">=1.4.4"
 semsql = ">=0.3.1"
 lark = ">=1.1.2"
@@ -33,15 +33,15 @@
 linkml-renderer = ">=0.1.2"
 airium = ">=0.2.5"
 ndex2 = "^3.5.0"
 pysolr = "^3.9.0"
 eutils = ">=0.6.0"
 requests-cache = "^1.0.1"
 click = "*"
-semsimian = ">=0.1.13"
+semsimian = "0.1.13"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 Sphinx = ">=6.1.3"
 pandas = ">=1.5.1"
 jupyter = ">=1.0.0"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `oaklib-0.5.6/src/oaklib/cli.py` & `oaklib-0.5.7/src/oaklib/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,18 @@
     ancestors_with_stats,
     default_stylemap_path,
     graph_to_image,
     graph_to_tree_display,
     shortest_paths,
     trim_graph,
 )
-from oaklib.utilities.subsets.slimmer_utils import roll_up_to_named_subset
+from oaklib.utilities.subsets.slimmer_utils import (
+    filter_redundant,
+    roll_up_to_named_subset,
+)
 from oaklib.utilities.table_filler import ColumnDependency, TableFiller, TableMetadata
 from oaklib.utilities.taxon.taxon_constraint_utils import parse_gain_loss_file
 from oaklib.utilities.validation.definition_ontology_rule import (
     TextAndLogicalDefinitionMatchOntologyRule,
 )
 from oaklib.utilities.validation.lint_utils import lint_ontology
 from oaklib.utilities.validation.rule_runner import RuleRunner
@@ -781,14 +784,21 @@
             query_terms = query_terms[1:]
             if isinstance(impl, SemanticSimilarityInterface):
                 chain_results(
                     impl.setwise_most_recent_common_ancestors(rest, predicates=this_predicates)
                 )
             else:
                 raise NotImplementedError
+        elif term.startswith(".nr"):
+            # graph query: non-redundant
+            params = _parse_params(term)
+            this_predicates = params.get("predicates", predicates)
+            rest = list(query_terms_iterator([query_terms[0]], impl))
+            query_terms = query_terms[1:]
+            chain_results(filter_redundant(impl, rest, this_predicates))
         else:
             # term is not query syntax: feed directly to search
             if not isinstance(impl, SearchInterface):
                 raise NotImplementedError(f"Search not implemented for {type(impl)}")
             cfg = create_search_configuration(term)
             logging.info(f"Search config: {term} => {cfg}")
             chain_results(impl.basic_search(cfg.search_terms[0], config=cfg))
```

### Comparing `oaklib-0.5.6/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml` & `oaklib-0.5.7/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/conf/mondo-g2d-input-spec.yaml` & `oaklib-0.5.7/src/oaklib/conf/mondo-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/conf/obograph-style.json` & `oaklib-0.5.7/src/oaklib/conf/obograph-style.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/converters/data_model_converter.py` & `oaklib-0.5.7/src/oaklib/converters/data_model_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/converters/logical_definition_flattener.py` & `oaklib-0.5.7/src/oaklib/converters/logical_definition_flattener.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/converters/obo_graph_to_cx_converter.py` & `oaklib-0.5.7/src/oaklib/converters/obo_graph_to_cx_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/converters/obo_graph_to_fhir_converter.py` & `oaklib-0.5.7/src/oaklib/converters/obo_graph_to_fhir_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/converters/obo_graph_to_obo_format_converter.py` & `oaklib-0.5.7/src/oaklib/converters/obo_graph_to_obo_format_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py` & `oaklib-0.5.7/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from dataclasses import dataclass
 from typing import Any, Tuple, Union
 
 import rdflib
-from rdflib import OWL, RDFS
+from rdflib import OWL, RDF, RDFS
 
 from oaklib import BasicOntologyInterface
 from oaklib.converters.data_model_converter import DataModelConverter
 from oaklib.datamodels.obograph import (
-    RDF,
     Edge,
     Graph,
     GraphDocument,
     Meta,
     Node,
     PropertyTypeEnum,
     PropertyValue,
```

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/association.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/association.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/association.py` & `oaklib-0.5.7/src/oaklib/datamodels/association.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/association.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/association.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/class_enrichment.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/class_enrichment.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/class_enrichment.py` & `oaklib-0.5.7/src/oaklib/datamodels/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/class_enrichment.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/cross_ontology_diff.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/cross_ontology_diff.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/cross_ontology_diff.py` & `oaklib-0.5.7/src/oaklib/datamodels/cross_ontology_diff.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/cross_ontology_diff.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/cross_ontology_diff.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/cx.py` & `oaklib-0.5.7/src/oaklib/datamodels/cx.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/cx.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/cx.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/fhir.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/fhir.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/fhir.py` & `oaklib-0.5.7/src/oaklib/datamodels/fhir.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/fhir.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/fhir.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/input_specification.py` & `oaklib-0.5.7/src/oaklib/datamodels/input_specification.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/input_specification.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/input_specification.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/item_list.py` & `oaklib-0.5.7/src/oaklib/datamodels/item_list.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/item_list.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/item_list.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/lexical_index.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/lexical_index.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/lexical_index.py` & `oaklib-0.5.7/src/oaklib/datamodels/lexical_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/lexical_index.schema.json` & `oaklib-0.5.7/src/oaklib/datamodels/lexical_index.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/lexical_index.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/lexical_index.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/mapping_cluster_datamodel.py` & `oaklib-0.5.7/src/oaklib/datamodels/mapping_cluster_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/mapping_cluster_datamodel.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/mapping_cluster_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.py` & `oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.schema.json` & `oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/obograph.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/obograph.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/obograph.py` & `oaklib-0.5.7/src/oaklib/datamodels/obograph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from obograph.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-05-03T08:52:36
+# Generation date: 2023-05-13T10:22:20
 # Schema: obographs_datamodel
 #
 # id: https://github.com/geneontology/obographs
 # description: A data model for graph-oriented representations of ontologies. Each ontology is represented as a
 #              Graph, and multiple ontologies can be connected together in a GraphDocument. The principle elements
 #              of a Graph are Node objects and Edge objects. A Node represents an arbitrary ontology element,
 #              including but not limited to the core terms in the ontology. Edges represent simple relationships
```

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/obograph.schema.json` & `oaklib-0.5.7/src/oaklib/datamodels/obograph.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/obograph.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/obograph.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.py` & `oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.schema.json` & `oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/oxo.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/oxo.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/oxo.py` & `oaklib-0.5.7/src/oaklib/datamodels/oxo.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/oxo.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/oxo.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/search.py` & `oaklib-0.5.7/src/oaklib/datamodels/search.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/search_datamodel.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/search_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/search_datamodel.py` & `oaklib-0.5.7/src/oaklib/datamodels/search_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/search_datamodel.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/search_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/similarity.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/similarity.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/similarity.py` & `oaklib-0.5.7/src/oaklib/datamodels/similarity.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/similarity.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/similarity.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.py` & `oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.schema.json` & `oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/taxon_constraints.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/taxon_constraints.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/taxon_constraints.py` & `oaklib-0.5.7/src/oaklib/datamodels/taxon_constraints.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/taxon_constraints.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/taxon_constraints.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/text_annotator.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/text_annotator.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/text_annotator.py` & `oaklib-0.5.7/src/oaklib/datamodels/text_annotator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/text_annotator.schema.json` & `oaklib-0.5.7/src/oaklib/datamodels/text_annotator.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/text_annotator.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/text_annotator.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.py` & `oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.schema.json` & `oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/value_set_configuration.owl.ttl` & `oaklib-0.5.7/src/oaklib/datamodels/value_set_configuration.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/value_set_configuration.py` & `oaklib-0.5.7/src/oaklib/datamodels/value_set_configuration.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/value_set_configuration.yaml` & `oaklib-0.5.7/src/oaklib/datamodels/value_set_configuration.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/datamodels/vocabulary.py` & `oaklib-0.5.7/src/oaklib/datamodels/vocabulary.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/__init__.py` & `oaklib-0.5.7/src/oaklib/implementations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 from functools import cache
 
 from class_resolver import ClassResolver
 
 from oaklib.implementations.aggregator.aggregator_implementation import (
     AggregatorImplementation,
 )
+from oaklib.implementations.agrkb.agrkb_implementation import AGRKBImplementation
 from oaklib.implementations.amigo.amigo_implementation import AmiGOImplementation
 from oaklib.implementations.cx.cx_implementation import CXImplementation
 from oaklib.implementations.eutils.pubmed_implementation import PubMedImplementation
 from oaklib.implementations.funowl.funowl_implementation import FunOwlImplementation
 from oaklib.implementations.gilda import GildaImplementation
 from oaklib.implementations.kgx.kgx_implementation import KGXImplementation
+from oaklib.implementations.monarch.monarch_implementation import MonarchImplementation
 from oaklib.implementations.ols import (
     BaseOlsImplementation,
     OlsImplementation,
     TIBOlsImplementation,
 )
 from oaklib.implementations.ontobee.ontobee_implementation import OntobeeImplementation
 from oaklib.implementations.ontoportal.agroportal_implementation import (
@@ -60,21 +62,23 @@
 from oaklib.interfaces import OntologyInterface
 
 __all__ = [
     "get_implementation_resolver",
     # Concrete classes
     "AggregatorImplementation",
     "AgroPortalImplementation",
+    "AGRKBImplementation",
     "AmiGOImplementation",
     "BioPortalImplementation",
     "CXImplementation",
     "EcoPortalImplementation",
     "MatPortalImplementation",
     "OlsImplementation",
     "TIBOlsImplementation",
+    "MonarchImplementation",
     "OntobeeImplementation",
     "ProntoImplementation",
     "SimpleOboImplementation",
     "SqlImplementation",
     "UbergraphImplementation",
     "LovImplementation",
     "SparqlImplementation",
```

### Comparing `oaklib-0.5.6/src/oaklib/implementations/aggregator/aggregator_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/aggregator/aggregator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/amigo/amigo_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/amigo/amigo_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 AMIGO_ENDPOINT = "http://golr.geneontology.org/solr/"
 
 logger = logging.getLogger(__name__)
 
 LIMIT = 10000
 
 # TODO: derive from schema
+DOCUMENT_CATEGORY = "document_category"
 BIOENTITY = "bioentity"
 BIOENTITY_LABEL = "bioentity_label"
 ANNOTATION_CLASS = "annotation_class"
 ANNOTATION_CLASS_LABEL = "annotation_class_label"
 ISA_PARTOF_CLOSURE = "isa_partof_closure"
 TAXON_CLOSURE = "taxon_closure"
 ASSIGNED_BY = "assigned_by"
@@ -127,15 +128,15 @@
         property_filter: Dict[PRED_CURIE, Any] = None,
         subject_closure_predicates: Optional[List[PRED_CURIE]] = None,
         predicate_closure_predicates: Optional[List[PRED_CURIE]] = None,
         object_closure_predicates: Optional[List[PRED_CURIE]] = None,
         include_modified: bool = False,
     ) -> Iterator[Association]:
         solr = self._solr
-        fq = {"document_category": ["annotation"]}
+        fq = {DOCUMENT_CATEGORY: ["annotation"]}
         if subjects:
             subjects = [_unnnormalize(s) for s in subjects]
             fq[BIOENTITY] = subjects
         if objects:
             objects = list(objects)
             fq[ISA_PARTOF_CLOSURE] = objects
         if self._source:
```

### Comparing `oaklib-0.5.6/src/oaklib/implementations/cx/cx_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/cx/cx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/eutils/eutils_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/eutils/eutils_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/eutils/pubmed_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/eutils/pubmed_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/funowl/funowl_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/funowl/funowl_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/gilda.py` & `oaklib-0.5.7/src/oaklib/implementations/gilda.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/kgx/kgx_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/kgx/kgx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/obograph/obograph_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/obograph/obograph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/ols/ols_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/ols/ols_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/ols/oxo_utils.py` & `oaklib-0.5.7/src/oaklib/implementations/ols/oxo_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/ontobee/ontobee_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/ontobee/ontobee_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/ontoportal/bioportal_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/ontoportal/bioportal_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py` & `oaklib-0.5.7/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/pronto/pronto_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/pronto/pronto_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/semsimian/semsimian_implementation.py` & `oaklib-0.5.7/src/oaklib/interfaces/semsim_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,35 @@
-"""Rust implementation of semantic similarity measures."""
-import inspect
 import logging
 import math
 import statistics
+from abc import ABC
 from collections import defaultdict
-from dataclasses import dataclass
-from typing import ClassVar, Iterable, Iterator, List, Optional, Tuple, Union
+from typing import Iterable, Iterator, List, Optional, Tuple
 
-from semsimian import get_intersection, jaccard_similarity, mrca_and_score
+import networkx as nx
 
 from oaklib.datamodels.similarity import (
     BestMatch,
     TermInfo,
     TermPairwiseSimilarity,
     TermSetPairwiseSimilarity,
 )
 from oaklib.datamodels.vocabulary import OWL_THING
 from oaklib.interfaces.basic_ontology_interface import BasicOntologyInterface
-from oaklib.interfaces.obograph_interface import GraphTraversalMethod, OboGraphInterface
-from oaklib.interfaces.search_interface import SearchInterface
-from oaklib.interfaces.semsim_interface import SemanticSimilarityInterface
+from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.types import CURIE, PRED_CURIE
+from oaklib.utilities.obograph_utils import as_digraph
+from oaklib.utilities.semsim.similarity_utils import setwise_jaccard_similarity
 
-wrapped_adapter: BasicOntologyInterface = None
 
-__all__ = [
-    "SemSimianImplementation",
-]
-
-
-@dataclass
-class SemSimianImplementation(SearchInterface, SemanticSimilarityInterface, OboGraphInterface):
-    """Rust implementation of semantic similarity measures."""
-
-    delegated_methods: ClassVar[List[str]] = [
-        BasicOntologyInterface.label,
-        BasicOntologyInterface.curie_to_uri,
-        BasicOntologyInterface.uri_to_curie,
-        BasicOntologyInterface.ontologies,
-        BasicOntologyInterface.obsoletes,
-        SearchInterface.basic_search,
-        OboGraphInterface.node,
-    ]
-
-    def __post_init__(self):
-        slug = self.resource.slug
-        from oaklib.selector import get_adapter
-
-        slug = slug.replace("semsimian:", "")
-        logging.info(f"Wrapping an existing OAK implementation to fetch {slug}")
-        self.wrapped_adapter = get_adapter(slug)
-        methods = dict(inspect.getmembers(self.wrapped_adapter))
-        for m in self.delegated_methods:
-            mn = m if isinstance(m, str) else m.__name__
-            setattr(SemSimianImplementation, mn, methods[mn])
+class SemanticSimilarityInterface(BasicOntologyInterface, ABC):
+    """
+    An interface for calculating similarity measures between pairs of terms or
+    collections of terms
+    """
 
     def most_recent_common_ancestors(
         self,
         subject: CURIE,
         object: CURIE,
         predicates: List[PRED_CURIE] = None,
         include_owl_thing: bool = True,
@@ -70,58 +42,94 @@
 
         :param subject:
         :param object:
         :param predicates:
         :param include_owl_thing:
         :return:
         """
-        # if isinstance(self, OboGraphInterface):
-        #     s_ancs = set(self.ancestors([subject], predicates))
-        #     o_ancs = set(self.ancestors([object], predicates))
-        #     common = s_ancs.intersection(o_ancs)
-        #     ancs_of_common = []
-        #     for ca in common:
-        #         for caa in self.ancestors(ca, predicates):
-        #             if caa != ca:
-        #                 ancs_of_common.append(caa)
-        #     n = 0
-        #     for a in common:
-        #         if a not in ancs_of_common:
-        #             yield a
-        #             n += 1
-        #     if n == 0:
-        #         yield OWL_THING
-        # else:
-        raise NotImplementedError
+        if isinstance(self, OboGraphInterface):
+            s_ancs = set(self.ancestors([subject], predicates))
+            o_ancs = set(self.ancestors([object], predicates))
+            common = s_ancs.intersection(o_ancs)
+            ancs_of_common = []
+            for ca in common:
+                for caa in self.ancestors(ca, predicates):
+                    if caa != ca:
+                        ancs_of_common.append(caa)
+            n = 0
+            for a in common:
+                if a not in ancs_of_common:
+                    yield a
+                    n += 1
+            if n == 0:
+                yield OWL_THING
+        else:
+            raise NotImplementedError
+
+    def setwise_most_recent_common_ancestors(
+        self,
+        subjects: List[CURIE],
+        predicates: List[PRED_CURIE] = None,
+        include_owl_thing: bool = True,
+    ) -> Iterable[CURIE]:
+        """
+        Most recent common ancestors (MRCAs) for a set of entities
+
+        The MRCAs are the set of Common Ancestors (CAs) that are not themselves proper
+        ancestors of another CA
+
+        :param subjects:
+        :param predicates:
+        :param include_owl_thing:
+        :return:
+        """
+        if not isinstance(self, OboGraphInterface):
+            raise NotImplementedError
+        ancs = []
+        for s in subjects:
+            ancs.append(set(self.ancestors([s], predicates)))
+        common = set.intersection(*ancs)
+        ancs_of_common = []
+        for ca in common:
+            for caa in self.ancestors(ca, predicates):
+                if caa != ca:
+                    ancs_of_common.append(caa)
+        n = 0
+        for a in common:
+            if a not in ancs_of_common:
+                yield a
+                n += 1
+        if n == 0 and include_owl_thing:
+            yield OWL_THING
 
     def multiset_most_recent_common_ancestors(
         self, subjects: List[CURIE], predicates: List[PRED_CURIE] = None, asymmetric=True
     ) -> Iterable[Tuple[CURIE, CURIE, CURIE]]:
         """
         All pairwise common ancestors for all pairs in a set of terms
 
         :param subjects:
         :param predicates:
         :param asymmetric:
         :return:
         """
-        # if isinstance(self, OboGraphInterface):
-        #     og = self.ancestor_graph(subjects, predicates)
-        #     dg = as_digraph(og)
-        #     pairs = []
-        #     subjects = [s for s in subjects if s in dg]
-        #     for s in subjects:
-        #         for o in subjects:
-        #             if asymmetric and s >= o:
-        #                 continue
-        #             pairs.append((s, o))
-        #     for (s, o), lca in nx.all_pairs_lowest_common_ancestor(dg, pairs=pairs):
-        #         yield s, o, lca
-        # else:
-        raise NotImplementedError
+        if isinstance(self, OboGraphInterface):
+            og = self.ancestor_graph(subjects, predicates)
+            dg = as_digraph(og)
+            pairs = []
+            subjects = [s for s in subjects if s in dg]
+            for s in subjects:
+                for o in subjects:
+                    if asymmetric and s >= o:
+                        continue
+                    pairs.append((s, o))
+            for (s, o), lca in nx.all_pairs_lowest_common_ancestor(dg, pairs=pairs):
+                yield s, o, lca
+        else:
+            raise NotImplementedError
 
     def common_ancestors(
         self,
         subject: CURIE,
         object: CURIE,
         predicates: List[PRED_CURIE] = None,
         subject_ancestors: List[CURIE] = None,
@@ -146,15 +154,15 @@
             subject_ancestors = set(self.ancestors(subject, predicates))
             object_ancestors = set(self.ancestors(object, predicates))
         else:
             raise NotImplementedError
         if include_owl_thing:
             subject_ancestors.add(OWL_THING)
             object_ancestors.add(OWL_THING)
-        for a in get_intersection(subject_ancestors, object_ancestors):
+        for a in subject_ancestors.intersection(object_ancestors):
             yield a
 
     def common_descendants(
         self,
         subject: CURIE,
         object: CURIE,
         predicates: List[PRED_CURIE] = None,
@@ -176,14 +184,39 @@
         """
         pairs = list(self.information_content_scores([curie], object_closure_predicates=predicates))
         if pairs:
             if len(pairs) > 1:
                 raise ValueError(f"Multiple values for IC for {curie} = {pairs}")
             return pairs[0][1]
 
+    def information_content_scores(
+        self,
+        curies: Iterable[CURIE],
+        predicates: List[PRED_CURIE] = None,
+        object_closure_predicates: List[PRED_CURIE] = None,
+        use_associations: bool = None,
+    ) -> Iterator[Tuple[CURIE, float]]:
+        """
+        Yields entity-score pairs for a given collection of entities.
+
+        The Information Content (IC) score for a term t is determined by:
+
+            IC(t) = -log2(Pr(t))
+
+        Where the probability Pr(t) is determined by the frequency of that term against
+        the whole corpus:
+
+            Pr(t) = freq(t)/|items|
+
+        :param curies:
+        :param object_closure_predicates:
+        :return:
+        """
+        raise NotImplementedError
+
     def pairwise_similarity(
         self,
         subject: CURIE,
         object: CURIE,
         predicates: List[PRED_CURIE] = None,
         subject_ancestors: List[CURIE] = None,
         object_ancestors: List[CURIE] = None,
@@ -212,35 +245,34 @@
             cas.remove(OWL_THING)
         logging.info(f"Retrieving IC for {len(cas)} common ancestors")
         ics = {
             a: ic
             for a, ic in self.information_content_scores(cas, object_closure_predicates=predicates)
         }
         if len(ics) > 0:
-            anc, max_ic = mrca_and_score(ics)
-
+            max_ic = max(ics.values())
+            best_mrcas = [a for a in ics.keys() if math.isclose(ics[a], max_ic, rel_tol=0.001)]
+            anc = best_mrcas[0]
         else:
             max_ic = 0.0
             anc = None
         logging.info(f"MRCA = {anc} with {max_ic}")
         sim = TermPairwiseSimilarity(
             subject_id=subject,
             object_id=object,
             ancestor_id=anc,
             ancestor_information_content=max_ic,
         )
         sim.ancestor_information_content = max_ic
         if subject_ancestors is None and isinstance(self, OboGraphInterface):
-            subject_ancestors = set(self.ancestors(subject, predicates=predicates))
-            subject_ancestors.add(subject)
+            subject_ancestors = self.ancestors(subject, predicates=predicates)
         if object_ancestors is None and isinstance(self, OboGraphInterface):
-            object_ancestors = set(self.ancestors(object, predicates=predicates))
-            object_ancestors.add(object)
+            object_ancestors = self.ancestors(object, predicates=predicates)
         if subject_ancestors is not None and object_ancestors is not None:
-            sim.jaccard_similarity = jaccard_similarity(subject_ancestors, object_ancestors)
+            sim.jaccard_similarity = setwise_jaccard_similarity(subject_ancestors, object_ancestors)
         if sim.ancestor_information_content and sim.jaccard_similarity:
             sim.phenodigm_score = math.sqrt(
                 sim.jaccard_similarity * sim.ancestor_information_content
             )
         return sim
 
     def termset_pairwise_similarity(
@@ -322,63 +354,7 @@
         :param predicates:
         :return:
         """
         objects = list(objects)
         for s in subjects:
             for o in objects:
                 yield self.pairwise_similarity(s, o, predicates=predicates)
-
-    def entities(self, filter_obsoletes=True, owl_type=None) -> Iterable[CURIE]:
-        """
-        Yields all known entity CURIEs.
-
-        :param filter_obsoletes: if True, exclude any obsolete/deprecated element
-        :param owl_type: CURIE for RDF metaclass for the object, e.g. owl:Class
-        :return: iterator
-        """
-        yield from self.wrapped_adapter.entities(filter_obsoletes=True, owl_type=None)
-
-    def ancestors(
-        self,
-        start_curies: Union[CURIE, List[CURIE]],
-        predicates: List[PRED_CURIE] = None,
-        reflexive: bool = True,
-        method: Optional[GraphTraversalMethod] = None,
-    ) -> Iterable[CURIE]:
-        """Returns a list of ancestors."""
-        yield from self.wrapped_adapter.ancestors(
-            start_curies=start_curies, predicates=predicates, reflexive=reflexive, method=method
-        )
-
-    def labels(self, curies: Iterable[CURIE], allow_none=True) -> Iterable[Tuple[CURIE, str]]:
-        """Returns labels for CURIEs."""
-        yield from self.wrapped_adapter.labels(curies, allow_none=allow_none)
-
-    def information_content_scores(
-        self,
-        curies: Iterable[CURIE],
-        predicates: List[PRED_CURIE] = None,
-        object_closure_predicates: List[PRED_CURIE] = None,
-        use_associations: bool = None,
-    ) -> Iterator[Tuple[CURIE, float]]:
-        """
-        Yields entity-score pairs for a given collection of entities.
-
-        The Information Content (IC) score for a term t is determined by:
-
-            IC(t) = -log2(Pr(t))
-
-        Where the probability Pr(t) is determined by the frequency of that term against
-        the whole corpus:
-
-            Pr(t) = freq(t)/|items|
-
-        :param curies:
-        :param object_closure_predicates:
-        :return:
-        """
-        yield from self.wrapped_adapter.information_content_scores(
-            curies=curies,
-            predicates=predicates,
-            object_closure_predicates=object_closure_predicates,
-            use_associations=use_associations,
-        )
```

### Comparing `oaklib-0.5.6/src/oaklib/implementations/simpleobo/simple_obo_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/simpleobo/simple_obo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/simpleobo/simple_obo_parser.py` & `oaklib-0.5.7/src/oaklib/implementations/simpleobo/simple_obo_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/sparql/abstract_sparql_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/sparql/abstract_sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/sparql/lov_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/sparql/lov_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/sparql/oak_metamodel_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/sparql/oak_metamodel_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/sparql/sparql_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/sparql/sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/sparql/sparql_query.py` & `oaklib-0.5.7/src/oaklib/implementations/sparql/sparql_query.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/sqldb/sql_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/sqldb/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/sqldb/sqlite_utils.py` & `oaklib-0.5.7/src/oaklib/implementations/sqldb/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/translator/translator_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/translator/translator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/ubergraph/ubergraph_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/ubergraph/ubergraph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/uniprot/uniprot_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/uniprot/uniprot_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/implementations/wikidata/wikidata_implementation.py` & `oaklib-0.5.7/src/oaklib/implementations/wikidata/wikidata_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/__init__.py` & `oaklib-0.5.7/src/oaklib/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/association_provider_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/association_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/basic_ontology_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/basic_ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/class_enrichment_calculation_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/class_enrichment_calculation_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/differ_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/differ_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/dumper_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/dumper_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/embedding_provider_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/embedding_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/mapping_provider_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/mapping_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/merge_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/merge_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/metadata_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/metadata_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/obograph_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/obograph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/obolegacy_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/obolegacy_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/ontology_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/owl_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/owl_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/patcher_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/patcher_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/rdf_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/rdf_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/relation_graph_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/relation_graph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/skos_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/skos_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/subsetter_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/subsetter_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/summary_statistics_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/summary_statistics_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/taxon_constraint_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/taxon_constraint_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/text_annotator_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/text_annotator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/interfaces/validator_interface.py` & `oaklib-0.5.7/src/oaklib/interfaces/validator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/heatmap_writer.py` & `oaklib-0.5.7/src/oaklib/io/heatmap_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/html_writer.py` & `oaklib-0.5.7/src/oaklib/io/html_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/obograph_writer.py` & `oaklib-0.5.7/src/oaklib/io/obograph_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/rollup_report_writer.py` & `oaklib-0.5.7/src/oaklib/io/rollup_report_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_axiom_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_axiom_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_csv_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_csv_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_fhir_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_fhir_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_info_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_info_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_json_lines_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_json_lines_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_json_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_kgcl_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_kgcl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_markdown_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_markdown_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_nl_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_nl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_obo_json_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_obo_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_obo_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_obo_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_owl_functional_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_owl_functional_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_rdf_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/io/streaming_yaml_writer.py` & `oaklib-0.5.7/src/oaklib/io/streaming_yaml_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/mappers/base_mapper.py` & `oaklib-0.5.7/src/oaklib/mappers/base_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/mappers/ontology_metadata_mapper.py` & `oaklib-0.5.7/src/oaklib/mappers/ontology_metadata_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/parsers/__init__.py` & `oaklib-0.5.7/src/oaklib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/parsers/association_parser.py` & `oaklib-0.5.7/src/oaklib/parsers/association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/parsers/association_parser_factory.py` & `oaklib-0.5.7/src/oaklib/parsers/association_parser_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/parsers/boomer_parser.py` & `oaklib-0.5.7/src/oaklib/parsers/boomer_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/parsers/gaf_association_parser.py` & `oaklib-0.5.7/src/oaklib/parsers/gaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/parsers/gencc_association_parser.py` & `oaklib-0.5.7/src/oaklib/parsers/gencc_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/parsers/hpoa_association_parser.py` & `oaklib-0.5.7/src/oaklib/parsers/hpoa_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/parsers/hpoa_g2p_association_parser.py` & `oaklib-0.5.7/src/oaklib/parsers/hpoa_g2p_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/parsers/kgx_association_parser.py` & `oaklib-0.5.7/src/oaklib/parsers/kgx_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/parsers/mim2gene_association_parser.py` & `oaklib-0.5.7/src/oaklib/parsers/mim2gene_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/parsers/pairwise_association_parser.py` & `oaklib-0.5.7/src/oaklib/parsers/pairwise_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/parsers/parser_base.py` & `oaklib-0.5.7/src/oaklib/parsers/parser_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/parsers/phaf_association_parser.py` & `oaklib-0.5.7/src/oaklib/parsers/phaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/parsers/xaf_association_parser.py` & `oaklib-0.5.7/src/oaklib/parsers/xaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/resource.py` & `oaklib-0.5.7/src/oaklib/resource.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/selector.py` & `oaklib-0.5.7/src/oaklib/selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,15 +287,14 @@
 
     :param scheme:
     :return: adapter (implementation) class that implements the OntologyInterface
     """
     if scheme == "http" or scheme == "https":
         raise NotImplementedError("Web requests not implemented yet")
     else:
-        # return SCHEME_DICT[scheme]
         from oaklib.implementations import get_implementation_resolver
 
         return get_implementation_resolver().lookup(scheme)
 
 
 def get_resource_imp_class_from_suffix_descriptor(
     suffix: str, resource: OntologyResource, descriptor: str
```

### Comparing `oaklib-0.5.6/src/oaklib/utilities/apikey_manager.py` & `oaklib-0.5.7/src/oaklib/utilities/apikey_manager.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/associations/association_differ.py` & `oaklib-0.5.7/src/oaklib/utilities/associations/association_differ.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/associations/association_index.py` & `oaklib-0.5.7/src/oaklib/utilities/associations/association_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/basic_utils.py` & `oaklib-0.5.7/src/oaklib/utilities/basic_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/graph/networkx_bridge.py` & `oaklib-0.5.7/src/oaklib/utilities/graph/networkx_bridge.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/graph/relationship_walker.py` & `oaklib-0.5.7/src/oaklib/utilities/graph/relationship_walker.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/identifier_utils.py` & `oaklib-0.5.7/src/oaklib/utilities/identifier_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/iterator_utils.py` & `oaklib-0.5.7/src/oaklib/utilities/iterator_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/kgcl_utilities.py` & `oaklib-0.5.7/src/oaklib/utilities/kgcl_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/label_utilities.py` & `oaklib-0.5.7/src/oaklib/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/lexical/lexical_indexer.py` & `oaklib-0.5.7/src/oaklib/utilities/lexical/lexical_indexer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/mapping/boomer_utils.py` & `oaklib-0.5.7/src/oaklib/utilities/mapping/boomer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/mapping/cross_ontology_diffs.py` & `oaklib-0.5.7/src/oaklib/utilities/mapping/cross_ontology_diffs.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/mapping/mapping_propagator.py` & `oaklib-0.5.7/src/oaklib/utilities/mapping/mapping_propagator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/mapping/mapping_validation.py` & `oaklib-0.5.7/src/oaklib/utilities/mapping/mapping_validation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/mapping/sssom_utils.py` & `oaklib-0.5.7/src/oaklib/utilities/mapping/sssom_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/ner_utilities.py` & `oaklib-0.5.7/src/oaklib/utilities/ner_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/nlp/natual_language_generation.py` & `oaklib-0.5.7/src/oaklib/utilities/nlp/natual_language_generation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/obograph_utils.py` & `oaklib-0.5.7/src/oaklib/utilities/obograph_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,23 +78,32 @@
     :return:
     """
     imgfile = graph_to_image(graph, seeds, configure=configure, stylemap=stylemap, imgfile=imgfile)
     subprocess.run(["open", imgfile])
 
 
 def graph_to_image(
-    graph: Graph, seeds=None, configure=None, stylemap=None, imgfile=None, view=None
-) -> str:
+    graph: Graph,
+    seeds: Optional[list[str]] = None,
+    configure: Optional[str] = None,
+    stylemap: Optional[str] = None,
+    imgfile: Optional[str] = None,
+    view: bool = None,
+    format="png",
+) -> None:
     """
-    Renders a graph to png using obographviz
+    Renders a graph to png using obographviz.
 
-    :param graph:
-    :param seeds:
-    :param configure:
-    :param stylemap:
+    :param graph: OboGraph object to visualize
+    :param seeds: list of node ids to highlight
+    :param configure: yaml string to configure the graph
+    :param stylemap: path to stylemap file following kgviz data model
+    :param imgfile: path to image file to write
+    :param view:
+    :param format: defaults to png
     :return:
     """
     g = {"graphs": [graph_as_dict(graph)]}
     logging.debug(f"graph = {g}")
     exec = "og2dot"
     if shutil.which(exec) is None:
         logging.error(f"No {exec}")
@@ -123,18 +132,18 @@
         logging.info(f"Writing to {temp_file_name}")
         json_dump = json.dumps(g)
         tmpfile.write(json_dump)
         logging.debug(f"JSON {json_dump}")
         tmpfile.flush()
 
         if imgfile is None:
-            imgfile = f"{temp_file_name}.png"
+            imgfile = f"{temp_file_name}.{format}"
         style_json = json.dumps(style).replace("'", "\\'")
         logging.debug(f"Style = {style_json}")
-        cmdtoks = [exec, "-S", style_json, "-t", "png", temp_file_name, "-o", imgfile]
+        cmdtoks = [exec, "-S", style_json, "-t", format, temp_file_name, "-o", imgfile]
         if stylemap is not None:
             cmdtoks += ["-s", stylemap]
         if seeds is not None:
             for seed in seeds:
                 cmdtoks += ["-H", seed]
         if sys.platform == "win32":
             cmdtoks = ["cmd.exe", "/c"] + cmdtoks
```

### Comparing `oaklib-0.5.6/src/oaklib/utilities/ontology_builder.py` & `oaklib-0.5.7/src/oaklib/utilities/ontology_builder.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/reasoning/relation_graph.py` & `oaklib-0.5.7/src/oaklib/utilities/reasoning/relation_graph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/semsim/similarity_utils.py` & `oaklib-0.5.7/src/oaklib/utilities/semsim/similarity_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/stats/hypergeometric.py` & `oaklib-0.5.7/src/oaklib/utilities/stats/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/subsets/slimmer_utils.py` & `oaklib-0.5.7/src/oaklib/utilities/subsets/slimmer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/subsets/subset_analysis.py` & `oaklib-0.5.7/src/oaklib/utilities/subsets/subset_analysis.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/subsets/value_set_expander.py` & `oaklib-0.5.7/src/oaklib/utilities/subsets/value_set_expander.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/table_filler.py` & `oaklib-0.5.7/src/oaklib/utilities/table_filler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/taxon/taxon_constraint_utils.py` & `oaklib-0.5.7/src/oaklib/utilities/taxon/taxon_constraint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/validation/definition_ontology_rule.py` & `oaklib-0.5.7/src/oaklib/utilities/validation/definition_ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/validation/disjointness_rule.py` & `oaklib-0.5.7/src/oaklib/utilities/validation/disjointness_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/validation/lint_utils.py` & `oaklib-0.5.7/src/oaklib/utilities/validation/lint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/validation/ontology_rule.py` & `oaklib-0.5.7/src/oaklib/utilities/validation/ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/src/oaklib/utilities/validation/rule_runner.py` & `oaklib-0.5.7/src/oaklib/utilities/validation/rule_runner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.6/PKG-INFO` & `oaklib-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaklib
-Version: 0.5.6
+Version: 0.5.7
 Summary: Ontology Access Kit: Python library for common ontology operations over a variety of backends
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,26 +23,26 @@
 Requires-Dist: eutils (>=0.6.0)
 Requires-Dist: funowl (>=0.1.12)
 Requires-Dist: gilda (>=0.10.1,<0.11.0) ; extra == "gilda"
 Requires-Dist: kgcl-rdflib (==0.5.0)
 Requires-Dist: kgcl-schema (==0.5.0)
 Requires-Dist: lark (>=1.1.2)
 Requires-Dist: linkml-renderer (>=0.1.2)
-Requires-Dist: linkml-runtime (>=1.2.15)
+Requires-Dist: linkml-runtime (>=1.5.3)
 Requires-Dist: ndex2 (>=3.5.0,<4.0.0)
 Requires-Dist: networkx (>=2.7.1)
 Requires-Dist: ols-client (>=0.1.1)
 Requires-Dist: ontoportal-client (>=0.0.3)
 Requires-Dist: prefixmaps (>=0.1.2)
 Requires-Dist: pronto (>=2.5.0)
 Requires-Dist: pysolr (>=3.9.0,<4.0.0)
 Requires-Dist: pystow (>=0.5.0)
 Requires-Dist: ratelimit (>=2.2.1)
 Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
-Requires-Dist: semsimian (>=0.1.13)
+Requires-Dist: semsimian (==0.1.13)
 Requires-Dist: semsql (>=0.3.1)
 Requires-Dist: sssom (>=0.3.26)
 Requires-Dist: sssom-schema (>=0.11.0)
 Description-Content-Type: text/markdown
 
 # Ontology Access Kit (OAK)
```

