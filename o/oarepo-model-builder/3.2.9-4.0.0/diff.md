# Comparing `tmp/oarepo-model-builder-3.2.9.tar.gz` & `tmp/oarepo-model-builder-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-3.2.9.tar", last modified: Tue Feb 21 14:30:37 2023, max compression
+gzip compressed data, was "oarepo-model-builder-4.0.0.tar", last modified: Fri May 19 19:07:51 2023, max compression
```

## Comparing `oarepo-model-builder-3.2.9.tar` & `oarepo-model-builder-4.0.0.tar`

### file list

```diff
@@ -1,198 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.742198 oarepo-model-builder-3.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-02-21 14:30:37.742198 oarepo-model-builder-3.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.706197 oarepo-model-builder-3.2.9/oarepo_model_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.710198 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/json_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/model_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/pyproject_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/python.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/python_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/setup_py.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.710198 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/templates/setup.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.714197 oarepo-model-builder-3.2.9/oarepo_model_builder/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/builtin_models/invenio.json
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/conflict_resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.714197 oarepo-model-builder-3.2.9/oarepo_model_builder/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/datatypes/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/datatypes/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/datatypes/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/datatypes/primitive_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/datatypes/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.718197 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_cli_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_resource_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_script_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.722197 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/imports.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_cli.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_ext.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_proxies.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_record_dumper.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_record_facets.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_record_permissions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_record_resource.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_record_resource_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_record_schema.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_record_service.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_record_service_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_version.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_views.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/script_import_sample_data.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/script_import_sample_data.sh.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.722197 oarepo-model-builder-3.2.9/oarepo_model_builder/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/merger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.726198 oarepo-model-builder-3.2.9/oarepo_model_builder/model_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/model_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/model_preprocessors/default_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/model_preprocessors/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/model_preprocessors/invenio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/model_preprocessors/invenio_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/model_preprocessors/opensearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.726198 oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/json_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/python.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.730198 oarepo-model-builder-3.2.9/oarepo_model_builder/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/profiles/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/profiles/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.730198 oarepo-model-builder-3.2.9/oarepo_model_builder/property_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/property_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/property_preprocessors/datatype_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/property_preprocessors/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/property_preprocessors/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.730198 oarepo-model-builder-3.2.9/oarepo_model_builder/stack/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/stack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/stack/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/stack/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.730198 oarepo-model-builder-3.2.9/oarepo_model_builder/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.730198 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/camelcase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.734197 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/cst/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/cst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/cst/call.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/cst/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/cst/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/cst/indented_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/cst/mergers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/cst/simple_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/deepmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/facet_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/hyphen_munch.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/json_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/python_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/utils/verbose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.738197 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/model_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/model_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/property_facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/property_jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/property_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/property_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/property_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/property_sortable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/root.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/oarepo_model_builder/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.710198 oarepo-model-builder-3.2.9/oarepo_model_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-02-21 14:30:37.000000 oarepo-model-builder-3.2.9/oarepo_model_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-02-21 14:30:37.000000 oarepo-model-builder-3.2.9/oarepo_model_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 14:30:37.000000 oarepo-model-builder-3.2.9/oarepo_model_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-02-21 14:30:37.000000 oarepo-model-builder-3.2.9/oarepo_model_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-21 14:30:37.000000 oarepo-model-builder-3.2.9/oarepo_model_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 14:30:37.000000 oarepo-model-builder-3.2.9/oarepo_model_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-02-21 14:30:37.742198 oarepo-model-builder-3.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:30:37.742198 oarepo-model-builder-3.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_builder_from_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_empty_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_fulltext_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_is_schema_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_json_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_json_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_jsonchema_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_jsonschema_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_mapping_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_marshmallow_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_model_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_overwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_plugin_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_python_mergers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_sample_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_schema_props.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_search_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_template_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_type_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-21 14:29:40.000000 oarepo-model-builder-3.2.9/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.435727 oarepo-model-builder-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-19 19:07:51.435727 oarepo-model-builder-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.395727 oarepo-model-builder-4.0.0/oarepo_model_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.399726 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/json_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/pyproject_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/python_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/setup_py.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.399726 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/templates/setup.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.399726 oarepo-model-builder-4.0.0/oarepo_model_builder/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/builtin_models/invenio.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.399726 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.403727 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/facets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.403727 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/marshmallow/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/marshmallow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/marshmallow/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/marshmallow/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/marshmallow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/marshmallow/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.407727 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/record_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/components/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.411727 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/containers/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/containers/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/containers/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/containers/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/primitive_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/generate_doc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.415727 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_api_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_app_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_pid_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_resource_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_ui_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_ui_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_script_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.419727 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/api_views.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/app_views.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/ext.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/imports.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/invenio_record_facets.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/permissions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/pid_provider.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/proxies.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/record_dumper.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/resource.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/resource_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/service.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/service_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/ui_serializer.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/version.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.419727 oarepo-model-builder-4.0.0/oarepo_model_builder/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.423727 oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/json_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.423727 oarepo-model-builder-4.0.0/oarepo_model_builder/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/profiles/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/profiles/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.423727 oarepo-model-builder-4.0.0/oarepo_model_builder/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/settings/opensearch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/settings/python.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.423727 oarepo-model-builder-4.0.0/oarepo_model_builder/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.427727 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/absolute_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/camelcase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.427727 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/cst/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/cst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/cst/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/cst/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/cst/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/cst/indented_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/cst/mergers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/cst/simple_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/deepmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/facet_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/import_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/python_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/utils/verbose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.427727 oarepo-model-builder-4.0.0/oarepo_model_builder/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/validation/extensibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/validation/model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/oarepo_model_builder/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.395727 oarepo-model-builder-4.0.0/oarepo_model_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-19 19:07:51.000000 oarepo-model-builder-4.0.0/oarepo_model_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-05-19 19:07:51.000000 oarepo-model-builder-4.0.0/oarepo_model_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:07:51.000000 oarepo-model-builder-4.0.0/oarepo_model_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-05-19 19:07:51.000000 oarepo-model-builder-4.0.0/oarepo_model_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-19 19:07:51.000000 oarepo-model-builder-4.0.0/oarepo_model_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-19 19:07:51.000000 oarepo-model-builder-4.0.0/oarepo_model_builder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-05-19 19:07:51.435727 oarepo-model-builder-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:07:51.435727 oarepo-model-builder-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/faker_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/multilang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_builder_from_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_cfg_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_datatype_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_datatype_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_empty_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)   396304 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26948 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_fulltext_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_jsonchema_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_mapping_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_marshmallow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_marshmallow_ui_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23597 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_overwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_pid_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_plugin_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_python_mergers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_sample_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_schema_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16438 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_simple_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_template_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_type_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-19 19:06:57.000000 oarepo-model-builder-4.0.0/tests/utils.py
```

### Comparing `oarepo-model-builder-3.2.9/LICENSE` & `oarepo-model-builder-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-3.2.9/PKG-INFO` & `oarepo-model-builder-4.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder
-Version: 3.2.9
+Version: 4.0.0
 Summary: A utility library that generates OARepo required data model files from a JSON specification file
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo model builder
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/builder.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,23 @@
-import copy
-import importlib
-import json
 from pathlib import Path
-from typing import Dict, List, Type, Union
+from typing import Any, Dict, Iterable, List, Type, Union
 
-import yaml
-
-from .builders import (
-    ModelBuilderStack,
-    OutputBuilder,
-    OutputBuilderComponent,
-    ReplaceElement,
-)
+from .builders import OutputBuilder
 from .fs import AbstractFileSystem, FileSystem
-from .model_preprocessors import ModelPreprocessor
 from .outputs import OutputBase
-from .property_preprocessors import PropertyPreprocessor
 from .schema import ModelSchema
-from .utils.cst import ConflictResolver
-from .validation import validate_model
+from .utils.dict import dict_get, dict_setdefault
+from .utils.import_class import import_class
 
 
 class ModelBuilder:
     """
     Processes a model file and generates/updates sources for the model
     """
 
-    model_preprocessor_classes: List[Type[ModelPreprocessor]]
-    """
-    Model preprocessor classes that are called after schema is loaded and before it is processed
-    """
-
     output_classes: List[Type[OutputBase]]
     """
     Mapping between output type and its handler class
     """
 
     filtered_output_classes: Dict[str, Type[OutputBase]]
     """
@@ -42,87 +25,51 @@
     """
 
     output_builder_classes: List[Type[OutputBuilder]]
     """
     A list of extension classes to be used in build. 
     """
 
-    property_preprocessor_classes: List[Type[PropertyPreprocessor]]
-    """
-    Processor classes (called before and after file builder is called)
-    """
-
     output_builders: List[OutputBuilder]
     """
     A list of output_builders. Each extension is responsible for generating one or more files
     """
 
-    output_builder_components: Dict[str, List[OutputBuilderComponent]]
-    """
-    A list of output builder components for an output builder
-    """
-
     outputs: Dict[Path, OutputBase]
     """
     Mapping between concrete output (file path relative to output dir) and instance of builder class
     """
 
-    property_preprocessors: List[PropertyPreprocessor]
-    """
-    Current instances of processor classes.
-    """
-
     filesystem: AbstractFileSystem
 
     overwrite: bool
     """
     If true, overwrite already existing files. If false, perform merge
     """
 
-    conflict_resolver: ConflictResolver
-    """
-    Resolver for conflicts
-    """
-
     def __init__(
         self,
         outputs: List[Type[OutputBase]] = (),
         output_builders: List[Type[OutputBuilder]] = (),
-        property_preprocessors: List[Type[PropertyPreprocessor]] = (),
-        model_preprocessors: List[Type[ModelPreprocessor]] = (),
-        output_builder_components: Dict[str, List[Type[OutputBuilderComponent]]] = None,
         filesystem=FileSystem(),
-        conflict_resolver: ConflictResolver = None,
         overwrite=False,
     ):
         """
         Initializes the builder
 
         :param output_builders:          A list of extension classes to use in builds
         :param outputs:     List of file builder classes that generate files
-        :param property_preprocessors: List of output type processor classes
         """
         self.output_builder_classes = [*output_builders]
         for o in outputs:
             assert o.TYPE, f"output_type not set up on class {o}"
         self.output_classes = [*(outputs or [])]
         self.outputs = {}
-        self.property_preprocessor_classes = [*(property_preprocessors or [])]
-        self.model_preprocessor_classes = [*(model_preprocessors or [])]
         self.filtered_output_classes = {o.TYPE: o for o in self.output_classes}
-        if output_builder_components:
-            self.output_builder_components = {
-                builder_type: [x() for x in components]
-                for builder_type, components in output_builder_components.items()
-            }
-        else:
-            self.output_builder_components = {}
         self.filesystem = filesystem
-        self.skip_schema_validation = False  # set to True in some tests
-        self.conflict_resolver = conflict_resolver
         self.overwrite = overwrite
 
     def get_output(self, output_type: str, path: Union[str, Path]):
         """
         Given a path, instantiate file builder on the path with the given output type
         and return it. If the builder on the path has already been requested, return
         the same instance of the builder.
@@ -140,114 +87,91 @@
             assert output_type == self.outputs[path].TYPE
         else:
             output = self.filtered_output_classes[output_type](self, path)
             output.begin()
             self.outputs[path] = output
         return output
 
-    def get_output_builder_components(self, output_builder_type):
-        return self.output_builder_components.get(output_builder_type, ())
-
     # main entry point
     def build(
         self,
         model: ModelSchema,
+        profile: str,
+        model_path: List[str],
         output_dir: Union[str, Path],
+        context: Dict[str, Any] = None,
     ):
         """
         compile the schema to output directory
 
-        :param model:      the model schema
+        :param model:       the model schema
+        :param profile:     the profile under which the builder runs
+        :param model_path:  path within the schema that will be converted to datatype and used by output builders
         :param output_dir:  output directory where to put generated files
+        :param context:     extra context supplied to datatype preparation
         :return:            the outputs (self.outputs)
         """
+
+        # deep copy the model
         if self.overwrite:
-            if not hasattr(self.filesystem, "overwrite"):
-                raise AttributeError(
-                    f"Filesystem of type {type(self.filesystem)} does not support overwrite"
-                )
             self.filesystem.overwrite = True
 
+        current_model = dict_setdefault(model.schema, model_path, default={})
+
         self.set_schema(model)
         self.filtered_output_classes = {
-            o.TYPE: o for o in self._filter_classes(self.output_classes, "output")
+            o.TYPE: o
+            for o in self._filter_classes(self.output_classes, current_model, "output")
         }
-        self.output_dir = Path(output_dir).absolute()  # noqa
+        self.output_dir = Path(output_dir).absolute()
         self.outputs = {}
 
-        self._validate_model(model)
-
-        self._run_model_preprocessors(model)
-
-        self._validate_model(model)
-
-        # noinspection PyTypeChecker
-        property_preprocessors: List[PropertyPreprocessor] = [
-            e(self)
-            for e in self._filter_classes(
-                self.property_preprocessor_classes, "property"
-            )
-        ]
-
-        self._run_output_builders(model, property_preprocessors)
+        self._run_output_builders(model, profile, model_path, context or {})
 
         self._save_outputs()
 
         return self.outputs
 
-    def _run_output_builders(self, model, property_preprocessors):
+    def _run_output_builders(
+        self, model: ModelSchema, profile: str, model_path: Iterable[str], context
+    ):
         output_builder_class: Type[OutputBuilder]
         for output_builder_class in self._filter_classes(
-            self.output_builder_classes, "builder"
+            self.output_builder_classes, dict_get(model.schema, model_path), "builder"
         ):
-            output_builder = output_builder_class(
-                builder=self, property_preprocessors=property_preprocessors
-            )
-            output_builder.build(model)
-
-    def _run_model_preprocessors(self, model):
-        for model_preprocessor in self._filter_classes(
-            self.model_preprocessor_classes, "model"
-        ):
-            model_preprocessor(self).transform(model, model.settings)
-
-    def _validate_model(self, model):
-        if not self.skip_schema_validation:
-            validate_model(model)
+            output_builder = output_builder_class(builder=self)
+            current_model = model.get_schema_section(profile, model_path, context)
+            output_builder.build(current_model=current_model, schema=model.schema)
 
     def _save_outputs(self):
         for output in sorted(self.outputs.values(), key=lambda x: x.path):
             output.finish()
             if output.executable:
                 self.filesystem.make_executable(output.path)
 
     def set_schema(self, schema):
         self.schema = schema
         self.settings = schema.settings
 
     # private methods
 
-    def _filter_classes(self, classes: List[Type[object]], plugin_type):
-        if (
-            "plugins" not in self.schema.current_model
-            or plugin_type not in self.schema.current_model.plugins
-        ):
+    def _filter_classes(self, classes: List[Type[object]], model, plugin_type):
+        if "plugins" not in model or plugin_type not in model["plugins"]:
             return classes
-        plugin_config = self.schema.current_model.plugins[plugin_type]
+        plugin_config = model["plugins"][plugin_type]
 
         disabled = plugin_config.get("disable", [])
         enabled = plugin_config.get("enable", [])
         included = plugin_config.get("include", [])
 
         if included:
             enabled = [*enabled]  # will be adding inclusions so make a copy
             classes = [*classes]
             for incl in included:
-                package_name, class_name = incl.split(":")
-                class_type = getattr(importlib.import_module(package_name), class_name)
+                class_type = import_class(incl)
                 classes.append(class_type)
                 if enabled and class_type.TYPE not in enabled:
                     enabled.append(class_type.TYPE)
 
         if disabled == "__all__":
             ret = []
         else:
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/builders/__init__.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_script_sample_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,185 +1,186 @@
-from __future__ import annotations
+import json
+from typing import Callable
 
-import copy
-import functools
-import inspect
-import sys
-from typing import TYPE_CHECKING, List, Union
-
-from oarepo_model_builder.property_preprocessors import PropertyPreprocessor
-from oarepo_model_builder.stack import ModelBuilderStack, ReplaceElement
-from oarepo_model_builder.utils.json_pathlib import JSONPaths
-from oarepo_model_builder.utils.verbose import log
-
-if TYPE_CHECKING:
-    from oarepo_model_builder.builder import ModelBuilder
-
-
-def process(path, priority=0, condition=None):
-    def wrapper(f):
-        @functools.wraps(f)
-        def wrapped(*args, **kwargs):
-            return f(*args, **kwargs)
-
-        wrapped.model_builder_path = path
-        wrapped.model_builder_priority = priority
-        wrapped.model_builder_condition = condition
-        return wrapped
-
-    return wrapper
-
-
-class OutputBuilder:
-    TYPE = None
-    stack: ModelBuilderStack
-
-    def __init__(
-        self, builder: ModelBuilder, property_preprocessors: List[PropertyPreprocessor]
-    ):
-        self.builder = builder
-        self.property_preprocessors = property_preprocessors
-        self.stack = None
-        self.silent_exceptions = False
-        # TODO: move this to metaclass and initialize only once per class
-        self.json_paths = JSONPaths()
-        arr = []
-        for name, method in inspect.getmembers(self, inspect.ismethod):
-            if not hasattr(method, "model_builder_priority"):
-                continue
-            arr.append(
-                (
-                    -method.model_builder_priority,
-                    -len(method.model_builder_path),
-                    method.model_builder_path,
-                    id(method),
-                    method.model_builder_condition,
-                    method,
-                )
-            )
-        arr.sort()
-        for _prior, _lpath, path, _mid, condition, method in arr:
-            self.json_paths.register(path, condition, method)
-
-    def begin(self, schema, settings):
-        self.schema = schema.schema
-        self.whole_schema = schema
-        self.current_model = schema.current_model
-        self.settings = settings
-        self.stack = ModelBuilderStack()
-        self.stack.push(None, schema.current_model)
-        log.enter(2, "Creating %s", self.TYPE)
-        self.silent_exceptions = False
-
-    def finish(self):
-        log.leave()
-
-    def build(self, schema):
-        self.begin(schema, schema.settings)
-
-        for proc in self.property_preprocessors:
-            proc.begin(schema, schema.settings)
-
-        self.build_children()
-
-        for proc in self.property_preprocessors:
-            proc.finish()
-
-        self.finish()
-
-    def build_node(self, key, data):
-        try:
-            data = copy.deepcopy(data)
-            self.stack.push(key, data)
-
-            try:
-                for property_preprocessor in self.property_preprocessors:
-                    data = (
-                        property_preprocessor.process(self.TYPE, data, self.stack)
-                        or data
-                    )
-            except ReplaceElement as e:
-                data = e
-            if isinstance(data, ReplaceElement):
-                self.stack.pop()
-                if data.data is not None:
-                    if isinstance(data.data, dict):
-                        for k, v in data.data.items():
-                            self.build_node(k, v)
-                    elif isinstance(data.data, (list, tuple)):
-                        for k, v in enumerate(data.data):
-                            self.build_node(k, v)
-                    else:
-                        raise AttributeError(
-                            f"Do not know how to handle {type(data.data)} in ReplaceElement"
-                        )
-                return
-            self.stack.top.data = data
-            self.process_stack_top()
-            self.stack.pop()
-        except Exception as e:
-            if not self.silent_exceptions:
-                self.silent_exceptions = True
-                print(f"Error on handling path {self.stack.path}: {e}", file=sys.stderr)
-            raise
-
-    def build_children(self):
-        data = self.stack.top.data
-        if isinstance(data, (list, tuple)):
-            for k, v in enumerate(data):
-                self.build_node(k, v)
-        elif isinstance(data, dict):
-            children = list(data.items())
-            for k, v in children:
-                self.build_node(k, v)
-
-    def process_stack_top(self):
-        try:
-            self.call_components(
-                "before_process_element", value=self.stack.top.data, stack=self.stack
-            )
-            for method in self.json_paths.match(
-                self.stack.path, self.stack.top.data, extra_data={"stack": self.stack}
-            ):
-                return method()
-            # do not skip stack top
-            if self.stack.level <= 1:
-                self.build_children()
-        finally:
-            self.call_components(
-                "after_process_element", value=self.stack.top.data, stack=self.stack
-            )
-
-    @process("/model")
-    def enter_model(self):
-        self.build_children()
-
-    def call_components(self, method_name, value, **kwargs):
-        for component in self.builder.get_output_builder_components(self.TYPE):
-            if hasattr(component, method_name):
-                value = getattr(component, method_name)(self, value, **kwargs) or value
+import faker
+import faker.providers
+from faker import Faker
+
+from oarepo_model_builder.datatypes import (
+    ArrayDataType,
+    DataType,
+    ObjectDataType,
+    Section,
+)
+
+from ..builder import ModelBuilder
+from ..builders.json_base import JSONBaseBuilder
+from ..entrypoints import load_entry_points_list
+
+
+class SampleDataGenerator(faker.Generator):
+    def __init__(self, **config):
+        super().__init__(**config)
+        self.formatters = set()
+
+    def set_formatter(self, name: str, method: Callable) -> None:
+        self.formatters.add(name)
+        return super().set_formatter(name, method)
+
+
+# provider for Faker
+class Provider:
+    def __init__(self, generator) -> None:
+        self.generator = generator
+
+    def random_float(self):
+        rnd = self.generator.random.randrange(-100, 100 + 1, 1)
+        return rnd / 10
+
+    def random_boolean(self):
+        rnd = self.generator.random.randrange(0, 2, 1)
+        return rnd == 1
+
+    def sample_object(self):
+        return {
+            self.generator.word(): self.generator.word()
+            for _ in range(self.generator.random.randrange(1, 5, 1))
+        }
+
+    def constant(self, value=None):
         return value
 
+    def language_dict(self):
+        return {lang: Faker(locale=lang).sentence() for lang in ("cs", "en")}
 
-class OutputBuilderComponent:
-    def before_process_element(
-        self, builder: OutputBuilder, value, *, stack: ModelBuilderStack, **kwargs
-    ):
-        return value
 
-    def after_process_element(
-        self, builder: OutputBuilder, value, *, stack: ModelBuilderStack, **kwargs
-    ):
-        return value
+SKIP = "skip"
 
 
-TEMPLATES = {
-    "setup_py": "templates/setup.py.jinja2",
-}
-
-__all__ = [
-    "process",
-    "OutputBuilder",
-    "ModelBuilderStack",
-    "ReplaceElement",
-    "TEMPLATES",
-]
+class SampleDataBuilder(JSONBaseBuilder):
+    TYPE = "script_sample_data"
+    output_file_type = "yaml"
+    output_file_name = ["sample", "file"]
+    parent_module_root_name = "jsonschemas"
+
+    def __init__(self, builder: ModelBuilder):
+        super().__init__(builder)
+        self.generator = SampleDataGenerator()
+        from faker.config import PROVIDERS
+
+        self.faker = faker.Faker(
+            generator=self.generator,
+            providers=[
+                "oarepo_model_builder.invenio.invenio_script_sample_data",
+                *PROVIDERS,
+            ],
+        )
+
+        self.sample_data_providers = load_entry_points_list(
+            "oarepo_model_builder.sample_data_providers", profile=None
+        ) + [faker_provider]
+
+    def build_node(self, node: DataType):
+        if not self.output.created:
+            return
+
+        sample: Section = node.section_sample
+        for __ in range(sample.config.get("count", 10)):
+            self.output.next_document()
+            generated = self.generate_sample_for_node_and_children(node)
+            self.output.merge(generated)
+
+    def generate_sample_for_node_and_children(self, node):
+        sample_section, sample = get_oarepo_sample(node)
+        if "sample" in sample:
+            return sample["sample"]
+        if sample.get("skip"):
+            return SKIP
+
+        if isinstance(node, ObjectDataType):
+            ret = {}
+            for k, v in sample_section.children.items():
+                v = self.generate_sample_for_node_and_children(v)
+                if v is not SKIP:
+                    ret[k] = v
+        elif isinstance(node, ArrayDataType):
+            count = sample.get("count")
+            if count is None:
+                count = self.faker.random_int(1, 5)
+            ret = {}
+            for __ in range(count):
+                v = self.generate_sample_for_node_and_children(sample_section.item)
+                if v is not SKIP:
+                    ret[json.dumps(v, sort_keys=True)] = v
+            ret = list(ret.values())
+        else:
+            ret = self.generate_fake(node, sample)
+        return ret
+
+    def generate_fake(self, node: DataType, config):
+        params = {}
+        method = None
+        params = config.get("params", params)
+
+        for provider in self.sample_data_providers:
+            ret = provider(self.faker, node.schema.schema["settings"], node, params)
+            if ret is not SKIP:
+                return ret
+        return SKIP
+
+
+def get_oarepo_sample(node):
+    sample_section = node.section_sample
+    sample = sample_section.config
+
+    if isinstance(sample, dict):
+        return sample_section, sample
+    if isinstance(sample, str):
+        return sample_section, {"faker": "constant", "params": {"value": sample}}
+    if isinstance(sample, (list, dict)):
+        if not node.key:
+            # array
+            return sample_section, {
+                "faker": "random_elements",
+                "params": {"elements": sample, "unique": True},
+            }
+        else:
+            # element
+            return sample_section, {
+                "faker": "random_element",
+                "params": {"elements": sample},
+            }
+
+    return sample_section, {}
+
+
+def faker_provider(faker, settings, node, params):
+    __, config = get_oarepo_sample(node)
+    method = config.get("faker")
+    if not method:
+        if node.key in faker.formatters:
+            method = node.key
+        else:
+            data_type = node.model_type
+            if data_type == "integer":
+                method = "random_int"
+            elif data_type == "number":
+                method = "random_float"
+            elif data_type == "double":
+                method = "random_float"
+            elif data_type == "float":
+                method = "random_float"
+            elif data_type == "boolean":
+                method = "random_boolean"
+            elif data_type == "date":
+                method = "date"
+            elif data_type == "object":
+                # it is an object with unknown properties, return a sample object
+                method = "sample_object"
+            elif data_type in ("string", "keyword", "fulltext", "fulltext+keyword"):
+                method = "sentence"
+            else:
+                print(
+                    f"Warning: do not know how to generate sample data for {data_type} at path {node.path}, using plain string rule"
+                )
+                method = "sentence"
+    return getattr(faker, method)(**params)
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/builders/model_saver.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/builders/model_saver.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,59 @@
+import os
 from pathlib import Path
 
-from oarepo_model_builder.datatypes import DataType, datatypes
-
+from ..datatypes import Section
 from ..outputs.cfg import CFGOutput
-from . import OutputBuilder, process
+from ..utils.dict import dict_get
+from . import OutputBuilder
 from .json_base import JSONBaseBuilder
 from .utils import ensure_parent_modules
 
 
 class ModelSaverBuilder(JSONBaseBuilder):
     TYPE = "model_saver"
     output_file_type = "json"
-    output_file_name = "saved-model-file"
+    output_file_name = ["saved-model", "file"]
     parent_module_root_name = "models"
 
-    @process("**")
-    def model_element(self):
-        self.model_element_enter()
-        self.build_children()
-        self.model_element_leave()
-
-    def enter_model(self):
-        # remove the special json base builder functionality
-        # TODO: better handling for this
-        pass
-
-    def model_element_enter(self):
-        super().model_element_enter()
-        if self.stack.top.schema_element_type in ("items", "property"):
-            datatype: DataType = datatypes.get_datatype(
-                self.stack.top.data,
-                self.stack.top.key,
-                self.current_model,
-                self.whole_schema,
-                self.stack,
-            )
-            if datatype:
-                marshmallow = datatype.marshmallow()
-                marshmallow.setdefault("imports", []).extend(
-                    [
-                        {"import": imp.import_path, "alias": imp.alias}
-                        if imp.alias
-                        else {
-                            "import": imp.import_path,
-                        }
-                        for imp in datatype.imports()
-                    ]
-                )
-                self.output.merge(
-                    {
-                        "marshmallow": marshmallow,
-                    }
-                )
-
-    def output_primitive(self, top, data):
-        if data is not None:
-            if not isinstance(data, (str, float, int, bool)):
-                data = str(data)
-        return super().output_primitive(top, data)
+    def build_node(self, node):
+        generated = self.generate(node)
+        self.output.merge({"model": generated})
+
+    def generate(self, node):
+        section: Section = node.section_model_saver
+        ret = {**node.definition}
+        ret.pop("properties", None)
+        ret.pop("items", None)
+        ret.update(**section.config)
+
+        if section.children:
+            properties = ret.setdefault("properties", {})
+            for k, v in section.children.items():
+                v = self.generate(v)
+                properties[k] = v
+        if section.item:
+            ret["items"] = self.generate(section.item)
+        return ret
 
-    def begin(self, schema, settings):
-        super().begin(schema, settings)
+    def begin(self, current_model, schema):
+        super().begin(current_model, schema)
 
-        output_name = self.current_model[self.output_file_name]
+        output_name = dict_get(self.current_model.definition, self.output_file_name)
         self.output = self.builder.get_output(self.output_file_type, output_name)
-        self.output.enter(self.whole_schema.model_field, {"type": "object"})
         ensure_parent_modules(
             self.builder, Path(output_name), ends_at=self.parent_module_root_name
         )
 
-    def finish(self):
-        self.output.leave()
-        # force clean output
-        super().finish()
-        self.output.force_clean_output()
-
 
 class ModelRegistrationBuilder(OutputBuilder):
     TYPE = "model_registration"
 
     def finish(self):
         super().finish()
         output: CFGOutput = self.builder.get_output("cfg", "setup.cfg")
+        module = self.current_model.definition["saved-model"]["module"]
         output.add_entry_point(
             "oarepo.models",
-            self.current_model.oarepo_models_setup_cfg,
-            f"{self.current_model.package}.models:{Path(self.current_model.saved_model_file).name}",
+            self.current_model.definition["saved-model"]["alias"],
+            f"{module}:{os.path.basename(self.current_model.definition['saved-model']['file'])}",
         )
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/builders/python.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/builders/python.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 class PythonBuilder(OutputBuilder):
     def module_to_path(self, module_name):
         mod = module_name.split(".")
         mod[-1] += ".py"
         return Path(*mod)
 
-    def create_parent_modules(self, python_path):
+    def create_parent_modules(self, python_path: Path):
         ensure_parent_modules(
             self.builder, python_path, max_depth=len(python_path.parts)
         )
 
     def class_to_path(self, class_name):
         return self.module_to_path(package_name(class_name))
+
+    def build_node(self, datatype):
+        "intended to be overridden in children"
+        pass
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/builders/setup_cfg.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/builders/setup_cfg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from pkg_resources import parse_version
 
 from oarepo_model_builder.builders import OutputBuilder
 from oarepo_model_builder.outputs.cfg import CFGOutput
-from oarepo_model_builder.utils.verbose import log
 
 
 class SetupCfgBuilder(OutputBuilder):
     TYPE = "setup_cfg"
 
     def finish(self):
         super().finish()
 
         output: CFGOutput = self.builder.get_output("cfg", "setup.cfg")
         output.setdefault(
-            "metadata", "name", self.current_model.package_base.replace("_", "-")
+            "metadata",
+            "name",
+            self.current_model.definition["module"]["base"].replace("_", "-"),
         )
         version = self.schema.get("version", "1.0.0dev1")
         output.setdefault("metadata", "version", version)
         if parse_version(output.get("metadata", "version").value) < parse_version(
             version
         ):
             output.set("metadata", "version", version)
         output.setdefault(
             "metadata",
             "description",
-            f"A sample application for {self.current_model.package}",
+            f"Repository model for {self.current_model.definition['model-name']}",
         )
         output.setdefault("metadata", "authors", "")
 
         output.setdefault("options", "python", ">=3.9")
 
         output.add_dependency("invenio_access", ">=1.4.4")
         output.add_dependency("invenio_app", ">=1.3.4")
@@ -45,23 +46,15 @@
         output.setdefault("options", "packages", "find:")
 
         output.setdefault(
             "options.package_data", "*", "*.json, *.rst, *.md, *.json5, *.jinja2"
         )
 
         if "runtime-dependencies" in self.schema:
-            for dep, value in self.schema.runtime_dependencies.items():
+            for dep, value in self.schema["runtime-dependencies"].items():
                 output.add_dependency(dep, ">=" + value)
 
         if "dev-dependencies" in self.schema:
-            for dep, value in self.schema.dev_dependencies.items():
+            for dep, value in self.schema["dev-dependencies"].items():
                 output.add_dependency(
                     dep, ">=" + value, group="options.extras_require", section="devs"
                 )
-
-        if output.created:
-            log(
-                log.INFO,
-                f"""To install the data model, run
-    poetry install -E {self.current_model.package}            
-            """,
-            )
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/builders/utils.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/builders/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/builtin_models/invenio.json` & `oarepo-model-builder-4.0.0/oarepo_model_builder/builtin_models/invenio.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6447916666666667%*

 * *Differences: {"'properties'": "{'id': {'ui': OrderedDict([('marshmallow', OrderedDict([('read', False), "*

 * *                 "('write', False)]))])}, 'created': {'type': 'datetime', 'marshmallow': {'read': "*

 * *                 "False}, 'ui': OrderedDict([('marshmallow', OrderedDict([('read', False), "*

 * *                 "('write', False)]))])}, 'updated': {'type': 'datetime', 'marshmallow': {'read': "*

 * *                 "False}, 'ui': OrderedDict([('marshmallow', OrderedDict([('read', False), "*

 * *                 "('write', False […]*

```diff
@@ -12,50 +12,86 @@
             "marshmallow": {
                 "read": false,
                 "write": false
             },
             "sample": {
                 "skip": true
             },
-            "type": "keyword"
+            "type": "keyword",
+            "ui": {
+                "marshmallow": {
+                    "read": false,
+                    "write": false
+                }
+            }
         },
         "created": {
             "facets": {
                 "searchable": true
             },
             "marshmallow": {
-                "read": true,
+                "read": false,
                 "write": false
             },
             "sample": {
                 "skip": true
             },
-            "type": "date"
+            "type": "datetime",
+            "ui": {
+                "marshmallow": {
+                    "read": false,
+                    "write": false
+                }
+            }
         },
         "id": {
             "facets": {
                 "searchable": true
             },
             "marshmallow": {
                 "read": false,
                 "write": false
             },
             "sample": {
                 "skip": true
             },
-            "type": "keyword"
+            "type": "keyword",
+            "ui": {
+                "marshmallow": {
+                    "read": false,
+                    "write": false
+                }
+            }
         },
         "updated": {
             "facets": {
                 "searchable": true
             },
             "marshmallow": {
-                "read": true,
+                "read": false,
                 "write": false
             },
             "sample": {
                 "skip": true
             },
-            "type": "date"
+            "type": "datetime",
+            "ui": {
+                "marshmallow": {
+                    "read": false,
+                    "write": false
+                }
+            }
+        }
+    },
+    "ui": {
+        "marshmallow": {
+            "base-classes": [
+                "InvenioUISchema"
+            ],
+            "imports": [
+                {
+                    "import": "oarepo_runtime.ui.marshmallow.InvenioUISchema"
+                }
+            ]
         }
     }
 }
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/cli.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 import sys
 import traceback
 from pathlib import Path
 
 import click
 import yaml
 
-from oarepo_model_builder.conflict_resolvers import (
-    AutomaticResolver,
-    InteractiveResolver,
-)
 from oarepo_model_builder.entrypoints import (
     create_builder_from_entrypoints,
     load_entry_points_dict,
     load_model,
 )
 from oarepo_model_builder.utils.verbose import log
 
@@ -70,26 +66,28 @@
 @click.option(
     "--isort/--skip-isort", default=True, help="Call isort on generated sources"
 )
 @click.option(
     "--black/--skip-black", default=True, help="Call black on generated sources"
 )
 @click.option(
-    "--resolve-conflicts", type=click.Choice(["replace", "keep", "comment", "debug"])
+    "--autoflake/--skip-autoflake",
+    default=True,
+    help="Call autoflake on generated sources",
 )
 @click.option(
     "--overwrite",
     type=bool,
     default=False,
     help="Do not merge with content in already existing files, overwrite them",
 )
 @click.option(
     "--profile",
     help="Run the builder with this profile",
-    default=["model"],
+    default=["record"],
     multiple=True,
 )
 @click.argument("model_filename", type=click.Path(exists=True), required=True)
 @click.argument(
     "included_models", nargs=-1, type=click.Path(exists=True), required=False
 )
 def run(
@@ -98,15 +96,15 @@
     sets,
     configs,
     model_filename,
     included_models,
     verbosity,
     isort,
     black,
-    resolve_conflicts,
+    autoflake,
     save_model,
     overwrite,
     profile,
     includes,
 ):
     """
     Compiles an oarepo model file given in MODEL_FILENAME into an Invenio repository model.
@@ -114,18 +112,18 @@
     try:
         run_internal(
             output_directory,
             model_filename,
             included_models,
             package,
             configs,
-            resolve_conflicts,
             sets,
             black,
             isort,
+            autoflake,
             verbosity,
             save_model,
             overwrite,
             profile,
             includes,
         )
     except Exception as e:
@@ -142,18 +140,18 @@
 
 def run_internal(
     output_directory,  # NOSONAR
     model_filename,
     included_models,
     package,
     configs,
-    resolve_conflicts,
     sets,
     black,
     isort,
+    autoflake,
     verbosity,
     save_model,
     overwrite,
     profiles,
     includes,
 ):
     # extend system's search path to add script's path in front (so that scripts called from the compiler are taken
@@ -192,52 +190,47 @@
     includes = {
         x.split("=", maxsplit=1)[0]: x.split("=", maxsplit=1)[1] for x in includes
     }
 
     # load model (and resolve includes) and optionally save it before the processing (for debugging)
     model = load_model(
         model_filename,
-        package,
         configs,
         black,
         isort,
+        autoflake,
         sets,
         merged_models=included_models,
         extra_included=includes,
     )
     if save_model:
         with open(save_model, "w") as f:
             yaml.dump(json.loads(json.dumps(model.schema)), f)
 
-    # set the output directory on the schema
-    model.schema["output-directory"] = output_directory
-
-    # create conflict resolver
-    if not resolve_conflicts or resolve_conflicts == "debug":
-        resolver = InteractiveResolver(resolve_conflicts == "debug")
-    else:
-        resolver = AutomaticResolver(resolve_conflicts)
-
     # for each profile on the command line, render it
     profiles_to_render = [y.strip() for x in profiles for y in x.split(",")]
     for profile in profiles_to_render:
         # load the builder
-        builder = create_builder_from_entrypoints(
-            profile=profile, conflict_resolver=resolver, overwrite=overwrite
-        )
+        builder = create_builder_from_entrypoints(profile=profile, overwrite=overwrite)
 
         # load profile handler
         try:
             profile_handler = load_entry_points_dict("oarepo_model_builder.profiles")[
                 profile
             ]()
         except KeyError:
             raise AttributeError(f"No profile handler for {profile} registered")
 
         # and call it
-        profile_handler.build(model, output_directory, builder)
+        profile_handler.build(
+            model,
+            profile,
+            profile_handler.default_model_path,
+            output_directory,
+            builder,
+        )
     log.leave("Done")
     print(f"Log saved to {Path(output_directory) / 'installation.log'}")
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/datatypes/__init__.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/datatypes/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,44 +17,59 @@
   minLength, maxLength, pattern
 
 flatten:
   object represented as flatten type in elasticsearch
 """
 
 
-from .containers import ArrayDataType, FlattenDataType, NestedDataType, ObjectDataType
-from .datatypes import DataType, Import, datatypes  # noqa
-from .dates import (
+from .containers import (  # noqa
+    ArrayDataType,
+    FlattenDataType,
+    NestedDataType,
+    ObjectDataType,
+)
+from .datatypes import DataType, DataTypeComponent, Import, Section, datatypes  # noqa
+from .dates import (  # noqa
     DateDataType,
     DateTimeDataType,
     EDTFDataType,
     EDTFIntervalType,
     TimeDataType,
 )
-from .primitive_types import NumberDataType  # noqa
+from .model import ModelDataType  # noqa
+from .primitive_types import NumberDataType  # noqa , just for export
 from .primitive_types import (
     BooleanDataType,
     DoubleDataType,
     FloatDataType,
     IntegerDataType,
 )
-from .strings import StringDataType  # noqa
-from .strings import FulltextDataType, FulltextKeywordDataType, KeywordDataType
+from .strings import (  # noqa , just for export; noqa
+    FulltextDataType,
+    FulltextKeywordDataType,
+    KeywordDataType,
+    StringDataType,
+    URLDataType,
+    UUIDDataType,
+)
 
 DEFAULT_DATATYPES = [
     IntegerDataType,
     FloatDataType,
     DoubleDataType,
     BooleanDataType,
     DateDataType,
     TimeDataType,
     DateTimeDataType,
     EDTFDataType,
     EDTFIntervalType,
     FulltextDataType,
     KeywordDataType,
     FulltextKeywordDataType,
+    UUIDDataType,
     ObjectDataType,
     NestedDataType,
     FlattenDataType,
     ArrayDataType,
+    URLDataType,
+    ModelDataType,
 ]
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/datatypes/datatypes.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/cfg.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,94 @@
-import copy
-from collections import namedtuple
-from typing import List, Union
-
-import importlib_metadata
-import marshmallow as ma
-from marshmallow import fields
-
-Import = namedtuple("Import", "import_path,alias")
-
-
-class DataType:
-    model_type = None
-    marshmallow_field = None
-    schema_type = None
-    mapping_type = None
-
-    class ModelSchema(ma.Schema):
-        type = fields.String(required=True)
-
-    def __init__(self, definition, key, model, schema, stack):
-        self.definition = definition
-        self.key = key
-        self.model = model
-        self.schema = schema
-        self.stack = stack
-
-    def _copy_definition(self, **extras):
-        ret = copy.deepcopy(self.definition)
-        for k, v in extras.items():
-            if v is not None:
-                ret[k] = v
-        return ret
-
-    def model_schema(self, **extras):
-        return None
-
-    def json_schema(self, **extras):
-        return self._copy_definition(type=self.schema_type, **extras)
-
-    def mapping(self, **extras):
-        return self._copy_definition(type=self.mapping_type, **extras)
-
-    def marshmallow(self, **extras):
-        ret = copy.deepcopy(self.definition.get("marshmallow", {}))
-        if self.marshmallow_field:
-            ret.setdefault("field-class", self.marshmallow_field)
-        ret.setdefault("validators", []).extend(self.marshmallow_validators())
-        for k, v in extras.items():
-            if v is not None:
-                ret[k] = v
-        return ret
-
-    def marshmallow_validators(self) -> List[str]:
-        return []
-
-    def imports(self, *extra) -> List[Import]:
-        return extra
-
-    def facet(self, key, definition={}, props_num=None, create=True):
-        return False
-
-    def dumper_class(self, data):  # NOSONAR
-        return None
-
-
-class DataTypes:
-    def __init__(self) -> None:
-        self.datatype_map = {}
-
-    def _prepare_datatypes(self):
-        if not self.datatype_map:
-            for entry in importlib_metadata.entry_points(
-                group="oarepo_model_builder.datatypes"
-            ):
-                for dt in entry.load():
-                    self.datatype_map[dt.model_type] = dt
-
-    def get_datatype(self, data, key, model, schema, stack) -> Union[DataType, None]:
-        datatype_class = self.get_datatype_class(data.get("type", None))
-        if datatype_class:
-            return datatype_class(data, key, model, schema, stack)
-        return None
-
-    def get_datatype_class(self, datatype_type):
-        self._prepare_datatypes()
-        return self.datatype_map.get(datatype_type)
+from configupdater import ConfigUpdater, Option
 
+from oarepo_model_builder.outputs import OutputBase
 
-datatypes = DataTypes()
+
+class CFGOutput(OutputBase):
+    TYPE = "cfg"
+
+    # high-level API
+
+    def add_entry_point(self, group, name, value):
+        """
+        Adds an entry point if it is not already present
+        """
+        line = f"{name} = {value}"
+        grp = self.create_multiline_value(
+            "options.entry_points", group, initial_value=line
+        )
+        for e in grp.as_list():
+            e = [x.strip() for x in e.split("=", maxsplit=1)]
+            if len(e) == 2 and e[0] == name and e[1] == value:
+                break
+        else:
+            grp.append(line)
+
+    def add_dependency(
+        self, package, version, group="options", section="install_requires", extras=None
+    ):
+        if extras:
+            line = f'{package}[{", ".join(extras)}]{version}'
+        else:
+            line = f"{package}{version}"
+        grp = self.create_multiline_value(group, section, line)
+        for e in grp.as_list():
+            if line == e.strip():
+                break
+        else:
+            grp.append(line)
+
+    # low-level API
+
+    def begin(self):
+        try:
+            with self.builder.filesystem.open(self.path) as f:
+                self.original_data = f.read()
+                self.cfg = ConfigUpdater()
+                self.cfg.read_string(self.original_data)
+                self.parsed = str(self.cfg)
+        except FileNotFoundError:
+            self.original_data = None
+            self.cfg = ConfigUpdater()
+            self.parsed = None
+
+    @property
+    def created(self):
+        return self.original_data is None
+
+    def get(self, section, key):
+        try:
+            tbl = self.cfg[section]
+            return tbl[key]
+        except KeyError:
+            return None
+
+    def get_section(self, section, create=False):
+        if create and section not in self.cfg:
+            self.cfg.add_section(section)
+            tbl = self.cfg[section]
+            tbl.add_before.space(2)
+            return tbl
+        return self.cfg[section]
+
+    def set(self, section, key, value):
+        tbl = self.get_section(section, create=True)
+        tbl[key] = value
+
+    def setdefault(self, section, key, value):
+        tbl = self.get_section(section, create=True)
+        return tbl.setdefault(key, value)
+
+    def create_multiline_value(self, section, name, initial_value="") -> Option:
+        tbl = self.get_section(section, create=True)
+        if name in tbl:
+            grp = tbl[name]
+        else:
+            grp = Option(name, value=initial_value)
+            tbl.add_option(grp)
+        return grp
+
+    def finish(self):
+        out = str(self.cfg)
+        if out != self.parsed:
+            with self.builder.filesystem.open(self.path, "w") as f:
+                f.write(out)
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/entrypoints.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/entrypoints.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,42 +4,24 @@
 from importlib import import_module
 from pathlib import Path
 
 import importlib_metadata
 
 from oarepo_model_builder.builder import ModelBuilder
 from oarepo_model_builder.schema import ModelSchema, remove_star_keys
-from oarepo_model_builder.utils.hyphen_munch import HyphenMunch
 
 
-def create_builder_from_entrypoints(profile="model", **kwargs):
+def create_builder_from_entrypoints(profile="record", **kwargs):
     # output classes do not depend on profile
     output_classes = load_entry_points_list("oarepo_model_builder.outputs", None)
     builder_classes = load_entry_points_list("oarepo_model_builder.builders", profile)
-    preprocess_classes = load_entry_points_list(
-        "oarepo_model_builder.property_preprocessors", profile
-    )
-    model_preprocessor_classes = load_entry_points_list(
-        "oarepo_model_builder.model_preprocessors", profile
-    )
-
-    builder_types = [x.TYPE for x in builder_classes]
-    output_builder_components = {
-        builder_type: load_entry_points_list(
-            f"oarepo_model_builder.builder_components.{builder_type}", profile
-        )
-        for builder_type in builder_types
-    }
 
     return ModelBuilder(
         output_builders=builder_classes,
         outputs=output_classes,
-        property_preprocessors=preprocess_classes,
-        model_preprocessors=model_preprocessor_classes,
-        output_builder_components=output_builder_components,
         **kwargs,
     )
 
 
 def load_entry_points_dict(name):
     return {
         ep.name: ep.load()
@@ -47,33 +29,42 @@
     }
 
 
 def load_entry_points_list(name, profile):
     ret = []
     loaded = {}
     group_name = f"{name}.{profile}" if profile else name
+    load_from_entry_point_internal(name, group_name, loaded, ret)
+    # inherit
+    inherit_group = f"{name}.{profile}.inherit" if profile else f"{name}.inherit"
+    for ep in importlib_metadata.entry_points().select(group=inherit_group):
+        inherit_from = ep.value
+        load_from_entry_point_internal(name, inherit_from, loaded, ret)
+    ret.sort()
+    return [x[1] for x in ret]
+
+
+def load_from_entry_point_internal(name, group_name, loaded_keys, loaded_entries):
     for ep in importlib_metadata.entry_points().select(group=group_name):
-        if ep.name in loaded:
+        if ep.name in loaded_keys:
             print(
                 f"WARNING: Entry point {ep.name} has already been registered to group {name}. "
-                f"Previous value {loaded[ep.name]}, new ignored value {ep.value}"
+                f"Previous value {loaded_keys[ep.name]}, new ignored value {ep.value}"
             )
             continue
         loaded_entry_point = ep.load()
-        ret.append((ep.name, loaded_entry_point))
-        loaded[ep.name] = ep.value
-    ret.sort()
-    return [x[1] for x in ret]
+        loaded_entries.append((ep.name, loaded_entry_point))
+        loaded_keys[ep.name] = ep.value
 
 
 def load_model_from_entrypoint(ep: importlib_metadata.EntryPoint):
     def load(schema):
         try:
             loaded_schema = ep.load()
-        except:
+        except:  # NOSONAR intentionally broad
             module = import_module(ep.module)
             split_attr = ep.attr.split(".")
             fn = f"{split_attr[-2]}.{split_attr[-1]}"
             if len(split_attr) > 2:
                 fn = reduce(lambda x, y: Path(x) / Path(y), split_attr[:-2]) / fn
             module_path = getattr(module, "__path__", [])
             if module_path:
@@ -94,18 +85,18 @@
     for ep in importlib_metadata.entry_points().select(group="oarepo.models"):
         ret[ep.name] = load_model_from_entrypoint(ep)
     return ret
 
 
 def load_model(
     model_filename,
-    package=None,
     configs=(),
     black=True,
     isort=True,
+    autoflake=True,
     sets=(),
     model_content=None,
     extra_included=None,
     merged_models=None,
 ):
     loaders = load_entry_points_dict("oarepo_model_builder.loaders")
     included_models = load_included_models_from_entry_points()
@@ -120,20 +111,19 @@
     )
     for config in configs:
         load_config(schema, config, loaders)
     for s in sets:
         k, v = s.split("=", 1)
         schema.schema[k] = v
     check_plugin_packages(schema)
-    if package and not schema.current_model.get("package"):
-        schema.current_model.package = package
     if "python" not in schema.settings:
-        schema.settings.python = HyphenMunch()
-    schema.settings.python.use_isort = isort
-    schema.settings.python.use_black = black
+        schema.settings["python"] = {}
+    schema.settings["python"]["use-isort"] = isort
+    schema.settings["python"]["use-black"] = black
+    schema.settings["python"]["use-autoflake"] = autoflake
     return schema
 
 
 def load_config(schema, config, loaders):
     old_loaders = schema.loaders
     schema.loaders = loaders
     try:
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/fs.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/fs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from io import StringIO
+from io import BytesIO, StringIO
 from pathlib import Path
 from typing import Dict
 
 
 class AbstractFileSystem:
     def open(self, path, *args, **kwargs):
         raise NotImplementedError()
@@ -46,21 +46,23 @@
 
 class InMemoryFileSystem(AbstractFileSystem):
     def __init__(self):
         self.files: Dict[str, StringIO] = {}
 
     def open(self, path: str, mode: str = "r"):
         path = Path(path).absolute()
-        if mode == "r":
+        if "r" in mode:
             if path not in self.files:
                 raise FileNotFoundError(
                     f"File {path} not found. Known files {[f for f in self.files]}"
                 )
+            if "b" in mode:
+                return BytesIO(self.files[path].getvalue())
             return StringIO(self.files[path].getvalue())
-        self.files[path] = StringIO()
+        self.files[path] = BytesIO() if "b" in mode else StringIO()
         self.files[path].close = lambda: None
         return self.files[path]
 
     def exists(self, path):
         path = Path(path).absolute()
         return path in self.files
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,21 +8,23 @@
     TYPE = "invenio_ext_setup_cfg"
 
     def finish(self):
         super().finish()
 
         output: CFGOutput = self.builder.get_output("cfg", "setup.cfg")
 
-        package_name, base_name = split_package_base_name(self.current_model.ext_class)
+        package_name, base_name = split_package_base_name(
+            self.current_model.definition["ext"]["class"]
+        )
 
         output.add_entry_point(
             "invenio_base.api_apps",
-            self.current_model.extension_suffix,
+            self.current_model.definition["ext"]["alias"],
             f"{package_name}:{base_name}",
         )
 
         # need to add ext to apps because cli depends on it
         output.add_entry_point(
             "invenio_base.apps",
-            self.current_model.extension_suffix,
+            self.current_model.definition["ext"]["alias"],
             f"{package_name}:{base_name}",
         )
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-from oarepo_model_builder.utils.jinja import package_name
-
 from ..builders import OutputBuilder
 from ..outputs.cfg import CFGOutput
 
 
 class InvenioRecordMetadataModelsSetupCfgBuilder(OutputBuilder):
     TYPE = "invenio_record_metadata_models_setup_cfg"
 
     def finish(self):
         super().finish()
 
         output: CFGOutput = self.builder.get_output("cfg", "setup.cfg")
 
-        metadata_package = package_name(self.current_model.record_metadata_class)
-
         output.add_entry_point(
             "invenio_db.models",
-            self.current_model.record_schema_metadata_setup_cfg,
-            metadata_package,
+            self.current_model.definition["record-metadata"]["alias"],
+            self.current_model.definition["record-metadata"]["module"],
         )
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,15 +9,25 @@
 
     def finish(self):
         super().finish()
 
         output: CFGOutput = self.builder.get_output("cfg", "setup.cfg")
 
         register_function = split_package_base_name(
-            self.current_model.create_blueprint_from_app
+            self.current_model.definition["api-blueprint"]["function"]
         )
 
         output.add_entry_point(
             "invenio_base.api_blueprints",
-            self.current_model.record_api_blueprints_setup_cfg,
+            self.current_model.definition["api-blueprint"]["alias"],
+            f"{register_function[0]}:{register_function[-1]}",
+        )
+
+        register_function = split_package_base_name(
+            self.current_model.definition["app-blueprint"]["function"]
+        )
+
+        output.add_entry_point(
+            "invenio_base.blueprints",
+            self.current_model.definition["app-blueprint"]["alias"],
             f"{register_function[0]}:{register_function[-1]}",
         )
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/invenio_record_service_config.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/invenio_record_service_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 from oarepo_model_builder.outputs.python import PythonOutput
-from oarepo_model_builder.utils.hyphen_munch import HyphenMunch
 
-from ..utils.jinja import base_name
+from ..datatypes import Section
+from ..datatypes.model import Link
 from .invenio_base import InvenioBaseClassPythonBuilder
 
 
 class InvenioRecordServiceConfigBuilder(InvenioBaseClassPythonBuilder):
     TYPE = "invenio_record_service_config"
-    class_config = "record-service-config-class"
-    template = "record-service-config"
+    section = "service-config"
+    template = "service-config"
 
     def process_template(self, python_path, template, **extra_kwargs):
         if self.parent_modules:
             self.create_parent_modules(python_path)
         output: PythonOutput = self.builder.get_output("python", python_path)
 
-        context = HyphenMunch(
-            settings=self.settings, current_model=self.current_model, **extra_kwargs
-        )
-        template = self.call_components(
-            "invenio_before_python_template", template, context=context
+        links_section: Section = self.current_model.section_links
+        imports = set()
+        link: Link
+        for s in links_section.config.values():
+            for link in s:
+                imports.update(link.imports)
+        imports = list(imports)
+
+        for ll in links_section.config.values():
+            ll.sort(key=lambda x: x.name or "")
+
+        context = dict(
+            settings=self.settings,
+            current_model=self.current_model,
+            links=links_section.config,
+            link_imports=imports,
+            **extra_kwargs,
         )
         output.merge(template, context)
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2` & `oarepo-model-builder-4.0.0/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from invenio_records_resources.services import SearchOptions as InvenioSearchOptions
+from flask_babelex import lazy_gettext as _
 from . import facets
 
-def _(x):
-    """Identity function for string extraction."""
-    return x
-
-{% for b in current_model.record_search_options_bases %}
+{% for b in vars.record_search_options_bases %}
 from {{ b|package_name }} import {{ b|base_name }}
 {% endfor %}
 
-class {{ current_model.record_search_options_class|base_name }}({% for b in current_model.record_search_options_bases %}{{ b|base_name }}, {% endfor %}InvenioSearchOptions):
-    """{{ current_model.record_class|base_name }} search options."""
+class {{ vars.record_search_options_class|base_name }}({% for b in vars.record_search_options_bases %}{{ b|base_name }}, {% endfor %}InvenioSearchOptions):
+    """{{ vars.record_class|base_name }} search options."""
 
     facets = {
 {% for dict in facets_definition %}
 {% for key, value in dict.items()%}
     '{{ key }}': {{ value }},
 {% endfor %}
 {% endfor %}
     }
     sort_options = {
-        {% if current_model.record_search_options_bases %}
-        **{{ current_model.record_search_options_bases[0]|base_name }}.sort_options,
+        {% if vars.record_search_options_bases %}
+        **{{ vars.record_search_options_bases[0]|base_name }}.sort_options,
         {% else %}
         **InvenioSearchOptions.sort_options,
         {% endif %}
 {% for dict in sort_definition %}
 {% for key, value in dict.items()%}
     '{{ key }}': {{ value }},
 {% endfor %}
 {% endfor %}
     }
 
 
-{{ current_model.invenio_record_search_options_extra_code }}
+{{ vars.invenio_record_search_options_extra_code }}
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/loaders/__init__.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/loaders/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 try:
     import json5
 except ImportError:
     import json as json5
 
 
-def json_loader(file_path, schema, content=None):
+def json_loader(
+    file_path, schema, content=None  # NOSONAR schema kept for extensibility
+):
     if content:
         return json5.loads(content)
     with open(file_path) as f:
         return json5.load(f)
 
 
-def yaml_loader(file_path, schema, content=None):
+def yaml_loader(
+    file_path, schema, content=None  # NOSONAR schema kept for extensibility
+):
     try:
         import yaml
     except ImportError:
         raise RuntimeError(
             "Loader for yaml not found. Please install pyyaml library to use yaml files"
         )
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/merger.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/merger.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,65 +6,83 @@
 
 import click
 import json5
 import libcst as cst
 import yaml
 
 from oarepo_model_builder.utils.cst import PythonContext, merge
-from oarepo_model_builder.utils.cst.common import ConflictResolver
 from oarepo_model_builder.utils.deepmerge import deepmerge
 
 
 @click.command()
 @click.argument("source", type=click.Path(file_okay=True, dir_okay=True, exists=True))
 @click.argument(
-    "destination", type=click.Path(file_okay=True, dir_okay=True, exists=True)
+    "destination", type=click.Path(file_okay=True, dir_okay=True, exists=False)
 )
 @click.option(
     "--result",
     type=click.Path(file_okay=True, dir_okay=True),
     help="Do not overwrite destination, write to this path instead",
 )
 @click.option(
     "--destination-first/--source-first",
     help="Take destination first and merge source only if it is not in destination. Normally merges destination into source and replaces destination with the result",
 )
-def merger(source, destination, result, destination_first):
+@click.option(
+    "--overwrite/--no-overwrite",
+    help="Do not perform merging but overwrite destination files with source files",
+)
+def merger(source, destination, result, destination_first, overwrite):
     source = Path(source)
     destination = Path(destination)
 
     if source.is_file():
-        if not destination.is_file():
+        if destination.exists() and not destination.is_file():
             click.echo(
                 "If source is a file, destination must be a file as well", err=True
             )
             sys.exit(1)
-        merge_file(source, destination, result or destination, destination_first)
+        merge_file(
+            source, destination, result or destination, destination_first, overwrite
+        )
     else:
         for fn in source.glob("**/*"):
+            if not fn.is_file():
+                continue
             relative_fn = fn.relative_to(source)
             merge_file(
                 fn,
                 destination.joinpath(relative_fn),
                 result.joinpath(relative_fn)
                 if result
                 else destination.joinpath(relative_fn),
                 destination_first,
+                overwrite,
             )
 
 
-def merge_file(source: Path, destination: Path, result: Path, destination_first: bool):
+def merge_file(
+    source: Path,
+    destination: Path,
+    result: Path,
+    destination_first: bool,
+    overwrite: bool,
+):
     source_suffix = source.suffix[1:]
     destination_suffix = destination.suffix[1:]
     if source_suffix != destination_suffix:
         raise AttributeError(
             f"Suffixes of source and destination files must match, have {source}, {destination}"
         )
-    if not destination.exists():
-        shutil.copy(source, destination)
+    result.parent.mkdir(parents=True, exist_ok=True)
+    if not destination.exists() or overwrite:
+        if source.is_file():
+            shutil.copy(source, result)
+        else:
+            shutil.copytree(source, result, dirs_exist_ok=True)
         return
     if source_suffix == "yaml":
         merge_json(
             source,
             destination,
             result,
             destination_first,
@@ -89,19 +107,21 @@
             json5.load,
             partial(json5.dump, indent=4, ensure_ascii=False),
         )
     elif source_suffix == "py":
         merge_python(source, destination, result, destination_first)
     else:
         raise NotImplementedError(
-            f"Merging file type {source_suffix} is not implemented yet"
+            f"Merging file type {source_suffix} (file {source}) is not implemented yet"
         )
 
 
-def merge_json(source, destination, result, destination_first, load_func, dump_func):
+def merge_json(
+    source, destination, result: Path, destination_first, load_func, dump_func
+):
     with open(source) as f:
         source_data = load_func(f)
     with open(destination) as f:
         destination_data = load_func(f)
     if destination_first:
         deepmerge(destination_data, source_data)
     else:
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/cfg.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/yaml.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,69 @@
-from configupdater import ConfigUpdater, Option
+import yaml
+from deepdiff import DeepDiff
 
-from oarepo_model_builder.outputs import OutputBase
+from ..utils.verbose import log
+from . import OutputBase
+from .json_stack import JSONStack
 
 
-class CFGOutput(OutputBase):
-    TYPE = "cfg"
-
-    # high-level API
-
-    def add_entry_point(self, group, name, value):
-        """
-        Adds an entry point if it is not already present
-        """
-        line = f"{name} = {value}"
-        grp = self.create_multiline_value(
-            "options.entry_points", group, initial_value=line
-        )
-        for e in grp.as_list():
-            e = [x.strip() for x in e.split("=", maxsplit=1)]
-            if len(e) == 2 and e[0] == name and e[1] == value:
-                break
-        else:
-            grp.append(line)
-
-    def add_dependency(
-        self, package, version, group="options", section="install_requires", extras=None
-    ):
-        if extras:
-            line = f'{package}[{", ".join(extras)}]{version}'
-        else:
-            line = f"{package}{version}"
-        grp = self.create_multiline_value(group, section, line)
-        for e in grp.as_list():
-            if line == e.strip():
-                break
-        else:
-            # TODO: this is a private api, but 'append' seems not to work on empty option
-            grp.append(line)
-
-    # low-level API
+class YAMLOutput(OutputBase):
+    IGNORE_NODE = JSONStack.IGNORED_NODE
+    IGNORE_SUBTREE = JSONStack.IGNORED_SUBTREE
+    TYPE = "yaml"
 
     def begin(self):
+        self._created = True
         try:
             with self.builder.filesystem.open(self.path) as f:
-                self.original_data = f.read()
-                self.cfg = ConfigUpdater()
-                self.cfg.read_string(self.original_data)
-                self.parsed = str(self.cfg)
+                self.original_data = yaml.load_all(f, yaml.SafeLoader)  # noqa
+                self._created = False
         except FileNotFoundError:
             self.original_data = None
-            self.cfg = ConfigUpdater()
-            self.parsed = None
+        except ValueError:
+            self.original_data = None
+
+        self.stack = JSONStack()
+        self.documents = []
+
+    def next_document(self):
+        if self.stack.value:
+            self.documents.append(self.stack.value)
+            self.stack = JSONStack()
+
+    def finish(self):
+        self.next_document()
+
+        if not self.documents and self.original_data:
+            # nothing generated, keep the file
+            return
+
+        self._created = False
+        if DeepDiff(self.documents, self.original_data):
+            self.builder.filesystem.mkdir(self.path.parent)
+            log(2, "Saving %s", self.path)
+            with self.builder.filesystem.open(self.path, mode="w") as f:
+                yaml.safe_dump_all(self.documents, f, allow_unicode=True)
 
     @property
     def created(self):
-        return self.original_data is None
+        return self._created
 
-    def get(self, section, key):
-        try:
-            tbl = self.cfg[section]
-            return tbl[key]
-        except KeyError:
-            return None
-
-    def get_section(self, section, create=False):
-        if create and section not in self.cfg:
-            self.cfg.add_section(section)
-            tbl = self.cfg[section]
-            tbl.add_before.space(2)
-            return tbl
-        return self.cfg[section]
-
-    def set(self, section, key, value):
-        tbl = self.get_section(section, create=True)
-        tbl[key] = value
-
-    def setdefault(self, section, key, value):
-        tbl = self.get_section(section, create=True)
-        return tbl.setdefault(key, value)
-
-    def create_multiline_value(self, section, name, initial_value="") -> Option:
-        tbl = self.get_section(section, create=True)
-        if name in tbl:
-            grp = tbl[name]
-        else:
-            grp = Option(name, value=initial_value)
-            tbl.add_option(grp)
-        return grp
+    @created.setter
+    def created(self, value):
+        self._created = value
+
+    def enter(self, key, el):
+        if key is not None:
+            self.stack.push(key, el)
+
+    def leave(self):
+        if not self.stack.empty:
+            self.stack.pop()
+
+    def primitive(self, key, value):
+        if key is not None:
+            self.stack.push(key, value)
+            self.stack.pop()
 
-    def finish(self):
-        out = str(self.cfg)
-        if out != self.parsed:
-            with self.builder.filesystem.open(self.path, "w") as f:
-                f.write(out)
+    def merge(self, value):
+        self.stack.merge(value)
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/diff.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/diff.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/json.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/json.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import copy
 import json
 
 from deepdiff import DeepDiff
 
+from ..utils.deepmerge import deepmerge
 from ..utils.verbose import log
 from . import OutputBase
 from .json_stack import JSONStack
 
 try:
     import json5
 except ImportError:
@@ -17,44 +19,40 @@
     IGNORE_SUBTREE = JSONStack.IGNORED_SUBTREE
     TYPE = "json"
 
     def begin(self):
         try:
             with self.builder.filesystem.open(self.path) as f:
                 self.original_data = json5.load(f)  # noqa
+                self.data = copy.deepcopy(self.original_data)
         except FileNotFoundError:
             self.original_data = None
+            self.data = {}
         except ValueError:
             self.original_data = None
-
-        self.stack = JSONStack()
+            self.data = {}
 
     @property
     def created(self):
         return self.original_data is None
 
     def force_clean_output(self):
         self.original_data = None
 
     def finish(self):
-        data = self.stack.value
-        if DeepDiff(data, self.original_data):
+        # create differing but non-empty files
+        if DeepDiff(self.data, self.original_data) and (
+            self.data or self.original_data
+        ):
             self.builder.filesystem.mkdir(self.path.parent)
             log(2, "Saving %s", self.path)
             with self.builder.filesystem.open(self.path, mode="w") as f:
-                json.dump(data, f, ensure_ascii=False, indent=4)
-
-    def enter(self, key, el):
-        if key is not None:
-            self.stack.push(key, el)
-
-    def leave(self):
-        if not self.stack.empty:
-            self.stack.pop()
-
-    def primitive(self, key, value):
-        if key is not None:
-            self.stack.push(key, value)
-            self.stack.pop()
+                json.dump(self.data, f, ensure_ascii=False, indent=4)
 
     def merge(self, value):
-        self.stack.merge(value)
+        self.data = deepmerge(value, self.data)
+
+    @property
+    def modified(self):
+        return DeepDiff(self.data, self.original_data) and (
+            self.data or self.original_data
+        )
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/json_stack.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/json_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                 elif isinstance(top, list):
                     if key < len(top):
                         top[key] = deepmerge(el, top[key])
                     else:
                         assert key == len(top)
                         top.append(el)
                 else:
-                    raise NotImplemented(
+                    raise NotImplementedError(
                         f"Set for datatype {type(top)} is not implemented"
                     )
                 self.stack.append(el)
         except Exception as e:
             raise JSONStackException(
                 f'Error pushing to json stack. Key "{key}", stack top {self.stack[-1]}'
             ) from e
@@ -75,7 +75,11 @@
         for t in reversed(self.stack):
             if t is not self.IGNORED_NODE:
                 return t
 
     def merge(self, value):
         real_top = self.real_top
         real_top.update(deepmerge(value, real_top, []))
+
+    def replace(self, value):
+        self.real_top.clear()
+        self.merge(value)
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/text.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/text.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/outputs/toml.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/outputs/toml.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/profiles/model.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/profiles/record.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,87 @@
 from pathlib import Path
-from typing import Union
+from typing import Any, Dict, List, Union
 
 import json5
 
 from oarepo_model_builder.builder import ModelBuilder
 from oarepo_model_builder.entrypoints import create_builder_from_entrypoints, load_model
 from oarepo_model_builder.fs import InMemoryFileSystem
 from oarepo_model_builder.profiles import Profile
 from oarepo_model_builder.profiles.extend import ExtendProfile
 from oarepo_model_builder.schema import ModelSchema
 from oarepo_model_builder.utils.deepmerge import deepmerge
+from oarepo_model_builder.utils.dict import dict_get
 
 
-class ModelProfile(Profile):
+class RecordProfile(Profile):
+    default_model_path = ("record",)
+
     def build(
         self,
         model: ModelSchema,
+        profile: str,
+        model_path: List[str],
         output_directory: Union[str, Path],
         builder: ModelBuilder,
+        **kwargs,
     ):
-        # at first handle "extend"
-        if "extend" in model.current_model:
-            self.handle_extend(model.current_model.extend, model, builder)
-        return super().build(model, output_directory, builder)
+        current_model = dict_get(model.schema, model_path)
+        if "extend" in current_model:
+            self.handle_extend(
+                current_model["extend"],
+                model,
+                profile,
+                model_path,
+                current_model,
+                builder,
+            )
+        return super().build(
+            model, profile, model_path, output_directory, builder, **kwargs
+        )
 
     def handle_extend(
-        self, extended_schema: str, model: ModelSchema, builder: ModelBuilder
+        self,
+        extended_schema: str,
+        model: ModelSchema,
+        profile: str,
+        model_path: List[str],
+        current_model: Dict[str, Any],
+        builder: ModelBuilder,
     ):
         """
         extending the model means:
             1. extended schema is read as a schema. If there is a json path behind it,
                it is used to select the model. by default /model is taken
             2. The model will be processed through "extend" profile with
                the output file "model.json5" stored in memory:
                   * properties ending with "-class" on model will be turned to array and suffix changed to -base-classes
                   * jsonschema and mapping will not be touched
                   * marshmallow will have all the properties marked as {read: false, write: false} so that they are not generated
             3. the resulting model will be merged as if use: was used
         """
 
-        extended_schema = extended_schema.split("#", maxsplit=1)
-        schema_location = extended_schema[0]
-        if len(extended_schema) == 1:
-            model_field = "model"
-        else:
-            model_field = extended_schema[1]
-            if model_field.startswith("/"):
-                model_field = model_field[1:]
-            if "/" in model_field:
-                raise ValueError("Can not currently process nested models")
+        loaded_schema = {"model": {"use": [extended_schema]}}
 
         extended_model = load_model(
-            schema_location,
-            package=None,
+            extended_schema.split("#", maxsplit=1)[0],
             configs=[],
             black=False,
             isort=False,
+            autoflake=False,
             sets=[],
             extra_included=model.included_schemas,
+            model_content=loaded_schema,
         )
-        extended_model.model_field = model_field
+        extended_model.model_field = "model"
 
         fs = InMemoryFileSystem()
         builder = create_builder_from_entrypoints(
             profile="extend",
-            conflict_resolver=builder.conflict_resolver,
             overwrite=builder.overwrite,
             filesystem=fs,
         )
 
-        ExtendProfile().build(extended_model, "", builder)
+        ExtendProfile().build(extended_model, profile, model_path, "", builder)
 
         loaded_model = json5.loads(fs.read("model.json5"))
-        deepmerge(model.current_model, loaded_model)
+        deepmerge(current_model, loaded_model)
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/schema.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,49 @@
 import copy
+import os
 import pathlib
 from pathlib import Path
 from typing import Callable, Dict, List, Union
 
-import munch
-import yaml
 from jsonpointer import resolve_pointer
-from yaml import SafeDumper
 
 from .exceptions import IncludedFileNotFoundException
 from .utils.deepmerge import deepmerge
-from .utils.hyphen_munch import HyphenMunch
-
-
-class Key(str):
-    def __new__(cls, value, *args, source=None, **kwargs):
-        ret = super().__new__(cls, value)
-        ret.sources = {source} if source else {}
-        return ret
-
-    @staticmethod
-    def annotate_keys_with_source(data, source):
-        if isinstance(data, dict):
-            return {
-                Key(k, source=source): Key.annotate_keys_with_source(v, source)
-                for k, v in data.items()
-            }
-        elif isinstance(data, (tuple, list)):
-            return [Key.annotate_keys_with_source(k, source) for k in data]
-        else:
-            return data
-
-    @staticmethod
-    def get_sources(data):
-        if isinstance(data, Key):
-            return data.sources
-        return []
-
-
-def key_representer(dumper, data):
-    return dumper.represent_str(str(data))
-
-
-yaml.add_representer(Key, key_representer)
-yaml.add_multi_representer(Key, key_representer)
-SafeDumper.add_representer(Key, key_representer)
-SafeDumper.add_multi_representer(Key, key_representer)
+from .validation import validate_model
 
 
 class ModelSchema:
     USE_KEYWORD = "use"
     REF_KEYWORD = "$ref"
 
     def __init__(
         self,
         file_path,
         content=None,
         included_models: Dict[str, Callable] = None,
         merged_models: List[Union[str, Path]] = None,
         loaders=None,
-        model_field="model",
+        validate=True,
+        source_locations=None,
     ):
         """
         Creates and parses model schema
 
         :param file_paths: list of paths on the filesystem to the model schema files. The content of these files will be merged before the processing.
         :param content:   if set, use this content, otherwise load the file_path
         :param included_models: a dictionary of file_id to callable that returns included json.
                 The callable expects a single parameter, an instance of this schema
         """
 
         self.file_path = file_path
         self.included_schemas = included_models or {}
         self.loaders = loaders
+        self.source_locations = [*(source_locations or [])]
+        self.source_locations.append(os.path.abspath(os.curdir))
+        self.source_locations.append(os.path.dirname(os.path.abspath(self.file_path)))
 
         if content is not None:
             self.schema = content
         else:
             self.schema = copy.deepcopy(self._load(file_path))
             for fp in merged_models or []:
                 self.schema = deepmerge(self.schema, copy.deepcopy(self._load(fp)))
@@ -85,53 +52,23 @@
 
         self._resolve_shortcuts(self.schema)
 
         # any star keys should be kept
         use_star_keys(self.schema)
 
         self.schema.setdefault("settings", {})
-        self.schema = munch.munchify(self.schema, factory=HyphenMunch)
-
-        self.model_field = model_field
 
-    def debug_print(self):
-        def _print(data, prefix):
-            if isinstance(data, dict):
-                print()
-                for k, v in sorted(data.items()):
-                    print(f"{prefix}{k}{Key.get_sources(k)}:", end="")
-                    _print(v, prefix + "  ")
-            elif isinstance(data, (list, tuple)):
-                print()
-                for v in sorted(data):
-                    _print(v, prefix + "-  ")
-            else:
-                print(f"{prefix}{data}")
-
-        _print(self.schema, "")
-        print()
-
-    def get(self, key):
-        return self.schema.get(key, None)
+        self._sections = {}
 
-    def set(self, key, value):
-        self.schema[key] = value
+        if validate:
+            validate_model(self)
 
     @property
     def settings(self):
-        return self.schema.settings
-
-    @property
-    def current_model(self):
-        return self.schema.get(self.model_field, {})
-
-    def merge(self, another):
-        self.schema = munch.munchify(
-            deepmerge(another, self.schema, []), factory=HyphenMunch
-        )
+        return self.schema.get("settings", {})
 
     def _load(self, file_path, content=None):
         """
         Loads a json/json5 file on the path
 
         :param file_path: file path on filesystem
         :return: parsed json
@@ -142,15 +79,15 @@
             extension = pathlib.Path(file_path).suffix.lower()[1:]
             if extension not in self.loaders:
                 raise RuntimeError(
                     f"Can not load {file_path} - no loader has been found for extension {extension} "
                     f"in entry point group oarepo_model_builder.loaders"
                 )
             loaded = self.loaders[extension](file_path, self, content=content)
-        return Key.annotate_keys_with_source(loaded, file_path)
+        return loaded
 
     def _fetch_included(self, file_path):
         included = self.included_schemas[file_path]
         if callable(included):
             return included(self)
         extension = pathlib.Path(included).suffix.lower()[1:]
         if extension not in self.loaders:
@@ -184,33 +121,38 @@
                 ret = self._load(file_path)
             else:
                 if file_id not in self.included_schemas:
                     raise IncludedFileNotFoundException(
                         f"Included file {file_id} not found in includes"
                     )
 
-                ret = self.included_schemas[file_id](self)
+                ret = self._fetch_included(file_id)
 
         if json_pointer_or_id:
             if json_pointer_or_id.startswith("/"):
                 ret = resolve_pointer(ret, json_pointer_or_id)
             else:
                 ret = resolve_id(ret, json_pointer_or_id)
                 if not ret:
                     raise IncludedFileNotFoundException(
                         f"Element with id {json_pointer_or_id} not found in {file_id}"
                     )
 
         ret = copy.deepcopy(ret)
+        if ret is None:
+            ret = {}
         ret.pop("$id", None)
         return ret
 
     def _resolve_file_path(self, file_id, source_locations):
+        if file_id in self.included_schemas:
+            return file_id
+        source_locations = [*(source_locations or []), *self.source_locations]
         for location in source_locations:
-            pth = Path(location).parent / file_id
+            pth = Path(location) / file_id
             if pth.exists():
                 return pth
         pth = self.abs_path.parent / file_id
         if pth.exists():
             return pth
         return None
 
@@ -224,16 +166,14 @@
 
     def _resolve_references(self, element, stack):
         if isinstance(element, dict):
             if self.USE_KEYWORD in element or self.REF_KEYWORD in element:
                 for key in element:
                     if key in (self.USE_KEYWORD, self.REF_KEYWORD):
                         break
-                else:
-                    raise  # just for making pycharm happy
                 included_name = element[key]
 
                 # if it is a dictionary, then probably it is a name of a property,
                 # so keep it
                 if isinstance(included_name, dict):
                     return self._resolve_references(element, stack)
 
@@ -243,29 +183,60 @@
                 if not isinstance(included_name, list):
                     included_name = [included_name]
                 for name in included_name:
                     if not name:
                         raise IncludedFileNotFoundException(
                             f"No file for use at path {'/'.join(stack)}"
                         )
-                    included_data = self._load_included_file(
-                        name, source_locations=Key.get_sources(key)
-                    )
+                    included_data = self._load_included_file(name)
                     deepmerge(element, included_data, [], listmerge="keep")
                 return self._resolve_references(element, stack)
             for k, v in element.items():
                 self._resolve_references(v, stack + [k])
         elif isinstance(element, list):
             for v in element:
                 self._resolve_references(v, stack)
 
     @property
     def abs_path(self):
         return Path(self.file_path).absolute()
 
+    def get_schema_section(self, profile, section, prepare_context=None):
+        if not isinstance(section, (tuple, list)):
+            section = (section,)
+        section = tuple(section)
+        key = (profile, section)
+        if key in self._sections:
+            return self._sections[key]
+        from oarepo_model_builder.datatypes import datatypes
+
+        data = self.schema
+        for p in section:
+            if p in data:
+                data = data[p]
+            else:
+                data = {}
+                break
+        if "type" not in data:
+            data["type"] = "model"
+        parsed_section = datatypes.get_datatype(
+            parent=None,
+            data=data,
+            key=None,
+            model=data,
+            schema=self,
+        )
+        prepare_context = prepare_context or {}
+        prepare_context.setdefault("profile", profile)
+        prepare_context.setdefault("profile_module", profile + "s")
+        prepare_context.setdefault("profile_upper", profile.upper())
+        parsed_section.prepare(prepare_context)
+        self._sections[key] = parsed_section
+        return parsed_section
+
 
 def resolve_id(json, element_id):
     if isinstance(json, dict):
         if "$id" in json and json["$id"] == element_id:
             return json
         continue_with = json.values()
     elif isinstance(json, (tuple, list)):
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/templates/__init__.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/templates/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,19 +14,17 @@
             )
         ):
             loaded_package = ep.load()
             base_path = Path(loaded_package.__file__).parent.absolute()
             for k, v in loaded_package.TEMPLATES.items():
                 self.mapping[k] = base_path.joinpath(v)
 
-    def get_template(self, template_key, settings):
+    def get_template(self, template_key, settings):  # NOSONAR
         # try to get the template key from settings
-        path = settings.python.templates.get(
-            template_key, self.mapping.get(template_key, None)
-        )
+        path = self.mapping.get(template_key, None)
         if not path:
             raise AttributeError(f"Template with key {template_key} has not been found")
         if isinstance(path, str):
             path = Path(path).absolute()
         if path.exists():
             with path.open() as f:
                 return f.read()
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/utils/cst/call.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/utils/cst/call.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import itertools
 
 from libcst import Arg
 
-from .common import IdentityMerger, MergerBase, PythonContext, merge
-from .mergers import call_mergers, expression_mergers
+from .common import IdentityMerger, MergerBase, PythonContext
+from .mergers import expression_mergers
 
 
 class CallMerger(MergerBase):
     def identity(self, context: PythonContext, node):
         return node.func
 
     def merge_internal(self, context: PythonContext, existing_node, new_node):
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/utils/cst/collections.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/utils/cst/collections.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 class DictMerger(MergerBase):
     def identity(self, context: PythonContext, node):
         return node
 
     def get_key(self, context, el):
         if hasattr(el, "key") and el.key:
             return el.key.value
-        # TODO: StarredDictElement might contain trailing comma, should remove it
         return context.to_source_code(el)
 
     def merge_internal(self, context: PythonContext, existing_node, new_node):
         ret = []
         mergers = expression_mergers
         existing_elements = {
             self.get_key(context, el): el for el in existing_node.elements
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/utils/cst/common.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/utils/cst/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import namedtuple
 from dataclasses import dataclass, field
 from enum import Enum
 from logging import getLogger
-from typing import Callable, List, Set, Union
+from typing import List, Set, Union
 
 from libcst import Arg, CSTNode, Element, Module
 
 from .mergers import module_mergers
 
 logger = getLogger("oarepo_model_builder.cst")
 
@@ -23,15 +23,15 @@
     KEEP_MERGED = 3
     REMOVE = 4
     NEW_AS_TODO = 5
 
 
 class ConflictResolver:
     def resolve_conflict(
-        self, context, existing_node, new_node, merged_node
+        self, context, existing_node, new_node, merged_node  # NOSONAR
     ) -> ConflictResolution:
         return ConflictResolution.KEEP_PREVIOUS
 
 
 @dataclass
 class PythonContextItem:
     existing_node: CSTNode
@@ -39,15 +39,14 @@
     operations: Set[OperationPerformed] = field(default_factory=set, init=False)
     new_as_comment: bool = field(default=False, init=False)
 
 
 @dataclass
 class PythonContext:
     cst: Module
-    conflict_resolver: ConflictResolver = None
     stack: List[PythonContextItem] = field(default_factory=list, init=False)
 
     REMOVED = object()
 
     def to_source_code(self, node):
         if not node:
             return ""
@@ -67,27 +66,25 @@
 
     def decide(
         self,
         existing_node: Union[CSTNode, None],
         new_node: Union[CSTNode, None],
         merged_node: Union[CSTNode, None],
     ) -> Union[CSTNode, object]:
-
         logger.debug(
             "\nDecide called with operations %s on node %s %s",
             self.top.operations,
             type(existing_node or new_node).__name__,
             id(existing_node),
         )
         logger.debug("Existing: %s", self.to_source_code(existing_node))
         logger.debug("New     : %s", self.to_source_code(new_node))
         logger.debug("Merged  : %s", self.to_source_code(merged_node))
 
         top = self.top
-        decider_called = False
         decision = None
         if existing_node is self.top.existing_node:
             # processing existing node. If there was any decision in children, do not decide here
             if top.operations:
                 decision = ConflictResolution.KEEP_MERGED
             if len(self.stack) > 1:
                 top = self.stack[-2]
@@ -95,38 +92,27 @@
             decision = ConflictResolution.KEEP_PREVIOUS
         if decision is None:
             if existing_node:
                 decision = ConflictResolution.KEEP_PREVIOUS
             else:
                 decision = ConflictResolution.KEEP_NEW
 
-            if self.conflict_resolver:
-                decision = self.conflict_resolver.resolve_conflict(
-                    self, existing_node, new_node, merged_node
-                )
-            decider_called = True
-
-        logger.debug(
-            "---> %s %s",
-            "<decider returned>" if decider_called else "<automatic>",
-            decision,
-        )
         logger.debug("")
         if decision == ConflictResolution.KEEP_PREVIOUS:
             return existing_node
         elif decision == ConflictResolution.KEEP_NEW:
             top.operations.add(OperationPerformed.ADD)
             return new_node
         elif decision == ConflictResolution.KEEP_MERGED:
             top.operations.add(OperationPerformed.CHANGE)
             return merged_node
         elif decision == ConflictResolution.REMOVE:
             top.operations.add(OperationPerformed.REMOVAL)
             return self.REMOVED
-        elif decision == ConflictResolution.NEW_AS_TODO:
+        elif decision == ConflictResolution.NEW_AS_TODO:  # NOSONAR
             top.new_as_comment = True
             return existing_node
         raise RuntimeError("Unknown decision")
 
 
 node_with_type = namedtuple("node_with_type", "node, type")
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/utils/cst/indented_nodes.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/utils/cst/indented_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,22 +39,21 @@
                     new_merger = mergers.get(type(new_node), IdentityMerger())
                     ret.append(new_merger.merge(context, None, new_node))
             last_type = existing.type
             found = False
             for idx, new in enumerate(new_list):
                 if new.type != existing.type:
                     break
-                if isinstance(existing.node, type(new.node)):
-                    if merger.identity(context, existing.node).deep_equals(
-                        merger.identity(context, new.node)
-                    ):
-                        ret.append(merger.merge(context, existing.node, new.node))
-                        del new_list[idx]
-                        found = True
-                        break
+                if isinstance(existing.node, type(new.node)) and merger.identity(
+                    context, existing.node
+                ).deep_equals(merger.identity(context, new.node)):
+                    ret.append(merger.merge(context, existing.node, new.node))
+                    del new_list[idx]
+                    found = True
+                    break
             if not found:
                 ret.append(merger.merge(context, existing.node, None))
 
         for node in new_list:
             merger = mergers.get(type(node.node), IdentityMerger())
             ret.append(merger.merge(context, None, node.node))
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/utils/cst/mergers.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/utils/cst/mergers.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/utils/cst/simple_nodes.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/utils/cst/simple_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from libcst import Assign, Integer, Name
+from libcst import Assign, Integer
 
 from .common import IdentityBaseMerger, IdentityMerger, MergerBase, PythonContext
 from .mergers import expression_mergers, simple_line_mergers
 
 log = logging.getLogger("oarepo_model_builder.cst")
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/utils/deepmerge.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/utils/deepmerge.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/utils/verbose.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/utils/verbose.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder/validation/__init__.py` & `oarepo-model-builder-4.0.0/oarepo_model_builder/validation/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-import json
-
 from marshmallow import ValidationError
-from munch import unmunchify
 
-from oarepo_model_builder.utils.hyphen_munch import HyphenMunch, munch
 from oarepo_model_builder.validation.model_validation import model_validator
 
 
 class InvalidModelException(Exception):
     pass
 
 
@@ -20,20 +16,16 @@
             subpath = f"{path}.{k}" if path else k
             yield from flatten_errors(v, subpath)
     else:
         yield str(err_data), path
 
 
 def validate_model(model):
-    # remove munch, keeping stuff like Path etc.
-    data = unmunchify(model.schema)
-    validator = model_validator.validator_class("root")()
     try:
-        loaded_data = validator.dump(validator.load(data))
-        model.schema = munch.munchify(loaded_data, HyphenMunch)
+        model.schema = model_validator.validate(model.schema)
         return True
     except ValidationError as e:
         msg = []
         for err, path in flatten_errors(e.messages_dict, ""):
             if path.endswith("._schema") and err == "Unknown field.":
                 continue
             msg.append(f"{path}: {err}")
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder.egg-info/PKG-INFO` & `oarepo-model-builder-4.0.0/oarepo_model_builder.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder
-Version: 3.2.9
+Version: 4.0.0
 Summary: A utility library that generates OARepo required data model files from a JSON specification file
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo model builder
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder.egg-info/SOURCES.txt` & `oarepo-model-builder-4.0.0/oarepo_model_builder.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 oarepo_model_builder/__init__.py
 oarepo_model_builder/builder.py
 oarepo_model_builder/cli.py
-oarepo_model_builder/conflict_resolvers.py
 oarepo_model_builder/entrypoints.py
 oarepo_model_builder/exceptions.py
 oarepo_model_builder/fs.py
+oarepo_model_builder/generate_doc.py
 oarepo_model_builder/merger.py
 oarepo_model_builder/schema.py
 oarepo_model_builder.egg-info/PKG-INFO
 oarepo_model_builder.egg-info/SOURCES.txt
 oarepo_model_builder.egg-info/dependency_links.txt
 oarepo_model_builder.egg-info/entry_points.txt
 oarepo_model_builder.egg-info/requires.txt
@@ -26,152 +26,182 @@
 oarepo_model_builder/builders/model_saver.py
 oarepo_model_builder/builders/pyproject_toml.py
 oarepo_model_builder/builders/python.py
 oarepo_model_builder/builders/python_structure.py
 oarepo_model_builder/builders/setup_cfg.py
 oarepo_model_builder/builders/setup_py.py
 oarepo_model_builder/builders/utils.py
+oarepo_model_builder/builders/templates/__init__.py
 oarepo_model_builder/builders/templates/setup.py.jinja2
 oarepo_model_builder/builtin_models/__init__.py
 oarepo_model_builder/builtin_models/invenio.json
 oarepo_model_builder/datatypes/__init__.py
-oarepo_model_builder/datatypes/containers.py
 oarepo_model_builder/datatypes/datatypes.py
 oarepo_model_builder/datatypes/dates.py
+oarepo_model_builder/datatypes/model.py
 oarepo_model_builder/datatypes/primitive_types.py
 oarepo_model_builder/datatypes/strings.py
+oarepo_model_builder/datatypes/components/__init__.py
+oarepo_model_builder/datatypes/components/enum.py
+oarepo_model_builder/datatypes/components/facets.py
+oarepo_model_builder/datatypes/components/sample.py
+oarepo_model_builder/datatypes/components/ui.py
+oarepo_model_builder/datatypes/components/marshmallow/__init__.py
+oarepo_model_builder/datatypes/components/marshmallow/array.py
+oarepo_model_builder/datatypes/components/marshmallow/field.py
+oarepo_model_builder/datatypes/components/marshmallow/graph.py
+oarepo_model_builder/datatypes/components/marshmallow/object.py
+oarepo_model_builder/datatypes/components/marshmallow/ui_array.py
+oarepo_model_builder/datatypes/components/marshmallow/ui_field.py
+oarepo_model_builder/datatypes/components/marshmallow/ui_object.py
+oarepo_model_builder/datatypes/components/model/__init__.py
+oarepo_model_builder/datatypes/components/model/app.py
+oarepo_model_builder/datatypes/components/model/blueprints.py
+oarepo_model_builder/datatypes/components/model/defaults.py
+oarepo_model_builder/datatypes/components/model/facets.py
+oarepo_model_builder/datatypes/components/model/jsonschema.py
+oarepo_model_builder/datatypes/components/model/mapping.py
+oarepo_model_builder/datatypes/components/model/marshmallow.py
+oarepo_model_builder/datatypes/components/model/model_saver.py
+oarepo_model_builder/datatypes/components/model/permissions.py
+oarepo_model_builder/datatypes/components/model/pid.py
+oarepo_model_builder/datatypes/components/model/plugins.py
+oarepo_model_builder/datatypes/components/model/proxy.py
+oarepo_model_builder/datatypes/components/model/record.py
+oarepo_model_builder/datatypes/components/model/record_dumper.py
+oarepo_model_builder/datatypes/components/model/record_metadata.py
+oarepo_model_builder/datatypes/components/model/resource.py
+oarepo_model_builder/datatypes/components/model/sample.py
+oarepo_model_builder/datatypes/components/model/service.py
+oarepo_model_builder/datatypes/components/model/ui.py
+oarepo_model_builder/datatypes/components/model/ui_marshmallow.py
+oarepo_model_builder/datatypes/components/model/utils.py
+oarepo_model_builder/datatypes/containers/__init__.py
+oarepo_model_builder/datatypes/containers/array.py
+oarepo_model_builder/datatypes/containers/flatten.py
+oarepo_model_builder/datatypes/containers/nested.py
+oarepo_model_builder/datatypes/containers/object.py
 oarepo_model_builder/invenio/__init__.py
+oarepo_model_builder/invenio/invenio_api_views.py
+oarepo_model_builder/invenio/invenio_app_views.py
 oarepo_model_builder/invenio/invenio_base.py
-oarepo_model_builder/invenio/invenio_cli.py
-oarepo_model_builder/invenio/invenio_cli_setup_cfg.py
 oarepo_model_builder/invenio/invenio_config.py
 oarepo_model_builder/invenio/invenio_ext.py
 oarepo_model_builder/invenio/invenio_ext_setup_cfg.py
 oarepo_model_builder/invenio/invenio_proxies.py
 oarepo_model_builder/invenio/invenio_record.py
 oarepo_model_builder/invenio/invenio_record_dumper.py
 oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py
+oarepo_model_builder/invenio/invenio_record_marshmallow.py
 oarepo_model_builder/invenio/invenio_record_metadata.py
 oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py
 oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py
 oarepo_model_builder/invenio/invenio_record_permissions.py
+oarepo_model_builder/invenio/invenio_record_pid_provider.py
 oarepo_model_builder/invenio/invenio_record_resource.py
 oarepo_model_builder/invenio/invenio_record_resource_config.py
 oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py
-oarepo_model_builder/invenio/invenio_record_schema.py
 oarepo_model_builder/invenio/invenio_record_search.py
 oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py
 oarepo_model_builder/invenio/invenio_record_service.py
 oarepo_model_builder/invenio/invenio_record_service_config.py
+oarepo_model_builder/invenio/invenio_record_ui_marshmallow.py
+oarepo_model_builder/invenio/invenio_record_ui_serializer.py
 oarepo_model_builder/invenio/invenio_script_sample_data.py
 oarepo_model_builder/invenio/invenio_version.py
-oarepo_model_builder/invenio/invenio_views.py
+oarepo_model_builder/invenio/templates/__init__.py
+oarepo_model_builder/invenio/templates/api_views.py.jinja2
+oarepo_model_builder/invenio/templates/app_views.py.jinja2
+oarepo_model_builder/invenio/templates/config.py.jinja2
+oarepo_model_builder/invenio/templates/ext.py.jinja2
 oarepo_model_builder/invenio/templates/imports.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_cli.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_config.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_ext.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_proxies.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_record.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_record_dumper.py.jinja2
 oarepo_model_builder/invenio/templates/invenio_record_facets.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_record_metadata.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_record_permissions.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_record_resource.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_record_resource_config.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_record_schema.py.jinja2
 oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_record_service.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_record_service_config.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_version.py.jinja2
-oarepo_model_builder/invenio/templates/invenio_views.py.jinja2
-oarepo_model_builder/invenio/templates/script_import_sample_data.py.jinja2
-oarepo_model_builder/invenio/templates/script_import_sample_data.sh.jinja2
+oarepo_model_builder/invenio/templates/marshmallow.py.jinja2
+oarepo_model_builder/invenio/templates/permissions.py.jinja2
+oarepo_model_builder/invenio/templates/pid_provider.py.jinja2
+oarepo_model_builder/invenio/templates/proxies.py.jinja2
+oarepo_model_builder/invenio/templates/record.py.jinja2
+oarepo_model_builder/invenio/templates/record_dumper.py.jinja2
+oarepo_model_builder/invenio/templates/record_metadata.py.jinja2
+oarepo_model_builder/invenio/templates/resource.py.jinja2
+oarepo_model_builder/invenio/templates/resource_config.py.jinja2
+oarepo_model_builder/invenio/templates/service.py.jinja2
+oarepo_model_builder/invenio/templates/service_config.py.jinja2
+oarepo_model_builder/invenio/templates/ui_serializer.py.jinja2
+oarepo_model_builder/invenio/templates/version.py.jinja2
 oarepo_model_builder/loaders/__init__.py
-oarepo_model_builder/model_preprocessors/__init__.py
-oarepo_model_builder/model_preprocessors/default_values.py
-oarepo_model_builder/model_preprocessors/extend.py
-oarepo_model_builder/model_preprocessors/invenio.py
-oarepo_model_builder/model_preprocessors/invenio_base_classes.py
-oarepo_model_builder/model_preprocessors/opensearch.py
 oarepo_model_builder/outputs/__init__.py
 oarepo_model_builder/outputs/cfg.py
 oarepo_model_builder/outputs/diff.py
 oarepo_model_builder/outputs/json.py
 oarepo_model_builder/outputs/json_stack.py
 oarepo_model_builder/outputs/jsonschema.py
 oarepo_model_builder/outputs/mapping.py
 oarepo_model_builder/outputs/python.py
 oarepo_model_builder/outputs/text.py
 oarepo_model_builder/outputs/toml.py
 oarepo_model_builder/outputs/yaml.py
 oarepo_model_builder/profiles/__init__.py
 oarepo_model_builder/profiles/extend.py
-oarepo_model_builder/profiles/model.py
-oarepo_model_builder/property_preprocessors/__init__.py
-oarepo_model_builder/property_preprocessors/datatype_preprocessor.py
-oarepo_model_builder/property_preprocessors/enum.py
-oarepo_model_builder/property_preprocessors/extend.py
-oarepo_model_builder/stack/__init__.py
-oarepo_model_builder/stack/schema.py
-oarepo_model_builder/stack/stack.py
+oarepo_model_builder/profiles/record.py
+oarepo_model_builder/settings/__init__.py
+oarepo_model_builder/settings/opensearch.json
+oarepo_model_builder/settings/python.json
 oarepo_model_builder/templates/__init__.py
 oarepo_model_builder/utils/__init__.py
+oarepo_model_builder/utils/absolute_class.py
 oarepo_model_builder/utils/camelcase.py
 oarepo_model_builder/utils/deepmerge.py
+oarepo_model_builder/utils/dict.py
 oarepo_model_builder/utils/facet_helpers.py
-oarepo_model_builder/utils/hyphen_munch.py
+oarepo_model_builder/utils/import_class.py
 oarepo_model_builder/utils/jinja.py
-oarepo_model_builder/utils/json_pathlib.py
+oarepo_model_builder/utils/properties.py
 oarepo_model_builder/utils/python_name.py
 oarepo_model_builder/utils/verbose.py
 oarepo_model_builder/utils/cst/__init__.py
 oarepo_model_builder/utils/cst/call.py
 oarepo_model_builder/utils/cst/collections.py
 oarepo_model_builder/utils/cst/common.py
 oarepo_model_builder/utils/cst/indented_nodes.py
 oarepo_model_builder/utils/cst/mergers.py
 oarepo_model_builder/utils/cst/simple_nodes.py
 oarepo_model_builder/validation/__init__.py
-oarepo_model_builder/validation/model.py
-oarepo_model_builder/validation/model_defaults.py
-oarepo_model_builder/validation/model_plugins.py
+oarepo_model_builder/validation/extensibility.py
 oarepo_model_builder/validation/model_validation.py
-oarepo_model_builder/validation/properties.py
-oarepo_model_builder/validation/property.py
-oarepo_model_builder/validation/property_facets.py
-oarepo_model_builder/validation/property_jsonschema.py
-oarepo_model_builder/validation/property_mapping.py
-oarepo_model_builder/validation/property_marshmallow.py
-oarepo_model_builder/validation/property_sample_data.py
-oarepo_model_builder/validation/property_sortable.py
-oarepo_model_builder/validation/registration.py
-oarepo_model_builder/validation/root.py
-oarepo_model_builder/validation/settings.py
 oarepo_model_builder/validation/utils.py
+tests/__init__.py
+tests/conftest.py
+tests/faker_constant.py
+tests/multilang.py
 tests/test_builder.py
 tests/test_builder_from_entrypoints.py
+tests/test_cfg_builders.py
+tests/test_datatype_prepare.py
+tests/test_datatype_validator.py
 tests/test_dependencies.py
 tests/test_empty_metadata.py
+tests/test_extend.py
 tests/test_facets.py
 tests/test_fulltext_keyword.py
-tests/test_is_schema_element.py
-tests/test_json_pathlib.py
-tests/test_json_stack.py
 tests/test_jsonchema_builder.py
-tests/test_jsonschema_output.py
 tests/test_loading.py
 tests/test_mapping_builder.py
 tests/test_marshmallow_builder.py
+tests/test_marshmallow_ui_builder.py
 tests/test_merge.py
 tests/test_model_saver.py
 tests/test_overwrite.py
+tests/test_pid_provider.py
 tests/test_plugin_configuration.py
 tests/test_python_mergers.py
 tests/test_raw.py
 tests/test_sample_builder.py
 tests/test_schema_props.py
 tests/test_search_options.py
 tests/test_shortcuts.py
-tests/test_stack.py
+tests/test_simple_builders.py
 tests/test_template_registry.py
 tests/test_type_shortcuts.py
-tests/test_validation.py
+tests/test_validation.py
+tests/utils.py
```

### Comparing `oarepo-model-builder-3.2.9/oarepo_model_builder.egg-info/entry_points.txt` & `oarepo-model-builder-4.0.0/oarepo_model_builder.egg-info/entry_points.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,88 +22,80 @@
 
 [oarepo.models]
 invenio = oarepo_model_builder.builtin_models:invenio.json
 
 [oarepo_model_builder.builders.extend]
 1000-model = oarepo_model_builder.builders.extend:ExtendBuilder
 
-[oarepo_model_builder.builders.model]
+[oarepo_model_builder.builders.record]
 0020-jsonschema = oarepo_model_builder.builders.jsonschema:JSONSchemaBuilder
 0030-mapping = oarepo_model_builder.builders.mapping:MappingBuilder
 0050-setup-cfg = oarepo_model_builder.builders.setup_cfg:SetupCfgBuilder
 0060-setup-py = oarepo_model_builder.builders.setup_py:SetupPyBuilder
 0070-pyproject-toml = oarepo_model_builder.builders.pyproject_toml:PyprojectTOMLBuilder
 0100-python_structure = oarepo_model_builder.builders.python_structure:PythonStructureBuilder
+0105-invenio_record_pid_provider = oarepo_model_builder.invenio.invenio_record_pid_provider:InvenioRecordPIDProviderBuilder
 0110-invenio_record = oarepo_model_builder.invenio.invenio_record:InvenioRecordBuilder
 0120-invenio_record_metadata = oarepo_model_builder.invenio.invenio_record_metadata:InvenioRecordMetadataBuilder
-0130-invenio_record_schema = oarepo_model_builder.invenio.invenio_record_schema:InvenioRecordSchemaBuilder
+0130-invenio_record_marshmallow = oarepo_model_builder.invenio.invenio_record_marshmallow:InvenioRecordMarshmallowBuilder
+0140-invenio_record_ui_marshmallow = oarepo_model_builder.invenio.invenio_record_ui_marshmallow:InvenioRecordUIMarshmallowBuilder
 0200-invenio_record_permissions = oarepo_model_builder.invenio.invenio_record_permissions:InvenioRecordPermissionsBuilder
 0300-invenio_record_search_options = oarepo_model_builder.invenio.invenio_record_search:InvenioRecordSearchOptionsBuilder
 0310-invenio_record_service_config = oarepo_model_builder.invenio.invenio_record_service_config:InvenioRecordServiceConfigBuilder
 0320-invenio_record_service = oarepo_model_builder.invenio.invenio_record_service:InvenioRecordServiceBuilder
 0340-invenio_record_dumper = oarepo_model_builder.invenio.invenio_record_dumper:InvenioRecordDumperBuilder
 0400-invenio_record_resource_config = oarepo_model_builder.invenio.invenio_record_resource_config:InvenioRecordResourceConfigBuilder
 0410-invenio_record_resource = oarepo_model_builder.invenio.invenio_record_resource:InvenioRecordResourceBuilder
-0420-invenio_views = oarepo_model_builder.invenio.invenio_views:InvenioViewsBuilder
+0420-invenio_api_views = oarepo_model_builder.invenio.invenio_api_views:InvenioAPIViewsBuilder
+0421-invenio_app_views = oarepo_model_builder.invenio.invenio_app_views:InvenioAPPViewsBuilder
+0430-ui_serializer = oarepo_model_builder.invenio.invenio_record_ui_serializer:InvenioRecordUISerializerBuilder
 0500-invenio_config = oarepo_model_builder.invenio.invenio_config:InvenioConfigBuilder
 0600-invenio_ext = oarepo_model_builder.invenio.invenio_ext:InvenioExtBuilder
 0610-invenio_ext_setup_cfg = oarepo_model_builder.invenio.invenio_ext_setup_cfg:InvenioExtSetupCfgBuilder
 0700-invenio_ext = oarepo_model_builder.invenio.invenio_proxies:InvenioProxiesBuilder
 0910-invenio_record_metadata_alembic_setup_cfg = oarepo_model_builder.invenio.invenio_record_metadata_alembic_setup_cfg:InvenioRecordMetadataAlembicSetupCfgBuilder
 0920-invenio_record_metadata_models_setup_cfg = oarepo_model_builder.invenio.invenio_record_metadata_models_setup_cfg:InvenioRecordMetadataModelsSetupCfgBuilder
 0930-invenio_resource_setup_cfg = oarepo_model_builder.invenio.invenio_record_resource_setup_cfg:InvenioRecordResourceSetupCfgBuilder
 0940-invenio_record_search_setup_cfg = oarepo_model_builder.invenio.invenio_record_search_setup_cfg:InvenioRecordSearchSetupCfgBuilder
 0950-invenio_record_jsonschemas_setup_cfg = oarepo_model_builder.invenio.invenio_record_jsonschemas_setup_cfg:InvenioRecordJSONSchemasSetupCfgBuilder
-1030-invenio_script_sample_data = oarepo_model_builder.invenio.invenio_script_sample_data:InvenioScriptSampleDataBuilder
+1030-invenio_script_sample_data = oarepo_model_builder.invenio.invenio_script_sample_data:SampleDataBuilder
 1050-invenio_version = oarepo_model_builder.invenio.invenio_version:InvenioVersionBuilder
 2000-model_saver = oarepo_model_builder.builders.model_saver:ModelSaverBuilder
 2010-model_registration = oarepo_model_builder.builders.model_saver:ModelRegistrationBuilder
-3000-cli = oarepo_model_builder.invenio.invenio_cli:InvenioCliBuilder
-3010-cli_setup = oarepo_model_builder.invenio.invenio_cli_setup_cfg:InvenioCliSetupCfgBuilder
 
 [oarepo_model_builder.datatypes]
 0100-default-datatypes = oarepo_model_builder.datatypes:DEFAULT_DATATYPES
 
+[oarepo_model_builder.datatypes.components]
+0100-default-datatypes = oarepo_model_builder.datatypes.components:DEFAULT_COMPONENTS
+
 [oarepo_model_builder.loaders]
 json = oarepo_model_builder.loaders:json_loader
 json5 = oarepo_model_builder.loaders:json_loader
 yaml = oarepo_model_builder.loaders:yaml_loader
 yml = oarepo_model_builder.loaders:yaml_loader
 
-[oarepo_model_builder.model_preprocessors.extend]
-1000-base-classes = oarepo_model_builder.model_preprocessors.extend:BaseClassesModelPreprocessor
-
-[oarepo_model_builder.model_preprocessors.model]
-01-default = oarepo_model_builder.model_preprocessors.default_values:DefaultValuesModelPreprocessor
-10-invenio = oarepo_model_builder.model_preprocessors.invenio:InvenioModelPreprocessor
-11-invenio = oarepo_model_builder.model_preprocessors.invenio_base_classes:InvenioBaseClassesModelPreprocessor
-20-opensearch = oarepo_model_builder.model_preprocessors.opensearch:OpensearchModelPreprocessor
-
 [oarepo_model_builder.outputs]
 cfg = oarepo_model_builder.outputs.cfg:CFGOutput
 diff = oarepo_model_builder.outputs.diff:DiffOutput
 json = oarepo_model_builder.outputs.json:JSONOutput
 jsonschema = oarepo_model_builder.outputs.jsonschema:JSONSchemaOutput
 mapping = oarepo_model_builder.outputs.mapping:MappingOutput
 python = oarepo_model_builder.outputs.python:PythonOutput
 text = oarepo_model_builder.outputs.text:TextOutput
 toml = oarepo_model_builder.outputs.toml:TOMLOutput
 yaml = oarepo_model_builder.outputs.yaml:YAMLOutput
 
 [oarepo_model_builder.profiles]
 extend = oarepo_model_builder.profiles.extend:ExtendProfile
-model = oarepo_model_builder.profiles.model:ModelProfile
+record = oarepo_model_builder.profiles.record:RecordProfile
 
-[oarepo_model_builder.property_preprocessors.extend]
-0100-type_shortcuts = oarepo_model_builder.property_preprocessors.type_shortcuts:TypeShortcutsPreprocessor
-1000-disable-marshmallow = oarepo_model_builder.property_preprocessors.extend:DisableMarshmallowPreprocessor
-
-[oarepo_model_builder.property_preprocessors.model]
-200-datatypes = oarepo_model_builder.property_preprocessors.datatype_preprocessor:DataTypePreprocessor
-300-enums = oarepo_model_builder.property_preprocessors.enum:EnumPreprocessor
+[oarepo_model_builder.settings]
+1000-python = oarepo_model_builder.settngs:python.json
+2000-opensearch = oarepo_model_builder.settngs:opensearch.json
 
 [oarepo_model_builder.templates]
 99-base_generic_templates = oarepo_model_builder.builders
 99-base_invenio_templates = oarepo_model_builder.invenio
 
 [oarepo_model_builder.validation]
 builtin-validation = oarepo_model_builder.validation.registration:validators
```

### Comparing `oarepo-model-builder-3.2.9/setup.cfg` & `oarepo-model-builder-4.0.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 [metadata]
 name = oarepo-model-builder
-version = 3.2.9
+version = 4.0.0
 description = A utility library that generates OARepo required data model files from a JSON specification file
 authors = Miroslav Bauer <bauer@cesnet.cz>, Miroslav Simek <simeki@vscht.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
 python = >=3.9
 install_requires = 
 	ConfigUpdater>=3.1.1,<4.0.0
 	Faker>11.3.0
 	Jinja2>=3.0.3,<4.0.0
 	PyYAML>=6.0,<7.0
-	black>21.11b1
+	black>23
 	click>=7.1
 	deepdiff>=5.6.0,<6.0.0
 	isort>=5.10.1,<6.0.0
 	json5>=0.9.6,<0.10.0
 	jsonpointer>=2.2,<3.0
 	lazy-object-proxy>=1.7.1,<2.0.0
 	libcst>=0.3.19
-	munch>=2.5.0,<3.0.0
 	tomlkit>=0.7.2
 	importlib_metadata>=4.0.0
 	marshmallow
 	marshmallow-union
 	marshmallow-oneofschema
+	autoflake
+	frozendict
+packages = find:
 
 [options.extras_require]
 devs = 
 	pytest>=7.1.2
+	black
+	isort
 tests = 
 	pytest>=7.1.2
 
 [options.package_data]
 * = *.json, *.rst, *.md, *.json5, *.jinja2
 
 [options.entry_points]
@@ -64,14 +68,16 @@
 oarepo_model_builder.loaders = 
 	json  = oarepo_model_builder.loaders:json_loader
 	json5  = oarepo_model_builder.loaders:json_loader
 	yaml  = oarepo_model_builder.loaders:yaml_loader
 	yml  = oarepo_model_builder.loaders:yaml_loader
 oarepo_model_builder.datatypes = 
 	0100-default-datatypes = oarepo_model_builder.datatypes:DEFAULT_DATATYPES
+oarepo_model_builder.datatypes.components = 
+	0100-default-datatypes = oarepo_model_builder.datatypes.components:DEFAULT_COMPONENTS
 oarepo.models = 
 	invenio  = oarepo_model_builder.builtin_models:invenio.json
 oarepo_model_builder.outputs = 
 	cfg  = oarepo_model_builder.outputs.cfg:CFGOutput
 	diff  = oarepo_model_builder.outputs.diff:DiffOutput
 	json  = oarepo_model_builder.outputs.json:JSONOutput
 	jsonschema  = oarepo_model_builder.outputs.jsonschema:JSONSchemaOutput
@@ -80,64 +86,56 @@
 	text  = oarepo_model_builder.outputs.text:TextOutput
 	toml  = oarepo_model_builder.outputs.toml:TOMLOutput
 	yaml  = oarepo_model_builder.outputs.yaml:YAMLOutput
 oarepo_model_builder.templates = 
 	99-base_generic_templates  = oarepo_model_builder.builders
 	99-base_invenio_templates  = oarepo_model_builder.invenio
 oarepo_model_builder.profiles = 
-	model = oarepo_model_builder.profiles.model:ModelProfile
+	record = oarepo_model_builder.profiles.record:RecordProfile
 	extend = oarepo_model_builder.profiles.extend:ExtendProfile
-oarepo_model_builder.builders.model = 
+oarepo_model_builder.builders.record = 
 	0020-jsonschema  = oarepo_model_builder.builders.jsonschema:JSONSchemaBuilder
 	0030-mapping  = oarepo_model_builder.builders.mapping:MappingBuilder
 	0050-setup-cfg  = oarepo_model_builder.builders.setup_cfg:SetupCfgBuilder
 	0060-setup-py  = oarepo_model_builder.builders.setup_py:SetupPyBuilder
 	0070-pyproject-toml  = oarepo_model_builder.builders.pyproject_toml:PyprojectTOMLBuilder
 	0100-python_structure  = oarepo_model_builder.builders.python_structure:PythonStructureBuilder
+	0105-invenio_record_pid_provider = oarepo_model_builder.invenio.invenio_record_pid_provider:InvenioRecordPIDProviderBuilder
 	0110-invenio_record  = oarepo_model_builder.invenio.invenio_record:InvenioRecordBuilder
 	0120-invenio_record_metadata  = oarepo_model_builder.invenio.invenio_record_metadata:InvenioRecordMetadataBuilder
-	0130-invenio_record_schema  = oarepo_model_builder.invenio.invenio_record_schema:InvenioRecordSchemaBuilder
+	0130-invenio_record_marshmallow  = oarepo_model_builder.invenio.invenio_record_marshmallow:InvenioRecordMarshmallowBuilder
+	0140-invenio_record_ui_marshmallow  = oarepo_model_builder.invenio.invenio_record_ui_marshmallow:InvenioRecordUIMarshmallowBuilder
 	0200-invenio_record_permissions  = oarepo_model_builder.invenio.invenio_record_permissions:InvenioRecordPermissionsBuilder
 	0300-invenio_record_search_options  = oarepo_model_builder.invenio.invenio_record_search:InvenioRecordSearchOptionsBuilder
 	0310-invenio_record_service_config  = oarepo_model_builder.invenio.invenio_record_service_config:InvenioRecordServiceConfigBuilder
 	0320-invenio_record_service  = oarepo_model_builder.invenio.invenio_record_service:InvenioRecordServiceBuilder
 	0340-invenio_record_dumper  = oarepo_model_builder.invenio.invenio_record_dumper:InvenioRecordDumperBuilder
 	0400-invenio_record_resource_config  = oarepo_model_builder.invenio.invenio_record_resource_config:InvenioRecordResourceConfigBuilder
 	0410-invenio_record_resource  = oarepo_model_builder.invenio.invenio_record_resource:InvenioRecordResourceBuilder
-	0420-invenio_views  = oarepo_model_builder.invenio.invenio_views:InvenioViewsBuilder
+	0420-invenio_api_views  = oarepo_model_builder.invenio.invenio_api_views:InvenioAPIViewsBuilder
+	0421-invenio_app_views  = oarepo_model_builder.invenio.invenio_app_views:InvenioAPPViewsBuilder
+	0430-ui_serializer  = oarepo_model_builder.invenio.invenio_record_ui_serializer:InvenioRecordUISerializerBuilder
 	0500-invenio_config  = oarepo_model_builder.invenio.invenio_config:InvenioConfigBuilder
 	0600-invenio_ext  = oarepo_model_builder.invenio.invenio_ext:InvenioExtBuilder
 	0610-invenio_ext_setup_cfg  = oarepo_model_builder.invenio.invenio_ext_setup_cfg:InvenioExtSetupCfgBuilder
 	0700-invenio_ext  = oarepo_model_builder.invenio.invenio_proxies:InvenioProxiesBuilder
 	0910-invenio_record_metadata_alembic_setup_cfg = oarepo_model_builder.invenio.invenio_record_metadata_alembic_setup_cfg:InvenioRecordMetadataAlembicSetupCfgBuilder
 	0920-invenio_record_metadata_models_setup_cfg = oarepo_model_builder.invenio.invenio_record_metadata_models_setup_cfg:InvenioRecordMetadataModelsSetupCfgBuilder
 	0930-invenio_resource_setup_cfg  = oarepo_model_builder.invenio.invenio_record_resource_setup_cfg:InvenioRecordResourceSetupCfgBuilder
 	0940-invenio_record_search_setup_cfg  = oarepo_model_builder.invenio.invenio_record_search_setup_cfg:InvenioRecordSearchSetupCfgBuilder
 	0950-invenio_record_jsonschemas_setup_cfg = oarepo_model_builder.invenio.invenio_record_jsonschemas_setup_cfg:InvenioRecordJSONSchemasSetupCfgBuilder
-	1030-invenio_script_sample_data  = oarepo_model_builder.invenio.invenio_script_sample_data:InvenioScriptSampleDataBuilder
+	1030-invenio_script_sample_data  = oarepo_model_builder.invenio.invenio_script_sample_data:SampleDataBuilder
 	1050-invenio_version  = oarepo_model_builder.invenio.invenio_version:InvenioVersionBuilder
 	2000-model_saver  = oarepo_model_builder.builders.model_saver:ModelSaverBuilder
 	2010-model_registration  = oarepo_model_builder.builders.model_saver:ModelRegistrationBuilder
-	3000-cli = oarepo_model_builder.invenio.invenio_cli:InvenioCliBuilder
-	3010-cli_setup = oarepo_model_builder.invenio.invenio_cli_setup_cfg:InvenioCliSetupCfgBuilder
-oarepo_model_builder.model_preprocessors.model = 
-	01-default  = oarepo_model_builder.model_preprocessors.default_values:DefaultValuesModelPreprocessor
-	10-invenio  = oarepo_model_builder.model_preprocessors.invenio:InvenioModelPreprocessor
-	11-invenio  = oarepo_model_builder.model_preprocessors.invenio_base_classes:InvenioBaseClassesModelPreprocessor
-	20-opensearch  = oarepo_model_builder.model_preprocessors.opensearch:OpensearchModelPreprocessor
-oarepo_model_builder.property_preprocessors.model = 
-	200-datatypes  = oarepo_model_builder.property_preprocessors.datatype_preprocessor:DataTypePreprocessor
-	300-enums  = oarepo_model_builder.property_preprocessors.enum:EnumPreprocessor
 oarepo_model_builder.builders.extend = 
 	1000-model  = oarepo_model_builder.builders.extend:ExtendBuilder
-oarepo_model_builder.model_preprocessors.extend = 
-	1000-base-classes = oarepo_model_builder.model_preprocessors.extend:BaseClassesModelPreprocessor
-oarepo_model_builder.property_preprocessors.extend = 
-	0100-type_shortcuts  = oarepo_model_builder.property_preprocessors.type_shortcuts:TypeShortcutsPreprocessor
-	1000-disable-marshmallow  = oarepo_model_builder.property_preprocessors.extend:DisableMarshmallowPreprocessor
+oarepo_model_builder.settings = 
+	1000-python  = oarepo_model_builder.settngs:python.json
+	2000-opensearch  = oarepo_model_builder.settngs:opensearch.json
 
 [tool:pytest]
 testpaths = 
 	tests
 
 [egg_info]
 tag_build =
```

### Comparing `oarepo-model-builder-3.2.9/tests/test_builder_from_entrypoints.py` & `oarepo-model-builder-4.0.0/tests/test_builder_from_entrypoints.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,110 +1,148 @@
 import json
 import os
-import re
 import sys
 from pathlib import Path
 
 from oarepo_model_builder.entrypoints import create_builder_from_entrypoints, load_model
 from oarepo_model_builder.fs import InMemoryFileSystem
 from tests.utils import assert_python_equals
 
+from .utils import strip_whitespaces
+
 OAREPO_USE = "use"
 
 
 def test_include_invenio():
     schema = load_model(
-        "test.yaml",
-        "test",
+        "test.yaml",  # NOSONAR
         model_content={
             "version": "1.0.0",
-            "model": {OAREPO_USE: "invenio", "properties": {"a": {"type": "keyword"}}},
+            "record": {
+                "module": {"qualified": "test"},
+                OAREPO_USE: "invenio",
+                "properties": {"a": {"type": "keyword"}},
+            },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ).read()
-    print(data)
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
-        """
+    assert (
+        strip_whitespaces(
+            """
 from invenio_records_resources.services.records.schema import BaseRecordSchema as InvenioBaseRecordSchema
 from marshmallow import ValidationError
-from marshmallow import validates as ma_validates
+from marshmallow import validate as ma_validate
 import marshmallow as ma
 from marshmallow import fields as ma_fields
 from marshmallow_utils import fields as mu_fields
 from marshmallow_utils import schemas as mu_schemas
-from oarepo_runtime.validation import validate_date
+
+
+
 
 class TestSchema(InvenioBaseRecordSchema):
-    \"""TestSchema schema.\"""
+
+    class Meta:
+        unknown = ma.RAISE
+
+
     a = ma_fields.String()
-    created = ma_fields.String(validate=[validate_date('%Y-%m-%d')], dump_only=True)
-    updated = ma_fields.String(validate=[validate_date('%Y-%m-%d')], dump_only=True)
-    """,
+    """
+        )
+        == strip_whitespaces(data)
+    )
+
+    data = builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py")
+    ).read()
+    print(data)
+    assert (
+        strip_whitespaces(
+            """
+from oarepo_runtime.ui.marshmallow import InvenioUISchema
+class TestUISchema(InvenioUISchema):
+    class Meta:
+        unknown = ma.RAISE
+    a = ma_fields.String()    """
+        )
+        in strip_whitespaces(data)
     )
 
     data = builder.filesystem.read(
         os.path.join("test", "records", "mappings", "os-v2", "test", "test-1.0.0.json")
     )
     data = json.loads(data)
     assert data == {
         "mappings": {
             "properties": {
                 "$schema": {"type": "keyword"},
                 "a": {"type": "keyword"},
-                "created": {"type": "date"},
+                "created": {
+                    "type": "date",
+                    "format": "strict_date_time||strict_date_time_no_millis",
+                },
                 "id": {"type": "keyword"},
-                "updated": {"type": "date"},
+                "updated": {
+                    "type": "date",
+                    "format": "strict_date_time||strict_date_time_no_millis",
+                },
             },
         }
     }
 
     data = builder.filesystem.read("setup.cfg")
-    assert f"version = 1.0.0" in data
+    assert "version = 1.0.0" in data
 
 
 def test_generate_multiple_times():
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
-            "model": {OAREPO_USE: "invenio", "properties": {"a": {"type": "keyword"}}},
+            "record": {
+                "module": {"qualified": "test"},
+                OAREPO_USE: "invenio",
+                "properties": {"a": {"type": "keyword"}},
+            },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
     snapshot_1 = filesystem.snapshot()
 
     # need to reload the schema because of caches ...
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
-            "model": {OAREPO_USE: "invenio", "properties": {"a": {"type": "keyword"}}},
+            "record": {
+                "module": {"qualified": "test"},
+                OAREPO_USE: "invenio",
+                "properties": {"a": {"type": "keyword"}},
+            },
         },
         isort=False,
         black=False,
     )
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
     snapshot_2 = filesystem.snapshot()
 
     assert snapshot_1.keys() == snapshot_2.keys()
 
     for k in snapshot_1:
         first_val = snapshot_1[k]
         second_val = snapshot_2[k]
@@ -117,57 +155,67 @@
             print("====================", file=sys.stderr)
             assert first_val == second_val
 
 
 def test_incremental_builder():
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
-            "model": {OAREPO_USE: "invenio", "properties": {"a": {"type": "keyword"}}},
+            "record": {
+                "module": {"qualified": "test"},
+                OAREPO_USE: "invenio",
+                "properties": {"a": {"type": "keyword"}},
+            },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
-            "model": {OAREPO_USE: "invenio", "properties": {"a": {"type": "keyword"}}},
+            "record": {
+                "module": {"qualified": "test"},
+                OAREPO_USE: "invenio",
+                "properties": {"a": {"type": "keyword"}},
+            },
         },
         isort=False,
         black=False,
     )
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
     snapshot_1 = filesystem.snapshot()
 
     snapshot_1.pop(
         Path.cwd() / "data/sample_data.yaml"
     )  # these are always regenerated and random, so do not check them
 
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
-            "model": {OAREPO_USE: "invenio", "properties": {"a": {"type": "keyword"}}},
+            "record": {
+                "module": {"qualified": "test"},
+                OAREPO_USE: "invenio",
+                "properties": {"a": {"type": "keyword"}},
+            },
         },
         isort=False,
         black=False,
     )
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
     snapshot_2 = filesystem.snapshot()
 
     ret = snapshot_2.pop(
         Path.cwd() / "data/sample_data.yaml"
     )  # these are always regenerated and random, so do not check them
 
     assert set(snapshot_1.keys()) == set(snapshot_2.keys())
```

### Comparing `oarepo-model-builder-3.2.9/tests/test_dependencies.py` & `oarepo-model-builder-4.0.0/tests/test_dependencies.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 from oarepo_model_builder.entrypoints import create_builder_from_entrypoints, load_model
 from oarepo_model_builder.fs import InMemoryFileSystem
 
 
 def test_no_dependencies():
     data = build()
     print(data)
@@ -25,18 +23,22 @@
     assert """test>=1.0.0""" in data
     assert data.index("devs =") < data.index("test>=1.0.0")
 
 
 def build(kwargs={}):
     schema = load_model(
         "test.yaml",
-        "test",
-        model_content={"model": {}, **kwargs},
+        model_content={
+            "record": {},
+            "settings": {"schema-server": "local://"},
+            "version": "1.0.0",
+            **kwargs,
+        },
         isort=False,
         black=False,
+        autoflake=False,
     )
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
-    builder.skip_schema_validation = True
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
     data = builder.filesystem.open("setup.cfg").read().strip()
     return data
```

### Comparing `oarepo-model-builder-3.2.9/tests/test_facets.py` & `oarepo-model-builder-4.0.0/tests/test_marshmallow_ui_builder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,631 +1,593 @@
 import os
-import re
 
-from oarepo_model_builder.entrypoints import create_builder_from_entrypoints, load_model
+import pytest
+
+from oarepo_model_builder.builder import ModelBuilder
 from oarepo_model_builder.fs import InMemoryFileSystem
+from oarepo_model_builder.invenio.invenio_record_resource_config import (
+    InvenioRecordResourceConfigBuilder,
+)
+from oarepo_model_builder.invenio.invenio_record_ui_marshmallow import (
+    InvenioRecordUIMarshmallowBuilder,
+)
+from oarepo_model_builder.invenio.invenio_record_ui_serializer import (
+    InvenioRecordUISerializerBuilder,
+)
+from oarepo_model_builder.outputs.python import PythonOutput
+from oarepo_model_builder.schema import ModelSchema
 
-DUMMY_YAML = "test.yaml"
+from .utils import strip_whitespaces
 
 
-def test_include_invenio():
-    schema = load_model(
-        DUMMY_YAML,
-        "test",
-        model_content={
-            "model": {
-                "use": "invenio",
-                "properties": {
-                    "a": "fulltext+keyword",
-                    "b": {
-                        "type": "keyword",
-                        "facets": {"field": 'TermsFacet(field="cosi")'},
-                    },
-                    "c": "fulltext",
+def get_test_schema(**props):
+    return ModelSchema(
+        "",
+        {
+            "settings": {
+                "python": {
+                    "use-isort": False,
+                    "use-black": False,
+                    "use-autoflake": False,
                 },
             },
+            "record": {"module": {"qualified": "test"}, "properties": props},
         },
-        isort=False,
-        black=False,
     )
 
-    filesystem = InMemoryFileSystem()
-    builder = create_builder_from_entrypoints(filesystem=filesystem)
-    builder.build(schema, "")
-
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
-        """
-\"""Facet definitions.\"""
-
-from invenio_records_resources.services.records.facets import TermsFacet
-from invenio_search.engine import dsl
-from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
-
-
-
-a_keyword = TermsFacet(field = "a.keyword")
-
-
-
-b = TermsFacet(field="cosi")
-
 
-
-_id = TermsFacet(field = "id")
-
-
-
-created = TermsFacet(field = "created")
-
-
-
-updated = TermsFacet(field = "updated")
-
-
-
-_schema = TermsFacet(field = "$schema")
-    """,
+@pytest.fixture
+def fulltext_builder():
+    return ModelBuilder(
+        output_builders=[
+            InvenioRecordUIMarshmallowBuilder,
+            InvenioRecordUISerializerBuilder,
+            InvenioRecordResourceConfigBuilder,
+        ],
+        outputs=[PythonOutput],
     )
 
 
-def test_nested():
-    schema = load_model(
-        DUMMY_YAML,
-        "test",
-        model_content={
-            "model": {
-                "use": "invenio",
-                "properties": {
-                    "b": {
-                        "type": "nested",
-                        "properties": {
-                            "c": {
-                                "type": "keyword",
-                            },
-                            "d": {"type": "fulltext+keyword"},
-                            "f": {
-                                "type": "nested",
-                                "properties": {"g": {"type": "keyword"}},
-                            },
-                        },
-                    }
-                },
-            },
-        },
-        isort=False,
-        black=False,
+def _test(fulltext_builder, string_type):
+    schema = get_test_schema(a={"type": string_type})
+    fulltext_builder.filesystem = InMemoryFileSystem()
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
     )
 
-    filesystem = InMemoryFileSystem()
-    builder = create_builder_from_entrypoints(filesystem=filesystem)
-
-    builder.build(schema, "")
-
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
-        """
-\"""Facet definitions.\"""
-
-from invenio_records_resources.services.records.facets import TermsFacet
-from invenio_search.engine import dsl
-from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
-
-
-
-
-b_c = NestedLabeledFacet(path =" b", nested_facet = TermsFacet(field = "b.c"))
-
-
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py")  # NOSONAR
+    ) as f:
+        data = f.read()
+    assert "a = ma_fields.String()" in data
 
-b_d_keyword = NestedLabeledFacet(path =" b", nested_facet=TermsFacet(field = "b.d.keyword"))
 
+def test_fulltext(fulltext_builder):
+    _test(fulltext_builder, "fulltext")
 
 
+def test_keyword(fulltext_builder):
+    _test(fulltext_builder, "keyword")
 
-b_f_g = NestedLabeledFacet(path =" b", nested_facet=NestedLabeledFacet(path =" b.f", nested_facet=TermsFacet(field = "b.f.g")))
 
+def test_fulltext_keyword(fulltext_builder):
+    _test(fulltext_builder, "fulltext+keyword")
 
 
-_id = TermsFacet(field = "id")
-
-
-
-created = TermsFacet(field = "created")
-
-
-
-updated = TermsFacet(field = "updated")
+def test_simple_array(fulltext_builder):
+    schema = get_test_schema(a={"type": "array", "items": {"type": "keyword"}})
+    fulltext_builder.filesystem = InMemoryFileSystem()
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py")
+    ) as f:
+        data = f.read()
+    assert "a = ma_fields.List(ma_fields.String())" in data
 
 
-_schema = TermsFacet(field = "$schema")
-    
-""",
+def test_array_of_objects(fulltext_builder):
+    schema = get_test_schema(
+        a={
+            "type": "array",
+            "items": {"type": "object", "properties": {"b": {"type": "integer"}}},
+        }
     )
-
-
-def test_object():
-    schema = load_model(
-        DUMMY_YAML,
-        "test",
-        model_content={
-            "model": {
-                "use": "invenio",
-                "properties": {
-                    "b": {
-                        "type": "object",
-                        "properties": {
-                            "c": {
-                                "type": "keyword",
-                            },
-                            "d": {"type": "fulltext+keyword"},
-                            "f": {
-                                "type": "object",
-                                "properties": {"g": {"type": "keyword"}},
-                            },
-                            "e": "fulltext",
-                        },
-                    }
-                },
-            },
-        },
-        isort=False,
-        black=False,
+    fulltext_builder.filesystem = InMemoryFileSystem()
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
     )
 
-    filesystem = InMemoryFileSystem()
-    builder = create_builder_from_entrypoints(filesystem=filesystem)
-
-    builder.build(schema, "")
-
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
-    print(data)
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
-        """
-        \"""Facet definitions.\"""
-
-from invenio_records_resources.services.records.facets import TermsFacet
-from invenio_search.engine import dsl
-from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
-
-
-
-
-b_c = TermsFacet(field = "b.c")
-
-
-
-b_d_keyword = TermsFacet(field = "b.d.keyword")
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py")
+    ) as f:
+        data = f.read()
+    assert (
+        strip_whitespaces(
+            """ 
+class TestUISchema(InvenioUISchema):
 
+    class Meta:
+        unknown = ma.RAISE
 
 
-b_f_g = TermsFacet(field = "b.f.g")
+    a = ma_fields.List(ma_fields.Nested(lambda: AItemUISchema()))
 
 
+class AItemUISchema(ma.Schema):
 
-_id = TermsFacet(field = "id")
+    class Meta:
+        unknown = ma.RAISE
 
 
-
-created = TermsFacet(field = "created")
-
-
-
-updated = TermsFacet(field = "updated")
-
-
-
-_schema = TermsFacet(field = "$schema")
-""",
+    b = ma_fields.Integer() """
+        )
+        in strip_whitespaces(data)
     )
 
 
-def test_nest_obj():
-    schema = load_model(
-        DUMMY_YAML,
-        "test",
-        model_content={
-            "model": {
-                "use": "invenio",
-                "properties": {
-                    "b_nes": {
-                        "type": "nested",
-                        "properties": {
-                            "c": {
-                                "type": "keyword",
-                            },
-                            "d": {"type": "fulltext+keyword"},
-                            "f": {
-                                "type": "object",
-                                "properties": {"g": {"type": "keyword"}},
-                            },
-                        },
-                    },
-                    "b_obj": {
-                        "type": "object",
-                        "properties": {
-                            "c": {
-                                "type": "keyword",
-                            },
-                            "d": {"type": "fulltext+keyword"},
-                            "f": {
-                                "type": "nested",
-                                "properties": {"g": {"type": "keyword"}},
-                            },
-                        },
-                    },
-                },
+def test_generate_nested_schema_same_file(fulltext_builder):
+    schema = get_test_schema(
+        a={
+            "type": "object",
+            "marshmallow": {"class": "B", "generate": True},
+            "ui": {"marshmallow": {"class": "BUISchema", "generate": True}},
+            "properties": {
+                "b": {
+                    "type": "keyword",
+                }
             },
-        },
-        isort=False,
-        black=False,
+        }
+    )
+    fulltext_builder.filesystem = InMemoryFileSystem()
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
     )
 
-    filesystem = InMemoryFileSystem()
-    builder = create_builder_from_entrypoints(filesystem=filesystem)
-
-    builder.build(schema, "")
-
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
-        """
-        \"""Facet definitions.\"""
-
-from invenio_records_resources.services.records.facets import TermsFacet
-from invenio_search.engine import dsl
-from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
-
-
-
-
-b_nes_c = NestedLabeledFacet(path ="b_nes", nested_facet=TermsFacet(field = "b_nes.c"))
-
-
-
-b_nes_d_keyword = NestedLabeledFacet(path ="b_nes", nested_facet=TermsFacet(field = "b_nes.d.keyword"))
-
-
-
-b_nes_f_g = NestedLabeledFacet(path ="b_nes", nested_facet=TermsFacet(field = "b_nes.f.g"))
-
-
-
-b_obj_c = TermsFacet(field = "b_obj.c")
-
-
-
-b_obj_d_keyword = TermsFacet(field = "b_obj.d.keyword")
-
-
-
-b_obj_f_g = NestedLabeledFacet(path ="b_obj.f", nested_facet=TermsFacet(field = "b_obj.f.g"))
-
-
-
-_id = TermsFacet(field = "id")
-
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py")
+    ) as f:
+        data = f.read()
+    assert (
+        strip_whitespaces(
+            """
+class TestUISchema(InvenioUISchema):
 
+    class Meta:
+        unknown = ma.RAISE
 
-created = TermsFacet(field = "created")
 
+    a = ma_fields.Nested(lambda: BUISchema())
 
 
-updated = TermsFacet(field = "updated")
+class BUISchema(ma.Schema):
 
+    class Meta:
+        unknown = ma.RAISE
 
 
-_schema = TermsFacet(field = "$schema")
-""",
+    b = ma_fields.String()    
+    """
+        )
+        in strip_whitespaces(data)
     )
 
 
-def test_array():
-    schema = load_model(
-        DUMMY_YAML,
-        "test",
-        model_content={
-            "model": {
-                "use": "invenio",
-                "properties": {
-                    "a[]": "keyword",
-                    "b[]": "fulltext",
-                    "c[]": "fulltext+keyword",
-                },
+def test_generate_nested_schema_different_file(fulltext_builder):
+    schema = get_test_schema(
+        a={
+            "type": "object",
+            "marshmallow": {
+                "class": "test.services.schema2.B",
+                "generate": True,
             },
-        },
-        isort=False,
-        black=False,
+            "ui": {
+                "marshmallow": {
+                    "class": "test.services.schema2.BUISchema",
+                    "generate": True,
+                }
+            },
+            "properties": {
+                "b": {
+                    "type": "keyword",
+                }
+            },
+        }
     )
-
-    filesystem = InMemoryFileSystem()
-    builder = create_builder_from_entrypoints(filesystem=filesystem)
-
-    builder.build(schema, "")
-
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
-        """
-        \"""Facet definitions.\"""
-
-from invenio_records_resources.services.records.facets import TermsFacet
-from invenio_search.engine import dsl
-from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
-
-
-
-
-a = TermsFacet(field = "a")
-
-
-
-c_keyword = TermsFacet(field = "c.keyword")
-
-
-_id = TermsFacet(field = "id")
-
-
-
-created = TermsFacet(field = "created")
-
-
-
-updated = TermsFacet(field = "updated")
-
-
-
-_schema = TermsFacet(field = "$schema")
-""",
+    fulltext_builder.filesystem = InMemoryFileSystem()
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
+
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py")
+    ) as f:
+        data = f.read()
+    assert (
+        strip_whitespaces(
+            """
+from test.services.schema2 import BUISchema
+class TestUISchema(InvenioUISchema):
+    class Meta:
+        unknown = ma.RAISE
+    a = ma_fields.Nested(lambda: BUISchema())
+    """
+        )
+        in strip_whitespaces(data)
     )
 
 
-def test_array_nested():
-    schema = load_model(
-        DUMMY_YAML,
-        "test",
-        model_content={
-            "model": {
-                "use": "invenio",
-                "properties": {
-                    "obj": {
-                        "type": "object",
-                        "properties": {
-                            "arr": {
-                                "type": "array",
-                                "items": {
-                                    "type": "nested",
-                                    "properties": {
-                                        "d": {"type": "keyword"},
-                                        "e": {
-                                            "type": "object",
-                                            "properties": {"f": "keyword"},
-                                        },
-                                    },
-                                },
-                            }
-                        },
-                    },
-                },
+def test_use_nested_schema_same_file(fulltext_builder):
+    schema = get_test_schema(
+        a={
+            "type": "object",
+            "marshmallow": {"class": "B", "generate": False},
+            "ui": {"marshmallow": {"class": "BUISchema", "generate": False}},
+            "properties": {
+                "b": {
+                    "type": "keyword",
+                }
             },
-        },
-        isort=False,
-        black=False,
+        }
+    )
+    fulltext_builder.filesystem = InMemoryFileSystem()
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
     )
 
-    filesystem = InMemoryFileSystem()
-    builder = create_builder_from_entrypoints(filesystem=filesystem)
-
-    builder.build(schema, "")
-
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
-        """
-        \"""Facet definitions.\"""
-
-from invenio_records_resources.services.records.facets import TermsFacet
-from invenio_search.engine import dsl
-from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
-
-
-obj_arr_d = NestedLabeledFacet(path ="obj.arr", nested_facet=TermsFacet(field = "obj.arr.d"))
-
-obj_arr_e_f = NestedLabeledFacet(path ="obj.arr", nested_facet=TermsFacet(field = "obj.arr.e.f"))
-
-
-_id = TermsFacet(field = "id")
-
-
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py")
+    ) as f:
+        data = f.read()
 
-created = TermsFacet(field = "created")
+    assert (
+        strip_whitespaces(
+            """
+class TestUISchema(InvenioUISchema):
 
+    class Meta:
+        unknown = ma.RAISE
 
 
-updated = TermsFacet(field = "updated")
+    a = ma_fields.Nested(lambda: BUISchema())
+"""
+        )
+        in strip_whitespaces(data)
+    )
 
+    assert strip_whitespaces("class BUISchema") not in strip_whitespaces(data)
 
 
-_schema = TermsFacet(field = "$schema")
-""",
+def test_use_nested_schema_different_file(fulltext_builder):
+    schema = get_test_schema(
+        a={
+            "type": "object",
+            "marshmallow": {"class": "c.B", "generate": False},
+            "ui": {"marshmallow": {"class": "c.BUISchema", "generate": False}},
+            "properties": {
+                "b": {
+                    "type": "keyword",
+                }
+            },
+        }
+    )
+    fulltext_builder.filesystem = InMemoryFileSystem()
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
+
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py")
+    ) as f:
+        data = f.read()
+
+    assert (
+        strip_whitespaces(
+            """
+from c import BUISchema
+from oarepo_runtime.ui.marshmallow import InvenioUISchema
+class TestUISchema(InvenioUISchema):
+    class Meta:
+        unknown = ma.RAISE
+    a = ma_fields.Nested(lambda: BUISchema())
+"""
+        )
+        in strip_whitespaces(data)
     )
 
 
-def test_top_facets():
-    schema = load_model(
-        DUMMY_YAML,
-        "test",
-        model_content={
-            "model": {
-                "use": "invenio",
-                "searchable": False,
+def test_generate_nested_schema_array(fulltext_builder):
+    schema = get_test_schema(
+        a={
+            "type": "array",
+            "items": {
+                "type": "object",
+                "marshmallow": {"class": "B", "generate": True},
+                "ui": {"marshmallow": {"class": "BUISchema", "generate": True}},
                 "properties": {
-                    "a": {"type": "fulltext+keyword", "facets": {"searchable": True}},
                     "b": {
                         "type": "keyword",
-                        "facets": {"field": 'TermsFacet(field="cosi")'},
-                    },
-                    "c": "keyword",
-                    "arr": {
-                        "type": "array",
-                        "facets": {"searchable": True},
-                        "items": {
-                            "type": "nested",
-                            "properties": {
-                                "d": {"type": "keyword"},
-                                "e": {"type": "object", "properties": {"f": "keyword"}},
-                            },
-                        },
-                    },
-                    "lst2": {
-                        "type": "array",
-                        "items": {"type": "keyword"},
-                        "facets": {"field": 'TermsFacet(field="cosi")'},
-                    },
-                    "lst[]": "keyword",
+                    }
                 },
             },
-        },
-        isort=False,
-        black=False,
+        }
     )
-
-    filesystem = InMemoryFileSystem()
-    builder = create_builder_from_entrypoints(filesystem=filesystem)
-    builder.build(schema, "")
-
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
-    print(data)
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
-        """
-\"""Facet definitions.\"""
-
-from invenio_records_resources.services.records.facets import TermsFacet
-from invenio_search.engine import dsl
-from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
-
-
-
-a_keyword = TermsFacet(field = "a.keyword")
-
-
-
-b = TermsFacet(field="cosi")
-
-
-
-arr_d = NestedLabeledFacet(path ="arr", nested_facet=TermsFacet(field = "arr.d"))
-
-arr_e_f = NestedLabeledFacet(path ="arr", nested_facet=TermsFacet(field = "arr.e.f"))
-
-lst2 = TermsFacet(field="cosi")
-
-_id = TermsFacet(field = "id")
-
-
-
-created = TermsFacet(field = "created")
-
-
-
-updated = TermsFacet(field = "updated")
-
-
-
-_schema = TermsFacet(field = "$schema")
-
-    """,
+    fulltext_builder.filesystem = InMemoryFileSystem()
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
+
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py")
+    ) as f:
+        data = f.read()
+    assert (
+        strip_whitespaces(
+            """
+class TestUISchema(InvenioUISchema):
+    class Meta:
+        unknown = ma.RAISE
+    a = ma_fields.List(ma_fields.Nested(lambda: BUISchema()))
+
+
+class BUISchema(ma.Schema):
+    class Meta:
+        unknown = ma.RAISE
+    b = ma_fields.String()
+"""
+        )
+        in strip_whitespaces(data)
+    )
+
+
+def test_extend_existing(fulltext_builder):
+    schema = get_test_schema(a={"type": "keyword"}, b={"type": "keyword"})
+    fulltext_builder.filesystem = InMemoryFileSystem()
+
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py"), "w"
+    ) as f:
+        f.write(
+            '''
+from invenio_records_resources.services.records.schema import BaseRecordSchema as InvenioBaseRecordSchema
+import marshmallow as ma
+import marshmallow.fields as ma_fields
+import marshmallow.validate as ma_valid
+class TestUISchema(ma.Schema):
+    """TestUISchema schema."""
+    a = ma_fields.String()'''
+        )
+
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
+    data = fulltext_builder.filesystem.read(
+        os.path.join("test", "services", "records", "ui_schema.py")
+    )
+    assert "b = ma_fields.String()" in data
+
+
+def test_generate_nested_schema_relative_same_package(fulltext_builder):
+    schema = get_test_schema(
+        a={
+            "type": "object",
+            "marshmallow": {
+                "class": ".schema2.B",
+                "generate": True,
+            },
+            "ui": {
+                "marshmallow": {
+                    "class": "..ui_schema2.BUISchema",
+                    "generate": True,
+                }
+            },
+            "properties": {
+                "b": {
+                    "type": "keyword",
+                }
+            },
+        }
+    )
+    fulltext_builder.filesystem = InMemoryFileSystem()
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
+
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py")
+    ) as f:
+        data = f.read()
+    assert (
+        strip_whitespaces(
+            """
+class TestUISchema(InvenioUISchema):
+    class Meta:
+        unknown = ma.RAISE
+    a = ma_fields.Nested(lambda: BUISchema())
+"""
+        )
+        in strip_whitespaces(data)
+    )
+
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema2.py")
+    ) as f:
+        data = f.read()
+    assert (
+        strip_whitespaces(
+            """
+class BUISchema(ma.Schema):
+    class Meta:
+        unknown = ma.RAISE
+    b = ma_fields.String()
+"""
+        )
+        in strip_whitespaces(data)
     )
 
 
-def test_searchable_true():
-    schema = load_model(
-        DUMMY_YAML,
-        "test",
-        model_content={
-            "model": {
-                "use": "invenio",
-                "properties": {
-                    "a": {"type": "fulltext+keyword", "facets": {"searchable": False}},
-                    "b": {
-                        "type": "keyword",
-                        "facets": {"field": 'TermsFacet(field="cosi")'},
-                    },
-                    "c": "fulltext",
-                    "f": {
-                        "type": "object",
-                        "facets": {"searchable": False},
-                        "properties": {"g": {"type": "keyword"}},
-                    },
-                },
+def test_generate_nested_schema_relative_same_file(fulltext_builder):
+    schema = get_test_schema(
+        a={
+            "type": "object",
+            "marshmallow": {
+                "class": ".B",
+                "generate": True,
             },
-        },
-        isort=False,
-        black=False,
+            "ui": {
+                "marshmallow": {
+                    "class": ".BUISchema",
+                    "generate": True,
+                }
+            },
+            "properties": {
+                "b": {
+                    "type": "keyword",
+                }
+            },
+        }
+    )
+    fulltext_builder.filesystem = InMemoryFileSystem()
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
+
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py")
+    ) as f:
+        data = f.read()
+
+    assert (
+        strip_whitespaces(
+            """
+class TestUISchema(InvenioUISchema):
+    class Meta:
+        unknown = ma.RAISE
+    a = ma_fields.Nested(lambda: BUISchema())
+
+class BUISchema(ma.Schema):
+    class Meta:
+        unknown = ma.RAISE
+    b = ma_fields.String()
+"""
+        )
+        in strip_whitespaces(data)
     )
 
-    filesystem = InMemoryFileSystem()
-    builder = create_builder_from_entrypoints(filesystem=filesystem)
-    builder.build(schema, "")
-    data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "facets.py")
-    ).read()
-    print(data)
-
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
-        """
-\"""Facet definitions.\"""
-
-from invenio_records_resources.services.records.facets import TermsFacet
-from invenio_search.engine import dsl
-from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
-
-
-
-
-b = TermsFacet(field="cosi")
-
-
-_id = TermsFacet(field = "id")
-
-
-
-created = TermsFacet(field = "created")
-
-
-
-updated = TermsFacet(field = "updated")
-
-
-
-_schema = TermsFacet(field = "$schema")
 
-    """,
+def test_generate_nested_schema_relative_upper(fulltext_builder):
+    schema = get_test_schema(
+        a={
+            "type": "object",
+            "marshmallow": {
+                "class": "...schema2.B",
+                "generate": True,
+            },
+            "ui": {
+                "marshmallow": {
+                    "class": "..schema2.BUISchema",
+                    "generate": True,
+                }
+            },
+            "properties": {
+                "b": {
+                    "type": "keyword",
+                }
+            },
+        }
     )
+    fulltext_builder.filesystem = InMemoryFileSystem()
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
+
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py")
+    ) as f:
+        data = f.read()
+
+    assert (
+        strip_whitespaces(
+            """
+from test.services.records.schema2 import BUISchema
+class TestUISchema(InvenioUISchema):
+    class Meta:
+        unknown = ma.RAISE
+    a = ma_fields.Nested(lambda: BUISchema())
+"""
+        )
+        in strip_whitespaces(data)
+    )
+
+
+def test_generate_json_serializer(fulltext_builder):
+    schema = get_test_schema(
+        a={
+            "type": "keyword",
+        }
+    )
+    fulltext_builder.filesystem = InMemoryFileSystem()
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "resources", "records", "ui.py")
+    ) as f:
+        data = f.read()
+    assert (
+        strip_whitespaces(
+            '''
+from flask_resources import BaseListSchema
+from flask_resources import MarshmallowSerializer
+from flask_resources.serializers import JSONSerializer
+
+from test.services.records.ui_schema import TestUISchema
+
+
+
+class TestUIJSONSerializer(MarshmallowSerializer):
+    """UI JSON serializer."""
+
+    def __init__(self):
+        """Initialise Serializer."""
+        super().__init__(
+            format_serializer_cls=JSONSerializer,
+            object_schema_cls=TestUISchema,
+            list_schema_cls=BaseListSchema,
+            schema_context={"object_key": "ui"},
+        )    
+    '''
+        )
+        == strip_whitespaces(data)
+    )
+
+
+def test_localized_date(fulltext_builder):
+    schema = get_test_schema(a={"type": "date"})
+    fulltext_builder.filesystem = InMemoryFileSystem()
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
+
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py")
+    ) as f:
+        data = f.read()
+    assert "a = l10n.LocalizedDate()" in data
+
+
+def test_metadata(fulltext_builder):
+    schema = get_test_schema(
+        metadata={"type": "object", "properties": {"a": {"type": "keyword"}}}
+    )
+    fulltext_builder.filesystem = InMemoryFileSystem()
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
+
+    with fulltext_builder.filesystem.open(
+        os.path.join("test", "services", "records", "ui_schema.py")
+    ) as f:
+        data = f.read()
+    assert "metadata = ma_fields.Nested(lambda: TestMetadataUISchema())" in data
```

### Comparing `oarepo-model-builder-3.2.9/tests/test_fulltext_keyword.py` & `oarepo-model-builder-4.0.0/tests/test_fulltext_keyword.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,58 +3,53 @@
 import json5
 import pytest
 
 from oarepo_model_builder.builder import ModelBuilder
 from oarepo_model_builder.builders.jsonschema import JSONSchemaBuilder
 from oarepo_model_builder.builders.mapping import MappingBuilder
 from oarepo_model_builder.fs import InMemoryFileSystem
-from oarepo_model_builder.model_preprocessors.default_values import (
-    DefaultValuesModelPreprocessor,
-)
-from oarepo_model_builder.model_preprocessors.opensearch import (
-    OpensearchModelPreprocessor,
-)
 from oarepo_model_builder.outputs.jsonschema import JSONSchemaOutput
 from oarepo_model_builder.outputs.mapping import MappingOutput
 from oarepo_model_builder.outputs.python import PythonOutput
-from oarepo_model_builder.property_preprocessors.datatype_preprocessor import (
-    DataTypePreprocessor,
-)
 from oarepo_model_builder.schema import ModelSchema
 
 
 def get_model_schema(field_type):
     return ModelSchema(
         "",
         {
             "settings": {
-                "python": {"use-isort": False, "use-black": False},
+                "python": {
+                    "use-isort": False,
+                    "use-black": False,
+                    "use-autoflake": False,
+                },
+            },
+            "record": {
+                "module": {"qualified": "test"},
+                "properties": {"a": {"type": field_type}},
             },
-            "model": {"package": "test", "properties": {"a": {"type": field_type}}},
         },
     )
 
 
 @pytest.fixture
 def fulltext_builder():
     return ModelBuilder(
         output_builders=[JSONSchemaBuilder, MappingBuilder],
         outputs=[JSONSchemaOutput, MappingOutput, PythonOutput],
-        model_preprocessors=[
-            DefaultValuesModelPreprocessor,
-            OpensearchModelPreprocessor,
-        ],
-        property_preprocessors=[DataTypePreprocessor],
     )
 
 
 def test_fulltext(fulltext_builder):
     schema = get_model_schema("fulltext")
     fulltext_builder.filesystem = InMemoryFileSystem()
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
     data = load_generated_jsonschema(fulltext_builder)
 
     assert data == {"type": "object", "properties": {"a": {"type": "string"}}}
 
     data = load_generated_mapping(fulltext_builder)
 
@@ -66,15 +61,17 @@
         }
     }
 
 
 def test_keyword(fulltext_builder):
     schema = get_model_schema("keyword")
     fulltext_builder.filesystem = InMemoryFileSystem()
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
     data = load_generated_jsonschema(fulltext_builder)
 
     assert data == {"type": "object", "properties": {"a": {"type": "string"}}}
 
     data = load_generated_mapping(fulltext_builder)
 
@@ -86,29 +83,28 @@
         }
     }
 
 
 def test_fulltext_keyword(fulltext_builder):
     schema = get_model_schema("fulltext+keyword")
     fulltext_builder.filesystem = InMemoryFileSystem()
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
     data = load_generated_jsonschema(fulltext_builder)
 
     assert data == {"type": "object", "properties": {"a": {"type": "string"}}}
 
     data = load_generated_mapping(fulltext_builder)
 
     assert data == {
         "mappings": {
             "properties": {
-                "a": {
-                    "fields": {"keyword": {"type": "keyword"}},
-                    "type": "text",
-                },
+                "a": {"fields": {"keyword": {"type": "keyword"}}, "type": "text"},
             }
         }
     }
 
 
 def load_generated_mapping(fulltext_builder):
     return json5.load(
```

### Comparing `oarepo-model-builder-3.2.9/tests/test_jsonchema_builder.py` & `oarepo-model-builder-4.0.0/tests/test_mapping_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,157 +1,163 @@
 import os
 
 from oarepo_model_builder.builder import ModelBuilder
-from oarepo_model_builder.builders import OutputBuilderComponent
-from oarepo_model_builder.builders.jsonschema import JSONSchemaBuilder
-from oarepo_model_builder.datatypes import datatypes
+from oarepo_model_builder.builders.mapping import MappingBuilder
 from oarepo_model_builder.fs import InMemoryFileSystem
-from oarepo_model_builder.model_preprocessors.default_values import (
-    DefaultValuesModelPreprocessor,
-)
-from oarepo_model_builder.outputs.jsonschema import JSONSchemaOutput
+from oarepo_model_builder.outputs.mapping import MappingOutput
 from oarepo_model_builder.outputs.python import PythonOutput
 from oarepo_model_builder.schema import ModelSchema
-from oarepo_model_builder.validation.model_validation import model_validator
-from tests.multilang import MultilangPreprocessor, MultilingualDataType, UIValidator
 
 try:
     import json5
 except ImportError:
     import json as json5
 
 
-def test_simple_jsonschema_builder():
-    data = build({"properties": {"a": {"type": "keyword", "ui": {"class": "bolder"}}}})
+def test_simple_mapping_builder():
+    model = {"properties": {"a": {"type": "keyword"}}}
+    data = build_model(model)
 
-    assert data == {"type": "object", "properties": {"a": {"type": "keyword"}}}
+    assert data == {"mappings": {"properties": {"a": {"type": "keyword"}}}}
 
 
-def test_required():
-    data = build(
-        {
-            "properties": {
-                "a": {
-                    "type": "keyword",
-                    "required": True,
-                    "ui": {"class": "bolder"},
-                }
-            }
-        }
-    )
+def test_simple_mapping_text_builder():
+    model = {"properties": {"a": {"type": "keyword", "mapping": {"type": "text"}}}}
+    data = build_model(model)
 
-    assert data == {
-        "type": "object",
-        "properties": {"a": {"type": "keyword"}},
-        "required": ["a"],
-    }
+    assert data == {"mappings": {"properties": {"a": {"type": "text"}}}}
 
 
-def test_required_inside_metadata():
-    data = build(
-        {
-            "properties": {
-                "metadata": {
-                    "properties": {
-                        "a": {
-                            "type": "keyword",
-                            "required": True,
-                            "ui": {"class": "bolder"},
-                        }
-                    }
-                }
-            }
-        }
-    )
-
-    assert data == {
-        "type": "object",
-        "properties": {
-            "metadata": {
-                "type": "object",
-                "properties": {"a": {"type": "keyword"}},
-                "required": ["a"],
-            }
-        },
-    }
-
-
-def test_min_length():
-    data = build({"properties": {"a": {"type": "keyword", "minLength": 5}}})
-    assert data == {
-        "type": "object",
-        "properties": {"a": {"type": "keyword", "minLength": 5}},
-    }
-
-
-def test_jsonschema_preprocessor():
-    data = build(
-        {"properties": {"a": {"type": "multilingual", "ui": {"class": "bolder"}}}},
-        property_preprocessors=[MultilangPreprocessor],
-    )
-
-    assert data == {
-        "type": "object",
+def test_array_mapping_builder():
+    model = {
         "properties": {
             "a": {
-                "type": "object",
-                "properties": {
-                    "lang": {"type": "string"},
-                    "value": {"type": "string"},
-                },
+                "type": "array",
+                "items": {"type": "keyword", "mapping": {"type": "text"}},
             }
-        },
+        }
     }
+    data = build_model(model)
 
-
-class TestJSONSchemaOutputComponent(OutputBuilderComponent):
-    def model_element_enter(self, builder, data, *, stack):
-        if "type" in data:
-            data["type"] = "integer"
-        return data
-
-
-def test_components():
-    data = build(
-        {"properties": {"a": {"type": "keyword", "ui": {"class": "bolder"}}}},
-        output_builder_components={
-            JSONSchemaOutput.TYPE: [TestJSONSchemaOutputComponent]
-        },
-    )
-
-    assert data == {"type": "object", "properties": {"a": {"type": "integer"}}}
+    assert data == {"mappings": {"properties": {"a": {"type": "text"}}}}
 
 
-def build(model, output_builder_components=None, property_preprocessors=None):
-    datatypes._prepare_datatypes()
-    if UIValidator not in model_validator.validator_map["property"]:
-        model_validator.validator_map["property"].append(UIValidator)
-    datatypes.datatype_map["multilingual"] = MultilingualDataType
+def build_model(model):
     builder = ModelBuilder(
-        output_builders=[JSONSchemaBuilder],
-        outputs=[JSONSchemaOutput, PythonOutput],
-        model_preprocessors=[DefaultValuesModelPreprocessor],
-        output_builder_components=output_builder_components,
+        output_builders=[MappingBuilder],
+        outputs=[MappingOutput, PythonOutput],
         filesystem=InMemoryFileSystem(),
-        property_preprocessors=property_preprocessors,
     )
     builder.build(
         model=ModelSchema(
             "",
             {
                 "settings": {
-                    "python": {"use-isort": False, "use-black": False},
-                },
-                "model": {
-                    "package": "test",
-                    **model,
+                    "python": {
+                        "use-isort": False,
+                        "use-black": False,
+                        "use-autoflake": False,
+                    },
+                    "opensearch": {"version": "os-v2"},
                 },
+                "record": {"module": {"qualified": "test"}, **model},
             },
         ),
+        profile="record",
+        model_path=["record"],
         output_dir="",
     )
     data = json5.load(
         builder.filesystem.open(
-            os.path.join("test", "records", "jsonschemas", "test-1.0.0.json")
+            os.path.join(
+                "test", "records", "mappings", "os-v2", "test", "test-1.0.0.json"
+            )
         )
     )
     return data
+
+
+def test_no_index():
+    model = {"properties": {"a": {"type": "keyword", "facets": {"searchable": False}}}}
+    data = build_model(model)
+
+    assert data == {
+        "mappings": {"properties": {"a": {"type": "keyword", "enabled": False}}}
+    }
+
+
+def test_no_index_on_model():
+    model = {"properties": {"a": {"type": "keyword"}}, "searchable": False}
+    data = build_model(model)
+
+    assert data == {
+        "mappings": {"properties": {"a": {"type": "keyword", "enabled": False}}}
+    }
+
+
+def test_override_no_index_on_model():
+    model = {
+        "properties": {"a": {"type": "keyword", "facets": {"searchable": True}}},
+        "searchable": False,
+    }
+    data = build_model(model)
+
+    assert data == {"mappings": {"properties": {"a": {"type": "keyword"}}}}
+
+
+def test_override_no_index_on_model():
+    model = {
+        "properties": {"a": {"type": "keyword", "facets": {"searchable": True}}},
+        "searchable": False,
+    }
+    data = build_model(model)
+
+    assert data == {"mappings": {"properties": {"a": {"type": "keyword"}}}}
+
+
+def test_deep_no_index():
+    model = {
+        "properties": {
+            "a": {
+                "type": "object",
+                "facets": {"searchable": False},
+                "properties": {"b": {"type": "keyword"}},
+            }
+        }
+    }
+    data = build_model(model)
+
+    assert data == {
+        "mappings": {
+            "properties": {
+                "a": {
+                    "type": "object",
+                    "enabled": False,
+                }
+            }
+        }
+    }
+
+
+def test_deep_no_index_children():
+    model = {
+        "properties": {
+            "a": {
+                "type": "object",
+                "properties": {
+                    "b": {"type": "keyword", "facets": {"searchable": False}}
+                },
+            }
+        }
+    }
+    data = build_model(model)
+
+    assert data == {
+        "mappings": {
+            "properties": {
+                "a": {
+                    "type": "object",
+                    "enabled": False,
+                }
+            }
+        }
+    }
```

### Comparing `oarepo-model-builder-3.2.9/tests/test_loading.py` & `oarepo-model-builder-4.0.0/tests/test_loading.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,74 +3,80 @@
 from oarepo_model_builder.loaders import json_loader
 from oarepo_model_builder.schema import ModelSchema
 
 DUMMY_PATH = "/tmp/path.json"  # NOSONAR checking as it is a virtual path
 
 
 def test_loading_from_string():
-    schema = ModelSchema(DUMMY_PATH, {})
+    schema = ModelSchema(DUMMY_PATH, {}, validate=False)
     assert schema.schema == {"settings": {}}
 
 
 def test_loading_from_empty_file():
     schema = ModelSchema(
-        Path(__file__).parent.joinpath("data/empty.json"), loaders={"json": json_loader}
+        Path(__file__).parent.joinpath("data/empty.json"),
+        loaders={"json": json_loader},
+        validate=False,
     )
     assert schema.schema == {"settings": {}}
 
 
 def test_loading_included_resource():
     schema = ModelSchema(
         DUMMY_PATH,
         {"a": {"use": "test1"}},
         {"test1": lambda schema: {"included": "test1"}},
+        validate=False,
     )
     assert schema.schema == {
         "settings": {},
         "a": {"included": "test1"},
     }
 
 
 def test_loading_included_resource_root():
     schema = ModelSchema(
         DUMMY_PATH,
         {"use": "test1"},
         {"test1": lambda schema: {"included": "test1"}},
+        validate=False,
     )
     assert schema.schema == {
         "settings": {},
         "included": "test1",
     }
 
 
 def test_loading_jsonpath_resource():
     schema = ModelSchema(
         DUMMY_PATH,
         {"use": "test1#/test/a"},
         {"test1": lambda schema: {"test": {"a": {"included": "test1"}}}},
+        validate=False,
     )
     assert schema.schema == {
         "settings": {},
         "included": "test1",
     }
 
 
 def test_loading_current():
-    schema = ModelSchema(DUMMY_PATH, {"b": {"use": "#/a"}, "a": {"a": True}})
+    schema = ModelSchema(
+        DUMMY_PATH, {"b": {"use": "#/a"}, "a": {"a": True}}, validate=False
+    )
     assert schema.schema == {
         "settings": {},
         "b": {"a": True},
         "a": {"a": True},
     }
 
 
 def test_loading_current_by_id():
     schema = ModelSchema(
-        DUMMY_PATH,
-        {"b": {"use": "#id"}, "a": {"$id": "id", "a": True}},
+        DUMMY_PATH, {"b": {"use": "#id"}, "a": {"$id": "id", "a": True}}, validate=False
     )
     assert schema.schema == {
         "settings": {},
         "b": {"a": True},
         "a": {"$id": "id", "a": True},
     }
 
@@ -78,12 +84,13 @@
 def test_loading_external_by_id():
     schema = ModelSchema(
         DUMMY_PATH,
         {
             "b": {"use": "aa#id"},
         },
         {"aa": lambda schema: {"a": {"$id": "id", "a": True}}},
+        validate=False,
     )
     assert schema.schema == {
         "settings": {},
         "b": {"a": True},
     }
```

### Comparing `oarepo-model-builder-3.2.9/tests/test_marshmallow_builder.py` & `oarepo-model-builder-4.0.0/tests/test_marshmallow_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,57 @@
 import os
-import re
 
 import pytest
 
 from oarepo_model_builder.builder import ModelBuilder
 from oarepo_model_builder.fs import InMemoryFileSystem
-from oarepo_model_builder.invenio.invenio_record_schema import (
-    InvenioRecordSchemaBuilder,
-)
-from oarepo_model_builder.model_preprocessors.default_values import (
-    DefaultValuesModelPreprocessor,
-)
-from oarepo_model_builder.model_preprocessors.invenio import InvenioModelPreprocessor
-from oarepo_model_builder.model_preprocessors.opensearch import (
-    OpensearchModelPreprocessor,
+from oarepo_model_builder.invenio.invenio_record_marshmallow import (
+    InvenioRecordMarshmallowBuilder,
 )
 from oarepo_model_builder.outputs.python import PythonOutput
-from oarepo_model_builder.property_preprocessors.datatype_preprocessor import (
-    DataTypePreprocessor,
-)
 from oarepo_model_builder.schema import ModelSchema
 
+from .utils import strip_whitespaces
+
 OAREPO_MARSHMALLOW = "marshmallow"
-B_SCHEMA = 'classB(ma.Schema):"""Bschema."""b=ma_fields.String()'
 
 
 def get_test_schema(**props):
     return ModelSchema(
         "",
         {
             "settings": {
-                "python": {"use-isort": False, "use-black": False},
+                "python": {
+                    "use-isort": False,
+                    "use-black": False,
+                    "use-autoflake": False,
+                },
             },
-            "model": {"package": "test", "properties": props},
+            "record": {"module": {"qualified": "test"}, "properties": props},
         },
     )
 
 
 @pytest.fixture
 def fulltext_builder():
     return ModelBuilder(
-        output_builders=[InvenioRecordSchemaBuilder],
+        output_builders=[InvenioRecordMarshmallowBuilder],
         outputs=[PythonOutput],
-        model_preprocessors=[
-            DefaultValuesModelPreprocessor,
-            OpensearchModelPreprocessor,
-            InvenioModelPreprocessor,
-        ],
-        property_preprocessors=[DataTypePreprocessor],
     )
 
 
 def _test(fulltext_builder, string_type):
     schema = get_test_schema(a={"type": string_type})
     fulltext_builder.filesystem = InMemoryFileSystem()
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
     with fulltext_builder.filesystem.open(
-        os.path.join("test", "services", "records", "schema.py")
+        os.path.join("test", "services", "records", "schema.py")  # NOSONAR
     ) as f:
         data = f.read()
     assert "a = ma_fields.String()" in data
 
 
 def test_fulltext(fulltext_builder):
     _test(fulltext_builder, "fulltext")
@@ -74,15 +64,17 @@
 def test_fulltext_keyword(fulltext_builder):
     _test(fulltext_builder, "fulltext+keyword")
 
 
 def test_simple_array(fulltext_builder):
     schema = get_test_schema(a={"type": "array", "items": {"type": "keyword"}})
     fulltext_builder.filesystem = InMemoryFileSystem()
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
     with fulltext_builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ) as f:
         data = f.read()
     assert "a = ma_fields.List(ma_fields.String())" in data
 
@@ -91,204 +83,270 @@
     schema = get_test_schema(
         a={
             "type": "array",
             "items": {"type": "object", "properties": {"b": {"type": "integer"}}},
         }
     )
     fulltext_builder.filesystem = InMemoryFileSystem()
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
     with fulltext_builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ) as f:
         data = f.read()
     assert (
-        'class AItemSchema(ma.Schema):\n    """AItemSchema schema."""\n    b = ma_fields.Integer()'
-        in data
+        strip_whitespaces(
+            """
+class TestSchema(ma.Schema):
+    class Meta:
+        unknown = ma.RAISE
+    a = ma_fields.List(ma_fields.Nested(lambda: AItemSchema()))
+
+class AItemSchema(ma.Schema):
+    class Meta:
+        unknown = ma.RAISE
+    b = ma_fields.Integer()
+"""
+        )
+        in strip_whitespaces(data)
     )
-    assert "a = ma_fields.List(ma_fields.Nested(lambda: AItemSchema()))" in data
 
 
 def test_generate_nested_schema_same_file(fulltext_builder):
     schema = get_test_schema(
         a={
             "type": "object",
-            OAREPO_MARSHMALLOW: {"schema-class": "B", "generate": True},
+            OAREPO_MARSHMALLOW: {"class": "B", "generate": True},
             "properties": {
                 "b": {
                     "type": "keyword",
                 }
             },
         }
     )
     fulltext_builder.filesystem = InMemoryFileSystem()
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
     with fulltext_builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ) as f:
         data = f.read()
     assert (
-        re.sub(
-            r"\s",
-            "",
-            """class B(ma.Schema):
-        \"""B schema.\"""
-        
-        b = ma_fields.String()""",
-        )
-        in re.sub(r"\s", "", data)
-    )
-    assert (
-        re.sub(
-            r"\s",
-            "",
-            """class TestSchema(ma.Schema):
-        \"""TestSchema schema.\"""
-        
-        a = ma_fields.Nested(lambda: B())""",
+        strip_whitespaces(
+            """
+class TestSchema(ma.Schema):
+
+    class Meta:
+        unknown = ma.RAISE
+
+
+    a = ma_fields.Nested(lambda: BSchema())
+
+
+class BSchema(ma.Schema):
+
+    class Meta:
+        unknown = ma.RAISE
+
+
+    b = ma_fields.String()        
+        """
         )
-        in re.sub(r"\s", "", data)
+        in strip_whitespaces(data)
     )
 
 
 def test_generate_nested_schema_different_file(fulltext_builder):
     schema = get_test_schema(
         a={
             "type": "object",
             OAREPO_MARSHMALLOW: {
-                "schema-class": "test.services.schema2.B",
+                "class": "test.services.schema2.B",
                 "generate": True,
             },
             "properties": {
                 "b": {
                     "type": "keyword",
                 }
             },
         }
     )
     fulltext_builder.filesystem = InMemoryFileSystem()
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
     with fulltext_builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ) as f:
         data = f.read()
 
     assert (
-        re.sub(
-            r"\s",
-            "",
-            """class TestSchema(ma.Schema):
-        \"""TestSchema schema.\"""
-    
-        a = ma_fields.Nested(lambda: B())""",
+        strip_whitespaces(
+            """
+from test.services.schema2 import BSchema
+
+class TestSchema(ma.Schema):
+    class Meta:
+        unknown = ma.RAISE
+    a = ma_fields.Nested(lambda: BSchema())        
+        """
         )
-        in re.sub(r"\s", "", data)
+        in strip_whitespaces(data)
     )
 
-    assert "from test.services.schema2 import B" in data
-
     with fulltext_builder.filesystem.open(
-        os.path.join("test", "services", "schema2.py")
+        os.path.join("test", "services", "schema2.py")  # NOSONAR
     ) as f:
         data = f.read()
-    assert B_SCHEMA in re.sub(r"\s", "", data)
+
+    assert (
+        strip_whitespaces(
+            """
+class BSchema(ma.Schema):
+    class Meta:
+        unknown = ma.RAISE
+
+    b = ma_fields.String()       
+        """
+        )
+        in strip_whitespaces(data)
+    )
 
 
 def test_use_nested_schema_same_file(fulltext_builder):
     schema = get_test_schema(
         a={
             "type": "object",
-            OAREPO_MARSHMALLOW: {"schema-class": "B", "generate": False},
+            OAREPO_MARSHMALLOW: {"class": "B", "generate": False},
             "properties": {
                 "b": {
                     "type": "keyword",
                 }
             },
         }
     )
     fulltext_builder.filesystem = InMemoryFileSystem()
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
     with fulltext_builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ) as f:
         data = f.read()
         print(data)
     assert (
-        re.sub(
-            r"\s",
-            "",
-            """class TestSchema(ma.Schema):
-        \"""TestSchema schema.\"""
-        
-        a = ma_fields.Nested(lambda: B())""",
+        strip_whitespaces(
+            """
+class TestSchema(ma.Schema):
+
+    class Meta:
+        unknown = ma.RAISE
+
+
+    a = ma_fields.Nested(lambda: B())"""
         )
-        in re.sub(r"\s", "", data)
+        in strip_whitespaces(data)
     )
-    assert "classB(ma.Schema)" not in re.sub(r"\s", "", data)
+    assert strip_whitespaces("class B") not in strip_whitespaces(data)
 
 
 def test_use_nested_schema_different_file(fulltext_builder):
     schema = get_test_schema(
         a={
             "type": "object",
-            OAREPO_MARSHMALLOW: {"schema-class": "c.B", "generate": False},
+            OAREPO_MARSHMALLOW: {"class": "c.B", "generate": False},
             "properties": {
                 "b": {
                     "type": "keyword",
                 }
             },
         }
     )
     fulltext_builder.filesystem = InMemoryFileSystem()
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
     with fulltext_builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ) as f:
         data = f.read()
-    assert re.sub(r"\s", "", "from c import B") in re.sub(r"\s", "", data)
+    assert strip_whitespaces("from c import B") in strip_whitespaces(data)
     assert (
-        'classTestSchema(ma.Schema):"""TestSchemaschema."""a=ma_fields.Nested(lambda:B())'
-        in re.sub(r"\s", "", data)
+        strip_whitespaces(
+            """
+class TestSchema(ma.Schema):
+
+    class Meta:
+        unknown = ma.RAISE
+
+
+    a = ma_fields.Nested(lambda: B())"""
+        )
+        in strip_whitespaces(data)
     )
 
 
 def test_generate_nested_schema_array(fulltext_builder):
     schema = get_test_schema(
         a={
             "type": "array",
             "items": {
                 "type": "object",
-                OAREPO_MARSHMALLOW: {"schema-class": "B", "generate": True},
+                OAREPO_MARSHMALLOW: {"class": "B", "generate": True},
                 "properties": {
                     "b": {
                         "type": "keyword",
                     }
                 },
             },
         }
     )
     fulltext_builder.filesystem = InMemoryFileSystem()
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
     with fulltext_builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ) as f:
         data = f.read()
-    assert B_SCHEMA in re.sub(r"\s", "", data)
     assert (
-        'classTestSchema(ma.Schema):"""TestSchemaschema."""a=ma_fields.List(ma_fields.Nested(lambda:B()))'
-        in re.sub(r"\s", "", data)
+        strip_whitespaces(
+            """
+class TestSchema(ma.Schema):
+
+    class Meta:
+        unknown = ma.RAISE
+
+
+    a = ma_fields.List(ma_fields.Nested(lambda: BSchema()))
+
+
+class BSchema(ma.Schema):
+
+    class Meta:
+        unknown = ma.RAISE
+
+
+    b = ma_fields.String()
+        """
+        )
+        in strip_whitespaces(data)
     )
 
 
 def test_extend_existing(fulltext_builder):
+    "Test that if there is a marshmallow file present on the filesystem it gets extended"
     schema = get_test_schema(a={"type": "keyword"}, b={"type": "keyword"})
     fulltext_builder.filesystem = InMemoryFileSystem()
 
     with fulltext_builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py"), "w"
     ) as f:
         f.write(
@@ -298,136 +356,185 @@
 import marshmallow.fields as ma_fields
 import marshmallow.validate as ma_valid
 class TestSchema(ma.Schema):
     """TestSchema schema."""
     a = ma_fields.String()'''
         )
 
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
     data = fulltext_builder.filesystem.read(
         os.path.join("test", "services", "records", "schema.py")
     )
     assert "b = ma_fields.String()" in data
 
 
 def test_generate_nested_schema_relative_same_package(fulltext_builder):
     schema = get_test_schema(
         a={
             "type": "object",
             OAREPO_MARSHMALLOW: {
-                "schema-class": ".schema2.B",
+                "class": "..schema2.B",
                 "generate": True,
             },
             "properties": {
                 "b": {
                     "type": "keyword",
                 }
             },
         }
     )
     fulltext_builder.filesystem = InMemoryFileSystem()
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
     with fulltext_builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ) as f:
         data = f.read()
 
     assert (
-        re.sub(
-            r"\s",
-            "",
-            """class TestSchema(ma.Schema):
-        \"""TestSchema schema.\"""
-    
-        a = ma_fields.Nested(lambda:B())""",
+        strip_whitespaces(
+            """
+
+from test.services.records.schema2 import BSchema
+
+class TestSchema(ma.Schema):
+
+    class Meta:
+        unknown = ma.RAISE
+
+
+    a = ma_fields.Nested(lambda: BSchema())        
+        """
         )
-        in re.sub(r"\s", "", data)
+        in strip_whitespaces(data)
     )
 
-    assert "from test.services.records.schema2 import B" in data
-
     with fulltext_builder.filesystem.open(
         os.path.join("test", "services", "records", "schema2.py")
     ) as f:
         data = f.read()
-    assert B_SCHEMA in re.sub(r"\s", "", data)
+    assert (
+        strip_whitespaces(
+            """
+class BSchema(ma.Schema):
+
+    class Meta:
+        unknown = ma.RAISE
+
+
+    b = ma_fields.String()        
+        """
+        )
+        in strip_whitespaces(data)
+    )
 
 
 def test_generate_nested_schema_relative_same_file(fulltext_builder):
     schema = get_test_schema(
         a={
             "type": "object",
             OAREPO_MARSHMALLOW: {
-                "schema-class": ".B",
+                "class": ".B",
                 "generate": True,
             },
             "properties": {
                 "b": {
                     "type": "keyword",
                 }
             },
         }
     )
     fulltext_builder.filesystem = InMemoryFileSystem()
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
     with fulltext_builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ) as f:
         data = f.read()
 
     assert (
-        re.sub(
-            r"\s",
-            "",
-            """class TestSchema(ma.Schema):
-        \"""TestSchema schema.\"""
+        strip_whitespaces(
+            """
+class TestSchema(ma.Schema):
+
+    class Meta:
+        unknown = ma.RAISE
+
+
+    a = ma_fields.Nested(lambda: BSchema())
+
 
-        a = ma_fields.Nested(lambda:B())""",
+class BSchema(ma.Schema):
+
+    class Meta:
+        unknown = ma.RAISE
+
+
+    b = ma_fields.String()
+            """
         )
-        in re.sub(r"\s", "", data)
+        in strip_whitespaces(data)
     )
 
 
 def test_generate_nested_schema_relative_upper(fulltext_builder):
     schema = get_test_schema(
         a={
             "type": "object",
             OAREPO_MARSHMALLOW: {
-                "schema-class": "..schema2.B",
+                "class": "...schema2.B",
                 "generate": True,
             },
             "properties": {
                 "b": {
                     "type": "keyword",
                 }
             },
         }
     )
     fulltext_builder.filesystem = InMemoryFileSystem()
-    fulltext_builder.build(schema, output_dir="")
+    fulltext_builder.build(
+        schema, profile="record", model_path=["record"], output_dir=""
+    )
 
     with fulltext_builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ) as f:
         data = f.read()
 
     assert (
-        re.sub(
-            r"\s",
-            "",
-            """class TestSchema(ma.Schema):
-        \"""TestSchema schema.\"""
+        strip_whitespaces(
+            """
+from test.services.schema2 import BSchema
+class TestSchema(ma.Schema):
+    class Meta:
+        unknown = ma.RAISE
 
-        a = ma_fields.Nested(lambda: B())""",
+    a = ma_fields.Nested(lambda: BSchema())
+        """
         )
-        in re.sub(r"\s", "", data)
+        in strip_whitespaces(data)
     )
 
-    assert "from test.services.schema2 import B" in data
-
     with fulltext_builder.filesystem.open(
         os.path.join("test", "services", "schema2.py")
     ) as f:
         data = f.read()
-    assert B_SCHEMA in re.sub(r"\s", "", data)
+    assert (
+        strip_whitespaces(
+            """
+class BSchema(ma.Schema):
+
+    class Meta:
+        unknown = ma.RAISE
+
+    b = ma_fields.String()
+        """
+        )
+        in strip_whitespaces(data)
+    )
```

### Comparing `oarepo-model-builder-3.2.9/tests/test_merge.py` & `oarepo-model-builder-4.0.0/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-3.2.9/tests/test_python_mergers.py` & `oarepo-model-builder-4.0.0/tests/test_python_mergers.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import libcst as cst
 
 from oarepo_model_builder.utils.cst import PythonContext, merge
 
 
 def test_new_class():
-    existing_module = "# comment start"
+    existing_module = "# comment start"  # NOSONAR
     included_module = """
 # comment before
 class Blah:
     # comment
     pass    
     """.strip()
     original_cst = cst.parse_module(existing_module)
@@ -241,21 +241,15 @@
             """.strip()
     original_cst = cst.parse_module(existing_module)
     included_cst = cst.parse_module(
         included_module, config=original_cst.config_for_parsing
     )
     transformed_cst = merge(PythonContext(included_cst), original_cst, included_cst)
 
-    assert (
-        transformed_cst.code.strip()
-        == """
-AAA = "123"
-BBB = "456"
-            """.strip()
-    )
+    assert transformed_cst.code.strip() == included_module
 
 
 def test_top_level_merged_vars():
     existing_module = "CCC='456'"
     included_module = """
 AAA = "123"
 BBB = "456"
@@ -321,15 +315,15 @@
     """
     original_cst = cst.parse_module(existing_module)
     included_cst = cst.parse_module(
         included_module, config=original_cst.config_for_parsing
     )
     transformed_cst = merge(PythonContext(included_cst), original_cst, included_cst)
 
-    assert re.sub(r"[\t\n ]", "", transformed_cst.code) == re.sub(
+    assert re.sub(r"[\t\n ]", "", transformed_cst.code) == re.sub(  # NOSONAR
         r"[\t\n ]",
         "",
         """
 class A:
 CCC=[1,2,3,4,5,6]
             """,
     )
```

### Comparing `oarepo-model-builder-3.2.9/tests/test_raw.py` & `oarepo-model-builder-4.0.0/tests/test_raw.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,89 @@
 import json
 import os
-import re
-from pathlib import Path
 
 from oarepo_model_builder.entrypoints import create_builder_from_entrypoints, load_model
 from oarepo_model_builder.fs import InMemoryFileSystem
-from tests.utils import assert_python_equals
+
+from .utils import strip_whitespaces
 
 
 def test_raw_type():
     schema = load_model(
         "test.yaml",
-        "test",
         model_content={
-            "model": {"use": "invenio", "properties": {"a": {"type": "flatten"}}},
+            "record": {
+                "use": "invenio",
+                "properties": {"a": {"type": "flattened"}},
+                "module": {"qualified": "test"},
+            },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ).read()
-    print(data)
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
-        """
+    assert (
+        strip_whitespaces(
+            """
 from invenio_records_resources.services.records.schema import BaseRecordSchema as InvenioBaseRecordSchema
 from marshmallow import ValidationError
-from marshmallow import validates as ma_validates
+from marshmallow import validate as ma_validate
 import marshmallow as ma
 from marshmallow import fields as ma_fields
 from marshmallow_utils import fields as mu_fields
 from marshmallow_utils import schemas as mu_schemas
-from oarepo_runtime.validation import validate_date
 class TestSchema(InvenioBaseRecordSchema):
-    \"""TestSchema schema.\"""
+    class Meta:
+        unknown = ma.RAISE
     a = ma_fields.Raw()
-    created = ma_fields.String(validate=[validate_date('%Y-%m-%d')], dump_only=True)
-    updated = ma_fields.String(validate=[validate_date('%Y-%m-%d')], dump_only=True)
-    """,
+    """
+        )
+        in strip_whitespaces(data)
     )
 
     data = builder.filesystem.read(
         os.path.join("test", "records", "mappings", "os-v2", "test", "test-1.0.0.json")
     )
     data = json.loads(data)
 
     assert data == {
         "mappings": {
             "properties": {
-                "a": {"type": "flatten"},
+                "a": {"type": "object", "enabled": False},
                 "id": {"type": "keyword"},
-                "created": {"type": "date"},
-                "updated": {"type": "date"},
+                "created": {
+                    "type": "date",
+                    "format": "strict_date_time||strict_date_time_no_millis",
+                },
+                "updated": {
+                    "type": "date",
+                    "format": "strict_date_time||strict_date_time_no_millis",
+                },
                 "$schema": {"type": "keyword"},
             },
         }
     }
 
     data = builder.filesystem.read(
         os.path.join("test", "records", "jsonschemas", "test-1.0.0.json")
     )
     data = json.loads(data)
     print(data)
     assert data == {
         "properties": {
             "a": {"type": "object"},
             "id": {"type": "string"},
-            "created": {"type": "string", "format": "date"},
-            "updated": {"type": "string", "format": "date"},
+            "created": {"type": "string", "format": "date-time"},
+            "updated": {"type": "string", "format": "date-time"},
             "$schema": {"type": "string"},
         },
         "type": "object",
     }
```

### Comparing `oarepo-model-builder-3.2.9/tests/test_sample_builder.py` & `oarepo-model-builder-4.0.0/tests/test_sample_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-from pathlib import Path
-
 import faker.config
 
-from oarepo_model_builder.entrypoints import create_builder_from_entrypoints
+from oarepo_model_builder.builder import ModelBuilder
 from oarepo_model_builder.fs import InMemoryFileSystem
-from oarepo_model_builder.invenio.invenio_script_sample_data import (
-    InvenioScriptSampleDataBuilder,
-)
+from oarepo_model_builder.invenio.invenio_script_sample_data import SampleDataBuilder
+from oarepo_model_builder.outputs.yaml import YAMLOutput
 from oarepo_model_builder.schema import ModelSchema
 
 
 def test_sample_builder_string():
     assert (
         build_sample_data(
             {
                 "a": {
-                    "type": "string",
+                    "type": "keyword",
                 }
             }
         )
         == "a: test\n"
     )
     assert (
         build_sample_data(
             {
                 "a": {
-                    "type": "string",
+                    "type": "keyword",
                 }
             },
             count=2,
         )
         == "a: test\n---\na: test\n"
     )
 
@@ -48,15 +45,15 @@
 
 
 def test_sample_builder_float():
     assert (
         build_sample_data(
             {
                 "a": {
-                    "type": "number",
+                    "type": "float",
                 }
             }
         )
         == "a: 1.2\n"
     )
 
 
@@ -77,18 +74,18 @@
     assert (
         build_sample_data(
             {
                 "obj": {
                     "type": "object",
                     "properties": {
                         "a": {
-                            "type": "string",
+                            "type": "keyword",
                         },
                         "b": {
-                            "type": "string",
+                            "type": "keyword",
                         },
                     },
                 }
             }
         ).strip()
         == """
 obj:
@@ -101,29 +98,29 @@
 def test_sample_builder_simple_array():
     assert (
         build_sample_data(
             {
                 "a": {
                     "type": "array",
                     "sample": {"count": 1},
-                    "items": {"type": "string"},
+                    "items": {"type": "keyword"},
                 }
             }
         )
         == "a:\n- test\n"
     )
 
     # makes items unique, so expect one
     assert (
         build_sample_data(
             {
                 "a": {
                     "type": "array",
                     "sample": {"count": 2},
-                    "items": {"type": "string"},
+                    "items": {"type": "keyword"},
                 }
             }
         )
         == "a:\n- test\n"
     )
 
 
@@ -135,18 +132,18 @@
                 "a": {
                     "type": "array",
                     "sample": {"count": 2},
                     "items": {
                         "type": "object",
                         "properties": {
                             "b": {
-                                "type": "string",
+                                "type": "keyword",
                             },
                             "c": {
-                                "type": "string",
+                                "type": "keyword",
                             },
                         },
                     },
                 }
             }
         ).strip()
         == """
@@ -156,25 +153,28 @@
     """.strip()
     )
 
 
 def build_sample_data(model, count=1):
     faker.config.PROVIDERS.clear()
     faker.config.PROVIDERS.append("tests.faker_constant")
-    builder = create_builder_from_entrypoints()
-    builder.filesystem = InMemoryFileSystem()
-    builder.output_dir = Path.cwd()
-    sample_builder = InvenioScriptSampleDataBuilder(
-        builder=builder, property_preprocessors=[]
+    builder = ModelBuilder(
+        output_builders=[SampleDataBuilder],
+        outputs=[YAMLOutput],
+        filesystem=InMemoryFileSystem(),
     )
     schema = ModelSchema(
         "test.json",
         {
-            "model": {"script-import-sample-data": "test.yaml", "properties": model},
+            "record": {
+                "sample": {"file": "test.yaml", "count": count},
+                "module": {"qualified": "test"},
+                "properties": {
+                    **model,
+                },
+            },
             "settings": {},
-            "sample": {"count": count},
         },
     )
-    sample_builder.build(schema)
-    builder._save_outputs()
+    builder.build(schema, "record", ["record"], output_dir="")
     sample_data = builder.filesystem.read("test.yaml")
     return sample_data
```

### Comparing `oarepo-model-builder-3.2.9/tests/test_schema_props.py` & `oarepo-model-builder-4.0.0/tests/test_search_options.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,125 @@
-import json
 import os
 import re
-from pathlib import Path
+
+import pytest
 
 from oarepo_model_builder.entrypoints import create_builder_from_entrypoints, load_model
 from oarepo_model_builder.fs import InMemoryFileSystem
-from tests.utils import assert_python_equals
 
+pytestmark = pytest.mark.skip()  # skip the tests for now ...
+
+
+DUMMY_YAML = "test.yaml"
 
-def test_enum():
+
+def test_sort():
     schema = load_model(
-        "test.yaml",
-        "test",
+        DUMMY_YAML,
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
-                "properties": {"a": {"type": "keyword", "enum": ["a", "b", "c"]}},
+                "properties": {
+                    "a": {
+                        "type": "fulltext+keyword",
+                        "sortable": {"key": "a_test"},
+                    },
+                    "b": {
+                        "type": "keyword",
+                        "facets": {"field": 'TermsFacet(field="cosi")'},
+                        "sortable": {"key": "b_test", "order": "desc"},
+                    },
+                },
             },
         },
         isort=False,
         black=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
-
     builder.build(schema, "")
 
     data = builder.filesystem.open(
-        os.path.join("test", "services", "records", "schema.py")
+        os.path.join("test", "services", "records", "search.py")
     ).read()
-    print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
-from invenio_records_resources.services.records.schema import BaseRecordSchema as InvenioBaseRecordSchema
-from marshmallow import ValidationError
-from marshmallow import validates as ma_validates
-import marshmallow as ma
-from marshmallow import fields as ma_fields
-from marshmallow_utils import fields as mu_fields
-from marshmallow_utils import schemas as mu_schemas
-
-from oarepo_runtime.validation import validate_date
-
-class TestSchema(InvenioBaseRecordSchema):
-    \"""TestSchema schema.\"""
-    
-    a = ma_fields.String(validate=[ma_valid.OneOf(["a", "b", "c"])])
-    created = ma_fields.String(validate=[validate_date('%Y-%m-%d')], dump_only=True)
-    updated = ma_fields.String(validate=[validate_date('%Y-%m-%d')], dump_only=True)
-""",
+from invenio_records_resources.services import SearchOptions as InvenioSearchOptions
+from flask_babelex import lazy_gettext as _
+from . import facets
+
+class TestSearchOptions(InvenioSearchOptions):
+    \"""TestRecord search options.\"""
+
+    facets = {
+    'a_keyword': facets.a_keyword,
+    'b': facets.b,
+    '_id': facets._id,
+    'created': facets.created,
+    'updated': facets.updated,
+    '_schema': facets._schema,
+    }
+    sort_options = {
+        **InvenioSearchOptions.sort_options,
+    'a_test': {'fields': ['a']},
+    'b_test': {'fields': ['-b']},
+    }
+    """,
     )
 
-    data = builder.filesystem.read(
-        os.path.join("test", "records", "jsonschemas", "test-1.0.0.json")
+
+def test_search_class():
+    schema = load_model(
+        DUMMY_YAML,
+        model_content={
+            "record": {
+                "use": "invenio",
+                "properties": {
+                    "a": {"type": "fulltext+keyword"},
+                    "b": {
+                        "type": "keyword",
+                        "facets": {"field": 'TermsFacet(field="cosi")'},
+                    },
+                },
+            },
+        },
+        isort=False,
+        black=False,
     )
-    data = json.loads(data)
+
+    filesystem = InMemoryFileSystem()
+    builder = create_builder_from_entrypoints(filesystem=filesystem)
+
+    builder.build(schema, "")
+
+    data = builder.filesystem.open(
+        os.path.join("test", "services", "records", "search.py")
+    ).read()
     print(data)
-    assert data == {
-        "properties": {
-            "$schema": {"type": "string"},
-            "a": {"type": "string", "enum": ["a", "b", "c"]},
-            "created": {"format": "date", "type": "string"},
-            "id": {"type": "string"},
-            "updated": {"format": "date", "type": "string"},
-        },
-        "type": "object",
-    }
+    assert re.sub(r"\s", "", data) == re.sub(
+        r"\s",
+        "",
+        """
+from invenio_records_resources.services import SearchOptions as InvenioSearchOptions
+from flask_babelex import lazy_gettext as _
+from . import facets
 
-    data = builder.filesystem.read(
-        os.path.join("test", "records", "mappings", "os-v2", "test", "test-1.0.0.json")
-    )
-    data = json.loads(data)
-    assert data == {
-        "mappings": {
-            "properties": {
-                "$schema": {"type": "keyword"},
-                "a": {"type": "keyword"},
-                "created": {"type": "date"},
-                "id": {"type": "keyword"},
-                "updated": {"type": "date"},
-            }
-        }
+
+class TestSearchOptions(InvenioSearchOptions):
+    \"""TestRecord search options.\"""
+
+    facets = {
+      'a_keyword': facets.a_keyword,
+      'b': facets.b,
+      '_id': facets._id,
+      'created': facets.created,
+      'updated': facets.updated,
+      '_schema': facets._schema,
     }
+    sort_options = {
+        **InvenioSearchOptions.sort_options,
+    }
+    """,
+    )
```

### Comparing `oarepo-model-builder-3.2.9/tests/test_shortcuts.py` & `oarepo-model-builder-4.0.0/tests/test_shortcuts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,186 +1,191 @@
 import json
 import os
-import re
-from pathlib import Path
 
 import yaml
 
 from oarepo_model_builder.entrypoints import create_builder_from_entrypoints, load_model
 from oarepo_model_builder.fs import InMemoryFileSystem
-from tests.utils import assert_python_equals
+
+from .utils import strip_whitespaces
 
 
 def test_array_shortcuts():
     schema = load_model(
         "test.yaml",  # NOSONAR
-        "test",
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
                 "properties": {"a[]": {"type": "keyword", "^required": True}},
+                "module": {"qualified": "test"},
             },
         },
         isort=False,
         black=False,
+        autoflake=False,
     )
 
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
     data = builder.filesystem.open(
         os.path.join("test", "services", "records", "schema.py")
     ).read()
-    print(data)
-    assert re.sub(r"\s", "", data) == re.sub(
-        r"\s",
-        "",
-        """
-from invenio_records_resources.services.records.schema import BaseRecordSchema as InvenioBaseRecordSchema
-from marshmallow import ValidationError
-from marshmallow import validates as ma_validates
-import marshmallow as ma
-from marshmallow import fields as ma_fields
-from marshmallow_utils import fields as mu_fields
-from marshmallow_utils import schemas as mu_schemas
+    assert (
+        strip_whitespaces(
+            """
+class TestSchema(InvenioBaseRecordSchema):
 
-from oarepo_runtime.validation import validate_date
+    class Meta:
+        unknown = ma.RAISE
 
-class TestSchema(InvenioBaseRecordSchema):
-    \"""TestSchema schema.\"""
-    a = ma_fields.List(ma_fields.String())        
-    created = ma_fields.String(validate=[validate_date('%Y-%m-%d')], dump_only=True)
-    updated = ma_fields.String(validate=[validate_date('%Y-%m-%d')], dump_only=True)
-    """,
+
+    a = ma_fields.List(ma_fields.String())    
+    """
+        )
+        in strip_whitespaces(data)
     )
 
     data = builder.filesystem.read(
         os.path.join("test", "records", "mappings", "os-v2", "test", "test-1.0.0.json")
     )
     data = json.loads(data)
     assert data == {
         "mappings": {
             "properties": {
                 "$schema": {"type": "keyword"},
-                "a": {
-                    "type": "keyword",
+                "a": {"type": "keyword"},
+                "created": {
+                    "type": "date",
+                    "format": "strict_date_time||strict_date_time_no_millis",
                 },
-                "created": {"type": "date"},
                 "id": {"type": "keyword"},
-                "updated": {"type": "date"},
+                "updated": {
+                    "type": "date",
+                    "format": "strict_date_time||strict_date_time_no_millis",
+                },
             }
         }
     }
 
     data = builder.filesystem.read(
         os.path.join("test", "records", "jsonschemas", "test-1.0.0.json")
     )
     data = json.loads(data)
     assert data == {
         "properties": {
             "$schema": {"type": "string"},
             "a": {"items": {"type": "string"}, "type": "array"},
-            "created": {"format": "date", "type": "string"},
+            "created": {"format": "date-time", "type": "string"},
             "id": {"type": "string"},
-            "updated": {"format": "date", "type": "string"},
+            "updated": {"format": "date-time", "type": "string"},
         },
-        "required": ["a"],
         "type": "object",
     }
 
 
 def test_singleline_type_shortcut():
     data = """
-model:
+record:
   properties:
     metadata:
       properties:
         title: fulltext
+  module:
+    qualified: test
 """
 
     schema = load_model(
         "test.yaml",
-        "test",
         model_content=yaml.safe_load(data),
         isort=False,
         black=False,
+        autoflake=False,
     )
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
 
 def test_object_shortcut():
     data = """
-model:
+record:
   properties:
     metadata{}:
       title: fulltext
+  module:
+    qualified: test
 """
 
     schema = load_model(
         "test.yaml",
-        "test",
         model_content=yaml.safe_load(data),
         isort=False,
         black=False,
+        autoflake=False,
     )
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
 
 def test_array_shortcut():
     data = """
-model:
+record:
+  module:
+    qualified: test
   properties:
     metadata[]:
       type: fulltext
 """
 
     schema = load_model(
         "test.yaml",
-        "test",
         model_content=yaml.safe_load(data),
         isort=False,
         black=False,
+        autoflake=False,
     )
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
 
 def test_array_single_line_shortcut():
     data = """
-model:
+record:
+  module:
+    qualified: test
   properties:
     metadata[]: fulltext
 """
 
     schema = load_model(
         "test.yaml",
-        "test",
         model_content=yaml.safe_load(data),
         isort=False,
         black=False,
+        autoflake=False,
     )
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
 
 
 def test_misc_shortcuts():
     data = """
-model:
+record:
+  module:
+    qualified: test
   properties:
     metadata:
       properties:
         title: fulltext
 """
     """
       description: fulltext+keyword
@@ -194,16 +199,16 @@
       "sources{nested}[]":
         source: fulltext
         period: edtf-interval
 """
 
     schema = load_model(
         "test.yaml",
-        "test",
         model_content=yaml.safe_load(data),
         isort=False,
         black=False,
+        autoflake=False,
     )
     filesystem = InMemoryFileSystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
-    builder.build(schema, "")
+    builder.build(schema, "record", ["record"], "")
```

### Comparing `oarepo-model-builder-3.2.9/tests/test_type_shortcuts.py` & `oarepo-model-builder-4.0.0/tests/test_type_shortcuts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 import os
 
 import json5
 
 from oarepo_model_builder.builder import ModelBuilder
 from oarepo_model_builder.builders.jsonschema import JSONSchemaBuilder
 from oarepo_model_builder.fs import InMemoryFileSystem
-from oarepo_model_builder.model_preprocessors.default_values import (
-    DefaultValuesModelPreprocessor,
-)
 from oarepo_model_builder.outputs.jsonschema import JSONSchemaOutput
 from oarepo_model_builder.outputs.python import PythonOutput
 from oarepo_model_builder.schema import ModelSchema
 
 
 def test_object():
     data = build_jsonschema(
         {"properties": {"a": {"properties": {"b": {"type": "keyword"}}}}}
     )
 
     assert data == {
         "type": "object",
         "properties": {
-            "a": {"type": "object", "properties": {"b": {"type": "keyword"}}}
+            "a": {"type": "object", "properties": {"b": {"type": "string"}}}
         },
     }
 
 
 def test_array():
     data = build_jsonschema({"properties": {"a": {"items": {"type": "keyword"}}}})
 
     assert data == {
         "type": "object",
-        "properties": {"a": {"type": "array", "items": {"type": "keyword"}}},
+        "properties": {"a": {"type": "array", "items": {"type": "string"}}},
     }
 
 
 def test_object_inside_array():
     data = build_jsonschema(
         {"properties": {"a": {"items": {"properties": {"b": {"type": "keyword"}}}}}}
     )
 
     assert data == {
         "type": "object",
         "properties": {
             "a": {
                 "type": "array",
-                "items": {"type": "object", "properties": {"b": {"type": "keyword"}}},
+                "items": {"type": "object", "properties": {"b": {"type": "string"}}},
             }
         },
     }
 
 
 def test_array_brackets():
     data = build_jsonschema(
@@ -57,39 +54,42 @@
     )
 
     assert data == {
         "type": "object",
         "properties": {
             "a": {
                 "type": "array",
-                "minItems": 5,
-                "items": {"type": "keyword"},
+                "items": {"type": "string"},
             }
         },
     }
 
 
 def build_jsonschema(model):
     builder = ModelBuilder(
         output_builders=[JSONSchemaBuilder],
         outputs=[JSONSchemaOutput, PythonOutput],
-        model_preprocessors=[DefaultValuesModelPreprocessor],
-        property_preprocessors=[],
         filesystem=InMemoryFileSystem(),
     )
     builder.build(
         model=ModelSchema(
             "",
             {
                 "settings": {
-                    "python": {"use-isort": False, "use-black": False},
+                    "python": {
+                        "use-isort": False,
+                        "use-black": False,
+                        "use-autoflake": False,
+                    },
                 },
-                "model": {"package": "test", **model},
+                "record": {"module": {"qualified": "test"}, **model},
             },
         ),
+        profile="record",
+        model_path=["record"],
         output_dir="",
     )
     return json5.load(
         builder.filesystem.open(
             os.path.join("test", "records", "jsonschemas", "test-1.0.0.json")
         )
     )
```

