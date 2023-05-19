# Comparing `tmp/genomehubs-2.6.9.tar.gz` & `tmp/genomehubs-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomehubs-2.6.9.tar", last modified: Mon Mar 20 15:37:08 2023, max compression
+gzip compressed data, was "genomehubs-2.7.0.tar", last modified: Fri May 19 10:18:51 2023, max compression
```

## Comparing `genomehubs-2.6.9.tar` & `genomehubs-2.7.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:08.381759 genomehubs-2.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-20 15:37:02.000000 genomehubs-2.6.9/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-20 15:37:02.000000 genomehubs-2.6.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-20 15:37:02.000000 genomehubs-2.6.9/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-03-20 15:37:02.000000 genomehubs-2.6.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-20 15:37:02.000000 genomehubs-2.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-20 15:37:02.000000 genomehubs-2.6.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-20 15:37:08.381759 genomehubs-2.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-03-20 15:37:02.000000 genomehubs-2.6.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-20 15:37:02.000000 genomehubs-2.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-20 15:37:08.381759 genomehubs-2.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-03-20 15:37:02.000000 genomehubs-2.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:08.369758 genomehubs-2.6.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:08.369758 genomehubs-2.6.9/src/genomehubs/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:08.373759 genomehubs-2.6.9/src/genomehubs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/config/dist.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/genomehubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:08.373759 genomehubs-2.6.9/src/genomehubs/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/btk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/busco.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/es_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    34131 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/gbif.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    35765 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    37686 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/taxon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/wikidata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/lib/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:08.377759 genomehubs-2.6.9/src/genomehubs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/ATTR_busco.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/ATTR_feature.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/ATTR_window_stats.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/analysis.json
--rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/assembly.json
--rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/assembly.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/btk.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/busco.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/busco_feature.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/feature.json
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/file.json
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/identifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/organelle.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/sample.types.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:08.381759 genomehubs-2.6.9/src/genomehubs/templates/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/analysis_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/analysis_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/assembly_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/assembly_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/attribute_types_by_group.json
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/attribute_values_by_taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/attributes_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/attributes_identifiers_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/attributes_names_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/file_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/file_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/max_nested_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/max_nested_value_by_key_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/max_nested_value_by_type.json
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/search_by_taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_attributes_by_taxon_id.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_by_any_name.json
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_by_name.json
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_by_specific_name.json
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_names.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_names_by_root.json
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/taxonomy_node_by_taxon_id.json
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/scripts/value_by_type_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/taxon.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/taxonomy.json
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/wikidata.names.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/window_full.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-20 15:37:02.000000 genomehubs-2.6.9/src/genomehubs/templates/window_stats.types.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:37:08.373759 genomehubs-2.6.9/src/genomehubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-20 15:37:08.000000 genomehubs-2.6.9/src/genomehubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-03-20 15:37:08.000000 genomehubs-2.6.9/src/genomehubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 15:37:08.000000 genomehubs-2.6.9/src/genomehubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-20 15:37:08.000000 genomehubs-2.6.9/src/genomehubs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-20 15:37:08.000000 genomehubs-2.6.9/src/genomehubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-20 15:37:08.000000 genomehubs-2.6.9/src/genomehubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:18:51.823337 genomehubs-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-19 10:18:44.000000 genomehubs-2.7.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-19 10:18:44.000000 genomehubs-2.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-19 10:18:44.000000 genomehubs-2.7.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-19 10:18:44.000000 genomehubs-2.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-19 10:18:44.000000 genomehubs-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-19 10:18:44.000000 genomehubs-2.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-19 10:18:51.823337 genomehubs-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-19 10:18:44.000000 genomehubs-2.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-19 10:18:44.000000 genomehubs-2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-19 10:18:51.827337 genomehubs-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-19 10:18:44.000000 genomehubs-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:18:51.811336 genomehubs-2.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:18:51.815336 genomehubs-2.7.0/src/genomehubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:18:51.815336 genomehubs-2.7.0/src/genomehubs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/config/dist.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/genomehubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:18:51.819337 genomehubs-2.7.0/src/genomehubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/btk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/busco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/es_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34258 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/gbif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35765 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37857 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/taxon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/wikidata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/lib/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:18:51.823337 genomehubs-2.7.0/src/genomehubs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/ATTR_busco.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/ATTR_feature.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/ATTR_window_stats.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/analysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/assembly.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/assembly.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/attributes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/btk.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/busco.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/busco_feature.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/identifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/organelle.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/sample.types.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:18:51.823337 genomehubs-2.7.0/src/genomehubs/templates/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/analysis_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/analysis_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/assembly_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/assembly_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/attribute_types_by_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/attribute_values_by_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/attributes_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/attributes_identifiers_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/attributes_names_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/file_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/file_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/max_nested_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/max_nested_value_by_key_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/max_nested_value_by_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/search_by_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_attributes_by_taxon_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_by_any_name.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_by_name.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_by_specific_name.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_names_by_root.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/taxonomy_node_by_taxon_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/scripts/value_by_type_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/taxon.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/taxonomy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/wikidata.names.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/window_full.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-19 10:18:44.000000 genomehubs-2.7.0/src/genomehubs/templates/window_stats.types.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:18:51.815336 genomehubs-2.7.0/src/genomehubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-19 10:18:51.000000 genomehubs-2.7.0/src/genomehubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-19 10:18:51.000000 genomehubs-2.7.0/src/genomehubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:18:51.000000 genomehubs-2.7.0/src/genomehubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-19 10:18:51.000000 genomehubs-2.7.0/src/genomehubs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-19 10:18:51.000000 genomehubs-2.7.0/src/genomehubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 10:18:51.000000 genomehubs-2.7.0/src/genomehubs.egg-info/top_level.txt
```

### Comparing `genomehubs-2.6.9/CONTRIBUTING.rst` & `genomehubs-2.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/LICENSE` & `genomehubs-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/PKG-INFO` & `genomehubs-2.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomehubs
-Version: 2.6.9
+Version: 2.7.0
 Summary: GenomeHubs
 Home-page: https://github.com/genomehubs/genomehubs
 Author: genomehubs
 Author-email: genomehubs@genomehubs.org
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/genomehubs/genomehubs/issues
 Project-URL: Source, https://github.com/genomehubs/genomehubs
```

### Comparing `genomehubs-2.6.9/README.rst` & `genomehubs-2.7.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     :alt: Install with Conda
     :target: https://anaconda.org/tolkit/genomehubs
 
 .. |platforms| image:: https://anaconda.org/tolkit/genomehubs/badges/platforms.svg
     :alt: Conda platforms
     :target: https://anaconda.org/tolkit/genomehubs
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/genomehubs/genomehubs/2.6.9.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/genomehubs/genomehubs/2.7.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/genomehubs/genomehubs/compare/2.6.9...main
+    :target: https://github.com/genomehubs/genomehubs/compare/2.7.0...main
 
 .. |license| image:: https://anaconda.org/tolkit/genomehubs/badges/license.svg
     :alt: MIT License
     :target: https://anaconda.org/tolkit/genomehubs
 
 .. end-badges
```

### Comparing `genomehubs-2.6.9/setup.cfg` & `genomehubs-2.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/setup.py` & `genomehubs-2.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="genomehubs",  # Required
-    version="2.6.9",
+    version="2.7.0",
     description="GenomeHubs",  # Optional
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
@@ -95,24 +95,27 @@
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=[
         "biopython>=1.78",
         "docopt>=0.6.2",
-        "elasticsearch>=7.8.1,<7.14.0",
+        "elasticsearch==8.7",
         "fastjsonschema>=2.15.3",
         "filetype>=1.0.7",
         "h3>=3.7.4",
         "Pillow>=8.0",
         "pyyaml",
         "sparqlwrapper>=1.4.1",
         "tolkein>=0.5.0",
         "ujson>=3.0.0",
     ],  # Optional
+    setup_requires=[
+        "wheel",
+    ],
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
     # Similar to `install_requires` above, these must be valid existing
```

### Comparing `genomehubs-2.6.9/src/genomehubs/config/dist.config.yaml` & `genomehubs-2.7.0/src/genomehubs/config/dist.config.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/genomehubs.py` & `genomehubs-2.7.0/src/genomehubs/genomehubs.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/attributes.py` & `genomehubs-2.7.0/src/genomehubs/lib/attributes.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/btk.py` & `genomehubs-2.7.0/src/genomehubs/lib/btk.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/busco.py` & `genomehubs-2.7.0/src/genomehubs/lib/busco.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/config.py` & `genomehubs-2.7.0/src/genomehubs/lib/config.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/directory.py` & `genomehubs-2.7.0/src/genomehubs/lib/directory.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/es_functions.py` & `genomehubs-2.7.0/src/genomehubs/lib/es_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 
 LOGGER = tolog.logger(__name__)
 
 
 def test_connection(opts, *, log=False):
     """Test connection to Elasticsearch."""
     connected = False
-    hosts = opts["es-host"]
-    with tolog.DisableLogger():
-        try:
-            es = Elasticsearch(
-                hosts=hosts, timeout=1800, max_retries=10, retry_on_timeout=True
-            )
-            connected = es.info()
-        except Exception:
-            pass
+    host = opts["es-host"][0]
+    host = f"http://{host}"
+    hosts = [host]
+    print(hosts)
+    # with tolog.DisableLogger():
+    # try:
+    es = Elasticsearch(hosts=hosts, timeout=1800, max_retries=10, retry_on_timeout=True)
+    connected = es.info()
+    #   pass
     if not connected:
         message = "Could not connect to Elasticsearch at '%s'" % ", ".join(hosts)
         if log:
             LOGGER.error(message)
             sys.exit(1)
         return False
     if log:
@@ -111,15 +111,15 @@
     except ProcessLookupError:
         pass
     sys.exit(1)
 
 
 def launch_es(opts, log=True):
     """Launch ElasticSearch."""
-    es = test_connection(opts)
+    es = test_connection(opts, log=log)
     if es:
         if log:
             LOGGER.info("ElasticSearch is already running")
     if not es:
         if any(host.startswith(("localhost", "127.0.0.1")) for host in opts["es-host"]):
             # Start Elasticsearch
             if "docker-contain" in opts and "es" in opts["docker-contain"]:
@@ -138,25 +138,25 @@
     return es
 
 
 def index_exists(es, index_name):
     """Test if Elasticsearch index exists."""
     es_client = client.IndicesClient(es)
     with tolog.DisableLogger():
-        res = es_client.exists(index_name)
+        res = es_client.exists(index=index_name)
     return res
 
 
 def index_create(es, index_name):
     """Create an Elasticsearch index if it does not already exist."""
     es_client = client.IndicesClient(es)
     res = index_exists(es, index_name)
     if not res:
         with tolog.DisableLogger():
-            res = es_client.create(index_name)
+            res = es_client.create(index=index_name)
     return res
 
 
 def load_mapping(es, mapping_name, mapping):
     """Load index mapping template into Elasticsearch."""
     es_client = client.IndicesClient(es)
     with tolog.DisableLogger():
```

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/files.py` & `genomehubs-2.7.0/src/genomehubs/lib/files.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/fill.py` & `genomehubs-2.7.0/src/genomehubs/lib/fill.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,14 +363,16 @@
             if summary.startswith("median"):
                 summary = "median"
         else:
             traverse_value = list(set(traverse_value))
         if summary == "range":
             attribute[summary] = value
             traverse_value = [min_value, max_value]
+        elif summary not in attribute and summary in {"mean", "median", "mode", "sum"}:
+            attribute[summary] = value
     return traverse_value, max_value, min_value
 
 
 # def iterate_values(attribute, meta):
 #     """Iterate through values adding prefixed values if appropriate."""
 #     prefixed_values = None
 #     if meta["type"] == "keyword":
```

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/gbif.py` & `genomehubs-2.7.0/src/genomehubs/lib/gbif.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/geo.py` & `genomehubs-2.7.0/src/genomehubs/lib/geo.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/hub.py` & `genomehubs-2.7.0/src/genomehubs/lib/hub.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/index.py` & `genomehubs-2.7.0/src/genomehubs/lib/index.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/init.py` & `genomehubs-2.7.0/src/genomehubs/lib/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
         if "taxonomy-format" in options["init"]:
             template, stream = taxonomy.index(taxonomy_name, options["init"])
             if "taxonomy-jsonl" in options["init"]:
                 stream = add_jsonl_to_taxonomy(
                     stream, options["init"]["taxonomy-jsonl"]
                 )
             if "taxonomy-root" in options["init"]:
+                es_functions.index_create(es, template["index_name"])
                 es_functions.load_mapping(es, template["name"], template["mapping"])
                 es_functions.index_stream(
                     es,
                     template["index_name"],
                     stream,
                     log=options["init"].get("log-es", True),
                     chunk_size=options["init"].get("es-batch", 500),
```

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/ncbi.py` & `genomehubs-2.7.0/src/genomehubs/lib/ncbi.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/parse.py` & `genomehubs-2.7.0/src/genomehubs/lib/parse.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/run.py` & `genomehubs-2.7.0/src/genomehubs/lib/run.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/sample.py` & `genomehubs-2.7.0/src/genomehubs/lib/sample.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/search.py` & `genomehubs-2.7.0/src/genomehubs/lib/search.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/taxon.py` & `genomehubs-2.7.0/src/genomehubs/lib/taxon.py`

 * *Files 0% similar despite different names*

```diff
@@ -821,23 +821,24 @@
             "node_depth": 1,
             "taxon_id": closest_taxon["_source"]["taxon_id"],
             "taxon_rank": closest_taxon["_source"]["taxon_rank"],
             "scientific_name": closest_taxon["_source"]["scientific_name"],
         }
     ]
     if "lineage" in closest_taxon["_source"]:
-        for ancestor in closest_taxon["_source"]["lineage"]:
-            lineage.append(
-                {
-                    "taxon_id": ancestor["taxon_id"],
-                    "taxon_rank": ancestor["taxon_rank"],
-                    "scientific_name": ancestor["scientific_name"],
-                    "node_depth": ancestor["node_depth"] + 1,
-                }
-            )
+        lineage.extend(
+            {
+                "taxon_id": ancestor["taxon_id"],
+                "taxon_rank": ancestor["taxon_rank"],
+                "scientific_name": ancestor["scientific_name"],
+                "node_depth": ancestor["node_depth"] + 1,
+            }
+            for ancestor in closest_taxon["_source"]["lineage"]
+            if ancestor["taxon_id"] != closest_taxon["_source"]["taxon_id"]
+        )
     desc_taxon["_source"]["lineage"] = lineage
     return desc_taxon
 
 
 def add_new_taxon(alt_taxon_id, new_taxa, obj, closest_taxon, *, blanks={"NA", "None"}):
     """Add a new taxon with alt_taxon_id to list of taxa."""
     # TODO: Allow creation of new higher taxa
@@ -1060,14 +1061,16 @@
             if alt_taxon_id in ancestors:
                 closest_rank = rank
                 if taxon in matches and obj["taxonomy"][anc_rank] in matches[taxon]:
                     closest_taxon = matches[taxon][obj["taxonomy"][anc_rank]][0]
                 else:
                     closest_taxon = matches[obj["taxonomy"][anc_rank]]["all"][0]
                 break
+            # immediate_anc = lineage[-1]
+            # if immediate_anc["rank"] != rank or immediate_anc["name"] != taxon:
             lineage.append({"rank": rank, "name": taxon})
         # create a new taxon if a closest ancestral taxon could be found
         create_new_taxon(
             alt_taxon_id,
             closest_taxon,
             closest_rank,
             lineage,
```

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/taxonomy.py` & `genomehubs-2.7.0/src/genomehubs/lib/taxonomy.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/test.py` & `genomehubs-2.7.0/src/genomehubs/lib/test.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/validate.py` & `genomehubs-2.7.0/src/genomehubs/lib/validate.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/wikidata.py` & `genomehubs-2.7.0/src/genomehubs/lib/wikidata.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/lib/window.py` & `genomehubs-2.7.0/src/genomehubs/lib/window.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/ATTR_busco.types.yaml` & `genomehubs-2.7.0/src/genomehubs/templates/ATTR_busco.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/ATTR_feature.types.yaml` & `genomehubs-2.7.0/src/genomehubs/templates/ATTR_feature.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/ATTR_window_stats.types.yaml` & `genomehubs-2.7.0/src/genomehubs/templates/ATTR_window_stats.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/analysis.json` & `genomehubs-2.7.0/src/genomehubs/templates/analysis.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/assembly.json` & `genomehubs-2.7.0/src/genomehubs/templates/assembly.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/attributes.json` & `genomehubs-2.7.0/src/genomehubs/templates/attributes.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/btk.types.yaml` & `genomehubs-2.7.0/src/genomehubs/templates/btk.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/busco.types.yaml` & `genomehubs-2.7.0/src/genomehubs/templates/busco.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/busco_feature.types.yaml` & `genomehubs-2.7.0/src/genomehubs/templates/busco_feature.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/feature.json` & `genomehubs-2.7.0/src/genomehubs/templates/feature.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999864718614718%*

 * *Differences: {"'mappings'": "{'properties': {'attributes': {'properties': {'flattened_value': "*

 * *               "OrderedDict([('type', 'flattened'), ('meta', OrderedDict([('description', 'Value "*

 * *               "of type flattened')]))])}}}}"}*

```diff
@@ -108,14 +108,20 @@
                     },
                     "double_value": {
                         "meta": {
                             "description": "Value of type double"
                         },
                         "type": "double"
                     },
+                    "flattened_value": {
+                        "meta": {
+                            "description": "Value of type flattened"
+                        },
+                        "type": "flattened"
+                    },
                     "float_value": {
                         "meta": {
                             "description": "Value of type float"
                         },
                         "type": "float"
                     },
                     "geo_point_value": {
```

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/file.json` & `genomehubs-2.7.0/src/genomehubs/templates/file.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/identifiers.json` & `genomehubs-2.7.0/src/genomehubs/templates/identifiers.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/organelle.types.yaml` & `genomehubs-2.7.0/src/genomehubs/templates/organelle.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/sample.json` & `genomehubs-2.7.0/src/genomehubs/templates/sample.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/sample.types.yaml` & `genomehubs-2.7.0/src/genomehubs/templates/sample.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/assembly_lookup.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/assembly_lookup.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/assembly_suggest.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/assembly_suggest.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/attribute_values_by_taxon.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/attribute_values_by_taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/max_nested_value_by_type.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/max_nested_value_by_type.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_by_any_name.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_by_any_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_by_lineage.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_by_name.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_by_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_by_specific_name.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_by_specific_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_lookup.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_lookup.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/taxon_suggest.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/taxon_suggest.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999847412109375%*

 * *Differences: {"'script'": "{'source': {'suggest': {'simple_phrase': {'phrase': {'collate': {'query': {'source': "*

 * *             "{'match_phrase': {'taxon_names.name': '{{suggestion}}'}}}}}}}}}"}*

```diff
@@ -6,15 +6,15 @@
                 "simple_phrase": {
                     "phrase": {
                         "collate": {
                             "prune": true,
                             "query": {
                                 "source": {
                                     "match_phrase": {
-                                        "taxon_names.name": "{{=|| ||=}}{{suggestion}}||={{ }}=||"
+                                        "taxon_names.name": "{{suggestion}}"
                                     }
                                 }
                             }
                         },
                         "confidence": "{{confidence}}{{^confidence}}1{{/confidence}}",
                         "direct_generator": [
                             {
```

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/scripts/value_by_type_by_lineage.json` & `genomehubs-2.7.0/src/genomehubs/templates/scripts/value_by_type_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/taxon.json` & `genomehubs-2.7.0/src/genomehubs/templates/taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/taxon.types.yaml` & `genomehubs-2.7.0/src/genomehubs/templates/taxon.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/taxonomy.json` & `genomehubs-2.7.0/src/genomehubs/templates/taxonomy.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/window_full.types.yaml` & `genomehubs-2.7.0/src/genomehubs/templates/window_full.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs/templates/window_stats.types.yaml` & `genomehubs-2.7.0/src/genomehubs/templates/window_stats.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.6.9/src/genomehubs.egg-info/PKG-INFO` & `genomehubs-2.7.0/src/genomehubs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomehubs
-Version: 2.6.9
+Version: 2.7.0
 Summary: GenomeHubs
 Home-page: https://github.com/genomehubs/genomehubs
 Author: genomehubs
 Author-email: genomehubs@genomehubs.org
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/genomehubs/genomehubs/issues
 Project-URL: Source, https://github.com/genomehubs/genomehubs
```

### Comparing `genomehubs-2.6.9/src/genomehubs.egg-info/SOURCES.txt` & `genomehubs-2.7.0/src/genomehubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

