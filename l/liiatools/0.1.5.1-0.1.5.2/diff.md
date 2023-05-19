# Comparing `tmp/liiatools-0.1.5.1.tar.gz` & `tmp/liiatools-0.1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liiatools-0.1.5.1.tar", max compression
+gzip compressed data, was "liiatools-0.1.5.2.tar", max compression
```

## Comparing `liiatools-0.1.5.1.tar` & `liiatools-0.1.5.2.tar`

### file list

```diff
@@ -1,129 +1,143 @@
--rw-r--r--   0        0        0     1084 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/LICENSE
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/__init__.py
--rw-r--r--   0        0        0      434 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/__main__.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/csdatatools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/csdatatools/datasets/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/csdatatools/datasets/cincensus/__init__.py
--rw-r--r--   0        0        0     4364 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/csdatatools/datasets/cincensus/filters.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/csdatatools/util/__init__.py
--rw-r--r--   0        0        0      280 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/csdatatools/util/stream.py
--rw-r--r--   0        0        0     1640 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/csdatatools/util/xml.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/__init__.py
--rw-r--r--   0        0        0      131 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/README.md
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/__init__.py
--rw-r--r--   0        0        0     7047 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/annex_a_cli.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/__init__.py
--rw-r--r--   0        0        0     4908 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/cleaner.py
--rw-r--r--   0        0        0    11751 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/configuration.py
--rw-r--r--   0        0        0      451 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/converters.py
--rw-r--r--   0        0        0     1381 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/degrade.py
--rw-r--r--   0        0        0     5122 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/file_creator.py
--rw-r--r--   0        0        0    12608 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/logger.py
--rw-r--r--   0        0        0      772 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/populate.py
--rw-r--r--   0        0        0      885 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/regex.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_la_agg/__init__.py
--rw-r--r--   0        0        0     2495 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_la_agg/configuration.py
--rw-r--r--   0        0        0     3052 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_la_agg/process.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_pan_agg/__init__.py
--rw-r--r--   0        0        0     2894 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_pan_agg/configuration.py
--rw-r--r--   0        0        0     2066 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_pan_agg/process.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/__init__.py
--rw-r--r--   0        0        0    11514 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/cin_cli.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/__init__.py
--rw-r--r--   0        0        0     6065 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/cin_record.py
--rw-r--r--   0        0        0     2644 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/configuration.py
--rw-r--r--   0        0        0      811 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/converter.py
--rw-r--r--   0        0        0     2906 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/file_creator.py
--rw-r--r--   0        0        0     6012 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/logger.py
--rw-r--r--   0        0        0      410 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/schema.py
--rw-r--r--   0        0        0     3860 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/validator.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_la_agg/__init__.py
--rw-r--r--   0        0        0     2487 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_la_agg/configuration.py
--rw-r--r--   0        0        0    10532 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_la_agg/process.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_pan_agg/__init__.py
--rw-r--r--   0        0        0     2885 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_pan_agg/configuration.py
--rw-r--r--   0        0        0    10132 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_pan_agg/process.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/__init__.py
--rw-r--r--   0        0        0     1547 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/columns.py
--rw-r--r--   0        0        0     5105 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/configuration.py
--rw-r--r--   0        0        0     1612 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/converters.py
--rw-r--r--   0        0        0     1248 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/degrade.py
--rw-r--r--   0        0        0     2993 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/file_creator.py
--rw-r--r--   0        0        0     3184 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/filters.py
--rw-r--r--   0        0        0     8547 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/logger.py
--rw-r--r--   0        0        0     1189 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/parse.py
--rw-r--r--   0        0        0     2000 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/populate.py
--rw-r--r--   0        0        0     5080 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/prep.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_la_agg/__init__.py
--rw-r--r--   0        0        0     2486 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_la_agg/configuration.py
--rw-r--r--   0        0        0     2425 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_la_agg/process.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_pan_agg/__init__.py
--rw-r--r--   0        0        0     2885 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_pan_agg/configuration.py
--rw-r--r--   0        0        0     1482 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_pan_agg/process.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_sufficiency/__init__.py
--rw-r--r--   0        0        0     2491 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_sufficiency/configuration.py
--rw-r--r--   0        0        0     1078 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_sufficiency/process.py
--rw-r--r--   0        0        0     4704 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/s903_cli.py
--rw-r--r--   0        0        0     6921 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/s903/s903_main_functions.py
--rw-r--r--   0        0        0        1 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/school_census/__init__.py
--rw-r--r--   0        0        0        1 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/school_census/lds_school_clean/__init__.py
--rw-r--r--   0        0        0        1 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/school_census/lds_school_la_agg/__init__.py
--rw-r--r--   0        0        0     6324 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/shared_functions/common.py
--rw-r--r--   0        0        0     1827 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/shared_functions/converters.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/__init__.py
--rw-r--r--   0        0        0      778 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/FTESum.py
--rw-r--r--   0        0        0      778 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/FTESum_2020.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/__init__.py
--rw-r--r--   0        0        0     2452 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/growth_tables.py
--rw-r--r--   0        0        0      851 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/pivotGen.py
--rw-r--r--   0        0        0      745 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/progressed.py
--rw-r--r--   0        0        0     2508 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority.py
--rw-r--r--   0        0        0     2842 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority_forecast_04.py
--rw-r--r--   0        0        0     3204 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority_forecast_5c.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/__init__.py
--rw-r--r--   0        0        0     5395 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/converter.py
--rw-r--r--   0        0        0     7134 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/file_operations.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/__init__.py
--rw-r--r--   0        0        0      980 2023-04-20 08:59:28.676817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validation_error.py
--rw-r--r--   0        0        0     7796 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validator.py
--rw-r--r--   0        0        0       24 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/env
--rw-r--r--   0        0        0     1628 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/main.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/spec/__init__.py
--rw-r--r--   0        0        0    23265 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/spec/wf_xmlschema.xsd
--rw-r--r--   0        0        0     4771 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/util/AppLogs.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/util/__init__.py
--rw-r--r--   0        0        0     2268 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/util/work_path.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/__init__.py
--rw-r--r--   0        0        0      829 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/csww_cli.py
--rw-r--r--   0        0        0      839 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/csww_main_functions.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/lds_csww_clean/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/lds_csww_la_agg/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/lds_csww_pan_agg/__init__.py
--rw-r--r--   0        0        0     9774 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/sample_data.py
--rw-r--r--   0        0        0      470 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/schema.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/annex_a/__init__.py
--rw-r--r--   0        0        0    11870 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/annex_a/annex-a-merge.yml
--rw-r--r--   0        0        0    45318 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/annex_a/data-map.yml
--rw-r--r--   0        0        0    10542 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/annex_a/la-agg.yml
--rw-r--r--   0        0        0     1757 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/annex_a/pan-agg.yml
--rw-r--r--   0        0        0    27319 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/annex_a/samples/Annex_A.xlsx
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/cin_census/__init__.py
--rw-r--r--   0        0        0      711 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/cin_census/agg.yml
--rw-r--r--   0        0        0    31534 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/cin_census/cin-2022.xsd
--rw-r--r--   0        0        0     3423 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/cin_census/samples/cin-2022.xml
--rw-r--r--   0        0        0      739 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/common/LA-codes.yml
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/common/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/s903/__init__.py
--rw-r--r--   0        0        0    10875 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/s903/config.yml
--rw-r--r--   0        0        0     3339 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/s903/la-agg.yml
--rw-r--r--   0        0        0     1792 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/s903/pan-agg.yml
--rw-r--r--   0        0        0      459 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/s903/samples/SSDA903_2020_episodes.csv
--rw-r--r--   0        0        0     1585 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/s903/sufficiency.yml
--rw-r--r--   0        0        0        1 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/school_census/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/social_work_workforce/__init__.py
--rw-r--r--   0        0        0     3716 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/social_work_workforce/samples/social_work_workforce_2022.xml
--rw-r--r--   0        0        0    17431 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/liiatools/spec/social_work_workforce/social_work_workforce_2022.xsd
--rw-r--r--   0        0        0     1049 2023-04-20 08:59:28.680817 liiatools-0.1.5.1/pyproject.toml
--rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 liiatools-0.1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/__init__.py
+-rw-r--r--   0        0        0      434 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/csdatatools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/csdatatools/datasets/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/csdatatools/datasets/cincensus/__init__.py
+-rw-r--r--   0        0        0     4364 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/csdatatools/datasets/cincensus/filters.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/csdatatools/util/__init__.py
+-rw-r--r--   0        0        0      280 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/csdatatools/util/stream.py
+-rw-r--r--   0        0        0     1640 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/csdatatools/util/xml.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/datasets/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/datasets/annex_a/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/datasets/annex_a/__init__.py
+-rw-r--r--   0        0        0     7047 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/datasets/annex_a/annex_a_cli.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/__init__.py
+-rw-r--r--   0        0        0     4908 2023-05-19 07:59:31.078974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/cleaner.py
+-rw-r--r--   0        0        0    11751 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/configuration.py
+-rw-r--r--   0        0        0      451 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/converters.py
+-rw-r--r--   0        0        0     1381 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/degrade.py
+-rw-r--r--   0        0        0     5122 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/file_creator.py
+-rw-r--r--   0        0        0    12608 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/logger.py
+-rw-r--r--   0        0        0      772 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/populate.py
+-rw-r--r--   0        0        0      885 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/regex.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_la_agg/__init__.py
+-rw-r--r--   0        0        0     2495 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_la_agg/configuration.py
+-rw-r--r--   0        0        0     3052 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_la_agg/process.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_pan_agg/__init__.py
+-rw-r--r--   0        0        0     2894 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_pan_agg/configuration.py
+-rw-r--r--   0        0        0     2066 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_pan_agg/process.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/__init__.py
+-rw-r--r--   0        0        0    12206 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/cin_cli.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/__init__.py
+-rw-r--r--   0        0        0     6065 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/cin_record.py
+-rw-r--r--   0        0        0     2644 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/configuration.py
+-rw-r--r--   0        0        0      811 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/converter.py
+-rw-r--r--   0        0        0     2757 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/file_creator.py
+-rw-r--r--   0        0        0     6012 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/logger.py
+-rw-r--r--   0        0        0      405 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/schema.py
+-rw-r--r--   0        0        0     3860 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/validator.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_la_agg/__init__.py
+-rw-r--r--   0        0        0     2487 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_la_agg/configuration.py
+-rw-r--r--   0        0        0    10532 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_la_agg/process.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_pan_agg/__init__.py
+-rw-r--r--   0        0        0     2885 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_pan_agg/configuration.py
+-rw-r--r--   0        0        0    10132 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_pan_agg/process.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/columns.py
+-rw-r--r--   0        0        0     5126 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/configuration.py
+-rw-r--r--   0        0        0     1612 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/converters.py
+-rw-r--r--   0        0        0     1248 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/degrade.py
+-rw-r--r--   0        0        0     2993 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/file_creator.py
+-rw-r--r--   0        0        0     3184 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/filters.py
+-rw-r--r--   0        0        0     8547 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/logger.py
+-rw-r--r--   0        0        0     1189 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/parse.py
+-rw-r--r--   0        0        0     1749 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/populate.py
+-rw-r--r--   0        0        0     5080 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/prep.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_la_agg/__init__.py
+-rw-r--r--   0        0        0     2486 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_la_agg/configuration.py
+-rw-r--r--   0        0        0     2425 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_la_agg/process.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_pan_agg/__init__.py
+-rw-r--r--   0        0        0     2885 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_pan_agg/configuration.py
+-rw-r--r--   0        0        0     1482 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_pan_agg/process.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_sufficiency/__init__.py
+-rw-r--r--   0        0        0     2491 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_sufficiency/configuration.py
+-rw-r--r--   0        0        0     1078 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_sufficiency/process.py
+-rw-r--r--   0        0        0     4704 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/s903_cli.py
+-rw-r--r--   0        0        0     7475 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/s903/s903_main_functions.py
+-rw-r--r--   0        0        0        1 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/school_census/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/school_census/lds_school_clean/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/school_census/lds_school_la_agg/__init__.py
+-rw-r--r--   0        0        0     8213 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/shared_functions/common.py
+-rw-r--r--   0        0        0     1827 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/shared_functions/converters.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/__init__.py
+-rw-r--r--   0        0        0      778 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/FTESum.py
+-rw-r--r--   0        0        0      778 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/FTESum_2020.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/__init__.py
+-rw-r--r--   0        0        0     2452 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/growth_tables.py
+-rw-r--r--   0        0        0      851 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/pivotGen.py
+-rw-r--r--   0        0        0      745 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/progressed.py
+-rw-r--r--   0        0        0     2508 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority.py
+-rw-r--r--   0        0        0     2842 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority_forecast_04.py
+-rw-r--r--   0        0        0     3204 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority_forecast_5c.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/__init__.py
+-rw-r--r--   0        0        0     5395 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/converter.py
+-rw-r--r--   0        0        0     7134 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/file_operations.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/__init__.py
+-rw-r--r--   0        0        0      980 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validation_error.py
+-rw-r--r--   0        0        0     7796 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validator.py
+-rw-r--r--   0        0        0       24 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/env
+-rw-r--r--   0        0        0     1628 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/main.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/spec/__init__.py
+-rw-r--r--   0        0        0    23265 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/spec/wf_xmlschema.xsd
+-rw-r--r--   0        0        0     4771 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/util/AppLogs.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/util/__init__.py
+-rw-r--r--   0        0        0     2268 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/util/work_path.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/__init__.py
+-rw-r--r--   0        0        0      829 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/csww_cli.py
+-rw-r--r--   0        0        0      839 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/csww_main_functions.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/lds_csww_clean/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/lds_csww_la_agg/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/lds_csww_pan_agg/__init__.py
+-rw-r--r--   0        0        0     9774 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/sample_data.py
+-rw-r--r--   0        0        0      470 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/schema.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/spec/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/spec/annex_a/__init__.py
+-rw-r--r--   0        0        0    11870 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/spec/annex_a/annex-a-merge.yml
+-rw-r--r--   0        0        0    45318 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/spec/annex_a/data-map.yml
+-rw-r--r--   0        0        0    10542 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/spec/annex_a/la-agg.yml
+-rw-r--r--   0        0        0     1757 2023-05-19 07:59:31.082974 liiatools-0.1.5.2/liiatools/spec/annex_a/pan-agg.yml
+-rw-r--r--   0        0        0    27319 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/annex_a/samples/Annex_A.xlsx
+-rw-r--r--   0        0        0    30559 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2017.xsd
+-rw-r--r--   0        0        0    30559 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2018.xsd
+-rw-r--r--   0        0        0    30559 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2019.xsd
+-rw-r--r--   0        0        0    30559 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2020.xsd
+-rw-r--r--   0        0        0    31267 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2021.xsd
+-rw-r--r--   0        0        0    31909 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2022.xsd
+-rw-r--r--   0        0        0    32229 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2023.xsd
+-rw-r--r--   0        0        0    32229 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2024.xsd
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/__init__.py
+-rw-r--r--   0        0        0      711 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/agg.yml
+-rw-r--r--   0        0        0     3423 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/cin_census/samples/cin-2022.xml
+-rw-r--r--   0        0        0      739 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/common/LA-codes.yml
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/common/__init__.py
+-rw-r--r--   0        0        0    11211 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2017.yml
+-rw-r--r--   0        0        0    11211 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2018.yml
+-rw-r--r--   0        0        0    11280 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2019.yml
+-rw-r--r--   0        0        0    11280 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2020.yml
+-rw-r--r--   0        0        0    11280 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2021.yml
+-rw-r--r--   0        0        0    11322 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2022.yml
+-rw-r--r--   0        0        0    11322 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2023.yml
+-rw-r--r--   0        0        0    11977 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/SSDA903_schema_2024.yml
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/__init__.py
+-rw-r--r--   0        0        0     3339 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/la-agg.yml
+-rw-r--r--   0        0        0     1792 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/pan-agg.yml
+-rw-r--r--   0        0        0      459 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/samples/SSDA903_2020_episodes.csv
+-rw-r--r--   0        0        0     1585 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/s903/sufficiency.yml
+-rw-r--r--   0        0        0        1 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/school_census/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/social_work_workforce/__init__.py
+-rw-r--r--   0        0        0     3716 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/social_work_workforce/samples/social_work_workforce_2022.xml
+-rw-r--r--   0        0        0    17431 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/liiatools/spec/social_work_workforce/social_work_workforce_2022.xsd
+-rw-r--r--   0        0        0     1049 2023-05-19 07:59:31.086974 liiatools-0.1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 liiatools-0.1.5.2/PKG-INFO
```

### Comparing `liiatools-0.1.5.1/LICENSE` & `liiatools-0.1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/csdatatools/datasets/cincensus/filters.py` & `liiatools-0.1.5.2/liiatools/csdatatools/datasets/cincensus/filters.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/csdatatools/util/xml.py` & `liiatools-0.1.5.2/liiatools/csdatatools/util/xml.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/annex_a/annex_a_cli.py` & `liiatools-0.1.5.2/liiatools/datasets/annex_a/annex_a_cli.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/cleaner.py` & `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/cleaner.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/configuration.py` & `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/degrade.py` & `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/degrade.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/file_creator.py` & `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/file_creator.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/logger.py` & `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/logger.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/populate.py` & `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/populate.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_clean/regex.py` & `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_clean/regex.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_la_agg/configuration.py` & `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_la_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_la_agg/process.py` & `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_la_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_pan_agg/configuration.py` & `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_pan_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/annex_a/lds_annexa_pan_agg/process.py` & `liiatools-0.1.5.2/liiatools/datasets/annex_a/lds_annexa_pan_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/cin_census/cin_cli.py` & `liiatools-0.1.5.2/liiatools/datasets/cin_census/cin_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import click_log
 import click as click
 from pathlib import Path
 import yaml
+from datetime import datetime
 
 
 # Dependencies for cleanfile()
 from sfdata_stream_parser.stream import events
 from liiatools.csdatatools.util.xml import dom_parse
 from liiatools.datasets.cin_census.lds_cin_clean.schema import Schema
 from liiatools.csdatatools.datasets.cincensus import filters
@@ -20,14 +21,18 @@
     converter,
 )
 from liiatools.spec import common as common_asset_dir
 from liiatools.datasets.shared_functions.common import (
     flip_dict,
     check_file_type,
     supported_file_types,
+    check_year,
+    check_year_within_range,
+    save_year_error,
+    save_incorrect_year_error
 )
 
 # Dependencies for la_agg()
 from liiatools.datasets.cin_census.lds_cin_la_agg import configuration as agg_config
 from liiatools.datasets.cin_census.lds_cin_la_agg import process as agg_process
 
 # Dependencies for pan_agg()
@@ -97,20 +102,36 @@
         )
         == "incorrect file type"
     ):
         return
     stream = dom_parse(input)
     stream = list(stream)
 
+    # Get year from input file
+    try:
+        filename = str(Path(input).resolve().stem)
+        input_year = check_year(filename)
+    except (AttributeError, ValueError):
+        save_year_error(input, la_log_dir)
+        return
+
+    # Check year is within acceptable range for data retention policy
+    years_to_go_back = 6
+    year_start_month = 6
+    reference_date = datetime.now()
+    if check_year_within_range(input_year, years_to_go_back, year_start_month, reference_date) is False:
+        save_incorrect_year_error(input, la_log_dir)
+        return
+
     # Configure stream
     config = clean_config.Config()
     la_name = flip_dict(config["data_codes"])[la_code]
     stream = filters.strip_text(stream)
     stream = filters.add_context(stream)
-    stream = filters.add_schema(stream, schema=Schema().schema)
+    stream = filters.add_schema(stream, schema=Schema(input_year).schema)
     stream = logger.inherit_LAchildID(stream)
 
     # Validate stream
     field_error = []
     LAchildID_error = []
     stream = validator.validate_elements(
         stream, LAchildID_error=LAchildID_error, field_error=field_error
@@ -164,15 +185,15 @@
         "CPPreviewDate",
     ]
     stream = validator.remove_invalid(stream, tag_list=tags)
 
     # Output result
     stream = cin_record.message_collector(stream)
     data = cin_record.export_table(stream)
-    data = file_creator.add_fields(input, data, la_name, la_log_dir, la_code)
+    data = file_creator.add_fields(input_year, data, la_name, la_code)
     file_creator.export_file(input, output, data)
     logger.save_errors_la(
         input,
         value_error=value_error,
         structural_error=structural_error,
         LAchildID_error=LAchildID_error,
         field_error=field_error,
```

### Comparing `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/cin_record.py` & `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/cin_record.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/configuration.py` & `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/converter.py` & `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/converter.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/file_creator.py` & `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/file_creator.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,26 +8,17 @@
 
 
 def convert_to_dataframe(data):
     data = data.export("df")
     return data
 
 
-def get_year(input, data, la_log_dir):
-    filename = Path(input).stem
-    try:
-        year = common.check_year(filename)
-        data["YEAR"] = year
-        return data
-    except AttributeError:
-        common.save_year_error(input, la_log_dir)
-        raise Exception(
-            f"{filename} was not processed as the filename did not contain a year, "
-            f"this error has been sent to the LA to be fixed"
-        )
+def get_year(data, year):
+    data["YEAR"] = year
+    return data
 
 
 def convert_to_datetime(data):
     data[["PersonBirthDate", "PersonDeathDate", "ExpectedPersonBirthDate"]] = data[
         ["PersonBirthDate", "PersonDeathDate", "ExpectedPersonBirthDate"]
     ].apply(pd.to_datetime)
     return data
@@ -80,19 +71,27 @@
     if data["PersonDeathDate"] is not None:
         data["PersonDeathDate"] = data["PersonDeathDate"].apply(
             lambda row: converters.to_month_only_dob(row)
         )
         return data
 
 
-def add_fields(input, data, la_name, la_log_dir, la_code):
-    """Adds YEAR, LA, PERSONSCHOOLYEAR to exported dataframe
-    Appends LA_code from config to LAChildID"""
+def add_fields(input_year, data, la_name, la_code):
+    """
+    Add YEAR, LA, PERSONSCHOOLYEAR to exported dataframe
+    Append LA_code from config to LAChildID
+
+    :param input_year: A string of the year of return for the current file
+    :param data: The dataframe to be cleaned
+    :param la_name: LA name
+    :param la_code: LA code
+    :return: Cleaned and degraded dataframe
+    """
     data = convert_to_dataframe(data)
-    data = get_year(input, data, la_log_dir)
+    data = get_year(data, input_year)
     data = convert_to_datetime(data)
     data = add_school_year(data)
     data = add_la_name(data, la_name)
     data = la_prefix(data, la_code)
     data = degrade_dob(data)
     data = degrade_expected_dob(data)
     data = degrade_death_date(data)
```

### Comparing `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/logger.py` & `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/logger.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_clean/validator.py` & `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_clean/validator.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_la_agg/configuration.py` & `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_la_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_la_agg/process.py` & `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_la_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_pan_agg/configuration.py` & `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_pan_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/cin_census/lds_cin_pan_agg/process.py` & `liiatools-0.1.5.2/liiatools/datasets/cin_census/lds_cin_pan_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/columns.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/columns.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/configuration.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,23 +71,22 @@
     stream = inherit_property(stream, "table_name")
     stream = inherit_property(stream, "expected_columns")
     stream = match_config_to_cell(stream, config=config["column_map"])
     return stream
 
 
 class Config(dict):
-    def __init__(self, *config_files):
+    def __init__(self, year, *config_files):
         super().__init__()
-
         if not config_files:
             config_files = ["DEFAULT_COLUMN_MAP", "DEFAULT_LA_MAP"]
 
         for file in config_files:
             if file == "DEFAULT_COLUMN_MAP":
-                file = DEFAULT_CONFIG_DIR / "config.yml"
+                file = DEFAULT_CONFIG_DIR / f"SSDA903_schema_{year}.yml"
             elif file == "DEFAULT_LA_MAP":
                 file = SHARED_CONFIG_DIR / "LA-codes.yml"
             self.load_config(file, conditional=False)
 
         self["config_date"] = datetime.datetime.now().isoformat()
         try:
             self["username"] = os.getlogin()
```

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/converters.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/converters.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/degrade.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/degrade.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/file_creator.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/file_creator.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/filters.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/filters.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/logger.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/logger.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/parse.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/parse.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/populate.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/populate.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,39 +5,32 @@
 from sfdata_stream_parser.filters.generic import streamfilter, pass_event
 
 from liiatools.datasets.shared_functions import common
 
 log = logging.getLogger(__name__)
 
 
-def add_year_column(stream, input, la_log_dir):
+def add_year_column(stream, year):
     """
     Searches the filename for the year by finding any four-digit number starting with 20
 
     :param stream: A filtered list of event objects of type StartTable
     :return: An updated list of event objects
     """
-    year = None
     for event in stream:
         if isinstance(event, events.StartTable):
-            try:
-                file_dir = event.filename
-                year = common.check_year(file_dir)
-                yield event.from_event(event, year=year)
-            except (AttributeError, ValueError):
-                common.save_year_error(input, la_log_dir)
+            yield event.from_event(event, year=year)
         elif isinstance(event, events.EndTable):
             yield event
             year = None
         elif isinstance(event, events.EndRow) and year is not None:
             yield event.from_event(event, year=year)
         else:
             yield event
 
-
 @streamfilter(check=lambda x: x.get("header") in ["CHILD"], fail_function=pass_event)
 def create_la_child_id(event, la_code):
     """
     Creates an identifier from a combination of the Child Unique ID and Local Authority so matching child IDs
     are not removed in the merging a de-duping steps
 
     :param event: A filtered list of event objects
```

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_clean/prep.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_clean/prep.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_la_agg/configuration.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_la_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_la_agg/process.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_la_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_pan_agg/configuration.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_pan_agg/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_pan_agg/process.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_pan_agg/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_sufficiency/configuration.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_sufficiency/configuration.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/lds_ssda903_sufficiency/process.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/lds_ssda903_sufficiency/process.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/s903_cli.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/s903_cli.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/s903/s903_main_functions.py` & `liiatools-0.1.5.2/liiatools/datasets/s903/s903_main_functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 import yaml
 import logging
 import click_log
+from datetime import datetime
 
 # dependencies for cleanfile()
 from liiatools.datasets.s903.lds_ssda903_clean import (
     configuration as clean_config,
     parse,
     populate,
     filters,
@@ -28,14 +29,18 @@
 from liiatools.datasets.s903.lds_ssda903_sufficiency import process as suff_process
 
 from liiatools.spec import common as common_asset_dir
 from liiatools.datasets.shared_functions.common import (
     flip_dict,
     check_file_type,
     supported_file_types,
+    check_year,
+    save_year_error,
+    save_incorrect_year_error,
+    check_year_within_range
 )
 
 log = logging.getLogger()
 click_log.basic_config(log)
 
 COMMON_CONFIG_DIR = Path(common_asset_dir.__file__).parent
 # Get all the possible LA codes that could be used
@@ -69,30 +74,44 @@
         input, drop_file_list=drop_file_list, la_log_dir=la_log_dir
     )
     if prep.check_blank_file(input, la_log_dir=la_log_dir) == "empty":
         return
     prep.drop_empty_rows(input, input)
 
     # Configuration
-    config = clean_config.Config()
+    try:
+        filename = str(Path(input).resolve().stem)
+        year = check_year(filename)
+    except (AttributeError, ValueError):
+        save_year_error(input, la_log_dir)
+        return
+    
+    years_to_go_back = 6
+    year_start_month = 6
+    reference_date = datetime.now()
+    if check_year_within_range(year, years_to_go_back, year_start_month, reference_date) is False:
+        save_incorrect_year_error(input, la_log_dir)
+        return
+
+    config = clean_config.Config(year)
     la_name = flip_dict(config["data_codes"])[la_code]
     if (
         check_file_type(
             input,
             file_types=[".csv"],
             supported_file_types=supported_file_types,
             la_log_dir=la_log_dir,
         )
         == "incorrect file type"
     ):
         return
 
     # Open & Parse file
     stream = parse.parse_csv(input=input)
-    stream = populate.add_year_column(stream, input=input, la_log_dir=la_log_dir)
+    stream = populate.add_year_column(stream, year)
 
     # Configure stream
     stream = clean_config.configure_stream(stream, config)
 
     # Clean stream
     stream = filters.clean(stream)
     stream = degrade.degrade(stream)
```

### Comparing `liiatools-0.1.5.1/liiatools/datasets/shared_functions/common.py` & `liiatools-0.1.5.2/liiatools/datasets/shared_functions/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -79,23 +79,69 @@
     """
     Save errors to a text file in the LA log directory
 
     :param input: The input file location, including file name and suffix, and be usable by a Path function
     :param la_log_dir: Path to the local authority's log folder
     :return: Text file containing the error information
     """
+    
     filename = Path(input).resolve().stem
     start_time = f"{datetime.now():%d-%m-%Y %Hh-%Mm-%Ss}"
     with open(
         f"{Path(la_log_dir, filename)}_error_log_{start_time}.txt",
         "a",
     ) as f:
         f.write(
             f"Could not process '{filename}' because no year was found in the name of the file"
         )
+        
+        
+def check_year_within_range(year, num_of_years, new_year_start_month, as_at_date):
+    """
+    Check that year is within permitted range of data retention policy
+    The new year begins on 1 June, hence we must include check for current month
+    The check is made with reference to the as_at_date which will normally be the current date
+
+    :param year: The year to check
+    :param num_of_years: The number of years to go back
+    :param new_year_start_month: The month which signifies start of a new year for data retention policy
+    :param as_at_date: The reference date against which we are checking the valid range
+    :return: True if year is within range, false otherwise
+    """
+
+    year_to_check = int(year)
+    current_year = as_at_date.year
+    current_month = as_at_date.month
+    if current_month < new_year_start_month:
+        earliest_allowed_year = current_year - num_of_years
+        latest_allowed_year = current_year 
+    else:
+        earliest_allowed_year = current_year - num_of_years + 1  # roll forward one year
+        latest_allowed_year = current_year + 1
+
+    return earliest_allowed_year <= year_to_check <= latest_allowed_year
+    
+
+def save_incorrect_year_error(input, la_log_dir):
+    """
+    Save errors to a text file in the LA log directory
+
+    :param input: The input file location, including file name and suffix, and be usable by a Path function
+    :param la_log_dir: Path to the local authority's log folder
+    :return: Text file containing the error information
+    """
+    filename = Path(input).resolve().stem
+    start_time = f"{datetime.now():%d-%m-%Y %Hh-%Mm-%Ss}"
+    with open(
+        f"{Path(la_log_dir, filename)}_error_log_{start_time}.txt",
+        "a",
+    ) as f:
+        f.write(
+            f"Could not process '{filename}'. This file is not within the year ranges of data retention policy."
+        )
 
 
 def check_year(filename):
     """
     Check a filename to see if it contains a year, if it does, return that year
     Expected year formats within string:
         2022
```

### Comparing `liiatools-0.1.5.1/liiatools/datasets/shared_functions/converters.py` & `liiatools-0.1.5.2/liiatools/datasets/shared_functions/converters.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/FTESum.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/FTESum.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/FTESum_2020.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/FTESum_2020.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/growth_tables.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/growth_tables.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/pivotGen.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/pivotGen.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/progressed.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/progressed.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority_forecast_04.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority_forecast_04.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority_forecast_5c.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/analysis/seniority_forecast_5c.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/converter.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/converter.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/file_operations.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/file_operations.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validation_error.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validation_error.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validator.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/dataprocessing/validation/validator.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/main.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/main.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/spec/wf_xmlschema.xsd` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/spec/wf_xmlschema.xsd`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/util/AppLogs.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/util/AppLogs.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/SWFtools/util/work_path.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/SWFtools/util/work_path.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/csww_cli.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/csww_cli.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/csww_main_functions.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/csww_main_functions.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/datasets/social_work_workforce/sample_data.py` & `liiatools-0.1.5.2/liiatools/datasets/social_work_workforce/sample_data.py`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/spec/annex_a/annex-a-merge.yml` & `liiatools-0.1.5.2/liiatools/spec/annex_a/annex-a-merge.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/spec/annex_a/data-map.yml` & `liiatools-0.1.5.2/liiatools/spec/annex_a/data-map.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/spec/annex_a/la-agg.yml` & `liiatools-0.1.5.2/liiatools/spec/annex_a/la-agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/spec/annex_a/pan-agg.yml` & `liiatools-0.1.5.2/liiatools/spec/annex_a/pan-agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/spec/annex_a/samples/Annex_A.xlsx` & `liiatools-0.1.5.2/liiatools/spec/annex_a/samples/Annex_A.xlsx`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/spec/cin_census/agg.yml` & `liiatools-0.1.5.2/liiatools/spec/cin_census/agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/spec/cin_census/cin-2022.xsd` & `liiatools-0.1.5.2/liiatools/spec/cin_census/CIN_schema_2022.xsd`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, Unicode text, UTF-8 text, with very long lines (319)*

 * *Files 10% similar despite different names*

```diff
@@ -1,1971 +1,1995 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 203f 3e0a 3c78 733a 7363 6865  F-8" ?>.<xs:sche
-00000030: 6d61 2078 6d6c 6e73 3a78 733d 2268 7474  ma xmlns:xs="htt
-00000040: 703a 2f2f 7777 772e 7733 2e6f 7267 2f32  p://www.w3.org/2
-00000050: 3030 312f 584d 4c53 6368 656d 6122 3e0a  001/XMLSchema">.
-00000060: 0a20 203c 7873 3a65 6c65 6d65 6e74 206e  .  <xs:element n
-00000070: 616d 653d 224d 6573 7361 6765 2220 7479  ame="Message" ty
-00000080: 7065 3d22 6d65 7373 6167 6574 7970 6522  pe="messagetype"
-00000090: 2f3e 0a0a 2020 3c78 733a 636f 6d70 6c65  />..  <xs:comple
-000000a0: 7854 7970 6520 6e61 6d65 3d22 6d65 7373  xType name="mess
-000000b0: 6167 6574 7970 6522 3e0a 2020 2020 3c78  agetype">.    <x
-000000c0: 733a 7365 7175 656e 6365 3e0a 2020 2020  s:sequence>.    
-000000d0: 2020 3c78 733a 656c 656d 656e 7420 6e61    <xs:element na
-000000e0: 6d65 3d22 4865 6164 6572 2220 7479 7065  me="Header" type
-000000f0: 3d22 6865 6164 6572 7479 7065 2220 6d69  ="headertype" mi
-00000100: 6e4f 6363 7572 733d 2230 2220 6d61 784f  nOccurs="0" maxO
-00000110: 6363 7572 733d 2231 222f 3e0a 2020 2020  ccurs="1"/>.    
-00000120: 2020 3c78 733a 656c 656d 656e 7420 6e61    <xs:element na
-00000130: 6d65 3d22 4368 696c 6472 656e 2220 7479  me="Children" ty
-00000140: 7065 3d22 6368 696c 6472 656e 7479 7065  pe="childrentype
-00000150: 2220 6d69 6e4f 6363 7572 733d 2231 2220  " minOccurs="1" 
-00000160: 6d61 784f 6363 7572 733d 2231 222f 3e0a  maxOccurs="1"/>.
-00000170: 2020 2020 3c2f 7873 3a73 6571 7565 6e63      </xs:sequenc
-00000180: 653e 0a20 203c 2f78 733a 636f 6d70 6c65  e>.  </xs:comple
-00000190: 7854 7970 653e 0a0a 2020 3c78 733a 636f  xType>..  <xs:co
-000001a0: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
-000001b0: 6865 6164 6572 7479 7065 223e 0a20 2020  headertype">.   
-000001c0: 203c 7873 3a73 6571 7565 6e63 653e 0a20   <xs:sequence>. 
-000001d0: 2020 2020 203c 7873 3a65 6c65 6d65 6e74       <xs:element
-000001e0: 206e 616d 653d 2243 6f6c 6c65 6374 696f   name="Collectio
-000001f0: 6e44 6574 6169 6c73 2220 7479 7065 3d22  nDetails" type="
-00000200: 636f 6c6c 6563 7469 6f6e 6465 7461 696c  collectiondetail
-00000210: 7374 7970 6522 206d 696e 4f63 6375 7273  stype" minOccurs
-00000220: 3d22 3022 206d 6178 4f63 6375 7273 3d22  ="0" maxOccurs="
-00000230: 3122 2f3e 0a20 2020 2020 203c 7873 3a65  1"/>.      <xs:e
-00000240: 6c65 6d65 6e74 206e 616d 653d 2253 6f75  lement name="Sou
-00000250: 7263 6522 2074 7970 653d 2273 6f75 7263  rce" type="sourc
-00000260: 6574 7970 6522 206d 696e 4f63 6375 7273  etype" minOccurs
-00000270: 3d22 3022 206d 6178 4f63 6375 7273 3d22  ="0" maxOccurs="
-00000280: 756e 626f 756e 6465 6422 2f3e 0a20 2020  unbounded"/>.   
-00000290: 203c 2f78 733a 7365 7175 656e 6365 3e0a   </xs:sequence>.
-000002a0: 2020 3c2f 7873 3a63 6f6d 706c 6578 5479    </xs:complexTy
-000002b0: 7065 3e0a 0a20 203c 7873 3a63 6f6d 706c  pe>..  <xs:compl
-000002c0: 6578 5479 7065 206e 616d 653d 2263 6f6c  exType name="col
-000002d0: 6c65 6374 696f 6e64 6574 6169 6c73 7479  lectiondetailsty
-000002e0: 7065 223e 0a20 2020 203c 7873 3a73 6571  pe">.    <xs:seq
-000002f0: 7565 6e63 653e 0a20 2020 2020 203c 7873  uence>.      <xs
-00000300: 3a65 6c65 6d65 6e74 206e 616d 653d 2243  :element name="C
-00000310: 6f6c 6c65 6374 696f 6e22 206d 696e 4f63  ollection" minOc
-00000320: 6375 7273 3d22 3022 206d 6178 4f63 6375  curs="0" maxOccu
-00000330: 7273 3d22 3122 3e0a 2020 2020 2020 2020  rs="1">.        
-00000340: 3c78 733a 7369 6d70 6c65 5479 7065 3e0a  <xs:simpleType>.
-00000350: 2020 2020 2020 2020 2020 3c78 733a 7265            <xs:re
-00000360: 7374 7269 6374 696f 6e20 6261 7365 3d22  striction base="
-00000370: 7873 3a73 7472 696e 6722 3e0a 2020 2020  xs:string">.    
-00000380: 2020 2020 2020 2020 3c78 733a 656e 756d          <xs:enum
-00000390: 6572 6174 696f 6e20 7661 6c75 653d 2243  eration value="C
-000003a0: 494e 222f 3e0a 2020 2020 2020 2020 2020  IN"/>.          
-000003b0: 3c2f 7873 3a72 6573 7472 6963 7469 6f6e  </xs:restriction
-000003c0: 3e0a 2020 2020 2020 2020 3c2f 7873 3a73  >.        </xs:s
-000003d0: 696d 706c 6554 7970 653e 0a20 2020 2020  impleType>.     
-000003e0: 203c 2f78 733a 656c 656d 656e 743e 0a20   </xs:element>. 
-000003f0: 2020 2020 203c 7873 3a65 6c65 6d65 6e74       <xs:element
-00000400: 206e 616d 653d 2259 6561 7222 2074 7970   name="Year" typ
-00000410: 653d 2278 733a 6759 6561 7222 206d 696e  e="xs:gYear" min
-00000420: 4f63 6375 7273 3d22 3022 206d 6178 4f63  Occurs="0" maxOc
-00000430: 6375 7273 3d22 3122 2f3e 0a20 2020 2020  curs="1"/>.     
-00000440: 203c 7873 3a65 6c65 6d65 6e74 206e 616d   <xs:element nam
-00000450: 653d 2252 6566 6572 656e 6365 4461 7465  e="ReferenceDate
-00000460: 2220 7479 7065 3d22 7873 3a64 6174 6522  " type="xs:date"
-00000470: 206d 696e 4f63 6375 7273 3d22 3022 206d   minOccurs="0" m
-00000480: 6178 4f63 6375 7273 3d22 3122 2f3e 0a20  axOccurs="1"/>. 
-00000490: 2020 203c 2f78 733a 7365 7175 656e 6365     </xs:sequence
-000004a0: 3e0a 2020 3c2f 7873 3a63 6f6d 706c 6578  >.  </xs:complex
-000004b0: 5479 7065 3e0a 0a20 203c 7873 3a63 6f6d  Type>..  <xs:com
-000004c0: 706c 6578 5479 7065 206e 616d 653d 2273  plexType name="s
-000004d0: 6f75 7263 6574 7970 6522 3e0a 2020 2020  ourcetype">.    
-000004e0: 3c78 733a 7365 7175 656e 6365 3e0a 2020  <xs:sequence>.  
-000004f0: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
-00000500: 6e61 6d65 3d22 536f 7572 6365 4c65 7665  name="SourceLeve
-00000510: 6c22 206d 696e 4f63 6375 7273 3d22 3022  l" minOccurs="0"
-00000520: 206d 6178 4f63 6375 7273 3d22 3122 3e0a   maxOccurs="1">.
-00000530: 2020 2020 2020 2020 3c78 733a 7369 6d70          <xs:simp
-00000540: 6c65 5479 7065 3e0a 2020 2020 2020 2020  leType>.        
-00000550: 2020 3c78 733a 7265 7374 7269 6374 696f    <xs:restrictio
-00000560: 6e20 6261 7365 3d22 7873 3a73 7472 696e  n base="xs:strin
-00000570: 6722 3e0a 2020 2020 2020 2020 2020 2020  g">.            
-00000580: 3c78 733a 656e 756d 6572 6174 696f 6e20  <xs:enumeration 
-00000590: 7661 6c75 653d 224c 222f 3e0a 2020 2020  value="L"/>.    
-000005a0: 2020 2020 2020 3c2f 7873 3a72 6573 7472        </xs:restr
-000005b0: 6963 7469 6f6e 3e0a 2020 2020 2020 2020  iction>.        
-000005c0: 3c2f 7873 3a73 696d 706c 6554 7970 653e  </xs:simpleType>
-000005d0: 0a20 2020 2020 203c 2f78 733a 656c 656d  .      </xs:elem
-000005e0: 656e 743e 0a20 2020 2020 203c 7873 3a65  ent>.      <xs:e
-000005f0: 6c65 6d65 6e74 206e 616d 653d 224c 4541  lement name="LEA
-00000600: 2220 6d69 6e4f 6363 7572 733d 2231 2220  " minOccurs="1" 
-00000610: 6d61 784f 6363 7572 733d 2231 223e 0a20  maxOccurs="1">. 
-00000620: 2020 2020 2020 203c 7873 3a73 696d 706c         <xs:simpl
-00000630: 6554 7970 653e 0a20 2020 2020 2020 2020  eType>.         
-00000640: 203c 7873 3a72 6573 7472 6963 7469 6f6e   <xs:restriction
-00000650: 2062 6173 653d 2278 733a 7374 7269 6e67   base="xs:string
-00000660: 2220 3e0a 2020 2020 2020 2020 2020 2020  " >.            
-00000670: 3c78 733a 7061 7474 6572 6e20 7661 6c75  <xs:pattern valu
-00000680: 653d 225c 647b 337d 222f 3e0a 2020 2020  e="\d{3}"/>.    
-00000690: 2020 2020 2020 3c2f 7873 3a72 6573 7472        </xs:restr
-000006a0: 6963 7469 6f6e 3e0a 2020 2020 2020 2020  iction>.        
-000006b0: 3c2f 7873 3a73 696d 706c 6554 7970 653e  </xs:simpleType>
-000006c0: 0a20 2020 2020 203c 2f78 733a 656c 656d  .      </xs:elem
-000006d0: 656e 743e 0a20 2020 2020 203c 7873 3a65  ent>.      <xs:e
-000006e0: 6c65 6d65 6e74 206e 616d 653d 2253 6f66  lement name="Sof
-000006f0: 7477 6172 6543 6f64 6522 2074 7970 653d  twareCode" type=
-00000700: 2278 733a 7374 7269 6e67 2220 6d69 6e4f  "xs:string" minO
-00000710: 6363 7572 733d 2230 2220 6d61 784f 6363  ccurs="0" maxOcc
-00000720: 7572 733d 2231 222f 3e0a 2020 2020 2020  urs="1"/>.      
-00000730: 3c78 733a 656c 656d 656e 7420 6e61 6d65  <xs:element name
-00000740: 3d22 5265 6c65 6173 6522 2074 7970 653d  ="Release" type=
-00000750: 2278 733a 7374 7269 6e67 2220 6d69 6e4f  "xs:string" minO
-00000760: 6363 7572 733d 2230 2220 6d61 784f 6363  ccurs="0" maxOcc
-00000770: 7572 733d 2231 222f 3e0a 2020 2020 2020  urs="1"/>.      
-00000780: 3c78 733a 656c 656d 656e 7420 6e61 6d65  <xs:element name
-00000790: 3d22 5365 7269 616c 4e6f 2220 6d69 6e4f  ="SerialNo" minO
-000007a0: 6363 7572 733d 2230 2220 6d61 784f 6363  ccurs="0" maxOcc
-000007b0: 7572 733d 2231 223e 0a20 2020 2020 2020  urs="1">.       
-000007c0: 203c 7873 3a73 696d 706c 6554 7970 653e   <xs:simpleType>
-000007d0: 0a20 2020 2020 2020 2020 203c 7873 3a72  .          <xs:r
-000007e0: 6573 7472 6963 7469 6f6e 2062 6173 653d  estriction base=
-000007f0: 2278 733a 7374 7269 6e67 2220 3e0a 2020  "xs:string" >.  
-00000800: 2020 2020 2020 2020 2020 3c78 733a 7061            <xs:pa
-00000810: 7474 6572 6e20 7661 6c75 653d 225c 647b  ttern value="\d{
-00000820: 337d 5c64 2a22 2f3e 0a20 2020 2020 2020  3}\d*"/>.       
-00000830: 2020 203c 2f78 733a 7265 7374 7269 6374     </xs:restrict
-00000840: 696f 6e3e 0a20 2020 2020 2020 203c 2f78  ion>.        </x
-00000850: 733a 7369 6d70 6c65 5479 7065 3e0a 2020  s:simpleType>.  
-00000860: 2020 2020 3c2f 7873 3a65 6c65 6d65 6e74      </xs:element
-00000870: 3e0a 2020 2020 2020 3c78 733a 656c 656d  >.      <xs:elem
-00000880: 656e 7420 6e61 6d65 3d22 4461 7465 5469  ent name="DateTi
-00000890: 6d65 2220 7479 7065 3d22 7873 3a64 6174  me" type="xs:dat
-000008a0: 6554 696d 6522 206d 696e 4f63 6375 7273  eTime" minOccurs
-000008b0: 3d22 3022 206d 6178 4f63 6375 7273 3d22  ="0" maxOccurs="
-000008c0: 3122 2f3e 0a20 2020 203c 2f78 733a 7365  1"/>.    </xs:se
-000008d0: 7175 656e 6365 3e0a 2020 3c2f 7873 3a63  quence>.  </xs:c
-000008e0: 6f6d 706c 6578 5479 7065 3e0a 0a20 203c  omplexType>..  <
-000008f0: 7873 3a63 6f6d 706c 6578 5479 7065 206e  xs:complexType n
-00000900: 616d 653d 2263 6869 6c64 7265 6e74 7970  ame="childrentyp
-00000910: 6522 3e0a 2020 2020 3c78 733a 7365 7175  e">.    <xs:sequ
-00000920: 656e 6365 3e0a 2020 2020 2020 3c78 733a  ence>.      <xs:
-00000930: 656c 656d 656e 7420 6e61 6d65 3d22 4368  element name="Ch
-00000940: 696c 6422 2074 7970 653d 2263 6869 6c64  ild" type="child
-00000950: 7479 7065 2220 6d69 6e4f 6363 7572 733d  type" minOccurs=
-00000960: 2231 2220 6d61 784f 6363 7572 733d 2275  "1" maxOccurs="u
-00000970: 6e62 6f75 6e64 6564 222f 3e0a 2020 2020  nbounded"/>.    
-00000980: 3c2f 7873 3a73 6571 7565 6e63 653e 0a20  </xs:sequence>. 
-00000990: 203c 2f78 733a 636f 6d70 6c65 7854 7970   </xs:complexTyp
-000009a0: 653e 0a0a 2020 3c78 733a 636f 6d70 6c65  e>..  <xs:comple
-000009b0: 7854 7970 6520 6e61 6d65 3d22 6368 696c  xType name="chil
-000009c0: 6474 7970 6522 3e0a 2020 2020 3c78 733a  dtype">.    <xs:
-000009d0: 7365 7175 656e 6365 3e0a 2020 2020 2020  sequence>.      
-000009e0: 3c78 733a 656c 656d 656e 7420 6e61 6d65  <xs:element name
-000009f0: 3d22 4368 696c 6449 6465 6e74 6966 6965  ="ChildIdentifie
-00000a00: 7273 2220 7479 7065 3d22 6368 696c 6469  rs" type="childi
-00000a10: 6465 6e74 6966 6965 7273 7479 7065 2220  dentifierstype" 
-00000a20: 6d69 6e4f 6363 7572 733d 2231 2220 6d61  minOccurs="1" ma
-00000a30: 784f 6363 7572 733d 2231 222f 3e0a 2020  xOccurs="1"/>.  
-00000a40: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
-00000a50: 6e61 6d65 3d22 4368 696c 6443 6861 7261  name="ChildChara
-00000a60: 6374 6572 6973 7469 6373 2220 7479 7065  cteristics" type
-00000a70: 3d22 6368 696c 6463 6861 7261 6374 6572  ="childcharacter
-00000a80: 6973 7469 6373 7479 7065 2220 6d69 6e4f  isticstype" minO
-00000a90: 6363 7572 733d 2231 2220 6d61 784f 6363  ccurs="1" maxOcc
-00000aa0: 7572 733d 2231 222f 3e0a 2020 2020 2020  urs="1"/>.      
-00000ab0: 3c78 733a 656c 656d 656e 7420 6e61 6d65  <xs:element name
-00000ac0: 3d22 4349 4e64 6574 6169 6c73 2220 7479  ="CINdetails" ty
-00000ad0: 7065 3d22 6369 6e64 6574 6169 6c73 7479  pe="cindetailsty
-00000ae0: 7065 2220 6d69 6e4f 6363 7572 733d 2231  pe" minOccurs="1
-00000af0: 2220 6d61 784f 6363 7572 733d 2275 6e62  " maxOccurs="unb
-00000b00: 6f75 6e64 6564 222f 3e0a 2020 2020 3c2f  ounded"/>.    </
-00000b10: 7873 3a73 6571 7565 6e63 653e 0a20 203c  xs:sequence>.  <
-00000b20: 2f78 733a 636f 6d70 6c65 7854 7970 653e  /xs:complexType>
-00000b30: 0a0a 2020 3c78 733a 636f 6d70 6c65 7854  ..  <xs:complexT
-00000b40: 7970 6520 6e61 6d65 3d22 6368 696c 6469  ype name="childi
-00000b50: 6465 6e74 6966 6965 7273 7479 7065 223e  dentifierstype">
-00000b60: 0a20 2020 203c 7873 3a73 6571 7565 6e63  .    <xs:sequenc
-00000b70: 653e 0a20 2020 2020 203c 7873 3a65 6c65  e>.      <xs:ele
-00000b80: 6d65 6e74 206e 616d 653d 224c 4163 6869  ment name="LAchi
-00000b90: 6c64 4944 2220 7479 7065 3d22 6e6f 6e45  ldID" type="nonE
-00000ba0: 6d70 7479 5374 7269 6e67 2220 6d69 6e4f  mptyString" minO
-00000bb0: 6363 7572 733d 2231 2220 6d61 784f 6363  ccurs="1" maxOcc
-00000bc0: 7572 733d 2231 222f 3e0a 2020 2020 2020  urs="1"/>.      
-00000bd0: 3c78 733a 656c 656d 656e 7420 6e61 6d65  <xs:element name
-00000be0: 3d22 5550 4e22 2074 7970 653d 2275 706e  ="UPN" type="upn
-00000bf0: 7479 7065 2220 6d69 6e4f 6363 7572 733d  type" minOccurs=
-00000c00: 2230 2220 6d61 784f 6363 7572 733d 2231  "0" maxOccurs="1
-00000c10: 222f 3e0a 2020 2020 2020 3c78 733a 656c  "/>.      <xs:el
-00000c20: 656d 656e 7420 6e61 6d65 3d22 466f 726d  ement name="Form
-00000c30: 6572 5550 4e22 2074 7970 653d 2275 706e  erUPN" type="upn
-00000c40: 7479 7065 2220 6d69 6e4f 6363 7572 733d  type" minOccurs=
-00000c50: 2230 2220 6d61 784f 6363 7572 733d 2231  "0" maxOccurs="1
-00000c60: 222f 3e0a 2020 2020 2020 3c78 733a 656c  "/>.      <xs:el
-00000c70: 656d 656e 7420 6e61 6d65 3d22 5550 4e75  ement name="UPNu
-00000c80: 6e6b 6e6f 776e 2220 7479 7065 3d22 756e  nknown" type="un
-00000c90: 6b6e 6f77 6e75 706e 7479 7065 2220 6d69  knownupntype" mi
-00000ca0: 6e4f 6363 7572 733d 2230 2220 6d61 784f  nOccurs="0" maxO
-00000cb0: 6363 7572 733d 2231 222f 3e0a 2020 2020  ccurs="1"/>.    
-00000cc0: 2020 3c78 733a 656c 656d 656e 7420 6e61    <xs:element na
-00000cd0: 6d65 3d22 5065 7273 6f6e 4269 7274 6844  me="PersonBirthD
-00000ce0: 6174 6522 2074 7970 653d 2278 733a 6461  ate" type="xs:da
-00000cf0: 7465 2220 6d69 6e4f 6363 7572 733d 2230  te" minOccurs="0
-00000d00: 2220 6d61 784f 6363 7572 733d 2231 222f  " maxOccurs="1"/
-00000d10: 3e0a 2020 2020 2020 3c78 733a 656c 656d  >.      <xs:elem
-00000d20: 656e 7420 6e61 6d65 3d22 4578 7065 6374  ent name="Expect
-00000d30: 6564 5065 7273 6f6e 4269 7274 6844 6174  edPersonBirthDat
-00000d40: 6522 2074 7970 653d 2278 733a 6461 7465  e" type="xs:date
-00000d50: 2220 6d69 6e4f 6363 7572 733d 2230 2220  " minOccurs="0" 
-00000d60: 6d61 784f 6363 7572 733d 2231 222f 3e0a  maxOccurs="1"/>.
-00000d70: 2020 2020 2020 3c78 733a 656c 656d 656e        <xs:elemen
-00000d80: 7420 6e61 6d65 3d22 4765 6e64 6572 4375  t name="GenderCu
-00000d90: 7272 656e 7422 2074 7970 653d 2267 656e  rrent" type="gen
-00000da0: 6465 7274 7970 6522 206d 696e 4f63 6375  dertype" minOccu
-00000db0: 7273 3d22 3122 206d 6178 4f63 6375 7273  rs="1" maxOccurs
-00000dc0: 3d22 3122 2f3e 0a20 2020 2020 203c 7873  ="1"/>.      <xs
-00000dd0: 3a65 6c65 6d65 6e74 206e 616d 653d 2250  :element name="P
-00000de0: 6572 736f 6e44 6561 7468 4461 7465 2220  ersonDeathDate" 
-00000df0: 7479 7065 3d22 7873 3a64 6174 6522 206d  type="xs:date" m
-00000e00: 696e 4f63 6375 7273 3d22 3022 206d 6178  inOccurs="0" max
-00000e10: 4f63 6375 7273 3d22 3122 2f3e 0a20 2020  Occurs="1"/>.   
-00000e20: 203c 2f78 733a 7365 7175 656e 6365 3e0a   </xs:sequence>.
-00000e30: 2020 3c2f 7873 3a63 6f6d 706c 6578 5479    </xs:complexTy
-00000e40: 7065 3e0a 0a20 203c 7873 3a63 6f6d 706c  pe>..  <xs:compl
-00000e50: 6578 5479 7065 206e 616d 653d 2263 6869  exType name="chi
-00000e60: 6c64 6368 6172 6163 7465 7269 7374 6963  ldcharacteristic
-00000e70: 7374 7970 6522 3e0a 2020 2020 3c78 733a  stype">.    <xs:
-00000e80: 7365 7175 656e 6365 3e0a 2020 2020 2020  sequence>.      
-00000e90: 3c78 733a 656c 656d 656e 7420 6e61 6d65  <xs:element name
-00000ea0: 3d22 4574 686e 6963 6974 7922 2074 7970  ="Ethnicity" typ
-00000eb0: 653d 2265 7468 6e69 6369 7479 7479 7065  e="ethnicitytype
-00000ec0: 2220 6d69 6e4f 6363 7572 733d 2231 2220  " minOccurs="1" 
-00000ed0: 6d61 784f 6363 7572 733d 2231 222f 3e0a  maxOccurs="1"/>.
-00000ee0: 2020 2020 2020 3c78 733a 656c 656d 656e        <xs:elemen
-00000ef0: 7420 6e61 6d65 3d22 4469 7361 6269 6c69  t name="Disabili
-00000f00: 7469 6573 2220 6d69 6e4f 6363 7572 733d  ties" minOccurs=
-00000f10: 2230 2220 6d61 784f 6363 7572 733d 2231  "0" maxOccurs="1
-00000f20: 223e 0a20 2020 2020 2020 203c 7873 3a63  ">.        <xs:c
-00000f30: 6f6d 706c 6578 5479 7065 3e0a 2020 2020  omplexType>.    
-00000f40: 2020 2020 2020 3c78 733a 7365 7175 656e        <xs:sequen
-00000f50: 6365 3e0a 2020 2020 2020 2020 2020 2020  ce>.            
-00000f60: 3c78 733a 656c 656d 656e 7420 6e61 6d65  <xs:element name
-00000f70: 3d22 4469 7361 6269 6c69 7479 2220 7479  ="Disability" ty
-00000f80: 7065 3d22 6469 7361 6269 6c69 7479 7479  pe="disabilityty
-00000f90: 7065 2220 206d 696e 4f63 6375 7273 3d22  pe"  minOccurs="
-00000fa0: 3122 206d 6178 4f63 6375 7273 3d22 756e  1" maxOccurs="un
-00000fb0: 626f 756e 6465 6422 2f3e 0a20 2020 2020  bounded"/>.     
-00000fc0: 2020 2020 203c 2f78 733a 7365 7175 656e       </xs:sequen
-00000fd0: 6365 3e0a 2020 2020 2020 2020 3c2f 7873  ce>.        </xs
-00000fe0: 3a63 6f6d 706c 6578 5479 7065 3e0a 2020  :complexType>.  
-00000ff0: 2020 2020 3c2f 7873 3a65 6c65 6d65 6e74      </xs:element
-00001000: 3e0a 2020 2020 3c2f 7873 3a73 6571 7565  >.    </xs:seque
-00001010: 6e63 653e 0a20 203c 2f78 733a 636f 6d70  nce>.  </xs:comp
-00001020: 6c65 7854 7970 653e 0a0a 2020 3c78 733a  lexType>..  <xs:
-00001030: 636f 6d70 6c65 7854 7970 6520 6e61 6d65  complexType name
-00001040: 3d22 6369 6e64 6574 6169 6c73 7479 7065  ="cindetailstype
-00001050: 223e 0a20 2020 203c 7873 3a73 6571 7565  ">.    <xs:seque
-00001060: 6e63 653e 0a20 2020 2020 203c 7873 3a65  nce>.      <xs:e
-00001070: 6c65 6d65 6e74 206e 616d 653d 2243 494e  lement name="CIN
-00001080: 7265 6665 7272 616c 4461 7465 2220 7479  referralDate" ty
-00001090: 7065 3d22 7873 3a64 6174 6522 206d 696e  pe="xs:date" min
-000010a0: 4f63 6375 7273 3d22 3122 206d 6178 4f63  Occurs="1" maxOc
-000010b0: 6375 7273 3d22 3122 2f3e 0a20 2020 2020  curs="1"/>.     
-000010c0: 203c 7873 3a65 6c65 6d65 6e74 206e 616d   <xs:element nam
-000010d0: 653d 2252 6566 6572 7261 6c53 6f75 7263  e="ReferralSourc
-000010e0: 6522 2074 7970 653d 2272 6566 6572 7261  e" type="referra
-000010f0: 6c73 6f75 7263 6574 7970 6522 206d 696e  lsourcetype" min
-00001100: 4f63 6375 7273 3d22 3122 206d 6178 4f63  Occurs="1" maxOc
-00001110: 6375 7273 3d22 3122 2f3e 0a20 2020 2020  curs="1"/>.     
-00001120: 203c 7873 3a65 6c65 6d65 6e74 206e 616d   <xs:element nam
-00001130: 653d 2250 7269 6d61 7279 4e65 6564 436f  e="PrimaryNeedCo
-00001140: 6465 2220 7479 7065 3d22 7072 696d 6172  de" type="primar
-00001150: 796e 6565 6463 6f64 6574 7970 6522 206d  yneedcodetype" m
-00001160: 696e 4f63 6375 7273 3d22 3022 206d 6178  inOccurs="0" max
-00001170: 4f63 6375 7273 3d22 3122 2f3e 0a20 2020  Occurs="1"/>.   
-00001180: 2020 203c 7873 3a65 6c65 6d65 6e74 206e     <xs:element n
-00001190: 616d 653d 2243 494e 636c 6f73 7572 6544  ame="CINclosureD
-000011a0: 6174 6522 2074 7970 653d 2278 733a 6461  ate" type="xs:da
-000011b0: 7465 2220 6d69 6e4f 6363 7572 733d 2230  te" minOccurs="0
-000011c0: 2220 6d61 784f 6363 7572 733d 2231 222f  " maxOccurs="1"/
-000011d0: 3e0a 2020 2020 2020 3c78 733a 656c 656d  >.      <xs:elem
-000011e0: 656e 7420 6e61 6d65 3d22 5265 6173 6f6e  ent name="Reason
-000011f0: 466f 7243 6c6f 7375 7265 2220 7479 7065  ForClosure" type
-00001200: 3d22 7265 6173 6f6e 666f 7263 6c6f 7375  ="reasonforclosu
-00001210: 7265 7479 7065 2220 6d69 6e4f 6363 7572  retype" minOccur
-00001220: 733d 2230 2220 6d61 784f 6363 7572 733d  s="0" maxOccurs=
-00001230: 2231 222f 3e0a 2020 2020 2020 3c78 733a  "1"/>.      <xs:
-00001240: 656c 656d 656e 7420 6e61 6d65 3d22 4461  element name="Da
-00001250: 7465 4f66 496e 6974 6961 6c43 5043 2220  teOfInitialCPC" 
-00001260: 7479 7065 3d22 7873 3a64 6174 6522 206d  type="xs:date" m
-00001270: 696e 4f63 6375 7273 3d22 3022 206d 6178  inOccurs="0" max
-00001280: 4f63 6375 7273 3d22 3122 2f3e 0a20 2020  Occurs="1"/>.   
-00001290: 2020 203c 7873 3a65 6c65 6d65 6e74 206e     <xs:element n
-000012a0: 616d 653d 2241 7373 6573 736d 656e 7473  ame="Assessments
-000012b0: 2220 7479 7065 3d22 6173 7365 7373 6d65  " type="assessme
-000012c0: 6e74 7374 7970 6522 206d 696e 4f63 6375  ntstype" minOccu
-000012d0: 7273 3d22 3022 206d 6178 4f63 6375 7273  rs="0" maxOccurs
-000012e0: 3d22 756e 626f 756e 6465 6422 2f3e 0a20  ="unbounded"/>. 
-000012f0: 2020 2020 203c 7873 3a65 6c65 6d65 6e74       <xs:element
-00001300: 206e 616d 653d 2243 494e 506c 616e 4461   name="CINPlanDa
-00001310: 7465 7322 2074 7970 653d 2263 696e 706c  tes" type="cinpl
-00001320: 616e 6461 7465 7374 7479 7065 2220 6d69  andatesttype" mi
-00001330: 6e4f 6363 7572 733d 2230 2220 6d61 784f  nOccurs="0" maxO
-00001340: 6363 7572 733d 2275 6e62 6f75 6e64 6564  ccurs="unbounded
-00001350: 222f 3e0a 2020 2020 2020 3c78 733a 656c  "/>.      <xs:el
-00001360: 656d 656e 7420 6e61 6d65 3d22 5365 6374  ement name="Sect
-00001370: 696f 6e34 3722 2074 7970 653d 2273 6563  ion47" type="sec
-00001380: 7469 6f6e 3437 7479 7065 2220 6d69 6e4f  tion47type" minO
-00001390: 6363 7572 733d 2230 2220 6d61 784f 6363  ccurs="0" maxOcc
-000013a0: 7572 733d 2275 6e62 6f75 6e64 6564 222f  urs="unbounded"/
-000013b0: 3e0a 2020 2020 2020 3c78 733a 656c 656d  >.      <xs:elem
-000013c0: 656e 7420 6e61 6d65 3d22 5265 6665 7272  ent name="Referr
-000013d0: 616c 4e46 4122 2074 7970 653d 2279 6573  alNFA" type="yes
-000013e0: 6e6f 7479 7065 2220 6d69 6e4f 6363 7572  notype" minOccur
-000013f0: 733d 2231 2220 6d61 784f 6363 7572 733d  s="1" maxOccurs=
-00001400: 2231 222f 3e0a 2020 2020 2020 3c78 733a  "1"/>.      <xs:
-00001410: 656c 656d 656e 7420 6e61 6d65 3d22 4368  element name="Ch
-00001420: 696c 6450 726f 7465 6374 696f 6e50 6c61  ildProtectionPla
-00001430: 6e73 2220 7479 7065 3d22 6368 696c 6470  ns" type="childp
-00001440: 726f 7465 6374 696f 6e70 6c61 6e73 7479  rotectionplansty
-00001450: 7065 2220 6d69 6e4f 6363 7572 733d 2230  pe" minOccurs="0
-00001460: 2220 6d61 784f 6363 7572 733d 2275 6e62  " maxOccurs="unb
-00001470: 6f75 6e64 6564 222f 3e0a 2020 2020 3c2f  ounded"/>.    </
-00001480: 7873 3a73 6571 7565 6e63 653e 0a20 203c  xs:sequence>.  <
-00001490: 2f78 733a 636f 6d70 6c65 7854 7970 653e  /xs:complexType>
-000014a0: 0a0a 2020 3c78 733a 636f 6d70 6c65 7854  ..  <xs:complexT
-000014b0: 7970 6520 6e61 6d65 3d22 6173 7365 7373  ype name="assess
-000014c0: 6d65 6e74 7374 7970 6522 3e0a 2020 2020  mentstype">.    
-000014d0: 3c78 733a 7365 7175 656e 6365 3e0a 2020  <xs:sequence>.  
-000014e0: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
-000014f0: 6e61 6d65 3d22 4173 7365 7373 6d65 6e74  name="Assessment
-00001500: 4163 7475 616c 5374 6172 7444 6174 6522  ActualStartDate"
-00001510: 2074 7970 653d 2278 733a 6461 7465 2220   type="xs:date" 
-00001520: 6d69 6e4f 6363 7572 733d 2231 2220 6d61  minOccurs="1" ma
-00001530: 784f 6363 7572 733d 2231 222f 3e0a 2020  xOccurs="1"/>.  
-00001540: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
-00001550: 6e61 6d65 3d22 4173 7365 7373 6d65 6e74  name="Assessment
-00001560: 496e 7465 726e 616c 5265 7669 6577 4461  InternalReviewDa
-00001570: 7465 2220 7479 7065 3d22 7873 3a64 6174  te" type="xs:dat
-00001580: 6522 206d 696e 4f63 6375 7273 3d22 3022  e" minOccurs="0"
-00001590: 206d 6178 4f63 6375 7273 3d22 3122 2f3e   maxOccurs="1"/>
-000015a0: 0a20 2020 2020 203c 7873 3a65 6c65 6d65  .      <xs:eleme
-000015b0: 6e74 206e 616d 653d 2241 7373 6573 736d  nt name="Assessm
-000015c0: 656e 7441 7574 686f 7269 7361 7469 6f6e  entAuthorisation
-000015d0: 4461 7465 2220 7479 7065 3d22 7873 3a64  Date" type="xs:d
-000015e0: 6174 6522 206d 696e 4f63 6375 7273 3d22  ate" minOccurs="
-000015f0: 3022 206d 6178 4f63 6375 7273 3d22 3122  0" maxOccurs="1"
-00001600: 2f3e 0a20 2020 2020 203c 7873 3a65 6c65  />.      <xs:ele
-00001610: 6d65 6e74 206e 616d 653d 2246 6163 746f  ment name="Facto
-00001620: 7273 4964 656e 7469 6669 6564 4174 4173  rsIdentifiedAtAs
-00001630: 7365 7373 6d65 6e74 2220 6d69 6e4f 6363  sessment" minOcc
-00001640: 7572 733d 2230 2220 6d61 784f 6363 7572  urs="0" maxOccur
-00001650: 733d 2231 223e 0a20 2020 2020 2020 203c  s="1">.        <
-00001660: 7873 3a63 6f6d 706c 6578 5479 7065 3e0a  xs:complexType>.
-00001670: 2020 2020 2020 2020 2020 3c78 733a 7365            <xs:se
-00001680: 7175 656e 6365 3e0a 2020 2020 2020 2020  quence>.        
-00001690: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
-000016a0: 6e61 6d65 3d22 4173 7365 7373 6d65 6e74  name="Assessment
-000016b0: 4661 6374 6f72 7322 2074 7970 653d 2261  Factors" type="a
-000016c0: 7373 6573 736d 656e 7466 6163 746f 7273  ssessmentfactors
-000016d0: 7479 7065 2220 6d69 6e4f 6363 7572 733d  type" minOccurs=
-000016e0: 2231 2220 6d61 784f 6363 7572 733d 2275  "1" maxOccurs="u
-000016f0: 6e62 6f75 6e64 6564 222f 3e0a 2020 2020  nbounded"/>.    
-00001700: 2020 2020 2020 3c2f 7873 3a73 6571 7565        </xs:seque
-00001710: 6e63 653e 0a20 2020 2020 2020 203c 2f78  nce>.        </x
-00001720: 733a 636f 6d70 6c65 7854 7970 653e 0a20  s:complexType>. 
-00001730: 2020 2020 203c 2f78 733a 656c 656d 656e       </xs:elemen
-00001740: 743e 0a20 2020 203c 2f78 733a 7365 7175  t>.    </xs:sequ
-00001750: 656e 6365 3e0a 2020 3c2f 7873 3a63 6f6d  ence>.  </xs:com
-00001760: 706c 6578 5479 7065 3e0a 0a20 203c 7873  plexType>..  <xs
-00001770: 3a63 6f6d 706c 6578 5479 7065 206e 616d  :complexType nam
-00001780: 653d 2263 696e 706c 616e 6461 7465 7374  e="cinplandatest
-00001790: 7479 7065 223e 0a20 2020 203c 7873 3a73  type">.    <xs:s
-000017a0: 6571 7565 6e63 653e 0a20 2020 2020 203c  equence>.      <
-000017b0: 7873 3a65 6c65 6d65 6e74 206e 616d 653d  xs:element name=
-000017c0: 2243 494e 506c 616e 5374 6172 7444 6174  "CINPlanStartDat
-000017d0: 6522 2074 7970 653d 2278 733a 6461 7465  e" type="xs:date
-000017e0: 2220 6d69 6e4f 6363 7572 733d 2231 2220  " minOccurs="1" 
-000017f0: 6d61 784f 6363 7572 733d 2231 222f 3e0a  maxOccurs="1"/>.
-00001800: 2020 2020 2020 3c78 733a 656c 656d 656e        <xs:elemen
-00001810: 7420 6e61 6d65 3d22 4349 4e50 6c61 6e45  t name="CINPlanE
-00001820: 6e64 4461 7465 2220 7479 7065 3d22 7873  ndDate" type="xs
-00001830: 3a64 6174 6522 206d 696e 4f63 6375 7273  :date" minOccurs
-00001840: 3d22 3022 206d 6178 4f63 6375 7273 3d22  ="0" maxOccurs="
-00001850: 3122 2f3e 0a20 2020 203c 2f78 733a 7365  1"/>.    </xs:se
-00001860: 7175 656e 6365 3e0a 2020 3c2f 7873 3a63  quence>.  </xs:c
-00001870: 6f6d 706c 6578 5479 7065 3e0a 0a20 203c  omplexType>..  <
-00001880: 7873 3a63 6f6d 706c 6578 5479 7065 206e  xs:complexType n
-00001890: 616d 653d 2273 6563 7469 6f6e 3437 7479  ame="section47ty
-000018a0: 7065 223e 0a20 2020 203c 7873 3a73 6571  pe">.    <xs:seq
-000018b0: 7565 6e63 653e 0a20 2020 2020 203c 7873  uence>.      <xs
-000018c0: 3a65 6c65 6d65 6e74 206e 616d 653d 2253  :element name="S
-000018d0: 3437 4163 7475 616c 5374 6172 7444 6174  47ActualStartDat
-000018e0: 6522 2074 7970 653d 2278 733a 6461 7465  e" type="xs:date
-000018f0: 2220 6d69 6e4f 6363 7572 733d 2231 2220  " minOccurs="1" 
-00001900: 6d61 784f 6363 7572 733d 2231 222f 3e0a  maxOccurs="1"/>.
-00001910: 2020 2020 2020 3c78 733a 656c 656d 656e        <xs:elemen
-00001920: 7420 6e61 6d65 3d22 496e 6974 6961 6c43  t name="InitialC
-00001930: 5043 7461 7267 6574 2220 7479 7065 3d22  PCtarget" type="
-00001940: 7873 3a64 6174 6522 206d 696e 4f63 6375  xs:date" minOccu
-00001950: 7273 3d22 3022 206d 6178 4f63 6375 7273  rs="0" maxOccurs
-00001960: 3d22 3122 2f3e 0a20 2020 2020 203c 7873  ="1"/>.      <xs
-00001970: 3a65 6c65 6d65 6e74 206e 616d 653d 2244  :element name="D
-00001980: 6174 654f 6649 6e69 7469 616c 4350 4322  ateOfInitialCPC"
-00001990: 2074 7970 653d 2278 733a 6461 7465 2220   type="xs:date" 
-000019a0: 6d69 6e4f 6363 7572 733d 2230 2220 6d61  minOccurs="0" ma
-000019b0: 784f 6363 7572 733d 2231 222f 3e0a 2020  xOccurs="1"/>.  
-000019c0: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
-000019d0: 6e61 6d65 3d22 4943 5043 6e6f 7452 6571  name="ICPCnotReq
-000019e0: 7569 7265 6422 2074 7970 653d 2279 6573  uired" type="yes
-000019f0: 6e6f 7479 7065 2220 6d69 6e4f 6363 7572  notype" minOccur
-00001a00: 733d 2231 2220 6d61 784f 6363 7572 733d  s="1" maxOccurs=
-00001a10: 2231 222f 3e0a 2020 2020 3c2f 7873 3a73  "1"/>.    </xs:s
-00001a20: 6571 7565 6e63 653e 0a20 203c 2f78 733a  equence>.  </xs:
-00001a30: 636f 6d70 6c65 7854 7970 653e 0a0a 2020  complexType>..  
-00001a40: 3c78 733a 636f 6d70 6c65 7854 7970 6520  <xs:complexType 
-00001a50: 6e61 6d65 3d22 6368 696c 6470 726f 7465  name="childprote
-00001a60: 6374 696f 6e70 6c61 6e73 7479 7065 223e  ctionplanstype">
-00001a70: 0a20 2020 203c 7873 3a73 6571 7565 6e63  .    <xs:sequenc
-00001a80: 653e 0a20 2020 2020 203c 7873 3a65 6c65  e>.      <xs:ele
-00001a90: 6d65 6e74 206e 616d 653d 2243 5050 7374  ment name="CPPst
-00001aa0: 6172 7444 6174 6522 2074 7970 653d 2278  artDate" type="x
-00001ab0: 733a 6461 7465 2220 6d69 6e4f 6363 7572  s:date" minOccur
-00001ac0: 733d 2231 2220 6d61 784f 6363 7572 733d  s="1" maxOccurs=
-00001ad0: 2231 222f 3e0a 2020 2020 2020 3c78 733a  "1"/>.      <xs:
-00001ae0: 656c 656d 656e 7420 6e61 6d65 3d22 4350  element name="CP
-00001af0: 5065 6e64 4461 7465 2220 7479 7065 3d22  PendDate" type="
-00001b00: 7873 3a64 6174 6522 206d 696e 4f63 6375  xs:date" minOccu
-00001b10: 7273 3d22 3022 206d 6178 4f63 6375 7273  rs="0" maxOccurs
-00001b20: 3d22 3122 2f3e 0a20 2020 2020 203c 7873  ="1"/>.      <xs
-00001b30: 3a65 6c65 6d65 6e74 206e 616d 653d 2249  :element name="I
-00001b40: 6e69 7469 616c 4361 7465 676f 7279 4f66  nitialCategoryOf
-00001b50: 4162 7573 6522 2074 7970 653d 2263 6174  Abuse" type="cat
-00001b60: 6567 6f72 796f 6661 6275 7365 2220 6d69  egoryofabuse" mi
-00001b70: 6e4f 6363 7572 733d 2231 2220 6d61 784f  nOccurs="1" maxO
-00001b80: 6363 7572 733d 2231 222f 3e0a 2020 2020  ccurs="1"/>.    
-00001b90: 2020 3c78 733a 656c 656d 656e 7420 6e61    <xs:element na
-00001ba0: 6d65 3d22 4c61 7465 7374 4361 7465 676f  me="LatestCatego
-00001bb0: 7279 4f66 4162 7573 6522 2074 7970 653d  ryOfAbuse" type=
-00001bc0: 2263 6174 6567 6f72 796f 6661 6275 7365  "categoryofabuse
-00001bd0: 2220 6d69 6e4f 6363 7572 733d 2231 2220  " minOccurs="1" 
-00001be0: 6d61 784f 6363 7572 733d 2231 222f 3e0a  maxOccurs="1"/>.
-00001bf0: 2020 2020 2020 3c78 733a 656c 656d 656e        <xs:elemen
-00001c00: 7420 6e61 6d65 3d22 4e75 6d62 6572 4f66  t name="NumberOf
-00001c10: 5072 6576 696f 7573 4350 5022 2074 7970  PreviousCPP" typ
-00001c20: 653d 2278 733a 706f 7369 7469 7665 496e  e="xs:positiveIn
-00001c30: 7465 6765 7222 206d 696e 4f63 6375 7273  teger" minOccurs
-00001c40: 3d22 3122 206d 6178 4f63 6375 7273 3d22  ="1" maxOccurs="
-00001c50: 3122 2f3e 0a20 2020 2020 203c 7873 3a65  1"/>.      <xs:e
-00001c60: 6c65 6d65 6e74 206e 616d 653d 2252 6576  lement name="Rev
-00001c70: 6965 7773 2220 6d69 6e4f 6363 7572 733d  iews" minOccurs=
-00001c80: 2230 2220 6d61 784f 6363 7572 733d 2231  "0" maxOccurs="1
-00001c90: 223e 0a20 2020 2020 2020 203c 7873 3a63  ">.        <xs:c
-00001ca0: 6f6d 706c 6578 5479 7065 3e0a 2020 2020  omplexType>.    
-00001cb0: 2020 2020 2020 3c78 733a 7365 7175 656e        <xs:sequen
-00001cc0: 6365 3e0a 2020 2020 2020 2020 2020 2020  ce>.            
-00001cd0: 3c78 733a 656c 656d 656e 7420 6e61 6d65  <xs:element name
-00001ce0: 3d22 4350 5072 6576 6965 7744 6174 6522  ="CPPreviewDate"
-00001cf0: 2074 7970 653d 2278 733a 6461 7465 2220   type="xs:date" 
-00001d00: 6d69 6e4f 6363 7572 733d 2231 2220 6d61  minOccurs="1" ma
-00001d10: 784f 6363 7572 733d 2275 6e62 6f75 6e64  xOccurs="unbound
-00001d20: 6564 222f 3e0a 2020 2020 2020 2020 2020  ed"/>.          
-00001d30: 3c2f 7873 3a73 6571 7565 6e63 653e 0a20  </xs:sequence>. 
-00001d40: 2020 2020 2020 203c 2f78 733a 636f 6d70         </xs:comp
-00001d50: 6c65 7854 7970 653e 0a20 2020 2020 203c  lexType>.      <
-00001d60: 2f78 733a 656c 656d 656e 743e 0a20 2020  /xs:element>.   
-00001d70: 203c 2f78 733a 7365 7175 656e 6365 3e0a   </xs:sequence>.
-00001d80: 2020 3c2f 7873 3a63 6f6d 706c 6578 5479    </xs:complexTy
-00001d90: 7065 3e0a 0a20 203c 7873 3a73 696d 706c  pe>..  <xs:simpl
-00001da0: 6554 7970 6520 6e61 6d65 3d22 6e6f 6e45  eType name="nonE
-00001db0: 6d70 7479 5374 7269 6e67 223e 0a20 2020  mptyString">.   
-00001dc0: 203c 7873 3a72 6573 7472 6963 7469 6f6e   <xs:restriction
-00001dd0: 2062 6173 653d 2278 733a 7374 7269 6e67   base="xs:string
-00001de0: 223e 0a20 2020 2020 203c 7873 3a6d 696e  ">.      <xs:min
-00001df0: 4c65 6e67 7468 2076 616c 7565 3d22 3122  Length value="1"
-00001e00: 2f3e 0a20 2020 203c 2f78 733a 7265 7374  />.    </xs:rest
-00001e10: 7269 6374 696f 6e3e 0a20 203c 2f78 733a  riction>.  </xs:
-00001e20: 7369 6d70 6c65 5479 7065 3e0a 0a20 203c  simpleType>..  <
-00001e30: 7873 3a73 696d 706c 6554 7970 6520 6e61  xs:simpleType na
-00001e40: 6d65 3d22 7965 736e 6f74 7970 6522 3e0a  me="yesnotype">.
-00001e50: 2020 2020 3c78 733a 7265 7374 7269 6374      <xs:restrict
-00001e60: 696f 6e20 6261 7365 3d22 6e6f 6e45 6d70  ion base="nonEmp
-00001e70: 7479 5374 7269 6e67 223e 0a20 2020 2020  tyString">.     
-00001e80: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
-00001e90: 2076 616c 7565 3d22 7472 7565 2220 2f3e   value="true" />
-00001ea0: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
-00001eb0: 7261 7469 6f6e 2076 616c 7565 3d22 6661  ration value="fa
-00001ec0: 6c73 6522 202f 3e0a 0920 203c 7873 3a65  lse" />..  <xs:e
-00001ed0: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
-00001ee0: 3d22 5452 5545 2220 2f3e 0a20 2020 2020  ="TRUE" />.     
-00001ef0: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
-00001f00: 2076 616c 7565 3d22 4641 4c53 4522 202f   value="FALSE" /
-00001f10: 3e0a 2020 2020 2020 3c78 733a 656e 756d  >.      <xs:enum
-00001f20: 6572 6174 696f 6e20 7661 6c75 653d 2230  eration value="0
-00001f30: 2220 2f3e 0a20 2020 2020 203c 7873 3a65  " />.      <xs:e
-00001f40: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
-00001f50: 3d22 3122 202f 3e0a 2020 2020 3c2f 7873  ="1" />.    </xs
-00001f60: 3a72 6573 7472 6963 7469 6f6e 3e0a 2020  :restriction>.  
-00001f70: 3c2f 7873 3a73 696d 706c 6554 7970 653e  </xs:simpleType>
-00001f80: 0a0a 2020 3c78 733a 7369 6d70 6c65 5479  ..  <xs:simpleTy
-00001f90: 7065 206e 616d 653d 2275 706e 7479 7065  pe name="upntype
-00001fa0: 223e 0a20 2020 203c 7873 3a72 6573 7472  ">.    <xs:restr
-00001fb0: 6963 7469 6f6e 2062 6173 653d 2278 733a  iction base="xs:
-00001fc0: 7374 7269 6e67 223e 0a20 2020 2020 203c  string">.      <
-00001fd0: 7873 3a70 6174 7465 726e 2076 616c 7565  xs:pattern value
-00001fe0: 3d22 5b41 2d5a 612d 7a5d 5c64 7b31 327d  ="[A-Za-z]\d{12}
-00001ff0: 222f 3e0a 2020 2020 2020 3c78 733a 7061  "/>.      <xs:pa
-00002000: 7474 6572 6e20 7661 6c75 653d 225b 412d  ttern value="[A-
-00002010: 5a61 2d7a 5d5c 647b 3131 7d5b 412d 5a61  Za-z]\d{11}[A-Za
-00002020: 2d7a 5d22 2f3e 0a20 2020 203c 2f78 733a  -z]"/>.    </xs:
-00002030: 7265 7374 7269 6374 696f 6e3e 0a20 203c  restriction>.  <
-00002040: 2f78 733a 7369 6d70 6c65 5479 7065 3e0a  /xs:simpleType>.
-00002050: 0a20 203c 7873 3a73 696d 706c 6554 7970  .  <xs:simpleTyp
-00002060: 6520 6e61 6d65 3d22 756e 6b6e 6f77 6e75  e name="unknownu
-00002070: 706e 7479 7065 223e 0a20 2020 203c 7873  pntype">.    <xs
-00002080: 3a72 6573 7472 6963 7469 6f6e 2062 6173  :restriction bas
-00002090: 653d 2278 733a 7374 7269 6e67 223e 0a20  e="xs:string">. 
-000020a0: 2020 2020 203c 7873 3a65 6e75 6d65 7261       <xs:enumera
-000020b0: 7469 6f6e 2076 616c 7565 3d22 554e 3122  tion value="UN1"
-000020c0: 202f 3e0a 2020 2020 2020 3c78 733a 656e   />.      <xs:en
-000020d0: 756d 6572 6174 696f 6e20 7661 6c75 653d  umeration value=
-000020e0: 2255 4e32 2220 2f3e 0a20 2020 2020 203c  "UN2" />.      <
-000020f0: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
-00002100: 616c 7565 3d22 554e 3322 202f 3e0a 2020  alue="UN3" />.  
-00002110: 2020 2020 3c78 733a 656e 756d 6572 6174      <xs:enumerat
-00002120: 696f 6e20 7661 6c75 653d 2255 4e34 2220  ion value="UN4" 
-00002130: 2f3e 0a20 2020 2020 203c 7873 3a65 6e75  />.      <xs:enu
-00002140: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-00002150: 554e 3522 202f 3e0a 2020 2020 2020 3c78  UN5" />.      <x
-00002160: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
-00002170: 6c75 653d 2255 4e36 2220 2f3e 0a20 2020  lue="UN6" />.   
-00002180: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
-00002190: 6f6e 2076 616c 7565 3d22 554e 3722 202f  on value="UN7" /
-000021a0: 3e0a 2020 2020 3c2f 7873 3a72 6573 7472  >.    </xs:restr
-000021b0: 6963 7469 6f6e 3e0a 2020 3c2f 7873 3a73  iction>.  </xs:s
-000021c0: 696d 706c 6554 7970 653e 0a0a 2020 3c78  impleType>..  <x
-000021d0: 733a 7369 6d70 6c65 5479 7065 206e 616d  s:simpleType nam
-000021e0: 653d 2267 656e 6465 7274 7970 6522 3e0a  e="gendertype">.
-000021f0: 2020 2020 3c78 733a 7265 7374 7269 6374      <xs:restrict
-00002200: 696f 6e20 6261 7365 3d22 6e6f 6e45 6d70  ion base="nonEmp
-00002210: 7479 5374 7269 6e67 223e 0a20 2020 2020  tyString">.     
-00002220: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
-00002230: 2076 616c 7565 3d22 3122 3e0a 2020 2020   value="1">.    
-00002240: 2020 2020 3c78 733a 616e 6e6f 7461 7469      <xs:annotati
-00002250: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
-00002260: 7469 6f6e 3e4d 616c 653c 2f78 733a 646f  tion>Male</xs:do
-00002270: 6375 6d65 6e74 6174 696f 6e3e 3c2f 7873  cumentation></xs
-00002280: 3a61 6e6e 6f74 6174 696f 6e3e 0a20 2020  :annotation>.   
-00002290: 2020 203c 2f78 733a 656e 756d 6572 6174     </xs:enumerat
-000022a0: 696f 6e3e 0a20 2020 2020 203c 7873 3a65  ion>.      <xs:e
-000022b0: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
-000022c0: 3d22 3222 3e0a 2020 2020 2020 2020 3c78  ="2">.        <x
-000022d0: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
-000022e0: 3a64 6f63 756d 656e 7461 7469 6f6e 3e46  :documentation>F
-000022f0: 656d 616c 653c 2f78 733a 646f 6375 6d65  emale</xs:docume
-00002300: 6e74 6174 696f 6e3e 3c2f 7873 3a61 6e6e  ntation></xs:ann
-00002310: 6f74 6174 696f 6e3e 0a20 2020 2020 203c  otation>.      <
-00002320: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
-00002330: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
-00002340: 7261 7469 6f6e 2076 616c 7565 3d22 3022  ration value="0"
-00002350: 3e0a 2020 2020 2020 2020 3c78 733a 616e  >.        <xs:an
-00002360: 6e6f 7461 7469 6f6e 3e3c 7873 3a64 6f63  notation><xs:doc
-00002370: 756d 656e 7461 7469 6f6e 3e4e 6f74 2072  umentation>Not r
-00002380: 6563 6f72 6465 6420 6f72 2075 6e62 6f72  ecorded or unbor
-00002390: 6e3c 2f78 733a 646f 6375 6d65 6e74 6174  n</xs:documentat
-000023a0: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
-000023b0: 696f 6e3e 0a20 2020 2020 203c 2f78 733a  ion>.      </xs:
-000023c0: 656e 756d 6572 6174 696f 6e3e 0a20 2020  enumeration>.   
-000023d0: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
-000023e0: 6f6e 2076 616c 7565 3d22 3922 3e0a 2020  on value="9">.  
-000023f0: 2020 2020 2020 3c78 733a 616e 6e6f 7461        <xs:annota
-00002400: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
-00002410: 7461 7469 6f6e 3e49 6e64 6574 6572 6d69  tation>Indetermi
-00002420: 6e61 7465 3c2f 7873 3a64 6f63 756d 656e  nate</xs:documen
-00002430: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
-00002440: 7461 7469 6f6e 3e0a 2020 2020 2020 3c2f  tation>.      </
-00002450: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0a  xs:enumeration>.
-00002460: 2020 2020 3c2f 7873 3a72 6573 7472 6963      </xs:restric
-00002470: 7469 6f6e 3e0a 2020 3c2f 7873 3a73 696d  tion>.  </xs:sim
-00002480: 706c 6554 7970 653e 0a0a 0a20 203c 7873  pleType>...  <xs
-00002490: 3a73 696d 706c 6554 7970 6520 6e61 6d65  :simpleType name
-000024a0: 3d22 6574 686e 6963 6974 7974 7970 6522  ="ethnicitytype"
-000024b0: 3e0a 2020 2020 3c78 733a 7265 7374 7269  >.    <xs:restri
-000024c0: 6374 696f 6e20 6261 7365 3d22 6e6f 6e45  ction base="nonE
-000024d0: 6d70 7479 5374 7269 6e67 223e 0a20 2020  mptyString">.   
-000024e0: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
-000024f0: 6f6e 2076 616c 7565 3d22 5742 5249 223e  on value="WBRI">
-00002500: 3c78 733a 616e 6e6f 7461 7469 6f6e 3e3c  <xs:annotation><
-00002510: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00002520: 3e57 6869 7465 2042 7269 7469 7368 3c2f  >White British</
-00002530: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00002540: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
-00002550: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
-00002560: 6e3e 0a20 2020 2020 203c 7873 3a65 6e75  n>.      <xs:enu
-00002570: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-00002580: 5749 5249 223e 3c78 733a 616e 6e6f 7461  WIRI"><xs:annota
-00002590: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
-000025a0: 7461 7469 6f6e 3e57 6869 7465 2049 7269  tation>White Iri
-000025b0: 7368 3c2f 7873 3a64 6f63 756d 656e 7461  sh</xs:documenta
-000025c0: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
-000025d0: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
-000025e0: 6174 696f 6e3e 0a20 2020 2020 203c 7873  ation>.      <xs
-000025f0: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
-00002600: 7565 3d22 5749 5254 223e 3c78 733a 616e  ue="WIRT"><xs:an
-00002610: 6e6f 7461 7469 6f6e 3e3c 7873 3a64 6f63  notation><xs:doc
-00002620: 756d 656e 7461 7469 6f6e 3e54 7261 7665  umentation>Trave
-00002630: 6c6c 6572 206f 6620 4972 6973 6820 6865  ller of Irish he
-00002640: 7269 7461 6765 3c2f 7873 3a64 6f63 756d  ritage</xs:docum
-00002650: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
-00002660: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
-00002670: 756d 6572 6174 696f 6e3e 0a20 2020 2020  umeration>.     
-00002680: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
-00002690: 2076 616c 7565 3d22 574f 5448 223e 3c78   value="WOTH"><x
-000026a0: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
-000026b0: 3a64 6f63 756d 656e 7461 7469 6f6e 3e41  :documentation>A
-000026c0: 6e79 206f 7468 6572 2057 6869 7465 2062  ny other White b
-000026d0: 6163 6b67 726f 756e 643c 2f78 733a 646f  ackground</xs:do
-000026e0: 6375 6d65 6e74 6174 696f 6e3e 3c2f 7873  cumentation></xs
-000026f0: 3a61 6e6e 6f74 6174 696f 6e3e 3c2f 7873  :annotation></xs
-00002700: 3a65 6e75 6d65 7261 7469 6f6e 3e0a 2020  :enumeration>.  
-00002710: 2020 2020 3c78 733a 656e 756d 6572 6174      <xs:enumerat
-00002720: 696f 6e20 7661 6c75 653d 2257 524f 4d22  ion value="WROM"
-00002730: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
-00002740: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
-00002750: 6e3e 4779 7073 792f 526f 6d61 3c2f 7873  n>Gypsy/Roma</xs
-00002760: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
-00002770: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
-00002780: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
-00002790: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
-000027a0: 7261 7469 6f6e 2076 616c 7565 3d22 4d57  ration value="MW
-000027b0: 4243 223e 3c78 733a 616e 6e6f 7461 7469  BC"><xs:annotati
-000027c0: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
-000027d0: 7469 6f6e 3e57 6869 7465 2061 6e64 2042  tion>White and B
-000027e0: 6c61 636b 2043 6172 6962 6265 616e 3c2f  lack Caribbean</
-000027f0: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00002800: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
-00002810: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
-00002820: 6e3e 0a20 2020 2020 203c 7873 3a65 6e75  n>.      <xs:enu
-00002830: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-00002840: 4d57 4241 223e 3c78 733a 616e 6e6f 7461  MWBA"><xs:annota
-00002850: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
-00002860: 7461 7469 6f6e 3e57 6869 7465 2061 6e64  tation>White and
-00002870: 2042 6c61 636b 2041 6672 6963 616e 3c2f   Black African</
-00002880: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00002890: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
-000028a0: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
-000028b0: 6e3e 0a20 2020 2020 203c 7873 3a65 6e75  n>.      <xs:enu
-000028c0: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-000028d0: 4d57 4153 223e 3c78 733a 616e 6e6f 7461  MWAS"><xs:annota
-000028e0: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
-000028f0: 7461 7469 6f6e 3e57 6869 7465 2061 6e64  tation>White and
-00002900: 2041 7369 616e 3c2f 7873 3a64 6f63 756d   Asian</xs:docum
-00002910: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
-00002920: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
-00002930: 756d 6572 6174 696f 6e3e 0a20 2020 2020  umeration>.     
-00002940: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
-00002950: 2076 616c 7565 3d22 4d4f 5448 223e 3c78   value="MOTH"><x
-00002960: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
-00002970: 3a64 6f63 756d 656e 7461 7469 6f6e 3e41  :documentation>A
-00002980: 6e79 206f 7468 6572 206d 6978 6564 2062  ny other mixed b
-00002990: 6163 6b67 726f 756e 643c 2f78 733a 646f  ackground</xs:do
-000029a0: 6375 6d65 6e74 6174 696f 6e3e 3c2f 7873  cumentation></xs
-000029b0: 3a61 6e6e 6f74 6174 696f 6e3e 3c2f 7873  :annotation></xs
-000029c0: 3a65 6e75 6d65 7261 7469 6f6e 3e0a 2020  :enumeration>.  
-000029d0: 2020 2020 3c78 733a 656e 756d 6572 6174      <xs:enumerat
-000029e0: 696f 6e20 7661 6c75 653d 2241 494e 4422  ion value="AIND"
-000029f0: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
-00002a00: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
-00002a10: 6e3e 496e 6469 616e 3c2f 7873 3a64 6f63  n>Indian</xs:doc
-00002a20: 756d 656e 7461 7469 6f6e 3e3c 2f78 733a  umentation></xs:
-00002a30: 616e 6e6f 7461 7469 6f6e 3e3c 2f78 733a  annotation></xs:
-00002a40: 656e 756d 6572 6174 696f 6e3e 0a20 2020  enumeration>.   
-00002a50: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
-00002a60: 6f6e 2076 616c 7565 3d22 4150 4b4e 223e  on value="APKN">
-00002a70: 3c78 733a 616e 6e6f 7461 7469 6f6e 3e3c  <xs:annotation><
-00002a80: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00002a90: 3e50 616b 6973 7461 6e69 3c2f 7873 3a64  >Pakistani</xs:d
-00002aa0: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
-00002ab0: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
-00002ac0: 733a 656e 756d 6572 6174 696f 6e3e 0a20  s:enumeration>. 
-00002ad0: 2020 2020 203c 7873 3a65 6e75 6d65 7261       <xs:enumera
-00002ae0: 7469 6f6e 2076 616c 7565 3d22 4142 414e  tion value="ABAN
-00002af0: 223e 3c78 733a 616e 6e6f 7461 7469 6f6e  "><xs:annotation
-00002b00: 3e3c 7873 3a64 6f63 756d 656e 7461 7469  ><xs:documentati
-00002b10: 6f6e 3e42 616e 676c 6164 6573 6869 3c2f  on>Bangladeshi</
-00002b20: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00002b30: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
-00002b40: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
-00002b50: 6e3e 0a20 2020 2020 203c 7873 3a65 6e75  n>.      <xs:enu
-00002b60: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-00002b70: 414f 5448 223e 3c78 733a 616e 6e6f 7461  AOTH"><xs:annota
-00002b80: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
-00002b90: 7461 7469 6f6e 3e41 6e79 206f 7468 6572  tation>Any other
-00002ba0: 2041 7369 616e 2062 6163 6b67 726f 756e   Asian backgroun
-00002bb0: 643c 2f78 733a 646f 6375 6d65 6e74 6174  d</xs:documentat
-00002bc0: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
-00002bd0: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
-00002be0: 7469 6f6e 3e0a 2020 2020 2020 3c78 733a  tion>.      <xs:
-00002bf0: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
-00002c00: 653d 2242 4352 4222 3e3c 7873 3a61 6e6e  e="BCRB"><xs:ann
-00002c10: 6f74 6174 696f 6e3e 3c78 733a 646f 6375  otation><xs:docu
-00002c20: 6d65 6e74 6174 696f 6e3e 4361 7269 6262  mentation>Caribb
-00002c30: 6561 6e3c 2f78 733a 646f 6375 6d65 6e74  ean</xs:document
-00002c40: 6174 696f 6e3e 3c2f 7873 3a61 6e6e 6f74  ation></xs:annot
-00002c50: 6174 696f 6e3e 3c2f 7873 3a65 6e75 6d65  ation></xs:enume
-00002c60: 7261 7469 6f6e 3e0a 2020 2020 2020 3c78  ration>.      <x
-00002c70: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
-00002c80: 6c75 653d 2242 4146 5222 3e3c 7873 3a61  lue="BAFR"><xs:a
-00002c90: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
-00002ca0: 6375 6d65 6e74 6174 696f 6e3e 4166 7269  cumentation>Afri
-00002cb0: 6361 6e3c 2f78 733a 646f 6375 6d65 6e74  can</xs:document
-00002cc0: 6174 696f 6e3e 3c2f 7873 3a61 6e6e 6f74  ation></xs:annot
-00002cd0: 6174 696f 6e3e 3c2f 7873 3a65 6e75 6d65  ation></xs:enume
-00002ce0: 7261 7469 6f6e 3e0a 2020 2020 2020 3c78  ration>.      <x
-00002cf0: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
-00002d00: 6c75 653d 2242 4f54 4822 3e3c 7873 3a61  lue="BOTH"><xs:a
-00002d10: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
-00002d20: 6375 6d65 6e74 6174 696f 6e3e 416e 7920  cumentation>Any 
-00002d30: 6f74 6865 7220 626c 6163 6b20 6261 636b  other black back
-00002d40: 6772 6f75 6e64 3c2f 7873 3a64 6f63 756d  ground</xs:docum
-00002d50: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
-00002d60: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
-00002d70: 756d 6572 6174 696f 6e3e 0a20 2020 2020  umeration>.     
-00002d80: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
-00002d90: 2076 616c 7565 3d22 4348 4e45 223e 3c78   value="CHNE"><x
-00002da0: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
-00002db0: 3a64 6f63 756d 656e 7461 7469 6f6e 3e43  :documentation>C
-00002dc0: 6869 6e65 7365 3c2f 7873 3a64 6f63 756d  hinese</xs:docum
-00002dd0: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
-00002de0: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
-00002df0: 756d 6572 6174 696f 6e3e 0a20 2020 2020  umeration>.     
-00002e00: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
-00002e10: 2076 616c 7565 3d22 4f4f 5448 223e 3c78   value="OOTH"><x
-00002e20: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
-00002e30: 3a64 6f63 756d 656e 7461 7469 6f6e 3e41  :documentation>A
-00002e40: 6e79 206f 7468 6572 2065 7468 6e69 6320  ny other ethnic 
-00002e50: 6772 6f75 703c 2f78 733a 646f 6375 6d65  group</xs:docume
-00002e60: 6e74 6174 696f 6e3e 3c2f 7873 3a61 6e6e  ntation></xs:ann
-00002e70: 6f74 6174 696f 6e3e 3c2f 7873 3a65 6e75  otation></xs:enu
-00002e80: 6d65 7261 7469 6f6e 3e0a 2020 2020 2020  meration>.      
-00002e90: 3c78 733a 656e 756d 6572 6174 696f 6e20  <xs:enumeration 
-00002ea0: 7661 6c75 653d 2252 4546 5522 3e3c 7873  value="REFU"><xs
-00002eb0: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
-00002ec0: 646f 6375 6d65 6e74 6174 696f 6e3e 5265  documentation>Re
-00002ed0: 6675 7365 643c 2f78 733a 646f 6375 6d65  fused</xs:docume
-00002ee0: 6e74 6174 696f 6e3e 3c2f 7873 3a61 6e6e  ntation></xs:ann
-00002ef0: 6f74 6174 696f 6e3e 3c2f 7873 3a65 6e75  otation></xs:enu
-00002f00: 6d65 7261 7469 6f6e 3e0a 2020 2020 2020  meration>.      
-00002f10: 3c78 733a 656e 756d 6572 6174 696f 6e20  <xs:enumeration 
-00002f20: 7661 6c75 653d 224e 4f42 5422 3e3c 7873  value="NOBT"><xs
-00002f30: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
-00002f40: 646f 6375 6d65 6e74 6174 696f 6e3e 496e  documentation>In
-00002f50: 666f 726d 6174 696f 6e20 6e6f 7420 7965  formation not ye
-00002f60: 7420 6f62 7461 696e 6564 3c2f 7873 3a64  t obtained</xs:d
-00002f70: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
-00002f80: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
-00002f90: 733a 656e 756d 6572 6174 696f 6e3e 0a20  s:enumeration>. 
-00002fa0: 2020 203c 2f78 733a 7265 7374 7269 6374     </xs:restrict
-00002fb0: 696f 6e3e 0a20 203c 2f78 733a 7369 6d70  ion>.  </xs:simp
-00002fc0: 6c65 5479 7065 3e0a 0a20 203c 7873 3a73  leType>..  <xs:s
-00002fd0: 696d 706c 6554 7970 6520 6e61 6d65 3d22  impleType name="
-00002fe0: 6469 7361 6269 6c69 7479 7479 7065 223e  disabilitytype">
-00002ff0: 0a20 2020 203c 7873 3a72 6573 7472 6963  .    <xs:restric
-00003000: 7469 6f6e 2062 6173 653d 226e 6f6e 456d  tion base="nonEm
-00003010: 7074 7953 7472 696e 6722 3e0a 2020 2020  ptyString">.    
-00003020: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
-00003030: 6e20 7661 6c75 653d 224e 4f4e 4522 3e3c  n value="NONE"><
-00003040: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
-00003050: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
-00003060: 4e6f 2064 6973 6162 696c 6974 793c 2f78  No disability</x
-00003070: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
-00003080: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
-00003090: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
-000030a0: 3e0a 2020 2020 2020 3c78 733a 656e 756d  >.      <xs:enum
-000030b0: 6572 6174 696f 6e20 7661 6c75 653d 224d  eration value="M
-000030c0: 4f42 223e 3c78 733a 616e 6e6f 7461 7469  OB"><xs:annotati
-000030d0: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
-000030e0: 7469 6f6e 3e4d 6f62 696c 6974 793c 2f78  tion>Mobility</x
-000030f0: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
-00003100: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
-00003110: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
-00003120: 3e0a 2020 2020 2020 3c78 733a 656e 756d  >.      <xs:enum
-00003130: 6572 6174 696f 6e20 7661 6c75 653d 2248  eration value="H
-00003140: 414e 4422 3e3c 7873 3a61 6e6e 6f74 6174  AND"><xs:annotat
-00003150: 696f 6e3e 3c78 733a 646f 6375 6d65 6e74  ion><xs:document
-00003160: 6174 696f 6e3e 4861 6e64 2066 756e 6374  ation>Hand funct
-00003170: 696f 6e3c 2f78 733a 646f 6375 6d65 6e74  ion</xs:document
-00003180: 6174 696f 6e3e 3c2f 7873 3a61 6e6e 6f74  ation></xs:annot
-00003190: 6174 696f 6e3e 3c2f 7873 3a65 6e75 6d65  ation></xs:enume
-000031a0: 7261 7469 6f6e 3e0a 2020 2020 2020 3c78  ration>.      <x
-000031b0: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
-000031c0: 6c75 653d 2250 4322 3e3c 7873 3a61 6e6e  lue="PC"><xs:ann
-000031d0: 6f74 6174 696f 6e3e 3c78 733a 646f 6375  otation><xs:docu
-000031e0: 6d65 6e74 6174 696f 6e3e 5065 7273 6f6e  mentation>Person
-000031f0: 616c 2063 6172 653c 2f78 733a 646f 6375  al care</xs:docu
-00003200: 6d65 6e74 6174 696f 6e3e 3c2f 7873 3a61  mentation></xs:a
-00003210: 6e6e 6f74 6174 696f 6e3e 3c2f 7873 3a65  nnotation></xs:e
-00003220: 6e75 6d65 7261 7469 6f6e 3e0a 2020 2020  numeration>.    
-00003230: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
-00003240: 6e20 7661 6c75 653d 2249 4e43 223e 3c78  n value="INC"><x
-00003250: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
-00003260: 3a64 6f63 756d 656e 7461 7469 6f6e 3e49  :documentation>I
-00003270: 6e63 6f6e 7469 6e65 6e63 653c 2f78 733a  ncontinence</xs:
-00003280: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
-00003290: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
-000032a0: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0a  xs:enumeration>.
-000032b0: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
-000032c0: 6174 696f 6e20 7661 6c75 653d 2243 4f4d  ation value="COM
-000032d0: 4d22 3e3c 7873 3a61 6e6e 6f74 6174 696f  M"><xs:annotatio
-000032e0: 6e3e 3c78 733a 646f 6375 6d65 6e74 6174  n><xs:documentat
-000032f0: 696f 6e3e 436f 6d6d 756e 6963 6174 696f  ion>Communicatio
-00003300: 6e3c 2f78 733a 646f 6375 6d65 6e74 6174  n</xs:documentat
-00003310: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
-00003320: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
-00003330: 7469 6f6e 3e0a 2020 2020 2020 3c78 733a  tion>.      <xs:
-00003340: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
-00003350: 653d 224c 4422 3e3c 7873 3a61 6e6e 6f74  e="LD"><xs:annot
-00003360: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
-00003370: 6e74 6174 696f 6e3e 4c65 6172 6e69 6e67  ntation>Learning
-00003380: 3c2f 7873 3a64 6f63 756d 656e 7461 7469  </xs:documentati
-00003390: 6f6e 3e3c 2f78 733a 616e 6e6f 7461 7469  on></xs:annotati
-000033a0: 6f6e 3e3c 2f78 733a 656e 756d 6572 6174  on></xs:enumerat
-000033b0: 696f 6e3e 0a20 2020 2020 203c 7873 3a65  ion>.      <xs:e
-000033c0: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
-000033d0: 3d22 4845 4152 223e 3c78 733a 616e 6e6f  ="HEAR"><xs:anno
-000033e0: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
-000033f0: 656e 7461 7469 6f6e 3e48 6561 7269 6e67  entation>Hearing
-00003400: 3c2f 7873 3a64 6f63 756d 656e 7461 7469  </xs:documentati
-00003410: 6f6e 3e3c 2f78 733a 616e 6e6f 7461 7469  on></xs:annotati
-00003420: 6f6e 3e3c 2f78 733a 656e 756d 6572 6174  on></xs:enumerat
-00003430: 696f 6e3e 0a20 2020 2020 203c 7873 3a65  ion>.      <xs:e
-00003440: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
-00003450: 3d22 5649 5322 3e3c 7873 3a61 6e6e 6f74  ="VIS"><xs:annot
-00003460: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
-00003470: 6e74 6174 696f 6e3e 5669 7369 6f6e 3c2f  ntation>Vision</
-00003480: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00003490: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
-000034a0: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
-000034b0: 6e3e 0a20 2020 2020 203c 7873 3a65 6e75  n>.      <xs:enu
+00000020: 462d 3822 203f 3e0d 0a3c 7873 3a73 6368  F-8" ?>..<xs:sch
+00000030: 656d 6120 786d 6c6e 733a 7873 3d22 6874  ema xmlns:xs="ht
+00000040: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00000050: 3230 3031 2f58 4d4c 5363 6865 6d61 223e  2001/XMLSchema">
+00000060: 0d0a 0d0a 2020 3c78 733a 656c 656d 656e  ....  <xs:elemen
+00000070: 7420 6e61 6d65 3d22 4d65 7373 6167 6522  t name="Message"
+00000080: 2074 7970 653d 226d 6573 7361 6765 7479   type="messagety
+00000090: 7065 222f 3e0d 0a0d 0a20 203c 7873 3a63  pe"/>....  <xs:c
+000000a0: 6f6d 706c 6578 5479 7065 206e 616d 653d  omplexType name=
+000000b0: 226d 6573 7361 6765 7479 7065 223e 0d0a  "messagetype">..
+000000c0: 2020 2020 3c78 733a 7365 7175 656e 6365      <xs:sequence
+000000d0: 3e0d 0a20 2020 2020 203c 7873 3a65 6c65  >..      <xs:ele
+000000e0: 6d65 6e74 206e 616d 653d 2248 6561 6465  ment name="Heade
+000000f0: 7222 2074 7970 653d 2268 6561 6465 7274  r" type="headert
+00000100: 7970 6522 206d 696e 4f63 6375 7273 3d22  ype" minOccurs="
+00000110: 3022 206d 6178 4f63 6375 7273 3d22 3122  0" maxOccurs="1"
+00000120: 2f3e 0d0a 2020 2020 2020 3c78 733a 656c  />..      <xs:el
+00000130: 656d 656e 7420 6e61 6d65 3d22 4368 696c  ement name="Chil
+00000140: 6472 656e 2220 7479 7065 3d22 6368 696c  dren" type="chil
+00000150: 6472 656e 7479 7065 2220 6d69 6e4f 6363  drentype" minOcc
+00000160: 7572 733d 2231 2220 6d61 784f 6363 7572  urs="1" maxOccur
+00000170: 733d 2231 222f 3e0d 0a20 2020 203c 2f78  s="1"/>..    </x
+00000180: 733a 7365 7175 656e 6365 3e0d 0a20 203c  s:sequence>..  <
+00000190: 2f78 733a 636f 6d70 6c65 7854 7970 653e  /xs:complexType>
+000001a0: 0d0a 0d0a 2020 3c78 733a 636f 6d70 6c65  ....  <xs:comple
+000001b0: 7854 7970 6520 6e61 6d65 3d22 6865 6164  xType name="head
+000001c0: 6572 7479 7065 223e 0d0a 2020 2020 3c78  ertype">..    <x
+000001d0: 733a 7365 7175 656e 6365 3e0d 0a20 2020  s:sequence>..   
+000001e0: 2020 203c 7873 3a65 6c65 6d65 6e74 206e     <xs:element n
+000001f0: 616d 653d 2243 6f6c 6c65 6374 696f 6e44  ame="CollectionD
+00000200: 6574 6169 6c73 2220 7479 7065 3d22 636f  etails" type="co
+00000210: 6c6c 6563 7469 6f6e 6465 7461 696c 7374  llectiondetailst
+00000220: 7970 6522 206d 696e 4f63 6375 7273 3d22  ype" minOccurs="
+00000230: 3022 206d 6178 4f63 6375 7273 3d22 3122  0" maxOccurs="1"
+00000240: 2f3e 0d0a 2020 2020 2020 3c78 733a 656c  />..      <xs:el
+00000250: 656d 656e 7420 6e61 6d65 3d22 536f 7572  ement name="Sour
+00000260: 6365 2220 7479 7065 3d22 736f 7572 6365  ce" type="source
+00000270: 7479 7065 2220 6d69 6e4f 6363 7572 733d  type" minOccurs=
+00000280: 2230 2220 6d61 784f 6363 7572 733d 2275  "0" maxOccurs="u
+00000290: 6e62 6f75 6e64 6564 222f 3e0d 0a20 2020  nbounded"/>..   
+000002a0: 203c 2f78 733a 7365 7175 656e 6365 3e0d   </xs:sequence>.
+000002b0: 0a20 203c 2f78 733a 636f 6d70 6c65 7854  .  </xs:complexT
+000002c0: 7970 653e 0d0a 0d0a 2020 3c78 733a 636f  ype>....  <xs:co
+000002d0: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
+000002e0: 636f 6c6c 6563 7469 6f6e 6465 7461 696c  collectiondetail
+000002f0: 7374 7970 6522 3e0d 0a20 2020 203c 7873  stype">..    <xs
+00000300: 3a73 6571 7565 6e63 653e 0d0a 2020 2020  :sequence>..    
+00000310: 2020 3c78 733a 656c 656d 656e 7420 6e61    <xs:element na
+00000320: 6d65 3d22 436f 6c6c 6563 7469 6f6e 2220  me="Collection" 
+00000330: 6d69 6e4f 6363 7572 733d 2230 2220 6d61  minOccurs="0" ma
+00000340: 784f 6363 7572 733d 2231 223e 0d0a 2020  xOccurs="1">..  
+00000350: 2020 2020 2020 3c78 733a 7369 6d70 6c65        <xs:simple
+00000360: 5479 7065 3e0d 0a20 2020 2020 2020 2020  Type>..         
+00000370: 203c 7873 3a72 6573 7472 6963 7469 6f6e   <xs:restriction
+00000380: 2062 6173 653d 2278 733a 7374 7269 6e67   base="xs:string
+00000390: 223e 0d0a 2020 2020 2020 2020 2020 2020  ">..            
+000003a0: 3c78 733a 656e 756d 6572 6174 696f 6e20  <xs:enumeration 
+000003b0: 7661 6c75 653d 2243 494e 222f 3e0d 0a20  value="CIN"/>.. 
+000003c0: 2020 2020 2020 2020 203c 2f78 733a 7265           </xs:re
+000003d0: 7374 7269 6374 696f 6e3e 0d0a 2020 2020  striction>..    
+000003e0: 2020 2020 3c2f 7873 3a73 696d 706c 6554      </xs:simpleT
+000003f0: 7970 653e 0d0a 2020 2020 2020 3c2f 7873  ype>..      </xs
+00000400: 3a65 6c65 6d65 6e74 3e0d 0a20 2020 2020  :element>..     
+00000410: 203c 7873 3a65 6c65 6d65 6e74 206e 616d   <xs:element nam
+00000420: 653d 2259 6561 7222 2074 7970 653d 2278  e="Year" type="x
+00000430: 733a 6759 6561 7222 206d 696e 4f63 6375  s:gYear" minOccu
+00000440: 7273 3d22 3022 206d 6178 4f63 6375 7273  rs="0" maxOccurs
+00000450: 3d22 3122 2f3e 0d0a 2020 2020 2020 3c78  ="1"/>..      <x
+00000460: 733a 656c 656d 656e 7420 6e61 6d65 3d22  s:element name="
+00000470: 5265 6665 7265 6e63 6544 6174 6522 2074  ReferenceDate" t
+00000480: 7970 653d 2278 733a 6461 7465 2220 6d69  ype="xs:date" mi
+00000490: 6e4f 6363 7572 733d 2230 2220 6d61 784f  nOccurs="0" maxO
+000004a0: 6363 7572 733d 2231 222f 3e0d 0a20 2020  ccurs="1"/>..   
+000004b0: 203c 2f78 733a 7365 7175 656e 6365 3e0d   </xs:sequence>.
+000004c0: 0a20 203c 2f78 733a 636f 6d70 6c65 7854  .  </xs:complexT
+000004d0: 7970 653e 0d0a 0d0a 2020 3c78 733a 636f  ype>....  <xs:co
+000004e0: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
+000004f0: 736f 7572 6365 7479 7065 223e 0d0a 2020  sourcetype">..  
+00000500: 2020 3c78 733a 7365 7175 656e 6365 3e0d    <xs:sequence>.
+00000510: 0a20 2020 2020 203c 7873 3a65 6c65 6d65  .      <xs:eleme
+00000520: 6e74 206e 616d 653d 2253 6f75 7263 654c  nt name="SourceL
+00000530: 6576 656c 2220 6d69 6e4f 6363 7572 733d  evel" minOccurs=
+00000540: 2230 2220 6d61 784f 6363 7572 733d 2231  "0" maxOccurs="1
+00000550: 223e 0d0a 2020 2020 2020 2020 3c78 733a  ">..        <xs:
+00000560: 7369 6d70 6c65 5479 7065 3e0d 0a20 2020  simpleType>..   
+00000570: 2020 2020 2020 203c 7873 3a72 6573 7472         <xs:restr
+00000580: 6963 7469 6f6e 2062 6173 653d 2278 733a  iction base="xs:
+00000590: 7374 7269 6e67 223e 0d0a 2020 2020 2020  string">..      
+000005a0: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
+000005b0: 6174 696f 6e20 7661 6c75 653d 224c 222f  ation value="L"/
+000005c0: 3e0d 0a20 2020 2020 2020 2020 203c 2f78  >..          </x
+000005d0: 733a 7265 7374 7269 6374 696f 6e3e 0d0a  s:restriction>..
+000005e0: 2020 2020 2020 2020 3c2f 7873 3a73 696d          </xs:sim
+000005f0: 706c 6554 7970 653e 0d0a 2020 2020 2020  pleType>..      
+00000600: 3c2f 7873 3a65 6c65 6d65 6e74 3e0d 0a20  </xs:element>.. 
+00000610: 2020 2020 203c 7873 3a65 6c65 6d65 6e74       <xs:element
+00000620: 206e 616d 653d 224c 4541 2220 6d69 6e4f   name="LEA" minO
+00000630: 6363 7572 733d 2231 2220 6d61 784f 6363  ccurs="1" maxOcc
+00000640: 7572 733d 2231 223e 0d0a 2020 2020 2020  urs="1">..      
+00000650: 2020 3c78 733a 7369 6d70 6c65 5479 7065    <xs:simpleType
+00000660: 3e0d 0a20 2020 2020 2020 2020 203c 7873  >..          <xs
+00000670: 3a72 6573 7472 6963 7469 6f6e 2062 6173  :restriction bas
+00000680: 653d 2278 733a 7374 7269 6e67 2220 3e0d  e="xs:string" >.
+00000690: 0a20 2020 2020 2020 2020 2020 203c 7873  .            <xs
+000006a0: 3a70 6174 7465 726e 2076 616c 7565 3d22  :pattern value="
+000006b0: 5c64 7b33 7d22 2f3e 0d0a 2020 2020 2020  \d{3}"/>..      
+000006c0: 2020 2020 3c2f 7873 3a72 6573 7472 6963      </xs:restric
+000006d0: 7469 6f6e 3e0d 0a20 2020 2020 2020 203c  tion>..        <
+000006e0: 2f78 733a 7369 6d70 6c65 5479 7065 3e0d  /xs:simpleType>.
+000006f0: 0a20 2020 2020 203c 2f78 733a 656c 656d  .      </xs:elem
+00000700: 656e 743e 0d0a 2020 2020 2020 3c78 733a  ent>..      <xs:
+00000710: 656c 656d 656e 7420 6e61 6d65 3d22 536f  element name="So
+00000720: 6674 7761 7265 436f 6465 2220 7479 7065  ftwareCode" type
+00000730: 3d22 7873 3a73 7472 696e 6722 206d 696e  ="xs:string" min
+00000740: 4f63 6375 7273 3d22 3022 206d 6178 4f63  Occurs="0" maxOc
+00000750: 6375 7273 3d22 3122 2f3e 0d0a 2020 2020  curs="1"/>..    
+00000760: 2020 3c78 733a 656c 656d 656e 7420 6e61    <xs:element na
+00000770: 6d65 3d22 5265 6c65 6173 6522 2074 7970  me="Release" typ
+00000780: 653d 2278 733a 7374 7269 6e67 2220 6d69  e="xs:string" mi
+00000790: 6e4f 6363 7572 733d 2230 2220 6d61 784f  nOccurs="0" maxO
+000007a0: 6363 7572 733d 2231 222f 3e0d 0a20 2020  ccurs="1"/>..   
+000007b0: 2020 203c 7873 3a65 6c65 6d65 6e74 206e     <xs:element n
+000007c0: 616d 653d 2253 6572 6961 6c4e 6f22 206d  ame="SerialNo" m
+000007d0: 696e 4f63 6375 7273 3d22 3022 206d 6178  inOccurs="0" max
+000007e0: 4f63 6375 7273 3d22 3122 3e0d 0a20 2020  Occurs="1">..   
+000007f0: 2020 2020 203c 7873 3a73 696d 706c 6554       <xs:simpleT
+00000800: 7970 653e 0d0a 2020 2020 2020 2020 2020  ype>..          
+00000810: 3c78 733a 7265 7374 7269 6374 696f 6e20  <xs:restriction 
+00000820: 6261 7365 3d22 7873 3a73 7472 696e 6722  base="xs:string"
+00000830: 203e 0d0a 2020 2020 2020 2020 2020 2020   >..            
+00000840: 3c78 733a 7061 7474 6572 6e20 7661 6c75  <xs:pattern valu
+00000850: 653d 225c 647b 337d 5c64 2a22 2f3e 0d0a  e="\d{3}\d*"/>..
+00000860: 2020 2020 2020 2020 2020 3c2f 7873 3a72            </xs:r
+00000870: 6573 7472 6963 7469 6f6e 3e0d 0a20 2020  estriction>..   
+00000880: 2020 2020 203c 2f78 733a 7369 6d70 6c65       </xs:simple
+00000890: 5479 7065 3e0d 0a20 2020 2020 203c 2f78  Type>..      </x
+000008a0: 733a 656c 656d 656e 743e 0d0a 2020 2020  s:element>..    
+000008b0: 2020 3c78 733a 656c 656d 656e 7420 6e61    <xs:element na
+000008c0: 6d65 3d22 4461 7465 5469 6d65 2220 7479  me="DateTime" ty
+000008d0: 7065 3d22 7873 3a64 6174 6554 696d 6522  pe="xs:dateTime"
+000008e0: 206d 696e 4f63 6375 7273 3d22 3022 206d   minOccurs="0" m
+000008f0: 6178 4f63 6375 7273 3d22 3122 2f3e 0d0a  axOccurs="1"/>..
+00000900: 2020 2020 3c2f 7873 3a73 6571 7565 6e63      </xs:sequenc
+00000910: 653e 0d0a 2020 3c2f 7873 3a63 6f6d 706c  e>..  </xs:compl
+00000920: 6578 5479 7065 3e0d 0a0d 0a20 203c 7873  exType>....  <xs
+00000930: 3a63 6f6d 706c 6578 5479 7065 206e 616d  :complexType nam
+00000940: 653d 2263 6869 6c64 7265 6e74 7970 6522  e="childrentype"
+00000950: 3e0d 0a20 2020 203c 7873 3a73 6571 7565  >..    <xs:seque
+00000960: 6e63 653e 0d0a 2020 2020 2020 3c78 733a  nce>..      <xs:
+00000970: 656c 656d 656e 7420 6e61 6d65 3d22 4368  element name="Ch
+00000980: 696c 6422 2074 7970 653d 2263 6869 6c64  ild" type="child
+00000990: 7479 7065 2220 6d69 6e4f 6363 7572 733d  type" minOccurs=
+000009a0: 2231 2220 6d61 784f 6363 7572 733d 2275  "1" maxOccurs="u
+000009b0: 6e62 6f75 6e64 6564 222f 3e0d 0a20 2020  nbounded"/>..   
+000009c0: 203c 2f78 733a 7365 7175 656e 6365 3e0d   </xs:sequence>.
+000009d0: 0a20 203c 2f78 733a 636f 6d70 6c65 7854  .  </xs:complexT
+000009e0: 7970 653e 0d0a 0d0a 2020 3c78 733a 636f  ype>....  <xs:co
+000009f0: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
+00000a00: 6368 696c 6474 7970 6522 3e0d 0a20 2020  childtype">..   
+00000a10: 203c 7873 3a73 6571 7565 6e63 653e 0d0a   <xs:sequence>..
+00000a20: 2020 2020 2020 3c78 733a 656c 656d 656e        <xs:elemen
+00000a30: 7420 6e61 6d65 3d22 4368 696c 6449 6465  t name="ChildIde
+00000a40: 6e74 6966 6965 7273 2220 7479 7065 3d22  ntifiers" type="
+00000a50: 6368 696c 6469 6465 6e74 6966 6965 7273  childidentifiers
+00000a60: 7479 7065 2220 6d69 6e4f 6363 7572 733d  type" minOccurs=
+00000a70: 2231 2220 6d61 784f 6363 7572 733d 2231  "1" maxOccurs="1
+00000a80: 222f 3e0d 0a20 2020 2020 203c 7873 3a65  "/>..      <xs:e
+00000a90: 6c65 6d65 6e74 206e 616d 653d 2243 6869  lement name="Chi
+00000aa0: 6c64 4368 6172 6163 7465 7269 7374 6963  ldCharacteristic
+00000ab0: 7322 2074 7970 653d 2263 6869 6c64 6368  s" type="childch
+00000ac0: 6172 6163 7465 7269 7374 6963 7374 7970  aracteristicstyp
+00000ad0: 6522 206d 696e 4f63 6375 7273 3d22 3122  e" minOccurs="1"
+00000ae0: 206d 6178 4f63 6375 7273 3d22 3122 2f3e   maxOccurs="1"/>
+00000af0: 0d0a 2020 2020 2020 3c78 733a 656c 656d  ..      <xs:elem
+00000b00: 656e 7420 6e61 6d65 3d22 4349 4e64 6574  ent name="CINdet
+00000b10: 6169 6c73 2220 7479 7065 3d22 6369 6e64  ails" type="cind
+00000b20: 6574 6169 6c73 7479 7065 2220 6d69 6e4f  etailstype" minO
+00000b30: 6363 7572 733d 2231 2220 6d61 784f 6363  ccurs="1" maxOcc
+00000b40: 7572 733d 2275 6e62 6f75 6e64 6564 222f  urs="unbounded"/
+00000b50: 3e0d 0a20 2020 203c 2f78 733a 7365 7175  >..    </xs:sequ
+00000b60: 656e 6365 3e0d 0a20 203c 2f78 733a 636f  ence>..  </xs:co
+00000b70: 6d70 6c65 7854 7970 653e 0d0a 0d0a 2020  mplexType>....  
+00000b80: 3c78 733a 636f 6d70 6c65 7854 7970 6520  <xs:complexType 
+00000b90: 6e61 6d65 3d22 6368 696c 6469 6465 6e74  name="childident
+00000ba0: 6966 6965 7273 7479 7065 223e 0d0a 2020  ifierstype">..  
+00000bb0: 2020 3c78 733a 7365 7175 656e 6365 3e0d    <xs:sequence>.
+00000bc0: 0a20 2020 2020 203c 7873 3a65 6c65 6d65  .      <xs:eleme
+00000bd0: 6e74 206e 616d 653d 224c 4163 6869 6c64  nt name="LAchild
+00000be0: 4944 2220 7479 7065 3d22 6e6f 6e45 6d70  ID" type="nonEmp
+00000bf0: 7479 5374 7269 6e67 2220 6d69 6e4f 6363  tyString" minOcc
+00000c00: 7572 733d 2231 2220 6d61 784f 6363 7572  urs="1" maxOccur
+00000c10: 733d 2231 222f 3e0d 0a20 2020 2020 203c  s="1"/>..      <
+00000c20: 7873 3a65 6c65 6d65 6e74 206e 616d 653d  xs:element name=
+00000c30: 2255 504e 2220 7479 7065 3d22 7570 6e74  "UPN" type="upnt
+00000c40: 7970 6522 206d 696e 4f63 6375 7273 3d22  ype" minOccurs="
+00000c50: 3022 206d 6178 4f63 6375 7273 3d22 3122  0" maxOccurs="1"
+00000c60: 2f3e 0d0a 2020 2020 2020 3c78 733a 656c  />..      <xs:el
+00000c70: 656d 656e 7420 6e61 6d65 3d22 466f 726d  ement name="Form
+00000c80: 6572 5550 4e22 2074 7970 653d 2275 706e  erUPN" type="upn
+00000c90: 7479 7065 2220 6d69 6e4f 6363 7572 733d  type" minOccurs=
+00000ca0: 2230 2220 6d61 784f 6363 7572 733d 2231  "0" maxOccurs="1
+00000cb0: 222f 3e0d 0a20 2020 2020 203c 7873 3a65  "/>..      <xs:e
+00000cc0: 6c65 6d65 6e74 206e 616d 653d 2255 504e  lement name="UPN
+00000cd0: 756e 6b6e 6f77 6e22 2074 7970 653d 2275  unknown" type="u
+00000ce0: 6e6b 6e6f 776e 7570 6e74 7970 6522 206d  nknownupntype" m
+00000cf0: 696e 4f63 6375 7273 3d22 3022 206d 6178  inOccurs="0" max
+00000d00: 4f63 6375 7273 3d22 3122 2f3e 0d0a 2020  Occurs="1"/>..  
+00000d10: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
+00000d20: 6e61 6d65 3d22 5065 7273 6f6e 4269 7274  name="PersonBirt
+00000d30: 6844 6174 6522 2074 7970 653d 2278 733a  hDate" type="xs:
+00000d40: 6461 7465 2220 6d69 6e4f 6363 7572 733d  date" minOccurs=
+00000d50: 2230 2220 6d61 784f 6363 7572 733d 2231  "0" maxOccurs="1
+00000d60: 222f 3e0d 0a20 2020 2020 203c 7873 3a65  "/>..      <xs:e
+00000d70: 6c65 6d65 6e74 206e 616d 653d 2245 7870  lement name="Exp
+00000d80: 6563 7465 6450 6572 736f 6e42 6972 7468  ectedPersonBirth
+00000d90: 4461 7465 2220 7479 7065 3d22 7873 3a64  Date" type="xs:d
+00000da0: 6174 6522 206d 696e 4f63 6375 7273 3d22  ate" minOccurs="
+00000db0: 3022 206d 6178 4f63 6375 7273 3d22 3122  0" maxOccurs="1"
+00000dc0: 2f3e 0d0a 2020 2020 2020 3c78 733a 656c  />..      <xs:el
+00000dd0: 656d 656e 7420 6e61 6d65 3d22 4765 6e64  ement name="Gend
+00000de0: 6572 4375 7272 656e 7422 2074 7970 653d  erCurrent" type=
+00000df0: 2267 656e 6465 7274 7970 6522 206d 696e  "gendertype" min
+00000e00: 4f63 6375 7273 3d22 3122 206d 6178 4f63  Occurs="1" maxOc
+00000e10: 6375 7273 3d22 3122 2f3e 0d0a 2020 2020  curs="1"/>..    
+00000e20: 2020 3c78 733a 656c 656d 656e 7420 6e61    <xs:element na
+00000e30: 6d65 3d22 5065 7273 6f6e 4465 6174 6844  me="PersonDeathD
+00000e40: 6174 6522 2074 7970 653d 2278 733a 6461  ate" type="xs:da
+00000e50: 7465 2220 6d69 6e4f 6363 7572 733d 2230  te" minOccurs="0
+00000e60: 2220 6d61 784f 6363 7572 733d 2231 222f  " maxOccurs="1"/
+00000e70: 3e0d 0a20 2020 203c 2f78 733a 7365 7175  >..    </xs:sequ
+00000e80: 656e 6365 3e0d 0a20 203c 2f78 733a 636f  ence>..  </xs:co
+00000e90: 6d70 6c65 7854 7970 653e 0d0a 0d0a 2020  mplexType>....  
+00000ea0: 3c78 733a 636f 6d70 6c65 7854 7970 6520  <xs:complexType 
+00000eb0: 6e61 6d65 3d22 6368 696c 6463 6861 7261  name="childchara
+00000ec0: 6374 6572 6973 7469 6373 7479 7065 223e  cteristicstype">
+00000ed0: 0d0a 2020 2020 3c78 733a 7365 7175 656e  ..    <xs:sequen
+00000ee0: 6365 3e0d 0a20 2020 2020 203c 7873 3a65  ce>..      <xs:e
+00000ef0: 6c65 6d65 6e74 206e 616d 653d 2245 7468  lement name="Eth
+00000f00: 6e69 6369 7479 2220 7479 7065 3d22 6574  nicity" type="et
+00000f10: 686e 6963 6974 7974 7970 6522 206d 696e  hnicitytype" min
+00000f20: 4f63 6375 7273 3d22 3122 206d 6178 4f63  Occurs="1" maxOc
+00000f30: 6375 7273 3d22 3122 2f3e 0d0a 2020 2020  curs="1"/>..    
+00000f40: 2020 3c78 733a 656c 656d 656e 7420 6e61    <xs:element na
+00000f50: 6d65 3d22 4469 7361 6269 6c69 7469 6573  me="Disabilities
+00000f60: 2220 6d69 6e4f 6363 7572 733d 2230 2220  " minOccurs="0" 
+00000f70: 6d61 784f 6363 7572 733d 2231 223e 0d0a  maxOccurs="1">..
+00000f80: 2020 2020 2020 2020 3c78 733a 636f 6d70          <xs:comp
+00000f90: 6c65 7854 7970 653e 0d0a 2020 2020 2020  lexType>..      
+00000fa0: 2020 2020 3c78 733a 7365 7175 656e 6365      <xs:sequence
+00000fb0: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00000fc0: 7873 3a65 6c65 6d65 6e74 206e 616d 653d  xs:element name=
+00000fd0: 2244 6973 6162 696c 6974 7922 2074 7970  "Disability" typ
+00000fe0: 653d 2264 6973 6162 696c 6974 7974 7970  e="disabilitytyp
+00000ff0: 6522 2020 6d69 6e4f 6363 7572 733d 2231  e"  minOccurs="1
+00001000: 2220 6d61 784f 6363 7572 733d 2275 6e62  " maxOccurs="unb
+00001010: 6f75 6e64 6564 222f 3e0d 0a20 2020 2020  ounded"/>..     
+00001020: 2020 2020 203c 2f78 733a 7365 7175 656e       </xs:sequen
+00001030: 6365 3e0d 0a20 2020 2020 2020 203c 2f78  ce>..        </x
+00001040: 733a 636f 6d70 6c65 7854 7970 653e 0d0a  s:complexType>..
+00001050: 2020 2020 2020 3c2f 7873 3a65 6c65 6d65        </xs:eleme
+00001060: 6e74 3e0d 0a20 2020 203c 2f78 733a 7365  nt>..    </xs:se
+00001070: 7175 656e 6365 3e0d 0a20 203c 2f78 733a  quence>..  </xs:
+00001080: 636f 6d70 6c65 7854 7970 653e 0d0a 0d0a  complexType>....
+00001090: 2020 3c78 733a 636f 6d70 6c65 7854 7970    <xs:complexTyp
+000010a0: 6520 6e61 6d65 3d22 6369 6e64 6574 6169  e name="cindetai
+000010b0: 6c73 7479 7065 223e 0d0a 2020 2020 3c78  lstype">..    <x
+000010c0: 733a 7365 7175 656e 6365 3e0d 0a20 2020  s:sequence>..   
+000010d0: 2020 203c 7873 3a65 6c65 6d65 6e74 206e     <xs:element n
+000010e0: 616d 653d 2243 494e 7265 6665 7272 616c  ame="CINreferral
+000010f0: 4461 7465 2220 7479 7065 3d22 7873 3a64  Date" type="xs:d
+00001100: 6174 6522 206d 696e 4f63 6375 7273 3d22  ate" minOccurs="
+00001110: 3122 206d 6178 4f63 6375 7273 3d22 3122  1" maxOccurs="1"
+00001120: 2f3e 0d0a 2020 2020 2020 3c78 733a 656c  />..      <xs:el
+00001130: 656d 656e 7420 6e61 6d65 3d22 5265 6665  ement name="Refe
+00001140: 7272 616c 536f 7572 6365 2220 7479 7065  rralSource" type
+00001150: 3d22 7265 6665 7272 616c 736f 7572 6365  ="referralsource
+00001160: 7479 7065 2220 6d69 6e4f 6363 7572 733d  type" minOccurs=
+00001170: 2231 2220 6d61 784f 6363 7572 733d 2231  "1" maxOccurs="1
+00001180: 222f 3e0d 0a20 2020 2020 203c 7873 3a65  "/>..      <xs:e
+00001190: 6c65 6d65 6e74 206e 616d 653d 2250 7269  lement name="Pri
+000011a0: 6d61 7279 4e65 6564 436f 6465 2220 7479  maryNeedCode" ty
+000011b0: 7065 3d22 7072 696d 6172 796e 6565 6463  pe="primaryneedc
+000011c0: 6f64 6574 7970 6522 206d 696e 4f63 6375  odetype" minOccu
+000011d0: 7273 3d22 3022 206d 6178 4f63 6375 7273  rs="0" maxOccurs
+000011e0: 3d22 3122 2f3e 0d0a 2020 2020 2020 3c78  ="1"/>..      <x
+000011f0: 733a 656c 656d 656e 7420 6e61 6d65 3d22  s:element name="
+00001200: 4349 4e63 6c6f 7375 7265 4461 7465 2220  CINclosureDate" 
+00001210: 7479 7065 3d22 7873 3a64 6174 6522 206d  type="xs:date" m
+00001220: 696e 4f63 6375 7273 3d22 3022 206d 6178  inOccurs="0" max
+00001230: 4f63 6375 7273 3d22 3122 2f3e 0d0a 2020  Occurs="1"/>..  
+00001240: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
+00001250: 6e61 6d65 3d22 5265 6173 6f6e 466f 7243  name="ReasonForC
+00001260: 6c6f 7375 7265 2220 7479 7065 3d22 7265  losure" type="re
+00001270: 6173 6f6e 666f 7263 6c6f 7375 7265 7479  asonforclosurety
+00001280: 7065 2220 6d69 6e4f 6363 7572 733d 2230  pe" minOccurs="0
+00001290: 2220 6d61 784f 6363 7572 733d 2231 222f  " maxOccurs="1"/
+000012a0: 3e0d 0a20 2020 2020 203c 7873 3a65 6c65  >..      <xs:ele
+000012b0: 6d65 6e74 206e 616d 653d 2244 6174 654f  ment name="DateO
+000012c0: 6649 6e69 7469 616c 4350 4322 2074 7970  fInitialCPC" typ
+000012d0: 653d 2278 733a 6461 7465 2220 6d69 6e4f  e="xs:date" minO
+000012e0: 6363 7572 733d 2230 2220 6d61 784f 6363  ccurs="0" maxOcc
+000012f0: 7572 733d 2231 222f 3e0d 0a20 2020 2020  urs="1"/>..     
+00001300: 203c 7873 3a65 6c65 6d65 6e74 206e 616d   <xs:element nam
+00001310: 653d 2241 7373 6573 736d 656e 7473 2220  e="Assessments" 
+00001320: 7479 7065 3d22 6173 7365 7373 6d65 6e74  type="assessment
+00001330: 7374 7970 6522 206d 696e 4f63 6375 7273  stype" minOccurs
+00001340: 3d22 3022 206d 6178 4f63 6375 7273 3d22  ="0" maxOccurs="
+00001350: 756e 626f 756e 6465 6422 2f3e 0d0a 2020  unbounded"/>..  
+00001360: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
+00001370: 6e61 6d65 3d22 4349 4e50 6c61 6e44 6174  name="CINPlanDat
+00001380: 6573 2220 7479 7065 3d22 6369 6e70 6c61  es" type="cinpla
+00001390: 6e64 6174 6573 7474 7970 6522 206d 696e  ndatesttype" min
+000013a0: 4f63 6375 7273 3d22 3022 206d 6178 4f63  Occurs="0" maxOc
+000013b0: 6375 7273 3d22 756e 626f 756e 6465 6422  curs="unbounded"
+000013c0: 2f3e 0d0a 2020 2020 2020 3c78 733a 656c  />..      <xs:el
+000013d0: 656d 656e 7420 6e61 6d65 3d22 5365 6374  ement name="Sect
+000013e0: 696f 6e34 3722 2074 7970 653d 2273 6563  ion47" type="sec
+000013f0: 7469 6f6e 3437 7479 7065 2220 6d69 6e4f  tion47type" minO
+00001400: 6363 7572 733d 2230 2220 6d61 784f 6363  ccurs="0" maxOcc
+00001410: 7572 733d 2275 6e62 6f75 6e64 6564 222f  urs="unbounded"/
+00001420: 3e0d 0a20 2020 2020 203c 7873 3a65 6c65  >..      <xs:ele
+00001430: 6d65 6e74 206e 616d 653d 2252 6566 6572  ment name="Refer
+00001440: 7261 6c4e 4641 2220 7479 7065 3d22 7965  ralNFA" type="ye
+00001450: 736e 6f74 7970 6522 206d 696e 4f63 6375  snotype" minOccu
+00001460: 7273 3d22 3122 206d 6178 4f63 6375 7273  rs="1" maxOccurs
+00001470: 3d22 3122 2f3e 0d0a 2020 2020 2020 3c78  ="1"/>..      <x
+00001480: 733a 656c 656d 656e 7420 6e61 6d65 3d22  s:element name="
+00001490: 4368 696c 6450 726f 7465 6374 696f 6e50  ChildProtectionP
+000014a0: 6c61 6e73 2220 7479 7065 3d22 6368 696c  lans" type="chil
+000014b0: 6470 726f 7465 6374 696f 6e70 6c61 6e73  dprotectionplans
+000014c0: 7479 7065 2220 6d69 6e4f 6363 7572 733d  type" minOccurs=
+000014d0: 2230 2220 6d61 784f 6363 7572 733d 2275  "0" maxOccurs="u
+000014e0: 6e62 6f75 6e64 6564 222f 3e0d 0a20 2020  nbounded"/>..   
+000014f0: 203c 2f78 733a 7365 7175 656e 6365 3e0d   </xs:sequence>.
+00001500: 0a20 203c 2f78 733a 636f 6d70 6c65 7854  .  </xs:complexT
+00001510: 7970 653e 0d0a 0d0a 2020 3c78 733a 636f  ype>....  <xs:co
+00001520: 6d70 6c65 7854 7970 6520 6e61 6d65 3d22  mplexType name="
+00001530: 6173 7365 7373 6d65 6e74 7374 7970 6522  assessmentstype"
+00001540: 3e0d 0a20 2020 203c 7873 3a73 6571 7565  >..    <xs:seque
+00001550: 6e63 653e 0d0a 2020 2020 2020 3c78 733a  nce>..      <xs:
+00001560: 656c 656d 656e 7420 6e61 6d65 3d22 4173  element name="As
+00001570: 7365 7373 6d65 6e74 4163 7475 616c 5374  sessmentActualSt
+00001580: 6172 7444 6174 6522 2074 7970 653d 2278  artDate" type="x
+00001590: 733a 6461 7465 2220 6d69 6e4f 6363 7572  s:date" minOccur
+000015a0: 733d 2231 2220 6d61 784f 6363 7572 733d  s="1" maxOccurs=
+000015b0: 2231 222f 3e0d 0a20 2020 2020 203c 7873  "1"/>..      <xs
+000015c0: 3a65 6c65 6d65 6e74 206e 616d 653d 2241  :element name="A
+000015d0: 7373 6573 736d 656e 7449 6e74 6572 6e61  ssessmentInterna
+000015e0: 6c52 6576 6965 7744 6174 6522 2074 7970  lReviewDate" typ
+000015f0: 653d 2278 733a 6461 7465 2220 6d69 6e4f  e="xs:date" minO
+00001600: 6363 7572 733d 2230 2220 6d61 784f 6363  ccurs="0" maxOcc
+00001610: 7572 733d 2231 222f 3e0d 0a20 2020 2020  urs="1"/>..     
+00001620: 203c 7873 3a65 6c65 6d65 6e74 206e 616d   <xs:element nam
+00001630: 653d 2241 7373 6573 736d 656e 7441 7574  e="AssessmentAut
+00001640: 686f 7269 7361 7469 6f6e 4461 7465 2220  horisationDate" 
+00001650: 7479 7065 3d22 7873 3a64 6174 6522 206d  type="xs:date" m
+00001660: 696e 4f63 6375 7273 3d22 3022 206d 6178  inOccurs="0" max
+00001670: 4f63 6375 7273 3d22 3122 2f3e 0d0a 2020  Occurs="1"/>..  
+00001680: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
+00001690: 6e61 6d65 3d22 4661 6374 6f72 7349 6465  name="FactorsIde
+000016a0: 6e74 6966 6965 6441 7441 7373 6573 736d  ntifiedAtAssessm
+000016b0: 656e 7422 206d 696e 4f63 6375 7273 3d22  ent" minOccurs="
+000016c0: 3022 206d 6178 4f63 6375 7273 3d22 3122  0" maxOccurs="1"
+000016d0: 3e0d 0a20 2020 2020 2020 203c 7873 3a63  >..        <xs:c
+000016e0: 6f6d 706c 6578 5479 7065 3e0d 0a20 2020  omplexType>..   
+000016f0: 2020 2020 2020 203c 7873 3a73 6571 7565         <xs:seque
+00001700: 6e63 653e 0d0a 2020 2020 2020 2020 2020  nce>..          
+00001710: 2020 3c78 733a 656c 656d 656e 7420 6e61    <xs:element na
+00001720: 6d65 3d22 4173 7365 7373 6d65 6e74 4661  me="AssessmentFa
+00001730: 6374 6f72 7322 2074 7970 653d 2261 7373  ctors" type="ass
+00001740: 6573 736d 656e 7466 6163 746f 7273 7479  essmentfactorsty
+00001750: 7065 2220 6d69 6e4f 6363 7572 733d 2231  pe" minOccurs="1
+00001760: 2220 6d61 784f 6363 7572 733d 2275 6e62  " maxOccurs="unb
+00001770: 6f75 6e64 6564 222f 3e0d 0a20 2020 2020  ounded"/>..     
+00001780: 2020 2020 203c 2f78 733a 7365 7175 656e       </xs:sequen
+00001790: 6365 3e0d 0a20 2020 2020 2020 203c 2f78  ce>..        </x
+000017a0: 733a 636f 6d70 6c65 7854 7970 653e 0d0a  s:complexType>..
+000017b0: 2020 2020 2020 3c2f 7873 3a65 6c65 6d65        </xs:eleme
+000017c0: 6e74 3e0d 0a20 2020 203c 2f78 733a 7365  nt>..    </xs:se
+000017d0: 7175 656e 6365 3e0d 0a20 203c 2f78 733a  quence>..  </xs:
+000017e0: 636f 6d70 6c65 7854 7970 653e 0d0a 0d0a  complexType>....
+000017f0: 2020 3c78 733a 636f 6d70 6c65 7854 7970    <xs:complexTyp
+00001800: 6520 6e61 6d65 3d22 6369 6e70 6c61 6e64  e name="cinpland
+00001810: 6174 6573 7474 7970 6522 3e0d 0a20 2020  atesttype">..   
+00001820: 203c 7873 3a73 6571 7565 6e63 653e 0d0a   <xs:sequence>..
+00001830: 2020 2020 2020 3c78 733a 656c 656d 656e        <xs:elemen
+00001840: 7420 6e61 6d65 3d22 4349 4e50 6c61 6e53  t name="CINPlanS
+00001850: 7461 7274 4461 7465 2220 7479 7065 3d22  tartDate" type="
+00001860: 7873 3a64 6174 6522 206d 696e 4f63 6375  xs:date" minOccu
+00001870: 7273 3d22 3122 206d 6178 4f63 6375 7273  rs="1" maxOccurs
+00001880: 3d22 3122 2f3e 0d0a 2020 2020 2020 3c78  ="1"/>..      <x
+00001890: 733a 656c 656d 656e 7420 6e61 6d65 3d22  s:element name="
+000018a0: 4349 4e50 6c61 6e45 6e64 4461 7465 2220  CINPlanEndDate" 
+000018b0: 7479 7065 3d22 7873 3a64 6174 6522 206d  type="xs:date" m
+000018c0: 696e 4f63 6375 7273 3d22 3022 206d 6178  inOccurs="0" max
+000018d0: 4f63 6375 7273 3d22 3122 2f3e 0d0a 2020  Occurs="1"/>..  
+000018e0: 2020 3c2f 7873 3a73 6571 7565 6e63 653e    </xs:sequence>
+000018f0: 0d0a 2020 3c2f 7873 3a63 6f6d 706c 6578  ..  </xs:complex
+00001900: 5479 7065 3e0d 0a0d 0a20 203c 7873 3a63  Type>....  <xs:c
+00001910: 6f6d 706c 6578 5479 7065 206e 616d 653d  omplexType name=
+00001920: 2273 6563 7469 6f6e 3437 7479 7065 223e  "section47type">
+00001930: 0d0a 2020 2020 3c78 733a 7365 7175 656e  ..    <xs:sequen
+00001940: 6365 3e0d 0a20 2020 2020 203c 7873 3a65  ce>..      <xs:e
+00001950: 6c65 6d65 6e74 206e 616d 653d 2253 3437  lement name="S47
+00001960: 4163 7475 616c 5374 6172 7444 6174 6522  ActualStartDate"
+00001970: 2074 7970 653d 2278 733a 6461 7465 2220   type="xs:date" 
+00001980: 6d69 6e4f 6363 7572 733d 2231 2220 6d61  minOccurs="1" ma
+00001990: 784f 6363 7572 733d 2231 222f 3e0d 0a20  xOccurs="1"/>.. 
+000019a0: 2020 2020 203c 7873 3a65 6c65 6d65 6e74       <xs:element
+000019b0: 206e 616d 653d 2249 6e69 7469 616c 4350   name="InitialCP
+000019c0: 4374 6172 6765 7422 2074 7970 653d 2278  Ctarget" type="x
+000019d0: 733a 6461 7465 2220 6d69 6e4f 6363 7572  s:date" minOccur
+000019e0: 733d 2230 2220 6d61 784f 6363 7572 733d  s="0" maxOccurs=
+000019f0: 2231 222f 3e0d 0a20 2020 2020 203c 7873  "1"/>..      <xs
+00001a00: 3a65 6c65 6d65 6e74 206e 616d 653d 2244  :element name="D
+00001a10: 6174 654f 6649 6e69 7469 616c 4350 4322  ateOfInitialCPC"
+00001a20: 2074 7970 653d 2278 733a 6461 7465 2220   type="xs:date" 
+00001a30: 6d69 6e4f 6363 7572 733d 2230 2220 6d61  minOccurs="0" ma
+00001a40: 784f 6363 7572 733d 2231 222f 3e0d 0a20  xOccurs="1"/>.. 
+00001a50: 2020 2020 203c 7873 3a65 6c65 6d65 6e74       <xs:element
+00001a60: 206e 616d 653d 2249 4350 436e 6f74 5265   name="ICPCnotRe
+00001a70: 7175 6972 6564 2220 7479 7065 3d22 7965  quired" type="ye
+00001a80: 736e 6f74 7970 6522 206d 696e 4f63 6375  snotype" minOccu
+00001a90: 7273 3d22 3122 206d 6178 4f63 6375 7273  rs="1" maxOccurs
+00001aa0: 3d22 3122 2f3e 0d0a 2020 2020 3c2f 7873  ="1"/>..    </xs
+00001ab0: 3a73 6571 7565 6e63 653e 0d0a 2020 3c2f  :sequence>..  </
+00001ac0: 7873 3a63 6f6d 706c 6578 5479 7065 3e0d  xs:complexType>.
+00001ad0: 0a0d 0a20 203c 7873 3a63 6f6d 706c 6578  ...  <xs:complex
+00001ae0: 5479 7065 206e 616d 653d 2263 6869 6c64  Type name="child
+00001af0: 7072 6f74 6563 7469 6f6e 706c 616e 7374  protectionplanst
+00001b00: 7970 6522 3e0d 0a20 2020 203c 7873 3a73  ype">..    <xs:s
+00001b10: 6571 7565 6e63 653e 0d0a 2020 2020 2020  equence>..      
+00001b20: 3c78 733a 656c 656d 656e 7420 6e61 6d65  <xs:element name
+00001b30: 3d22 4350 5073 7461 7274 4461 7465 2220  ="CPPstartDate" 
+00001b40: 7479 7065 3d22 7873 3a64 6174 6522 206d  type="xs:date" m
+00001b50: 696e 4f63 6375 7273 3d22 3122 206d 6178  inOccurs="1" max
+00001b60: 4f63 6375 7273 3d22 3122 2f3e 0d0a 2020  Occurs="1"/>..  
+00001b70: 2020 2020 3c78 733a 656c 656d 656e 7420      <xs:element 
+00001b80: 6e61 6d65 3d22 4350 5065 6e64 4461 7465  name="CPPendDate
+00001b90: 2220 7479 7065 3d22 7873 3a64 6174 6522  " type="xs:date"
+00001ba0: 206d 696e 4f63 6375 7273 3d22 3022 206d   minOccurs="0" m
+00001bb0: 6178 4f63 6375 7273 3d22 3122 2f3e 0d0a  axOccurs="1"/>..
+00001bc0: 2020 2020 2020 3c78 733a 656c 656d 656e        <xs:elemen
+00001bd0: 7420 6e61 6d65 3d22 496e 6974 6961 6c43  t name="InitialC
+00001be0: 6174 6567 6f72 794f 6641 6275 7365 2220  ategoryOfAbuse" 
+00001bf0: 7479 7065 3d22 6361 7465 676f 7279 6f66  type="categoryof
+00001c00: 6162 7573 6522 206d 696e 4f63 6375 7273  abuse" minOccurs
+00001c10: 3d22 3122 206d 6178 4f63 6375 7273 3d22  ="1" maxOccurs="
+00001c20: 3122 2f3e 0d0a 2020 2020 2020 3c78 733a  1"/>..      <xs:
+00001c30: 656c 656d 656e 7420 6e61 6d65 3d22 4c61  element name="La
+00001c40: 7465 7374 4361 7465 676f 7279 4f66 4162  testCategoryOfAb
+00001c50: 7573 6522 2074 7970 653d 2263 6174 6567  use" type="categ
+00001c60: 6f72 796f 6661 6275 7365 2220 6d69 6e4f  oryofabuse" minO
+00001c70: 6363 7572 733d 2231 2220 6d61 784f 6363  ccurs="1" maxOcc
+00001c80: 7572 733d 2231 222f 3e0d 0a20 2020 2020  urs="1"/>..     
+00001c90: 203c 7873 3a65 6c65 6d65 6e74 206e 616d   <xs:element nam
+00001ca0: 653d 224e 756d 6265 724f 6650 7265 7669  e="NumberOfPrevi
+00001cb0: 6f75 7343 5050 2220 7479 7065 3d22 7873  ousCPP" type="xs
+00001cc0: 3a70 6f73 6974 6976 6549 6e74 6567 6572  :positiveInteger
+00001cd0: 2220 6d69 6e4f 6363 7572 733d 2231 2220  " minOccurs="1" 
+00001ce0: 6d61 784f 6363 7572 733d 2231 222f 3e0d  maxOccurs="1"/>.
+00001cf0: 0a20 2020 2020 203c 7873 3a65 6c65 6d65  .      <xs:eleme
+00001d00: 6e74 206e 616d 653d 2252 6576 6965 7773  nt name="Reviews
+00001d10: 2220 6d69 6e4f 6363 7572 733d 2230 2220  " minOccurs="0" 
+00001d20: 6d61 784f 6363 7572 733d 2231 223e 0d0a  maxOccurs="1">..
+00001d30: 2020 2020 2020 2020 3c78 733a 636f 6d70          <xs:comp
+00001d40: 6c65 7854 7970 653e 0d0a 2020 2020 2020  lexType>..      
+00001d50: 2020 2020 3c78 733a 7365 7175 656e 6365      <xs:sequence
+00001d60: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+00001d70: 7873 3a65 6c65 6d65 6e74 206e 616d 653d  xs:element name=
+00001d80: 2243 5050 7265 7669 6577 4461 7465 2220  "CPPreviewDate" 
+00001d90: 7479 7065 3d22 7873 3a64 6174 6522 206d  type="xs:date" m
+00001da0: 696e 4f63 6375 7273 3d22 3122 206d 6178  inOccurs="1" max
+00001db0: 4f63 6375 7273 3d22 756e 626f 756e 6465  Occurs="unbounde
+00001dc0: 6422 2f3e 0d0a 2020 2020 2020 2020 2020  d"/>..          
+00001dd0: 3c2f 7873 3a73 6571 7565 6e63 653e 0d0a  </xs:sequence>..
+00001de0: 2020 2020 2020 2020 3c2f 7873 3a63 6f6d          </xs:com
+00001df0: 706c 6578 5479 7065 3e0d 0a20 2020 2020  plexType>..     
+00001e00: 203c 2f78 733a 656c 656d 656e 743e 0d0a   </xs:element>..
+00001e10: 2020 2020 3c2f 7873 3a73 6571 7565 6e63      </xs:sequenc
+00001e20: 653e 0d0a 2020 3c2f 7873 3a63 6f6d 706c  e>..  </xs:compl
+00001e30: 6578 5479 7065 3e0d 0a0d 0a20 203c 7873  exType>....  <xs
+00001e40: 3a73 696d 706c 6554 7970 6520 6e61 6d65  :simpleType name
+00001e50: 3d22 6e6f 6e45 6d70 7479 5374 7269 6e67  ="nonEmptyString
+00001e60: 223e 0d0a 2020 2020 3c78 733a 7265 7374  ">..    <xs:rest
+00001e70: 7269 6374 696f 6e20 6261 7365 3d22 7873  riction base="xs
+00001e80: 3a73 7472 696e 6722 3e0d 0a20 2020 2020  :string">..     
+00001e90: 203c 7873 3a6d 696e 4c65 6e67 7468 2076   <xs:minLength v
+00001ea0: 616c 7565 3d22 3122 2f3e 0d0a 2020 2020  alue="1"/>..    
+00001eb0: 3c2f 7873 3a72 6573 7472 6963 7469 6f6e  </xs:restriction
+00001ec0: 3e0d 0a20 203c 2f78 733a 7369 6d70 6c65  >..  </xs:simple
+00001ed0: 5479 7065 3e0d 0a0d 0a20 203c 7873 3a73  Type>....  <xs:s
+00001ee0: 696d 706c 6554 7970 6520 6e61 6d65 3d22  impleType name="
+00001ef0: 7965 736e 6f74 7970 6522 3e0d 0a20 2020  yesnotype">..   
+00001f00: 203c 7873 3a72 6573 7472 6963 7469 6f6e   <xs:restriction
+00001f10: 2062 6173 653d 226e 6f6e 456d 7074 7953   base="nonEmptyS
+00001f20: 7472 696e 6722 3e0d 0a20 2020 2020 203c  tring">..      <
+00001f30: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
+00001f40: 616c 7565 3d22 7472 7565 2220 2f3e 0d0a  alue="true" />..
+00001f50: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
+00001f60: 6174 696f 6e20 7661 6c75 653d 2266 616c  ation value="fal
+00001f70: 7365 2220 2f3e 0d0a 0920 203c 7873 3a65  se" />...  <xs:e
+00001f80: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+00001f90: 3d22 5452 5545 2220 2f3e 0d0a 2020 2020  ="TRUE" />..    
+00001fa0: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
+00001fb0: 6e20 7661 6c75 653d 2246 414c 5345 2220  n value="FALSE" 
+00001fc0: 2f3e 0d0a 2020 2020 2020 3c78 733a 656e  />..      <xs:en
+00001fd0: 756d 6572 6174 696f 6e20 7661 6c75 653d  umeration value=
+00001fe0: 2230 2220 2f3e 0d0a 2020 2020 2020 3c78  "0" />..      <x
+00001ff0: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
+00002000: 6c75 653d 2231 2220 2f3e 0d0a 2020 2020  lue="1" />..    
+00002010: 3c2f 7873 3a72 6573 7472 6963 7469 6f6e  </xs:restriction
+00002020: 3e0d 0a20 203c 2f78 733a 7369 6d70 6c65  >..  </xs:simple
+00002030: 5479 7065 3e0d 0a0d 0a20 203c 7873 3a73  Type>....  <xs:s
+00002040: 696d 706c 6554 7970 6520 6e61 6d65 3d22  impleType name="
+00002050: 7570 6e74 7970 6522 3e0d 0a20 2020 203c  upntype">..    <
+00002060: 7873 3a72 6573 7472 6963 7469 6f6e 2062  xs:restriction b
+00002070: 6173 653d 2278 733a 7374 7269 6e67 223e  ase="xs:string">
+00002080: 0d0a 2020 2020 2020 3c78 733a 7061 7474  ..      <xs:patt
+00002090: 6572 6e20 7661 6c75 653d 225b 412d 5a61  ern value="[A-Za
+000020a0: 2d7a 5d5c 647b 3132 7d22 2f3e 0d0a 2020  -z]\d{12}"/>..  
+000020b0: 2020 2020 3c78 733a 7061 7474 6572 6e20      <xs:pattern 
+000020c0: 7661 6c75 653d 225b 412d 5a61 2d7a 5d5c  value="[A-Za-z]\
+000020d0: 647b 3131 7d5b 412d 5a61 2d7a 5d22 2f3e  d{11}[A-Za-z]"/>
+000020e0: 0d0a 2020 2020 3c2f 7873 3a72 6573 7472  ..    </xs:restr
+000020f0: 6963 7469 6f6e 3e0d 0a20 203c 2f78 733a  iction>..  </xs:
+00002100: 7369 6d70 6c65 5479 7065 3e0d 0a0d 0a20  simpleType>.... 
+00002110: 203c 7873 3a73 696d 706c 6554 7970 6520   <xs:simpleType 
+00002120: 6e61 6d65 3d22 756e 6b6e 6f77 6e75 706e  name="unknownupn
+00002130: 7479 7065 223e 0d0a 2020 2020 3c78 733a  type">..    <xs:
+00002140: 7265 7374 7269 6374 696f 6e20 6261 7365  restriction base
+00002150: 3d22 7873 3a73 7472 696e 6722 3e0d 0a20  ="xs:string">.. 
+00002160: 2020 2020 203c 7873 3a65 6e75 6d65 7261       <xs:enumera
+00002170: 7469 6f6e 2076 616c 7565 3d22 554e 3122  tion value="UN1"
+00002180: 202f 3e0d 0a20 2020 2020 203c 7873 3a65   />..      <xs:e
+00002190: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+000021a0: 3d22 554e 3222 202f 3e0d 0a20 2020 2020  ="UN2" />..     
+000021b0: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
+000021c0: 2076 616c 7565 3d22 554e 3322 202f 3e0d   value="UN3" />.
+000021d0: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
+000021e0: 7261 7469 6f6e 2076 616c 7565 3d22 554e  ration value="UN
+000021f0: 3422 202f 3e0d 0a20 2020 2020 203c 7873  4" />..      <xs
+00002200: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
+00002210: 7565 3d22 554e 3522 202f 3e0d 0a20 2020  ue="UN5" />..   
+00002220: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
+00002230: 6f6e 2076 616c 7565 3d22 554e 3622 202f  on value="UN6" /
+00002240: 3e0d 0a20 2020 2020 203c 7873 3a65 6e75  >..      <xs:enu
+00002250: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
+00002260: 554e 3722 202f 3e0d 0a20 2020 203c 2f78  UN7" />..    </x
+00002270: 733a 7265 7374 7269 6374 696f 6e3e 0d0a  s:restriction>..
+00002280: 2020 3c2f 7873 3a73 696d 706c 6554 7970    </xs:simpleTyp
+00002290: 653e 0d0a 0d0a 2020 3c78 733a 7369 6d70  e>....  <xs:simp
+000022a0: 6c65 5479 7065 206e 616d 653d 2267 656e  leType name="gen
+000022b0: 6465 7274 7970 6522 3e0d 0a20 2020 203c  dertype">..    <
+000022c0: 7873 3a72 6573 7472 6963 7469 6f6e 2062  xs:restriction b
+000022d0: 6173 653d 226e 6f6e 456d 7074 7953 7472  ase="nonEmptyStr
+000022e0: 696e 6722 3e0d 0a20 2020 2020 203c 7873  ing">..      <xs
+000022f0: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
+00002300: 7565 3d22 3122 3e0d 0a20 2020 2020 2020  ue="1">..       
+00002310: 203c 7873 3a61 6e6e 6f74 6174 696f 6e3e   <xs:annotation>
+00002320: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
+00002330: 6e3e 4d61 6c65 3c2f 7873 3a64 6f63 756d  n>Male</xs:docum
+00002340: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
+00002350: 6e6f 7461 7469 6f6e 3e0d 0a20 2020 2020  notation>..     
+00002360: 203c 2f78 733a 656e 756d 6572 6174 696f   </xs:enumeratio
+00002370: 6e3e 0d0a 2020 2020 2020 3c78 733a 656e  n>..      <xs:en
+00002380: 756d 6572 6174 696f 6e20 7661 6c75 653d  umeration value=
+00002390: 2232 223e 0d0a 2020 2020 2020 2020 3c78  "2">..        <x
+000023a0: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
+000023b0: 3a64 6f63 756d 656e 7461 7469 6f6e 3e46  :documentation>F
+000023c0: 656d 616c 653c 2f78 733a 646f 6375 6d65  emale</xs:docume
+000023d0: 6e74 6174 696f 6e3e 3c2f 7873 3a61 6e6e  ntation></xs:ann
+000023e0: 6f74 6174 696f 6e3e 0d0a 2020 2020 2020  otation>..      
+000023f0: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
+00002400: 3e0d 0a20 2020 2020 203c 7873 3a65 6e75  >..      <xs:enu
+00002410: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
+00002420: 3022 3e0d 0a20 2020 2020 2020 203c 7873  0">..        <xs
+00002430: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
+00002440: 646f 6375 6d65 6e74 6174 696f 6e3e 4e6f  documentation>No
+00002450: 7420 7265 636f 7264 6564 206f 7220 756e  t recorded or un
+00002460: 626f 726e 3c2f 7873 3a64 6f63 756d 656e  born</xs:documen
+00002470: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
+00002480: 7461 7469 6f6e 3e0d 0a20 2020 2020 203c  tation>..      <
+00002490: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
+000024a0: 0d0a 2020 2020 2020 3c78 733a 656e 756d  ..      <xs:enum
+000024b0: 6572 6174 696f 6e20 7661 6c75 653d 2239  eration value="9
+000024c0: 223e 0d0a 2020 2020 2020 2020 3c78 733a  ">..        <xs:
+000024d0: 616e 6e6f 7461 7469 6f6e 3e3c 7873 3a64  annotation><xs:d
+000024e0: 6f63 756d 656e 7461 7469 6f6e 3e49 6e64  ocumentation>Ind
+000024f0: 6574 6572 6d69 6e61 7465 3c2f 7873 3a64  eterminate</xs:d
+00002500: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
+00002510: 733a 616e 6e6f 7461 7469 6f6e 3e0d 0a20  s:annotation>.. 
+00002520: 2020 2020 203c 2f78 733a 656e 756d 6572       </xs:enumer
+00002530: 6174 696f 6e3e 0d0a 2020 2020 3c2f 7873  ation>..    </xs
+00002540: 3a72 6573 7472 6963 7469 6f6e 3e0d 0a20  :restriction>.. 
+00002550: 203c 2f78 733a 7369 6d70 6c65 5479 7065   </xs:simpleType
+00002560: 3e0d 0a0d 0a0d 0a20 203c 7873 3a73 696d  >......  <xs:sim
+00002570: 706c 6554 7970 6520 6e61 6d65 3d22 6574  pleType name="et
+00002580: 686e 6963 6974 7974 7970 6522 3e0d 0a20  hnicitytype">.. 
+00002590: 2020 203c 7873 3a72 6573 7472 6963 7469     <xs:restricti
+000025a0: 6f6e 2062 6173 653d 226e 6f6e 456d 7074  on base="nonEmpt
+000025b0: 7953 7472 696e 6722 3e0d 0a20 2020 2020  yString">..     
+000025c0: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
+000025d0: 2076 616c 7565 3d22 5742 5249 223e 3c78   value="WBRI"><x
+000025e0: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
+000025f0: 3a64 6f63 756d 656e 7461 7469 6f6e 3e57  :documentation>W
+00002600: 6869 7465 2042 7269 7469 7368 3c2f 7873  hite British</xs
+00002610: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
+00002620: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
+00002630: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
+00002640: 0d0a 2020 2020 2020 3c78 733a 656e 756d  ..      <xs:enum
+00002650: 6572 6174 696f 6e20 7661 6c75 653d 2257  eration value="W
+00002660: 4952 4922 3e3c 7873 3a61 6e6e 6f74 6174  IRI"><xs:annotat
+00002670: 696f 6e3e 3c78 733a 646f 6375 6d65 6e74  ion><xs:document
+00002680: 6174 696f 6e3e 5768 6974 6520 4972 6973  ation>White Iris
+00002690: 683c 2f78 733a 646f 6375 6d65 6e74 6174  h</xs:documentat
+000026a0: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
+000026b0: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
+000026c0: 7469 6f6e 3e0d 0a20 2020 2020 203c 7873  tion>..      <xs
+000026d0: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
+000026e0: 7565 3d22 5749 5254 223e 3c78 733a 616e  ue="WIRT"><xs:an
+000026f0: 6e6f 7461 7469 6f6e 3e3c 7873 3a64 6f63  notation><xs:doc
+00002700: 756d 656e 7461 7469 6f6e 3e54 7261 7665  umentation>Trave
+00002710: 6c6c 6572 206f 6620 4972 6973 6820 6865  ller of Irish he
+00002720: 7269 7461 6765 3c2f 7873 3a64 6f63 756d  ritage</xs:docum
+00002730: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
+00002740: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
+00002750: 756d 6572 6174 696f 6e3e 0d0a 2020 2020  umeration>..    
+00002760: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
+00002770: 6e20 7661 6c75 653d 2257 4f54 4822 3e3c  n value="WOTH"><
+00002780: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
+00002790: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+000027a0: 416e 7920 6f74 6865 7220 5768 6974 6520  Any other White 
+000027b0: 6261 636b 6772 6f75 6e64 3c2f 7873 3a64  background</xs:d
+000027c0: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
+000027d0: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
+000027e0: 733a 656e 756d 6572 6174 696f 6e3e 0d0a  s:enumeration>..
+000027f0: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
+00002800: 6174 696f 6e20 7661 6c75 653d 2257 524f  ation value="WRO
+00002810: 4d22 3e3c 7873 3a61 6e6e 6f74 6174 696f  M"><xs:annotatio
+00002820: 6e3e 3c78 733a 646f 6375 6d65 6e74 6174  n><xs:documentat
+00002830: 696f 6e3e 4779 7073 792f 526f 6d61 3c2f  ion>Gypsy/Roma</
+00002840: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
+00002850: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
+00002860: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
+00002870: 6e3e 0d0a 2020 2020 2020 3c78 733a 656e  n>..      <xs:en
+00002880: 756d 6572 6174 696f 6e20 7661 6c75 653d  umeration value=
+00002890: 224d 5742 4322 3e3c 7873 3a61 6e6e 6f74  "MWBC"><xs:annot
+000028a0: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
+000028b0: 6e74 6174 696f 6e3e 5768 6974 6520 616e  ntation>White an
+000028c0: 6420 426c 6163 6b20 4361 7269 6262 6561  d Black Caribbea
+000028d0: 6e3c 2f78 733a 646f 6375 6d65 6e74 6174  n</xs:documentat
+000028e0: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
+000028f0: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
+00002900: 7469 6f6e 3e0d 0a20 2020 2020 203c 7873  tion>..      <xs
+00002910: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
+00002920: 7565 3d22 4d57 4241 223e 3c78 733a 616e  ue="MWBA"><xs:an
+00002930: 6e6f 7461 7469 6f6e 3e3c 7873 3a64 6f63  notation><xs:doc
+00002940: 756d 656e 7461 7469 6f6e 3e57 6869 7465  umentation>White
+00002950: 2061 6e64 2042 6c61 636b 2041 6672 6963   and Black Afric
+00002960: 616e 3c2f 7873 3a64 6f63 756d 656e 7461  an</xs:documenta
+00002970: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
+00002980: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
+00002990: 6174 696f 6e3e 0d0a 2020 2020 2020 3c78  ation>..      <x
+000029a0: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
+000029b0: 6c75 653d 224d 5741 5322 3e3c 7873 3a61  lue="MWAS"><xs:a
+000029c0: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
+000029d0: 6375 6d65 6e74 6174 696f 6e3e 5768 6974  cumentation>Whit
+000029e0: 6520 616e 6420 4173 6961 6e3c 2f78 733a  e and Asian</xs:
+000029f0: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
+00002a00: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
+00002a10: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0d  xs:enumeration>.
+00002a20: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
+00002a30: 7261 7469 6f6e 2076 616c 7565 3d22 4d4f  ration value="MO
+00002a40: 5448 223e 3c78 733a 616e 6e6f 7461 7469  TH"><xs:annotati
+00002a50: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
+00002a60: 7469 6f6e 3e41 6e79 206f 7468 6572 206d  tion>Any other m
+00002a70: 6978 6564 2062 6163 6b67 726f 756e 643c  ixed background<
+00002a80: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
+00002a90: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
+00002aa0: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
+00002ab0: 6f6e 3e0d 0a20 2020 2020 203c 7873 3a65  on>..      <xs:e
+00002ac0: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+00002ad0: 3d22 4149 4e44 223e 3c78 733a 616e 6e6f  ="AIND"><xs:anno
+00002ae0: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
+00002af0: 656e 7461 7469 6f6e 3e49 6e64 6961 6e3c  entation>Indian<
+00002b00: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
+00002b10: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
+00002b20: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
+00002b30: 6f6e 3e0d 0a20 2020 2020 203c 7873 3a65  on>..      <xs:e
+00002b40: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+00002b50: 3d22 4150 4b4e 223e 3c78 733a 616e 6e6f  ="APKN"><xs:anno
+00002b60: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
+00002b70: 656e 7461 7469 6f6e 3e50 616b 6973 7461  entation>Pakista
+00002b80: 6e69 3c2f 7873 3a64 6f63 756d 656e 7461  ni</xs:documenta
+00002b90: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
+00002ba0: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
+00002bb0: 6174 696f 6e3e 0d0a 2020 2020 2020 3c78  ation>..      <x
+00002bc0: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
+00002bd0: 6c75 653d 2241 4241 4e22 3e3c 7873 3a61  lue="ABAN"><xs:a
+00002be0: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
+00002bf0: 6375 6d65 6e74 6174 696f 6e3e 4261 6e67  cumentation>Bang
+00002c00: 6c61 6465 7368 693c 2f78 733a 646f 6375  ladeshi</xs:docu
+00002c10: 6d65 6e74 6174 696f 6e3e 3c2f 7873 3a61  mentation></xs:a
+00002c20: 6e6e 6f74 6174 696f 6e3e 3c2f 7873 3a65  nnotation></xs:e
+00002c30: 6e75 6d65 7261 7469 6f6e 3e0d 0a20 2020  numeration>..   
+00002c40: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
+00002c50: 6f6e 2076 616c 7565 3d22 414f 5448 223e  on value="AOTH">
+00002c60: 3c78 733a 616e 6e6f 7461 7469 6f6e 3e3c  <xs:annotation><
+00002c70: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
+00002c80: 3e41 6e79 206f 7468 6572 2041 7369 616e  >Any other Asian
+00002c90: 2062 6163 6b67 726f 756e 643c 2f78 733a   background</xs:
+00002ca0: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
+00002cb0: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
+00002cc0: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0d  xs:enumeration>.
+00002cd0: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
+00002ce0: 7261 7469 6f6e 2076 616c 7565 3d22 4243  ration value="BC
+00002cf0: 5242 223e 3c78 733a 616e 6e6f 7461 7469  RB"><xs:annotati
+00002d00: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
+00002d10: 7469 6f6e 3e43 6172 6962 6265 616e 3c2f  tion>Caribbean</
+00002d20: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
+00002d30: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
+00002d40: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
+00002d50: 6e3e 0d0a 2020 2020 2020 3c78 733a 656e  n>..      <xs:en
+00002d60: 756d 6572 6174 696f 6e20 7661 6c75 653d  umeration value=
+00002d70: 2242 4146 5222 3e3c 7873 3a61 6e6e 6f74  "BAFR"><xs:annot
+00002d80: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
+00002d90: 6e74 6174 696f 6e3e 4166 7269 6361 6e3c  ntation>African<
+00002da0: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
+00002db0: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
+00002dc0: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
+00002dd0: 6f6e 3e0d 0a20 2020 2020 203c 7873 3a65  on>..      <xs:e
+00002de0: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+00002df0: 3d22 424f 5448 223e 3c78 733a 616e 6e6f  ="BOTH"><xs:anno
+00002e00: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
+00002e10: 656e 7461 7469 6f6e 3e41 6e79 206f 7468  entation>Any oth
+00002e20: 6572 2062 6c61 636b 2062 6163 6b67 726f  er black backgro
+00002e30: 756e 643c 2f78 733a 646f 6375 6d65 6e74  und</xs:document
+00002e40: 6174 696f 6e3e 3c2f 7873 3a61 6e6e 6f74  ation></xs:annot
+00002e50: 6174 696f 6e3e 3c2f 7873 3a65 6e75 6d65  ation></xs:enume
+00002e60: 7261 7469 6f6e 3e0d 0a20 2020 2020 203c  ration>..      <
+00002e70: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
+00002e80: 616c 7565 3d22 4348 4e45 223e 3c78 733a  alue="CHNE"><xs:
+00002e90: 616e 6e6f 7461 7469 6f6e 3e3c 7873 3a64  annotation><xs:d
+00002ea0: 6f63 756d 656e 7461 7469 6f6e 3e43 6869  ocumentation>Chi
+00002eb0: 6e65 7365 3c2f 7873 3a64 6f63 756d 656e  nese</xs:documen
+00002ec0: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
+00002ed0: 7461 7469 6f6e 3e3c 2f78 733a 656e 756d  tation></xs:enum
+00002ee0: 6572 6174 696f 6e3e 0d0a 2020 2020 2020  eration>..      
+00002ef0: 3c78 733a 656e 756d 6572 6174 696f 6e20  <xs:enumeration 
+00002f00: 7661 6c75 653d 224f 4f54 4822 3e3c 7873  value="OOTH"><xs
+00002f10: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
+00002f20: 646f 6375 6d65 6e74 6174 696f 6e3e 416e  documentation>An
+00002f30: 7920 6f74 6865 7220 6574 686e 6963 2067  y other ethnic g
+00002f40: 726f 7570 3c2f 7873 3a64 6f63 756d 656e  roup</xs:documen
+00002f50: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
+00002f60: 7461 7469 6f6e 3e3c 2f78 733a 656e 756d  tation></xs:enum
+00002f70: 6572 6174 696f 6e3e 0d0a 2020 2020 2020  eration>..      
+00002f80: 3c78 733a 656e 756d 6572 6174 696f 6e20  <xs:enumeration 
+00002f90: 7661 6c75 653d 2252 4546 5522 3e3c 7873  value="REFU"><xs
+00002fa0: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
+00002fb0: 646f 6375 6d65 6e74 6174 696f 6e3e 5265  documentation>Re
+00002fc0: 6675 7365 643c 2f78 733a 646f 6375 6d65  fused</xs:docume
+00002fd0: 6e74 6174 696f 6e3e 3c2f 7873 3a61 6e6e  ntation></xs:ann
+00002fe0: 6f74 6174 696f 6e3e 3c2f 7873 3a65 6e75  otation></xs:enu
+00002ff0: 6d65 7261 7469 6f6e 3e0d 0a20 2020 2020  meration>..     
+00003000: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
+00003010: 2076 616c 7565 3d22 4e4f 4254 223e 3c78   value="NOBT"><x
+00003020: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
+00003030: 3a64 6f63 756d 656e 7461 7469 6f6e 3e49  :documentation>I
+00003040: 6e66 6f72 6d61 7469 6f6e 206e 6f74 2079  nformation not y
+00003050: 6574 206f 6274 6169 6e65 643c 2f78 733a  et obtained</xs:
+00003060: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
+00003070: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
+00003080: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0d  xs:enumeration>.
+00003090: 0a20 2020 203c 2f78 733a 7265 7374 7269  .    </xs:restri
+000030a0: 6374 696f 6e3e 0d0a 2020 3c2f 7873 3a73  ction>..  </xs:s
+000030b0: 696d 706c 6554 7970 653e 0d0a 0d0a 2020  impleType>....  
+000030c0: 3c78 733a 7369 6d70 6c65 5479 7065 206e  <xs:simpleType n
+000030d0: 616d 653d 2264 6973 6162 696c 6974 7974  ame="disabilityt
+000030e0: 7970 6522 3e0d 0a20 2020 203c 7873 3a72  ype">..    <xs:r
+000030f0: 6573 7472 6963 7469 6f6e 2062 6173 653d  estriction base=
+00003100: 226e 6f6e 456d 7074 7953 7472 696e 6722  "nonEmptyString"
+00003110: 3e0d 0a20 2020 2020 203c 7873 3a65 6e75  >..      <xs:enu
+00003120: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
+00003130: 4e4f 4e45 223e 3c78 733a 616e 6e6f 7461  NONE"><xs:annota
+00003140: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
+00003150: 7461 7469 6f6e 3e4e 6f20 6469 7361 6269  tation>No disabi
+00003160: 6c69 7479 3c2f 7873 3a64 6f63 756d 656e  lity</xs:documen
+00003170: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
+00003180: 7461 7469 6f6e 3e3c 2f78 733a 656e 756d  tation></xs:enum
+00003190: 6572 6174 696f 6e3e 0d0a 2020 2020 2020  eration>..      
+000031a0: 3c78 733a 656e 756d 6572 6174 696f 6e20  <xs:enumeration 
+000031b0: 7661 6c75 653d 224d 4f42 223e 3c78 733a  value="MOB"><xs:
+000031c0: 616e 6e6f 7461 7469 6f6e 3e3c 7873 3a64  annotation><xs:d
+000031d0: 6f63 756d 656e 7461 7469 6f6e 3e4d 6f62  ocumentation>Mob
+000031e0: 696c 6974 793c 2f78 733a 646f 6375 6d65  ility</xs:docume
+000031f0: 6e74 6174 696f 6e3e 3c2f 7873 3a61 6e6e  ntation></xs:ann
+00003200: 6f74 6174 696f 6e3e 3c2f 7873 3a65 6e75  otation></xs:enu
+00003210: 6d65 7261 7469 6f6e 3e0d 0a20 2020 2020  meration>..     
+00003220: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
+00003230: 2076 616c 7565 3d22 4841 4e44 223e 3c78   value="HAND"><x
+00003240: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
+00003250: 3a64 6f63 756d 656e 7461 7469 6f6e 3e48  :documentation>H
+00003260: 616e 6420 6675 6e63 7469 6f6e 3c2f 7873  and function</xs
+00003270: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
+00003280: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
+00003290: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
+000032a0: 0d0a 2020 2020 2020 3c78 733a 656e 756d  ..      <xs:enum
+000032b0: 6572 6174 696f 6e20 7661 6c75 653d 2250  eration value="P
+000032c0: 4322 3e3c 7873 3a61 6e6e 6f74 6174 696f  C"><xs:annotatio
+000032d0: 6e3e 3c78 733a 646f 6375 6d65 6e74 6174  n><xs:documentat
+000032e0: 696f 6e3e 5065 7273 6f6e 616c 2063 6172  ion>Personal car
+000032f0: 653c 2f78 733a 646f 6375 6d65 6e74 6174  e</xs:documentat
+00003300: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
+00003310: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
+00003320: 7469 6f6e 3e0d 0a20 2020 2020 203c 7873  tion>..      <xs
+00003330: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
+00003340: 7565 3d22 494e 4322 3e3c 7873 3a61 6e6e  ue="INC"><xs:ann
+00003350: 6f74 6174 696f 6e3e 3c78 733a 646f 6375  otation><xs:docu
+00003360: 6d65 6e74 6174 696f 6e3e 496e 636f 6e74  mentation>Incont
+00003370: 696e 656e 6365 3c2f 7873 3a64 6f63 756d  inence</xs:docum
+00003380: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
+00003390: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
+000033a0: 756d 6572 6174 696f 6e3e 0d0a 2020 2020  umeration>..    
+000033b0: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
+000033c0: 6e20 7661 6c75 653d 2243 4f4d 4d22 3e3c  n value="COMM"><
+000033d0: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
+000033e0: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+000033f0: 436f 6d6d 756e 6963 6174 696f 6e3c 2f78  Communication</x
+00003400: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00003410: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
+00003420: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
+00003430: 3e0d 0a20 2020 2020 203c 7873 3a65 6e75  >..      <xs:enu
+00003440: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
+00003450: 4c44 223e 3c78 733a 616e 6e6f 7461 7469  LD"><xs:annotati
+00003460: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
+00003470: 7469 6f6e 3e4c 6561 726e 696e 673c 2f78  tion>Learning</x
+00003480: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00003490: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
+000034a0: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
+000034b0: 3e0d 0a20 2020 2020 203c 7873 3a65 6e75  >..      <xs:enu
 000034c0: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-000034d0: 4245 4822 3e3c 7873 3a61 6e6e 6f74 6174  BEH"><xs:annotat
-000034e0: 696f 6e3e 3c78 733a 646f 6375 6d65 6e74  ion><xs:document
-000034f0: 6174 696f 6e3e 4265 6861 7669 6f75 723c  ation>Behaviour<
-00003500: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
-00003510: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
-00003520: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
-00003530: 6f6e 3e0a 2020 2020 2020 3c78 733a 656e  on>.      <xs:en
+000034d0: 4845 4152 223e 3c78 733a 616e 6e6f 7461  HEAR"><xs:annota
+000034e0: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
+000034f0: 7461 7469 6f6e 3e48 6561 7269 6e67 3c2f  tation>Hearing</
+00003500: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
+00003510: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
+00003520: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
+00003530: 6e3e 0d0a 2020 2020 2020 3c78 733a 656e  n>..      <xs:en
 00003540: 756d 6572 6174 696f 6e20 7661 6c75 653d  umeration value=
-00003550: 2243 4f4e 223e 3c78 733a 616e 6e6f 7461  "CON"><xs:annota
+00003550: 2256 4953 223e 3c78 733a 616e 6e6f 7461  "VIS"><xs:annota
 00003560: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
-00003570: 7461 7469 6f6e 3e43 6f6e 7363 696f 7573  tation>Conscious
-00003580: 6e65 7373 3c2f 7873 3a64 6f63 756d 656e  ness</xs:documen
-00003590: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
-000035a0: 7461 7469 6f6e 3e3c 2f78 733a 656e 756d  tation></xs:enum
-000035b0: 6572 6174 696f 6e3e 0a20 2020 2020 203c  eration>.      <
-000035c0: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
-000035d0: 616c 7565 3d22 4155 5422 3e3c 7873 3a61  alue="AUT"><xs:a
-000035e0: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
-000035f0: 6375 6d65 6e74 6174 696f 6e3e 4175 7469  cumentation>Auti
-00003600: 736d 3c2f 7873 3a64 6f63 756d 656e 7461  sm</xs:documenta
-00003610: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
-00003620: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
-00003630: 6174 696f 6e3e 0a20 2020 2020 203c 7873  ation>.      <xs
-00003640: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
-00003650: 7565 3d22 4444 4122 3e3c 7873 3a61 6e6e  ue="DDA"><xs:ann
-00003660: 6f74 6174 696f 6e3e 3c78 733a 646f 6375  otation><xs:docu
-00003670: 6d65 6e74 6174 696f 6e3e 4f74 6865 723c  mentation>Other<
-00003680: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
-00003690: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
-000036a0: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
-000036b0: 6f6e 3e0a 2020 2020 3c2f 7873 3a72 6573  on>.    </xs:res
-000036c0: 7472 6963 7469 6f6e 3e0a 2020 3c2f 7873  triction>.  </xs
-000036d0: 3a73 696d 706c 6554 7970 653e 0a0a 2020  :simpleType>..  
-000036e0: 3c78 733a 7369 6d70 6c65 5479 7065 206e  <xs:simpleType n
-000036f0: 616d 653d 2272 6566 6572 7261 6c73 6f75  ame="referralsou
-00003700: 7263 6574 7970 6522 3e0a 2020 2020 3c78  rcetype">.    <x
-00003710: 733a 7265 7374 7269 6374 696f 6e20 6261  s:restriction ba
-00003720: 7365 3d22 6e6f 6e45 6d70 7479 5374 7269  se="nonEmptyStri
-00003730: 6e67 223e 0a20 2020 2020 203c 7873 3a65  ng">.      <xs:e
-00003740: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
-00003750: 3d22 3141 223e 3c78 733a 616e 6e6f 7461  ="1A"><xs:annota
-00003760: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
-00003770: 7461 7469 6f6e 3e49 4e44 4956 4944 5541  tation>INDIVIDUA
-00003780: 4c20 e280 9320 6661 6d69 6c79 206d 656d  L ... family mem
-00003790: 6265 722c 2072 656c 6174 6976 6520 6f72  ber, relative or
-000037a0: 2063 6172 6572 3c2f 7873 3a64 6f63 756d   carer</xs:docum
-000037b0: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
-000037c0: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
-000037d0: 756d 6572 6174 696f 6e3e 0a20 2020 2020  umeration>.     
-000037e0: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
-000037f0: 2076 616c 7565 3d22 3142 223e 3c78 733a   value="1B"><xs:
-00003800: 616e 6e6f 7461 7469 6f6e 3e3c 7873 3a64  annotation><xs:d
-00003810: 6f63 756d 656e 7461 7469 6f6e 3e49 4e44  ocumentation>IND
-00003820: 4956 4944 5541 4c20 e280 9320 6163 7175  IVIDUAL ... acqu
-00003830: 6169 6e74 616e 6365 2028 696e 636c 7564  aintance (includ
-00003840: 696e 6720 6e65 6967 6862 6f75 7273 2061  ing neighbours a
-00003850: 6e64 2063 6869 6c64 206d 696e 6465 7273  nd child minders
-00003860: 293c 2f78 733a 646f 6375 6d65 6e74 6174  )</xs:documentat
-00003870: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
-00003880: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
-00003890: 7469 6f6e 3e0a 2020 2020 2020 3c78 733a  tion>.      <xs:
-000038a0: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
-000038b0: 653d 2231 4322 3e3c 7873 3a61 6e6e 6f74  e="1C"><xs:annot
-000038c0: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
-000038d0: 6e74 6174 696f 6e3e 494e 4449 5649 4455  ntation>INDIVIDU
-000038e0: 414c 20e2 8093 2073 656c 663c 2f78 733a  AL ... self</xs:
-000038f0: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
-00003900: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
-00003910: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0a  xs:enumeration>.
-00003920: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
-00003930: 6174 696f 6e20 7661 6c75 653d 2231 4422  ation value="1D"
-00003940: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
-00003950: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
-00003960: 6e3e 494e 4449 5649 4455 414c 20e2 8093  n>INDIVIDUAL ...
-00003970: 206f 7468 6572 2028 696e 636c 7564 696e   other (includin
-00003980: 6720 7374 7261 6e67 6572 7329 3c2f 7873  g strangers)</xs
-00003990: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
-000039a0: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
-000039b0: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
-000039c0: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
-000039d0: 7261 7469 6f6e 2076 616c 7565 3d22 3241  ration value="2A
-000039e0: 223e 3c78 733a 616e 6e6f 7461 7469 6f6e  "><xs:annotation
-000039f0: 3e3c 7873 3a64 6f63 756d 656e 7461 7469  ><xs:documentati
-00003a00: 6f6e 3e53 4348 4f4f 4c53 3c2f 7873 3a64  on>SCHOOLS</xs:d
-00003a10: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
-00003a20: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
-00003a30: 733a 656e 756d 6572 6174 696f 6e3e 0a20  s:enumeration>. 
-00003a40: 2020 2020 203c 7873 3a65 6e75 6d65 7261       <xs:enumera
-00003a50: 7469 6f6e 2076 616c 7565 3d22 3242 223e  tion value="2B">
-00003a60: 3c78 733a 616e 6e6f 7461 7469 6f6e 3e3c  <xs:annotation><
-00003a70: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00003a80: 3e45 4455 4341 5449 4f4e 2053 4552 5649  >EDUCATION SERVI
-00003a90: 4345 533c 2f78 733a 646f 6375 6d65 6e74  CES</xs:document
-00003aa0: 6174 696f 6e3e 3c2f 7873 3a61 6e6e 6f74  ation></xs:annot
-00003ab0: 6174 696f 6e3e 3c2f 7873 3a65 6e75 6d65  ation></xs:enume
-00003ac0: 7261 7469 6f6e 3e0a 2020 2020 2020 3c78  ration>.      <x
-00003ad0: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
-00003ae0: 6c75 653d 2233 4122 3e3c 7873 3a61 6e6e  lue="3A"><xs:ann
-00003af0: 6f74 6174 696f 6e3e 3c78 733a 646f 6375  otation><xs:docu
-00003b00: 6d65 6e74 6174 696f 6e3e 4845 414c 5448  mentation>HEALTH
-00003b10: 2053 4552 5649 4345 5320 e280 9320 6765   SERVICES ... ge
-00003b20: 6e65 7261 6c20 7072 6163 7469 7469 6f6e  neral practition
-00003b30: 6572 2028 4750 293c 2f78 733a 646f 6375  er (GP)</xs:docu
-00003b40: 6d65 6e74 6174 696f 6e3e 3c2f 7873 3a61  mentation></xs:a
-00003b50: 6e6e 6f74 6174 696f 6e3e 3c2f 7873 3a65  nnotation></xs:e
-00003b60: 6e75 6d65 7261 7469 6f6e 3e0a 2020 2020  numeration>.    
-00003b70: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
-00003b80: 6e20 7661 6c75 653d 2233 4222 3e3c 7873  n value="3B"><xs
-00003b90: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
-00003ba0: 646f 6375 6d65 6e74 6174 696f 6e3e 4845  documentation>HE
-00003bb0: 414c 5448 2053 4552 5649 4345 5320 e280  ALTH SERVICES ..
-00003bc0: 9320 6865 616c 7468 2076 6973 6974 6f72  . health visitor
-00003bd0: 3c2f 7873 3a64 6f63 756d 656e 7461 7469  </xs:documentati
-00003be0: 6f6e 3e3c 2f78 733a 616e 6e6f 7461 7469  on></xs:annotati
-00003bf0: 6f6e 3e3c 2f78 733a 656e 756d 6572 6174  on></xs:enumerat
-00003c00: 696f 6e3e 0a20 2020 2020 203c 7873 3a65  ion>.      <xs:e
-00003c10: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
-00003c20: 3d22 3343 223e 3c78 733a 616e 6e6f 7461  ="3C"><xs:annota
-00003c30: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
-00003c40: 7461 7469 6f6e 3e48 4541 4c54 4820 5345  tation>HEALTH SE
-00003c50: 5256 4943 4553 20e2 8093 2073 6368 6f6f  RVICES ... schoo
-00003c60: 6c20 6e75 7273 653c 2f78 733a 646f 6375  l nurse</xs:docu
-00003c70: 6d65 6e74 6174 696f 6e3e 3c2f 7873 3a61  mentation></xs:a
-00003c80: 6e6e 6f74 6174 696f 6e3e 3c2f 7873 3a65  nnotation></xs:e
-00003c90: 6e75 6d65 7261 7469 6f6e 3e0a 2020 2020  numeration>.    
-00003ca0: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
-00003cb0: 6e20 7661 6c75 653d 2233 4422 3e3c 7873  n value="3D"><xs
-00003cc0: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
-00003cd0: 646f 6375 6d65 6e74 6174 696f 6e3e 4845  documentation>HE
-00003ce0: 414c 5448 2053 4552 5649 4345 5320 e280  ALTH SERVICES ..
-00003cf0: 9320 6f74 6865 7220 7072 696d 6172 7920  . other primary 
-00003d00: 6865 616c 7468 2073 6572 7669 6365 733c  health services<
-00003d10: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
-00003d20: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
-00003d30: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
-00003d40: 6f6e 3e0a 2020 2020 2020 3c78 733a 656e  on>.      <xs:en
-00003d50: 756d 6572 6174 696f 6e20 7661 6c75 653d  umeration value=
-00003d60: 2233 4522 3e3c 7873 3a61 6e6e 6f74 6174  "3E"><xs:annotat
-00003d70: 696f 6e3e 3c78 733a 646f 6375 6d65 6e74  ion><xs:document
-00003d80: 6174 696f 6e3e 4845 414c 5448 2053 4552  ation>HEALTH SER
-00003d90: 5649 4345 5320 e280 9320 4126 616d 703b  VICES ... A&amp;
-00003da0: 4520 2861 6363 6964 656e 7420 616e 6420  E (accident and 
-00003db0: 656d 6572 6765 6e63 7920 6465 7061 7274  emergency depart
-00003dc0: 6d65 6e74 293c 2f78 733a 646f 6375 6d65  ment)</xs:docume
-00003dd0: 6e74 6174 696f 6e3e 3c2f 7873 3a61 6e6e  ntation></xs:ann
-00003de0: 6f74 6174 696f 6e3e 3c2f 7873 3a65 6e75  otation></xs:enu
-00003df0: 6d65 7261 7469 6f6e 3e0a 2020 2020 2020  meration>.      
-00003e00: 3c78 733a 656e 756d 6572 6174 696f 6e20  <xs:enumeration 
-00003e10: 7661 6c75 653d 2233 4622 3e3c 7873 3a61  value="3F"><xs:a
-00003e20: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
-00003e30: 6375 6d65 6e74 6174 696f 6e3e 4845 414c  cumentation>HEAL
-00003e40: 5448 2053 4552 5649 4345 5320 e280 9320  TH SERVICES ... 
-00003e50: 6f74 6865 7220 2866 6f72 2065 7861 6d70  other (for examp
-00003e60: 6c65 2068 6f73 7069 6365 2920 3c2f 7873  le hospice) </xs
-00003e70: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
-00003e80: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
-00003e90: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
-00003ea0: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
-00003eb0: 7261 7469 6f6e 2076 616c 7565 3d22 3422  ration value="4"
-00003ec0: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
-00003ed0: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
-00003ee0: 6e3e 484f 5553 494e 4720 2d20 6c6f 6361  n>HOUSING - loca
-00003ef0: 6c20 6175 7468 6f72 6974 7920 686f 7573  l authority hous
-00003f00: 696e 6720 6f72 2068 6f75 7369 6e67 2061  ing or housing a
-00003f10: 7373 6f63 6961 7469 6f6e 3c2f 7873 3a64  ssociation</xs:d
-00003f20: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
-00003f30: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
-00003f40: 733a 656e 756d 6572 6174 696f 6e3e 0a20  s:enumeration>. 
-00003f50: 2020 2020 203c 7873 3a65 6e75 6d65 7261       <xs:enumera
-00003f60: 7469 6f6e 2076 616c 7565 3d22 3541 223e  tion value="5A">
-00003f70: 3c78 733a 616e 6e6f 7461 7469 6f6e 3e3c  <xs:annotation><
-00003f80: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00003f90: 3e4c 4120 5345 5256 4943 4553 20e2 8093  >LA SERVICES ...
-00003fa0: 2073 6f63 6961 6c20 6361 7265 2066 6f72   social care for
-00003fb0: 2065 7861 6d70 6c65 2061 6475 6c74 7320   example adults 
-00003fc0: 736f 6369 616c 2063 6172 6520 7365 7276  social care serv
-00003fd0: 6963 6573 3c2f 7873 3a64 6f63 756d 656e  ices</xs:documen
-00003fe0: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
-00003ff0: 7461 7469 6f6e 3e3c 2f78 733a 656e 756d  tation></xs:enum
-00004000: 6572 6174 696f 6e3e 0a20 2020 2020 203c  eration>.      <
-00004010: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
-00004020: 616c 7565 3d22 3542 223e 3c78 733a 616e  alue="5B"><xs:an
-00004030: 6e6f 7461 7469 6f6e 3e3c 7873 3a64 6f63  notation><xs:doc
-00004040: 756d 656e 7461 7469 6f6e 3e4c 4120 5345  umentation>LA SE
-00004050: 5256 4943 4553 20e2 8093 206f 7468 6572  RVICES ... other
-00004060: 2069 6e74 6572 6e61 6c20 2864 6570 6172   internal (depar
-00004070: 746d 656e 7420 6f74 6865 7220 7468 616e  tment other than
-00004080: 2073 6f63 6961 6c20 6361 7265 2069 6e20   social care in 
-00004090: 6c6f 6361 6c20 6175 7468 6f72 6974 6965  local authoritie
-000040a0: 732c 2066 6f72 2065 7861 6d70 6c65 2c20  s, for example, 
-000040b0: 796f 7574 6820 6f66 6665 6e64 696e 6720  youth offending 
-000040c0: 2865 7863 6c75 6469 6e67 2068 6f75 7369  (excluding housi
-000040d0: 6e67 2929 3c2f 7873 3a64 6f63 756d 656e  ng))</xs:documen
-000040e0: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
-000040f0: 7461 7469 6f6e 3e3c 2f78 733a 656e 756d  tation></xs:enum
-00004100: 6572 6174 696f 6e3e 0a20 2020 2020 203c  eration>.      <
-00004110: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
-00004120: 616c 7565 3d22 3543 223e 3c78 733a 616e  alue="5C"><xs:an
-00004130: 6e6f 7461 7469 6f6e 3e3c 7873 3a64 6f63  notation><xs:doc
-00004140: 756d 656e 7461 7469 6f6e 3e4c 4120 5345  umentation>LA SE
-00004150: 5256 4943 4553 20e2 8093 2065 7874 6572  RVICES ... exter
-00004160: 6e61 6c2c 2066 6f72 2065 7861 6d70 6c65  nal, for example
-00004170: 2c20 6672 6f6d 2061 6e6f 7468 6572 206c  , from another l
-00004180: 6f63 616c 2061 7574 686f 7269 7479 e280  ocal authority..
-00004190: 9973 2061 6475 6c74 7320 736f 6369 616c  .s adults social
-000041a0: 2063 6172 6520 7365 7276 6963 6573 3c2f   care services</
-000041b0: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-000041c0: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
-000041d0: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
-000041e0: 6e3e 0a20 2020 2020 203c 7873 3a65 6e75  n>.      <xs:enu
-000041f0: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-00004200: 3622 3e3c 7873 3a61 6e6e 6f74 6174 696f  6"><xs:annotatio
-00004210: 6e3e 3c78 733a 646f 6375 6d65 6e74 6174  n><xs:documentat
-00004220: 696f 6e3e 504f 4c49 4345 3c2f 7873 3a64  ion>POLICE</xs:d
-00004230: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
-00004240: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
-00004250: 733a 656e 756d 6572 6174 696f 6e3e 0a20  s:enumeration>. 
-00004260: 2020 2020 203c 7873 3a65 6e75 6d65 7261       <xs:enumera
-00004270: 7469 6f6e 2076 616c 7565 3d22 3722 3e3c  tion value="7"><
-00004280: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
-00004290: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
-000042a0: 4f54 4845 5220 4c45 4741 4c20 4147 454e  OTHER LEGAL AGEN
-000042b0: 4359 20e2 8093 2069 6e63 6c75 6469 6e67  CY ... including
-000042c0: 2063 6f75 7274 732c 2070 726f 6261 7469   courts, probati
-000042d0: 6f6e 2c20 696d 6d69 6772 6174 696f 6e2c  on, immigration,
-000042e0: 2043 4146 4341 5353 2028 4368 696c 6472   CAFCASS (Childr
-000042f0: 656e 2061 6e64 2046 616d 696c 7920 436f  en and Family Co
-00004300: 7572 7420 4164 7669 736f 7279 2061 6e64  urt Advisory and
-00004310: 2053 7570 706f 7274 2053 6572 7669 6365   Support Service
-00004320: 2920 6f72 2070 7269 736f 6e3c 2f78 733a  ) or prison</xs:
-00004330: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
-00004340: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
-00004350: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0a  xs:enumeration>.
-00004360: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
-00004370: 6174 696f 6e20 7661 6c75 653d 2238 223e  ation value="8">
-00004380: 3c78 733a 616e 6e6f 7461 7469 6f6e 3e3c  <xs:annotation><
-00004390: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-000043a0: 3e4f 5448 4552 20e2 8093 2069 6e63 6c75  >OTHER ... inclu
-000043b0: 6469 6e67 2063 6869 6c64 7265 6ee2 8099  ding children...
-000043c0: 7320 6365 6e74 7265 732c 2069 6e64 6570  s centres, indep
-000043d0: 656e 6465 6e74 2061 6765 6e63 7920 7072  endent agency pr
-000043e0: 6f76 6964 6572 7320 6f72 2076 6f6c 756e  oviders or volun
-000043f0: 7461 7279 206f 7267 616e 6973 6174 696f  tary organisatio
-00004400: 6e73 3c2f 7873 3a64 6f63 756d 656e 7461  ns</xs:documenta
-00004410: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
-00004420: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
-00004430: 6174 696f 6e3e 0a20 2020 2020 203c 7873  ation>.      <xs
-00004440: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
-00004450: 7565 3d22 3922 3e3c 7873 3a61 6e6e 6f74  ue="9"><xs:annot
-00004460: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
-00004470: 6e74 6174 696f 6e3e 414e 4f4e 594d 4f55  ntation>ANONYMOU
-00004480: 533c 2f78 733a 646f 6375 6d65 6e74 6174  S</xs:documentat
-00004490: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
-000044a0: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
-000044b0: 7469 6f6e 3e0a 2020 2020 2020 3c78 733a  tion>.      <xs:
-000044c0: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
-000044d0: 653d 2231 3022 3e3c 7873 3a61 6e6e 6f74  e="10"><xs:annot
-000044e0: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
-000044f0: 6e74 6174 696f 6e3e 554e 4b4e 4f57 4e3c  ntation>UNKNOWN<
-00004500: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
-00004510: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
-00004520: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
-00004530: 6f6e 3e0a 2020 2020 3c2f 7873 3a72 6573  on>.    </xs:res
-00004540: 7472 6963 7469 6f6e 3e0a 2020 3c2f 7873  triction>.  </xs
-00004550: 3a73 696d 706c 6554 7970 653e 0a0a 2020  :simpleType>..  
-00004560: 3c78 733a 7369 6d70 6c65 5479 7065 206e  <xs:simpleType n
-00004570: 616d 653d 2263 6174 6567 6f72 796f 6661  ame="categoryofa
-00004580: 6275 7365 223e 0a20 2020 203c 7873 3a72  buse">.    <xs:r
-00004590: 6573 7472 6963 7469 6f6e 2062 6173 653d  estriction base=
-000045a0: 226e 6f6e 456d 7074 7953 7472 696e 6722  "nonEmptyString"
-000045b0: 3e0a 2020 2020 2020 3c78 733a 656e 756d  >.      <xs:enum
-000045c0: 6572 6174 696f 6e20 7661 6c75 653d 224e  eration value="N
-000045d0: 4547 223e 3c78 733a 616e 6e6f 7461 7469  EG"><xs:annotati
-000045e0: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
-000045f0: 7469 6f6e 3e4e 6567 6c65 6374 3c2f 7873  tion>Neglect</xs
-00004600: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
-00004610: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
-00004620: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
-00004630: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
-00004640: 7261 7469 6f6e 2076 616c 7565 3d22 5048  ration value="PH
-00004650: 5922 3e3c 7873 3a61 6e6e 6f74 6174 696f  Y"><xs:annotatio
-00004660: 6e3e 3c78 733a 646f 6375 6d65 6e74 6174  n><xs:documentat
-00004670: 696f 6e3e 5068 7973 6963 616c 2061 6275  ion>Physical abu
-00004680: 7365 3c2f 7873 3a64 6f63 756d 656e 7461  se</xs:documenta
-00004690: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
-000046a0: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
-000046b0: 6174 696f 6e3e 0a20 2020 2020 203c 7873  ation>.      <xs
-000046c0: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
-000046d0: 7565 3d22 5341 4222 3e3c 7873 3a61 6e6e  ue="SAB"><xs:ann
-000046e0: 6f74 6174 696f 6e3e 3c78 733a 646f 6375  otation><xs:docu
-000046f0: 6d65 6e74 6174 696f 6e3e 5365 7875 616c  mentation>Sexual
-00004700: 2061 6275 7365 3c2f 7873 3a64 6f63 756d   abuse</xs:docum
-00004710: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
-00004720: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
-00004730: 756d 6572 6174 696f 6e3e 0a20 2020 2020  umeration>.     
-00004740: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
-00004750: 2076 616c 7565 3d22 454d 4f22 3e3c 7873   value="EMO"><xs
-00004760: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
-00004770: 646f 6375 6d65 6e74 6174 696f 6e3e 456d  documentation>Em
-00004780: 6f74 696f 6e61 6c20 6162 7573 653c 2f78  otional abuse</x
-00004790: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
-000047a0: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
-000047b0: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
-000047c0: 3e0a 2020 2020 2020 3c78 733a 656e 756d  >.      <xs:enum
-000047d0: 6572 6174 696f 6e20 7661 6c75 653d 224d  eration value="M
-000047e0: 554c 223e 3c78 733a 616e 6e6f 7461 7469  UL"><xs:annotati
-000047f0: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
-00004800: 7469 6f6e 3e4d 756c 7469 706c 652f 6e6f  tion>Multiple/no
-00004810: 7420 7265 636f 6d6d 656e 6465 643c 2f78  t recommended</x
-00004820: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
-00004830: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
-00004840: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
-00004850: 3e0a 2020 2020 3c2f 7873 3a72 6573 7472  >.    </xs:restr
-00004860: 6963 7469 6f6e 3e0a 2020 3c2f 7873 3a73  iction>.  </xs:s
-00004870: 696d 706c 6554 7970 653e 0a0a 2020 2020  impleType>..    
-00004880: 3c78 733a 7369 6d70 6c65 5479 7065 206e  <xs:simpleType n
-00004890: 616d 653d 2270 7269 6d61 7279 6e65 6564  ame="primaryneed
-000048a0: 636f 6465 7479 7065 223e 0a20 2020 203c  codetype">.    <
-000048b0: 7873 3a72 6573 7472 6963 7469 6f6e 2062  xs:restriction b
-000048c0: 6173 653d 2278 733a 7374 7269 6e67 223e  ase="xs:string">
-000048d0: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
-000048e0: 7261 7469 6f6e 2076 616c 7565 3d22 4e31  ration value="N1
-000048f0: 223e 3c78 733a 616e 6e6f 7461 7469 6f6e  "><xs:annotation
-00004900: 3e3c 7873 3a64 6f63 756d 656e 7461 7469  ><xs:documentati
-00004910: 6f6e 3e41 6275 7365 206f 7220 6e65 676c  on>Abuse or negl
-00004920: 6563 743c 2f78 733a 646f 6375 6d65 6e74  ect</xs:document
-00004930: 6174 696f 6e3e 3c2f 7873 3a61 6e6e 6f74  ation></xs:annot
-00004940: 6174 696f 6e3e 3c2f 7873 3a65 6e75 6d65  ation></xs:enume
-00004950: 7261 7469 6f6e 3e0a 2020 2020 2020 3c78  ration>.      <x
-00004960: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
-00004970: 6c75 653d 224e 3222 3e3c 7873 3a61 6e6e  lue="N2"><xs:ann
-00004980: 6f74 6174 696f 6e3e 3c78 733a 646f 6375  otation><xs:docu
-00004990: 6d65 6e74 6174 696f 6e3e 4368 696c 6427  mentation>Child'
-000049a0: 7320 6469 7361 6269 6c69 7479 3c2f 7873  s disability</xs
-000049b0: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
-000049c0: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
-000049d0: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
-000049e0: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
-000049f0: 7261 7469 6f6e 2076 616c 7565 3d22 4e33  ration value="N3
-00004a00: 223e 3c78 733a 616e 6e6f 7461 7469 6f6e  "><xs:annotation
-00004a10: 3e3c 7873 3a64 6f63 756d 656e 7461 7469  ><xs:documentati
-00004a20: 6f6e 3e50 6172 656e 7461 6c20 6469 7361  on>Parental disa
-00004a30: 6269 6c69 7479 206f 7220 696c 6c6e 6573  bility or illnes
-00004a40: 733c 2f78 733a 646f 6375 6d65 6e74 6174  s</xs:documentat
-00004a50: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
-00004a60: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
-00004a70: 7469 6f6e 3e0a 2020 2020 2020 3c78 733a  tion>.      <xs:
-00004a80: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
-00004a90: 653d 224e 3422 3e3c 7873 3a61 6e6e 6f74  e="N4"><xs:annot
-00004aa0: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
-00004ab0: 6e74 6174 696f 6e3e 4661 6d69 6c79 2069  ntation>Family i
-00004ac0: 6e20 6163 7574 6520 7374 7265 7373 3c2f  n acute stress</
-00004ad0: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00004ae0: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
-00004af0: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
-00004b00: 6e3e 0a20 2020 2020 203c 7873 3a65 6e75  n>.      <xs:enu
-00004b10: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-00004b20: 4e35 223e 3c78 733a 616e 6e6f 7461 7469  N5"><xs:annotati
-00004b30: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
-00004b40: 7469 6f6e 3e46 616d 696c 7920 6479 7366  tion>Family dysf
-00004b50: 756e 6374 696f 6e3c 2f78 733a 646f 6375  unction</xs:docu
-00004b60: 6d65 6e74 6174 696f 6e3e 3c2f 7873 3a61  mentation></xs:a
-00004b70: 6e6e 6f74 6174 696f 6e3e 3c2f 7873 3a65  nnotation></xs:e
-00004b80: 6e75 6d65 7261 7469 6f6e 3e0a 2020 2020  numeration>.    
-00004b90: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
-00004ba0: 6e20 7661 6c75 653d 224e 3622 3e3c 7873  n value="N6"><xs
-00004bb0: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
-00004bc0: 646f 6375 6d65 6e74 6174 696f 6e3e 536f  documentation>So
-00004bd0: 6369 616c 6c79 2075 6e61 6363 6570 7461  cially unaccepta
-00004be0: 626c 6520 6265 6861 7669 6f75 723c 2f78  ble behaviour</x
-00004bf0: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
-00004c00: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
-00004c10: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
-00004c20: 3e0a 2020 2020 2020 3c78 733a 656e 756d  >.      <xs:enum
-00004c30: 6572 6174 696f 6e20 7661 6c75 653d 224e  eration value="N
-00004c40: 3722 3e3c 7873 3a61 6e6e 6f74 6174 696f  7"><xs:annotatio
-00004c50: 6e3e 3c78 733a 646f 6375 6d65 6e74 6174  n><xs:documentat
-00004c60: 696f 6e3e 4c6f 7720 696e 636f 6d65 3c2f  ion>Low income</
-00004c70: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00004c80: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
-00004c90: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
-00004ca0: 6e3e 0a20 2020 2020 203c 7873 3a65 6e75  n>.      <xs:enu
-00004cb0: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-00004cc0: 4e38 223e 3c78 733a 616e 6e6f 7461 7469  N8"><xs:annotati
-00004cd0: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
-00004ce0: 7469 6f6e 3e41 6273 656e 7420 7061 7265  tion>Absent pare
-00004cf0: 6e74 696e 673c 2f78 733a 646f 6375 6d65  nting</xs:docume
-00004d00: 6e74 6174 696f 6e3e 3c2f 7873 3a61 6e6e  ntation></xs:ann
-00004d10: 6f74 6174 696f 6e3e 3c2f 7873 3a65 6e75  otation></xs:enu
-00004d20: 6d65 7261 7469 6f6e 3e0a 2020 2020 2020  meration>.      
-00004d30: 3c78 733a 656e 756d 6572 6174 696f 6e20  <xs:enumeration 
-00004d40: 7661 6c75 653d 224e 3922 3e3c 7873 3a61  value="N9"><xs:a
-00004d50: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
-00004d60: 6375 6d65 6e74 6174 696f 6e3e 4361 7365  cumentation>Case
-00004d70: 7320 6f74 6865 7220 7468 616e 2063 6869  s other than chi
-00004d80: 6c64 7265 6e20 696e 206e 6565 643c 2f78  ldren in need</x
-00004d90: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
-00004da0: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
-00004db0: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
-00004dc0: 3e0a 2020 2020 2020 3c78 733a 656e 756d  >.      <xs:enum
-00004dd0: 6572 6174 696f 6e20 7661 6c75 653d 224e  eration value="N
-00004de0: 3022 3e3c 7873 3a61 6e6e 6f74 6174 696f  0"><xs:annotatio
-00004df0: 6e3e 3c78 733a 646f 6375 6d65 6e74 6174  n><xs:documentat
-00004e00: 696f 6e3e 4e6f 7420 7374 6174 6564 3c2f  ion>Not stated</
-00004e10: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00004e20: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
-00004e30: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
-00004e40: 6e3e 0a20 2020 203c 2f78 733a 7265 7374  n>.    </xs:rest
-00004e50: 7269 6374 696f 6e3e 0a20 203c 2f78 733a  riction>.  </xs:
-00004e60: 7369 6d70 6c65 5479 7065 3e0a 0a0a 2020  simpleType>...  
-00004e70: 3c78 733a 7369 6d70 6c65 5479 7065 206e  <xs:simpleType n
-00004e80: 616d 653d 2272 6561 736f 6e66 6f72 636c  ame="reasonforcl
-00004e90: 6f73 7572 6574 7970 6522 3e0a 2020 2020  osuretype">.    
-00004ea0: 3c78 733a 7265 7374 7269 6374 696f 6e20  <xs:restriction 
-00004eb0: 6261 7365 3d22 7873 3a73 7472 696e 6722  base="xs:string"
-00004ec0: 3e0a 2020 2020 2020 3c78 733a 656e 756d  >.      <xs:enum
-00004ed0: 6572 6174 696f 6e20 7661 6c75 653d 2252  eration value="R
-00004ee0: 4331 223e 3c78 733a 616e 6e6f 7461 7469  C1"><xs:annotati
-00004ef0: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
-00004f00: 7469 6f6e 3e41 646f 7074 6564 3c2f 7873  tion>Adopted</xs
-00004f10: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
-00004f20: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
-00004f30: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
-00004f40: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
-00004f50: 7261 7469 6f6e 2076 616c 7565 3d22 5243  ration value="RC
-00004f60: 3222 3e3c 7873 3a61 6e6e 6f74 6174 696f  2"><xs:annotatio
-00004f70: 6e3e 3c78 733a 646f 6375 6d65 6e74 6174  n><xs:documentat
-00004f80: 696f 6e3e 4469 6564 3c2f 7873 3a64 6f63  ion>Died</xs:doc
-00004f90: 756d 656e 7461 7469 6f6e 3e3c 2f78 733a  umentation></xs:
-00004fa0: 616e 6e6f 7461 7469 6f6e 3e3c 2f78 733a  annotation></xs:
-00004fb0: 656e 756d 6572 6174 696f 6e3e 0a20 2020  enumeration>.   
-00004fc0: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
-00004fd0: 6f6e 2076 616c 7565 3d22 5243 3322 3e3c  on value="RC3"><
-00004fe0: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
-00004ff0: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
-00005000: 4368 696c 6420 6172 7261 6e67 656d 656e  Child arrangemen
-00005010: 7473 206f 7264 6572 3c2f 7873 3a64 6f63  ts order</xs:doc
-00005020: 756d 656e 7461 7469 6f6e 3e3c 2f78 733a  umentation></xs:
-00005030: 616e 6e6f 7461 7469 6f6e 3e3c 2f78 733a  annotation></xs:
-00005040: 656e 756d 6572 6174 696f 6e3e 0a20 2020  enumeration>.   
-00005050: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
-00005060: 6f6e 2076 616c 7565 3d22 5243 3422 3e3c  on value="RC4"><
-00005070: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
-00005080: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
-00005090: 5370 6563 6961 6c20 6775 6172 6469 616e  Special guardian
-000050a0: 7368 6970 206f 7264 6572 3c2f 7873 3a64  ship order</xs:d
-000050b0: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
-000050c0: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
-000050d0: 733a 656e 756d 6572 6174 696f 6e3e 0a20  s:enumeration>. 
-000050e0: 2020 2020 203c 7873 3a65 6e75 6d65 7261       <xs:enumera
-000050f0: 7469 6f6e 2076 616c 7565 3d22 5243 3522  tion value="RC5"
-00005100: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
-00005110: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
-00005120: 6e3e 5472 616e 7366 6572 7265 6420 746f  n>Transferred to
-00005130: 2073 6572 7669 6365 7320 6f66 2061 6e6f   services of ano
-00005140: 7468 6572 206c 6f63 616c 2061 7574 686f  ther local autho
-00005150: 7269 7479 3c2f 7873 3a64 6f63 756d 656e  rity</xs:documen
-00005160: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
-00005170: 7461 7469 6f6e 3e3c 2f78 733a 656e 756d  tation></xs:enum
-00005180: 6572 6174 696f 6e3e 0a20 2020 2020 203c  eration>.      <
-00005190: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
-000051a0: 616c 7565 3d22 5243 3622 3e3c 7873 3a61  alue="RC6"><xs:a
-000051b0: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
-000051c0: 6375 6d65 6e74 6174 696f 6e3e 5472 616e  cumentation>Tran
-000051d0: 7366 6572 7265 6420 746f 2061 6475 6c74  sferred to adult
-000051e0: 2073 6f63 6961 6c20 6361 7265 2073 6572   social care ser
-000051f0: 7669 6365 733c 2f78 733a 646f 6375 6d65  vices</xs:docume
-00005200: 6e74 6174 696f 6e3e 3c2f 7873 3a61 6e6e  ntation></xs:ann
-00005210: 6f74 6174 696f 6e3e 3c2f 7873 3a65 6e75  otation></xs:enu
-00005220: 6d65 7261 7469 6f6e 3e0a 2020 2020 2020  meration>.      
-00005230: 3c78 733a 656e 756d 6572 6174 696f 6e20  <xs:enumeration 
-00005240: 7661 6c75 653d 2252 4337 223e 3c78 733a  value="RC7"><xs:
-00005250: 616e 6e6f 7461 7469 6f6e 3e3c 7873 3a64  annotation><xs:d
-00005260: 6f63 756d 656e 7461 7469 6f6e 3e53 6572  ocumentation>Ser
-00005270: 7669 6365 7320 6365 6173 6564 2066 6f72  vices ceased for
-00005280: 2061 6e79 206f 7468 6572 2072 6561 736f   any other reaso
-00005290: 6e2c 2069 6e63 6c75 6469 6e67 2063 6869  n, including chi
-000052a0: 6c64 206e 6f20 6c6f 6e67 6572 2069 6e20  ld no longer in 
-000052b0: 6e65 6564 3c2f 7873 3a64 6f63 756d 656e  need</xs:documen
-000052c0: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
-000052d0: 7461 7469 6f6e 3e3c 2f78 733a 656e 756d  tation></xs:enum
-000052e0: 6572 6174 696f 6e3e 0a20 2020 2020 203c  eration>.      <
-000052f0: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
-00005300: 616c 7565 3d22 5243 3822 3e3c 7873 3a61  alue="RC8"><xs:a
-00005310: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
-00005320: 6375 6d65 6e74 6174 696f 6e3e 4361 7365  cumentation>Case
-00005330: 2063 6c6f 7365 6420 6166 7465 7220 6173   closed after as
-00005340: 7365 7373 6d65 6e74 2c20 6e6f 2066 7572  sessment, no fur
-00005350: 7468 6572 2061 6374 696f 6e3c 2f78 733a  ther action</xs:
-00005360: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
-00005370: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
-00005380: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0a  xs:enumeration>.
-00005390: 2020 2020 3c2f 7873 3a72 6573 7472 6963      </xs:restric
-000053a0: 7469 6f6e 3e0a 2020 3c2f 7873 3a73 696d  tion>.  </xs:sim
-000053b0: 706c 6554 7970 653e 0a0a 2020 2020 3c78  pleType>..    <x
-000053c0: 733a 7369 6d70 6c65 5479 7065 206e 616d  s:simpleType nam
-000053d0: 653d 2261 7373 6573 736d 656e 7466 6163  e="assessmentfac
-000053e0: 746f 7273 7479 7065 223e 0a20 2020 203c  torstype">.    <
-000053f0: 7873 3a72 6573 7472 6963 7469 6f6e 2062  xs:restriction b
-00005400: 6173 653d 226e 6f6e 456d 7074 7953 7472  ase="nonEmptyStr
-00005410: 696e 6722 3e0a 2020 2020 2020 3c78 733a  ing">.      <xs:
-00005420: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
-00005430: 653d 2231 4122 3e3c 7873 3a61 6e6e 6f74  e="1A"><xs:annot
-00005440: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
-00005450: 6e74 6174 696f 6e3e 416c 636f 686f 6c20  ntation>Alcohol 
-00005460: 6d69 7375 7365 3a20 636f 6e63 6572 6e73  misuse: concerns
-00005470: 2061 626f 7574 2061 6c63 6f68 6f6c 206d   about alcohol m
-00005480: 6973 7573 6520 6279 2074 6865 2063 6869  isuse by the chi
-00005490: 6c64 3c2f 7873 3a64 6f63 756d 656e 7461  ld</xs:documenta
-000054a0: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
-000054b0: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
-000054c0: 6174 696f 6e3e 0a20 2020 2020 203c 7873  ation>.      <xs
-000054d0: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
-000054e0: 7565 3d22 3142 223e 3c78 733a 616e 6e6f  ue="1B"><xs:anno
-000054f0: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
-00005500: 656e 7461 7469 6f6e 3e41 6c63 6f68 6f6c  entation>Alcohol
-00005510: 206d 6973 7573 653a 2063 6f6e 6365 726e   misuse: concern
-00005520: 7320 6162 6f75 7420 616c 636f 686f 6c20  s about alcohol 
-00005530: 6d69 7375 7365 2062 7920 7468 6520 7061  misuse by the pa
-00005540: 7265 6e74 2873 292f 6361 7265 7228 7329  rent(s)/carer(s)
-00005550: 3c2f 7873 3a64 6f63 756d 656e 7461 7469  </xs:documentati
-00005560: 6f6e 3e3c 2f78 733a 616e 6e6f 7461 7469  on></xs:annotati
-00005570: 6f6e 3e3c 2f78 733a 656e 756d 6572 6174  on></xs:enumerat
-00005580: 696f 6e3e 0a20 2020 2020 203c 7873 3a65  ion>.      <xs:e
-00005590: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
-000055a0: 3d22 3143 223e 3c78 733a 616e 6e6f 7461  ="1C"><xs:annota
-000055b0: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
-000055c0: 7461 7469 6f6e 3e41 6c63 6f68 6f6c 206d  tation>Alcohol m
-000055d0: 6973 7573 653a 2063 6f6e 6365 726e 7320  isuse: concerns 
-000055e0: 6162 6f75 7420 616c 636f 686f 6c20 6d69  about alcohol mi
-000055f0: 7375 7365 2062 7920 616e 6f74 6865 7220  suse by another 
-00005600: 7065 7273 6f6e 206c 6976 696e 6720 696e  person living in
-00005610: 2074 6865 2068 6f75 7365 686f 6c64 3c2f   the household</
-00005620: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00005630: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
-00005640: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
-00005650: 6e3e 0a20 2020 2020 203c 7873 3a65 6e75  n>.      <xs:enu
-00005660: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-00005670: 3241 223e 3c78 733a 616e 6e6f 7461 7469  2A"><xs:annotati
-00005680: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
-00005690: 7469 6f6e 3e44 7275 6720 6d69 7375 7365  tion>Drug misuse
-000056a0: 3a20 636f 6e63 6572 6e73 2061 626f 7574  : concerns about
-000056b0: 2064 7275 6720 6d69 7375 7365 2062 7920   drug misuse by 
-000056c0: 7468 6520 6368 696c 643c 2f78 733a 646f  the child</xs:do
-000056d0: 6375 6d65 6e74 6174 696f 6e3e 3c2f 7873  cumentation></xs
-000056e0: 3a61 6e6e 6f74 6174 696f 6e3e 3c2f 7873  :annotation></xs
-000056f0: 3a65 6e75 6d65 7261 7469 6f6e 3e0a 2020  :enumeration>.  
-00005700: 2020 2020 3c78 733a 656e 756d 6572 6174      <xs:enumerat
-00005710: 696f 6e20 7661 6c75 653d 2232 4222 3e3c  ion value="2B"><
-00005720: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
-00005730: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
-00005740: 4472 7567 206d 6973 7573 653a 2063 6f6e  Drug misuse: con
-00005750: 6365 726e 7320 6162 6f75 7420 6472 7567  cerns about drug
-00005760: 206d 6973 7573 6520 6279 2074 6865 2070   misuse by the p
-00005770: 6172 656e 7428 7329 2f63 6172 6572 2873  arent(s)/carer(s
-00005780: 293c 2f78 733a 646f 6375 6d65 6e74 6174  )</xs:documentat
-00005790: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
-000057a0: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
-000057b0: 7469 6f6e 3e0a 2020 2020 2020 3c78 733a  tion>.      <xs:
-000057c0: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
-000057d0: 653d 2232 4322 3e3c 7873 3a61 6e6e 6f74  e="2C"><xs:annot
-000057e0: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
-000057f0: 6e74 6174 696f 6e3e 4472 7567 206d 6973  ntation>Drug mis
-00005800: 7573 653a 2063 6f6e 6365 726e 7320 6162  use: concerns ab
-00005810: 6f75 7420 6472 7567 206d 6973 7573 6520  out drug misuse 
-00005820: 6279 2061 6e6f 7468 6572 2070 6572 736f  by another perso
-00005830: 6e20 6c69 7669 6e67 2069 6e20 7468 6520  n living in the 
-00005840: 686f 7573 6568 6f6c 643c 2f78 733a 646f  household</xs:do
-00005850: 6375 6d65 6e74 6174 696f 6e3e 3c2f 7873  cumentation></xs
-00005860: 3a61 6e6e 6f74 6174 696f 6e3e 3c2f 7873  :annotation></xs
-00005870: 3a65 6e75 6d65 7261 7469 6f6e 3e0a 2020  :enumeration>.  
-00005880: 2020 2020 3c78 733a 656e 756d 6572 6174      <xs:enumerat
-00005890: 696f 6e20 7661 6c75 653d 2233 4122 3e3c  ion value="3A"><
-000058a0: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
-000058b0: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
-000058c0: 446f 6d65 7374 6963 2076 696f 6c65 6e63  Domestic violenc
-000058d0: 653a 2063 6f6e 6365 726e 7320 6162 6f75  e: concerns abou
-000058e0: 7420 7468 6520 6368 696c 6420 6265 696e  t the child bein
-000058f0: 6720 7468 6520 7375 626a 6563 7420 6f66  g the subject of
-00005900: 2064 6f6d 6573 7469 6320 7669 6f6c 656e   domestic violen
-00005910: 6365 3c2f 7873 3a64 6f63 756d 656e 7461  ce</xs:documenta
-00005920: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
-00005930: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
-00005940: 6174 696f 6e3e 0a20 2020 2020 203c 7873  ation>.      <xs
-00005950: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
-00005960: 7565 3d22 3342 223e 3c78 733a 616e 6e6f  ue="3B"><xs:anno
-00005970: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
-00005980: 656e 7461 7469 6f6e 3e44 6f6d 6573 7469  entation>Domesti
-00005990: 6320 7669 6f6c 656e 6365 3a20 636f 6e63  c violence: conc
-000059a0: 6572 6e73 2061 626f 7574 2074 6865 2063  erns about the c
-000059b0: 6869 6c64 e280 9973 2070 6172 656e 7428  hild...s parent(
-000059c0: 7329 2f63 6172 6572 2873 2920 6265 696e  s)/carer(s) bein
-000059d0: 6720 7468 6520 7375 626a 6563 7420 6f66  g the subject of
-000059e0: 2064 6f6d 6573 7469 6320 7669 6f6c 656e   domestic violen
-000059f0: 6365 3c2f 7873 3a64 6f63 756d 656e 7461  ce</xs:documenta
-00005a00: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
-00005a10: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
-00005a20: 6174 696f 6e3e 0a20 2020 2020 203c 7873  ation>.      <xs
-00005a30: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
-00005a40: 7565 3d22 3343 223e 3c78 733a 616e 6e6f  ue="3C"><xs:anno
-00005a50: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
-00005a60: 656e 7461 7469 6f6e 3e44 6f6d 6573 7469  entation>Domesti
-00005a70: 6320 7669 6f6c 656e 6365 3a20 636f 6e63  c violence: conc
-00005a80: 6572 6e73 2061 626f 7574 2061 6e6f 7468  erns about anoth
-00005a90: 6572 2070 6572 736f 6e20 6c69 7669 6e67  er person living
-00005aa0: 2069 6e20 7468 6520 686f 7573 6568 6f6c   in the househol
-00005ab0: 6420 6265 696e 6720 7468 6520 7375 626a  d being the subj
-00005ac0: 6563 7420 6f66 2064 6f6d 6573 7469 6320  ect of domestic 
-00005ad0: 7669 6f6c 656e 6365 3c2f 7873 3a64 6f63  violence</xs:doc
-00005ae0: 756d 656e 7461 7469 6f6e 3e3c 2f78 733a  umentation></xs:
-00005af0: 616e 6e6f 7461 7469 6f6e 3e3c 2f78 733a  annotation></xs:
-00005b00: 656e 756d 6572 6174 696f 6e3e 0a20 2020  enumeration>.   
-00005b10: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
-00005b20: 6f6e 2076 616c 7565 3d22 3441 223e 3c78  on value="4A"><x
-00005b30: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
-00005b40: 3a64 6f63 756d 656e 7461 7469 6f6e 3e4d  :documentation>M
-00005b50: 656e 7461 6c20 6865 616c 7468 3a20 636f  ental health: co
-00005b60: 6e63 6572 6e73 2061 626f 7574 2074 6865  ncerns about the
-00005b70: 206d 656e 7461 6c20 6865 616c 7468 206f   mental health o
-00005b80: 6620 7468 6520 6368 696c 643c 2f78 733a  f the child</xs:
-00005b90: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
-00005ba0: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
-00005bb0: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0a  xs:enumeration>.
-00005bc0: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
-00005bd0: 6174 696f 6e20 7661 6c75 653d 2234 4222  ation value="4B"
-00005be0: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
-00005bf0: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
-00005c00: 6e3e 4d65 6e74 616c 2068 6561 6c74 683a  n>Mental health:
-00005c10: 2063 6f6e 6365 726e 7320 6162 6f75 7420   concerns about 
-00005c20: 7468 6520 6d65 6e74 616c 2068 6561 6c74  the mental healt
-00005c30: 6820 6f66 2074 6865 2070 6172 656e 7428  h of the parent(
-00005c40: 7329 2f63 6172 6572 2873 293c 2f78 733a  s)/carer(s)</xs:
-00005c50: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
-00005c60: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
-00005c70: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0a  xs:enumeration>.
-00005c80: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
-00005c90: 6174 696f 6e20 7661 6c75 653d 2234 4322  ation value="4C"
-00005ca0: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
-00005cb0: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
-00005cc0: 6e3e 4d65 6e74 616c 2068 6561 6c74 683a  n>Mental health:
-00005cd0: 2063 6f6e 6365 726e 7320 6162 6f75 7420   concerns about 
-00005ce0: 7468 6520 6d65 6e74 616c 2068 6561 6c74  the mental healt
-00005cf0: 6820 6f66 2061 6e6f 7468 6572 2070 6572  h of another per
-00005d00: 736f 6e20 696e 2074 6865 2066 616d 696c  son in the famil
-00005d10: 792f 686f 7573 6568 6f6c 643c 2f78 733a  y/household</xs:
-00005d20: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
-00005d30: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
-00005d40: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0a  xs:enumeration>.
-00005d50: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
-00005d60: 6174 696f 6e20 7661 6c75 653d 2235 4122  ation value="5A"
-00005d70: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
-00005d80: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
-00005d90: 6e3e 4c65 6172 6e69 6e67 2064 6973 6162  n>Learning disab
-00005da0: 696c 6974 793a 2063 6f6e 6365 726e 7320  ility: concerns 
-00005db0: 6162 6f75 7420 7468 6520 6368 696c 64e2  about the child.
-00005dc0: 8099 7320 6c65 6172 6e69 6e67 2064 6973  ..s learning dis
-00005dd0: 6162 696c 6974 793c 2f78 733a 646f 6375  ability</xs:docu
-00005de0: 6d65 6e74 6174 696f 6e3e 3c2f 7873 3a61  mentation></xs:a
-00005df0: 6e6e 6f74 6174 696f 6e3e 3c2f 7873 3a65  nnotation></xs:e
-00005e00: 6e75 6d65 7261 7469 6f6e 3e0a 2020 2020  numeration>.    
-00005e10: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
-00005e20: 6e20 7661 6c75 653d 2235 4222 3e3c 7873  n value="5B"><xs
-00005e30: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
-00005e40: 646f 6375 6d65 6e74 6174 696f 6e3e 4c65  documentation>Le
-00005e50: 6172 6e69 6e67 2064 6973 6162 696c 6974  arning disabilit
-00005e60: 793a 2063 6f6e 6365 726e 7320 6162 6f75  y: concerns abou
-00005e70: 7420 7468 6520 7061 7265 6e74 2873 292f  t the parent(s)/
-00005e80: 6361 7265 7228 7329 206c 6561 726e 696e  carer(s) learnin
-00005e90: 6720 6469 7361 6269 6c69 7479 3c2f 7873  g disability</xs
-00005ea0: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
-00005eb0: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
-00005ec0: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
-00005ed0: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
-00005ee0: 7261 7469 6f6e 2076 616c 7565 3d22 3543  ration value="5C
-00005ef0: 223e 3c78 733a 616e 6e6f 7461 7469 6f6e  "><xs:annotation
-00005f00: 3e3c 7873 3a64 6f63 756d 656e 7461 7469  ><xs:documentati
-00005f10: 6f6e 3e4c 6561 726e 696e 6720 6469 7361  on>Learning disa
-00005f20: 6269 6c69 7479 3a20 636f 6e63 6572 6e73  bility: concerns
-00005f30: 2061 626f 7574 2061 6e6f 7468 6572 2070   about another p
-00005f40: 6572 736f 6e20 696e 2074 6865 2066 616d  erson in the fam
-00005f50: 696c 792f 686f 7573 6568 6f6c 64e2 8099  ily/household...
-00005f60: 7320 6c65 6172 6e69 6e67 2064 6973 6162  s learning disab
-00005f70: 696c 6974 793c 2f78 733a 646f 6375 6d65  ility</xs:docume
-00005f80: 6e74 6174 696f 6e3e 3c2f 7873 3a61 6e6e  ntation></xs:ann
-00005f90: 6f74 6174 696f 6e3e 3c2f 7873 3a65 6e75  otation></xs:enu
-00005fa0: 6d65 7261 7469 6f6e 3e0a 2020 2020 2020  meration>.      
-00005fb0: 3c78 733a 656e 756d 6572 6174 696f 6e20  <xs:enumeration 
-00005fc0: 7661 6c75 653d 2236 4122 3e3c 7873 3a61  value="6A"><xs:a
-00005fd0: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
-00005fe0: 6375 6d65 6e74 6174 696f 6e3e 5068 7973  cumentation>Phys
-00005ff0: 6963 616c 2064 6973 6162 696c 6974 7920  ical disability 
-00006000: 6f72 2069 6c6c 6e65 7373 3a20 636f 6e63  or illness: conc
-00006010: 6572 6e73 2061 626f 7574 2061 2070 6879  erns about a phy
-00006020: 7369 6361 6c20 6469 7361 6269 6c69 7479  sical disability
-00006030: 206f 7220 696c 6c6e 6573 7320 6f66 2074   or illness of t
-00006040: 6865 2063 6869 6c64 3c2f 7873 3a64 6f63  he child</xs:doc
-00006050: 756d 656e 7461 7469 6f6e 3e3c 2f78 733a  umentation></xs:
-00006060: 616e 6e6f 7461 7469 6f6e 3e3c 2f78 733a  annotation></xs:
-00006070: 656e 756d 6572 6174 696f 6e3e 0a20 2020  enumeration>.   
-00006080: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
-00006090: 6f6e 2076 616c 7565 3d22 3642 223e 3c78  on value="6B"><x
-000060a0: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
-000060b0: 3a64 6f63 756d 656e 7461 7469 6f6e 3e50  :documentation>P
-000060c0: 6879 7369 6361 6c20 6469 7361 6269 6c69  hysical disabili
-000060d0: 7479 206f 7220 696c 6c6e 6573 733a 2063  ty or illness: c
-000060e0: 6f6e 6365 726e 7320 6162 6f75 7420 6120  oncerns about a 
-000060f0: 7068 7973 6963 616c 2064 6973 6162 696c  physical disabil
-00006100: 6974 7920 6f72 2069 6c6c 6e65 7373 206f  ity or illness o
-00006110: 6620 7468 6520 7061 7265 6e74 2873 292f  f the parent(s)/
-00006120: 6361 7265 7228 7329 3c2f 7873 3a64 6f63  carer(s)</xs:doc
-00006130: 756d 656e 7461 7469 6f6e 3e3c 2f78 733a  umentation></xs:
-00006140: 616e 6e6f 7461 7469 6f6e 3e3c 2f78 733a  annotation></xs:
-00006150: 656e 756d 6572 6174 696f 6e3e 0a20 2020  enumeration>.   
-00006160: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
-00006170: 6f6e 2076 616c 7565 3d22 3643 223e 3c78  on value="6C"><x
-00006180: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
-00006190: 3a64 6f63 756d 656e 7461 7469 6f6e 3e50  :documentation>P
-000061a0: 6879 7369 6361 6c20 6469 7361 6269 6c69  hysical disabili
-000061b0: 7479 206f 7220 696c 6c6e 6573 733a 2063  ty or illness: c
-000061c0: 6f6e 6365 726e 7320 6162 6f75 7420 6120  oncerns about a 
-000061d0: 7068 7973 6963 616c 2064 6973 6162 696c  physical disabil
-000061e0: 6974 7920 6f72 2069 6c6c 6e65 7373 206f  ity or illness o
-000061f0: 6620 616e 6f74 6865 7220 7065 7273 6f6e  f another person
-00006200: 2069 6e20 7468 6520 6661 6d69 6c79 2f68   in the family/h
-00006210: 6f75 7365 686f 6c64 3c2f 7873 3a64 6f63  ousehold</xs:doc
-00006220: 756d 656e 7461 7469 6f6e 3e3c 2f78 733a  umentation></xs:
-00006230: 616e 6e6f 7461 7469 6f6e 3e3c 2f78 733a  annotation></xs:
-00006240: 656e 756d 6572 6174 696f 6e3e 0a20 2020  enumeration>.   
-00006250: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
-00006260: 6f6e 2076 616c 7565 3d22 3741 223e 3c78  on value="7A"><x
-00006270: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
-00006280: 3a64 6f63 756d 656e 7461 7469 6f6e 3e59  :documentation>Y
-00006290: 6f75 6e67 2063 6172 6572 3a20 636f 6e63  oung carer: conc
-000062a0: 6572 6e73 2074 6861 7420 7365 7276 6963  erns that servic
-000062b0: 6573 206d 6179 2062 6520 7265 7175 6972  es may be requir
-000062c0: 6564 206f 7220 7468 6520 6368 696c 64e2  ed or the child.
-000062d0: 8099 7320 6865 616c 7468 206f 7220 6465  ..s health or de
-000062e0: 7665 6c6f 706d 656e 7420 6d61 7920 6265  velopment may be
-000062f0: 2069 6d70 6169 7265 6420 6475 6520 746f   impaired due to
-00006300: 2074 6865 6972 2063 6172 696e 6720 7265   their caring re
-00006310: 7370 6f6e 7369 6269 6c69 7469 6573 3c2f  sponsibilities</
-00006320: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00006330: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
-00006340: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
-00006350: 6e3e 0a20 2020 2020 203c 7873 3a65 6e75  n>.      <xs:enu
-00006360: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-00006370: 3842 223e 3c78 733a 616e 6e6f 7461 7469  8B"><xs:annotati
-00006380: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
-00006390: 7469 6f6e 3e50 7269 7661 7465 6c79 2066  tion>Privately f
-000063a0: 6f73 7465 7265 643a 2063 6f6e 6365 726e  ostered: concern
-000063b0: 7320 7468 6174 2073 6572 7669 6365 7320  s that services 
-000063c0: 6d61 7920 6265 2072 6571 7569 7265 6420  may be required 
-000063d0: 6f72 2074 6865 2063 6869 6c64 206d 6179  or the child may
-000063e0: 2062 6520 6174 2072 6973 6b20 6173 2061   be at risk as a
-000063f0: 2070 7269 7661 7465 6c79 2066 6f73 7465   privately foste
-00006400: 7265 6420 6368 696c 6420 2d20 6f76 6572  red child - over
-00006410: 7365 6173 2063 6869 6c64 7265 6e20 7768  seas children wh
-00006420: 6f20 696e 7465 6e64 2074 6f20 7265 7475  o intend to retu
-00006430: 726e 3c2f 7873 3a64 6f63 756d 656e 7461  rn</xs:documenta
-00006440: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
-00006450: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
-00006460: 6174 696f 6e3e 0a20 2020 2020 203c 7873  ation>.      <xs
-00006470: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
-00006480: 7565 3d22 3843 223e 3c78 733a 616e 6e6f  ue="8C"><xs:anno
-00006490: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
-000064a0: 656e 7461 7469 6f6e 3e50 7269 7661 7465  entation>Private
-000064b0: 6c79 2066 6f73 7465 7265 643a 2063 6f6e  ly fostered: con
-000064c0: 6365 726e 7320 7468 6174 2073 6572 7669  cerns that servi
-000064d0: 6365 7320 6d61 7920 6265 2072 6571 7569  ces may be requi
-000064e0: 7265 6420 6f72 2074 6865 2063 6869 6c64  red or the child
-000064f0: 206d 6179 2062 6520 6174 2072 6973 6b20   may be at risk 
-00006500: 6173 2061 2070 7269 7661 7465 6c79 2066  as a privately f
-00006510: 6f73 7465 7265 6420 6368 696c 6420 2d20  ostered child - 
-00006520: 6f76 6572 7365 6173 2063 6869 6c64 7265  overseas childre
-00006530: 6e20 7768 6f20 696e 7465 6e64 2074 6f20  n who intend to 
-00006540: 7374 6179 3c2f 7873 3a64 6f63 756d 656e  stay</xs:documen
-00006550: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
-00006560: 7461 7469 6f6e 3e3c 2f78 733a 656e 756d  tation></xs:enum
-00006570: 6572 6174 696f 6e3e 0a20 2020 2020 203c  eration>.      <
-00006580: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
-00006590: 616c 7565 3d22 3844 223e 3c78 733a 616e  alue="8D"><xs:an
-000065a0: 6e6f 7461 7469 6f6e 3e3c 7873 3a64 6f63  notation><xs:doc
-000065b0: 756d 656e 7461 7469 6f6e 3e50 7269 7661  umentation>Priva
-000065c0: 7465 6c79 2066 6f73 7465 7265 643a 2063  tely fostered: c
-000065d0: 6f6e 6365 726e 7320 7468 6174 2073 6572  oncerns that ser
-000065e0: 7669 6365 7320 6d61 7920 6265 2072 6571  vices may be req
-000065f0: 7569 7265 6420 6f72 2074 6865 2063 6869  uired or the chi
-00006600: 6c64 206d 6179 2062 6520 6174 2072 6973  ld may be at ris
-00006610: 6b20 6173 2061 2070 7269 7661 7465 6c79  k as a privately
-00006620: 2066 6f73 7465 7265 6420 6368 696c 6420   fostered child 
-00006630: 2d20 554b 2063 6869 6c64 7265 6e20 696e  - UK children in
-00006640: 2065 6475 6361 7469 6f6e 616c 2070 6c61   educational pla
-00006650: 6365 6d65 6e74 733c 2f78 733a 646f 6375  cements</xs:docu
-00006660: 6d65 6e74 6174 696f 6e3e 3c2f 7873 3a61  mentation></xs:a
-00006670: 6e6e 6f74 6174 696f 6e3e 3c2f 7873 3a65  nnotation></xs:e
-00006680: 6e75 6d65 7261 7469 6f6e 3e0a 2020 2020  numeration>.    
-00006690: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
-000066a0: 6e20 7661 6c75 653d 2238 4522 3e3c 7873  n value="8E"><xs
-000066b0: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
-000066c0: 646f 6375 6d65 6e74 6174 696f 6e3e 5072  documentation>Pr
-000066d0: 6976 6174 656c 7920 666f 7374 6572 6564  ivately fostered
-000066e0: 3a20 636f 6e63 6572 6e73 2074 6861 7420  : concerns that 
-000066f0: 7365 7276 6963 6573 206d 6179 2062 6520  services may be 
-00006700: 7265 7175 6972 6564 206f 7220 7468 6520  required or the 
-00006710: 6368 696c 6420 6d61 7920 6265 2061 7420  child may be at 
-00006720: 7269 736b 2061 7320 6120 7072 6976 6174  risk as a privat
-00006730: 656c 7920 666f 7374 6572 6564 2063 6869  ely fostered chi
-00006740: 6c64 202d 2055 4b20 6368 696c 6472 656e  ld - UK children
-00006750: 206d 616b 696e 6720 616c 7465 726e 6174   making alternat
-00006760: 6976 6520 6661 6d69 6c79 2061 7272 616e  ive family arran
-00006770: 6765 6d65 6e74 733c 2f78 733a 646f 6375  gements</xs:docu
-00006780: 6d65 6e74 6174 696f 6e3e 3c2f 7873 3a61  mentation></xs:a
-00006790: 6e6e 6f74 6174 696f 6e3e 3c2f 7873 3a65  nnotation></xs:e
-000067a0: 6e75 6d65 7261 7469 6f6e 3e0a 2020 2020  numeration>.    
-000067b0: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
-000067c0: 6e20 7661 6c75 653d 2238 4622 3e3c 7873  n value="8F"><xs
-000067d0: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
-000067e0: 646f 6375 6d65 6e74 6174 696f 6e3e 5072  documentation>Pr
-000067f0: 6976 6174 656c 7920 666f 7374 6572 6564  ivately fostered
-00006800: 3a20 636f 6e63 6572 6e73 2074 6861 7420  : concerns that 
-00006810: 7365 7276 6963 6573 206d 6179 2062 6520  services may be 
-00006820: 7265 7175 6972 6564 206f 7220 7468 6520  required or the 
-00006830: 6368 696c 6420 6d61 7920 6265 2061 7420  child may be at 
-00006840: 7269 736b 2061 7320 6120 7072 6976 6174  risk as a privat
-00006850: 656c 7920 666f 7374 6572 6564 2063 6869  ely fostered chi
-00006860: 6c64 202d 206f 7468 6572 3c2f 7873 3a64  ld - other</xs:d
-00006870: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
-00006880: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
-00006890: 733a 656e 756d 6572 6174 696f 6e3e 0a20  s:enumeration>. 
-000068a0: 2020 2020 203c 7873 3a65 6e75 6d65 7261       <xs:enumera
-000068b0: 7469 6f6e 2076 616c 7565 3d22 3941 223e  tion value="9A">
-000068c0: 3c78 733a 616e 6e6f 7461 7469 6f6e 3e3c  <xs:annotation><
-000068d0: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-000068e0: 3e55 4153 433a 2063 6f6e 6365 726e 7320  >UASC: concerns 
-000068f0: 7468 6174 2073 6572 7669 6365 7320 6d61  that services ma
-00006900: 7920 6265 2072 6571 7569 7265 6420 6f72  y be required or
-00006910: 2074 6865 2063 6869 6c64 206d 6179 2062   the child may b
-00006920: 6520 6174 2072 6973 6b20 6f66 2068 6172  e at risk of har
-00006930: 6d20 6173 2061 6e20 756e 6163 636f 6d70  m as an unaccomp
-00006940: 616e 6965 6420 6173 796c 756d 2d73 6565  anied asylum-see
-00006950: 6b69 6e67 2063 6869 6c64 3c2f 7873 3a64  king child</xs:d
-00006960: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
-00006970: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
-00006980: 733a 656e 756d 6572 6174 696f 6e3e 0a20  s:enumeration>. 
-00006990: 2020 2020 203c 7873 3a65 6e75 6d65 7261       <xs:enumera
-000069a0: 7469 6f6e 2076 616c 7565 3d22 3130 4122  tion value="10A"
-000069b0: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
-000069c0: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
-000069d0: 6e3e 4d69 7373 696e 673a 2063 6f6e 6365  n>Missing: conce
-000069e0: 726e 7320 7468 6174 2073 6572 7669 6365  rns that service
-000069f0: 7320 6d61 7920 6265 2072 6571 7569 7265  s may be require
-00006a00: 6420 6f72 2074 6865 2063 6869 6c64 206d  d or the child m
-00006a10: 6179 2062 6520 6174 2072 6973 6b20 6f66  ay be at risk of
-00006a20: 2068 6172 6d20 6475 6520 746f 2067 6f69   harm due to goi
-00006a30: 6e67 2f62 6569 6e67 206d 6973 7369 6e67  ng/being missing
-00006a40: 3c2f 7873 3a64 6f63 756d 656e 7461 7469  </xs:documentati
-00006a50: 6f6e 3e3c 2f78 733a 616e 6e6f 7461 7469  on></xs:annotati
-00006a60: 6f6e 3e3c 2f78 733a 656e 756d 6572 6174  on></xs:enumerat
-00006a70: 696f 6e3e 0a20 2020 2020 203c 7873 3a65  ion>.      <xs:e
-00006a80: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
-00006a90: 3d22 3131 4122 3e3c 7873 3a61 6e6e 6f74  ="11A"><xs:annot
-00006aa0: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
-00006ab0: 6e74 6174 696f 6e3e 4368 696c 6420 7365  ntation>Child se
-00006ac0: 7875 616c 2065 7870 6c6f 6974 6174 696f  xual exploitatio
-00006ad0: 6e3a 2063 6f6e 6365 726e 7320 7468 6174  n: concerns that
-00006ae0: 2073 6572 7669 6365 7320 6d61 7920 6265   services may be
-00006af0: 2072 6571 7569 7265 6420 6f72 2074 6865   required or the
-00006b00: 2063 6869 6c64 206d 6179 2062 6520 6174   child may be at
-00006b10: 2072 6973 6b20 6f66 2068 6172 6d20 6475   risk of harm du
-00006b20: 6520 746f 2063 6869 6c64 2073 6578 7561  e to child sexua
-00006b30: 6c20 6578 706c 6f69 7461 7469 6f6e 3c2f  l exploitation</
-00006b40: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00006b50: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
-00006b60: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
-00006b70: 6e3e 0a20 2020 2020 203c 7873 3a65 6e75  n>.      <xs:enu
-00006b80: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-00006b90: 3132 4122 3e3c 7873 3a61 6e6e 6f74 6174  12A"><xs:annotat
-00006ba0: 696f 6e3e 3c78 733a 646f 6375 6d65 6e74  ion><xs:document
-00006bb0: 6174 696f 6e3e 5472 6166 6669 636b 696e  ation>Traffickin
-00006bc0: 673a 2063 6f6e 6365 726e 7320 7468 6174  g: concerns that
-00006bd0: 2073 6572 7669 6365 7320 6d61 7920 6265   services may be
-00006be0: 2072 6571 7569 7265 6420 6f72 2074 6865   required or the
-00006bf0: 2063 6869 6c64 206d 6179 2062 6520 6174   child may be at
-00006c00: 2072 6973 6b20 6f66 2068 6172 6d20 6475   risk of harm du
-00006c10: 6520 746f 2074 7261 6666 6963 6b69 6e67  e to trafficking
-00006c20: 3c2f 7873 3a64 6f63 756d 656e 7461 7469  </xs:documentati
-00006c30: 6f6e 3e3c 2f78 733a 616e 6e6f 7461 7469  on></xs:annotati
-00006c40: 6f6e 3e3c 2f78 733a 656e 756d 6572 6174  on></xs:enumerat
-00006c50: 696f 6e3e 0a20 2020 2020 203c 7873 3a65  ion>.      <xs:e
-00006c60: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
-00006c70: 3d22 3133 4122 3e3c 7873 3a61 6e6e 6f74  ="13A"><xs:annot
-00006c80: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
-00006c90: 6e74 6174 696f 6e3e 4761 6e67 733a 2063  ntation>Gangs: c
-00006ca0: 6f6e 6365 726e 7320 7468 6174 2073 6572  oncerns that ser
-00006cb0: 7669 6365 7320 6d61 7920 6265 2072 6571  vices may be req
-00006cc0: 7569 7265 6420 6f72 2074 6865 2063 6869  uired or the chi
-00006cd0: 6c64 206d 6179 2062 6520 6174 2072 6973  ld may be at ris
-00006ce0: 6b20 6f66 2068 6172 6d20 6265 6361 7573  k of harm becaus
-00006cf0: 6520 6f66 2069 6e76 6f6c 7665 6d65 6e74  e of involvement
-00006d00: 2069 6e2f 7769 7468 2067 616e 6773 3c2f   in/with gangs</
-00006d10: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-00006d20: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
-00006d30: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
-00006d40: 6e3e 0a20 2020 2020 203c 7873 3a65 6e75  n>.      <xs:enu
-00006d50: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-00006d60: 3134 4122 3e3c 7873 3a61 6e6e 6f74 6174  14A"><xs:annotat
-00006d70: 696f 6e3e 3c78 733a 646f 6375 6d65 6e74  ion><xs:document
-00006d80: 6174 696f 6e3e 536f 6369 616c 6c79 2075  ation>Socially u
-00006d90: 6e61 6363 6570 7461 626c 6520 6265 6861  nacceptable beha
-00006da0: 7669 6f75 723a 2063 6f6e 6365 726e 7320  viour: concerns 
-00006db0: 7468 6174 2073 6572 7669 6365 7320 6d61  that services ma
-00006dc0: 7920 6265 2072 6571 7569 7265 6420 6f72  y be required or
-00006dd0: 2074 6865 2063 6869 6c64 206d 6179 2062   the child may b
-00006de0: 6520 6174 2072 6973 6b20 6475 6520 746f  e at risk due to
-00006df0: 2074 6865 6972 2073 6f63 6961 6c6c 7920   their socially 
-00006e00: 756e 6163 6365 7074 6162 6c65 2062 6568  unacceptable beh
-00006e10: 6176 696f 7572 3c2f 7873 3a64 6f63 756d  aviour</xs:docum
-00006e20: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
-00006e30: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
-00006e40: 756d 6572 6174 696f 6e3e 0a20 2020 2020  umeration>.     
-00006e50: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
-00006e60: 2076 616c 7565 3d22 3135 4122 3e3c 7873   value="15A"><xs
-00006e70: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
-00006e80: 646f 6375 6d65 6e74 6174 696f 6e3e 5365  documentation>Se
-00006e90: 6c66 2d68 6172 6d3a 2063 6f6e 6365 726e  lf-harm: concern
-00006ea0: 7320 7468 6174 2073 6572 7669 6365 7320  s that services 
-00006eb0: 6d61 7920 6265 2072 6571 7569 7265 6420  may be required 
-00006ec0: 6f72 2064 7565 2074 6f20 7375 7370 6563  or due to suspec
-00006ed0: 7465 642f 6163 7475 616c 2073 656c 662d  ted/actual self-
-00006ee0: 6861 726d 696e 6720 6368 696c 6420 6d61  harming child ma
-00006ef0: 7920 6265 2061 7420 7269 736b 206f 6620  y be at risk of 
-00006f00: 6861 726d 3c2f 7873 3a64 6f63 756d 656e  harm</xs:documen
-00006f10: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
-00006f20: 7461 7469 6f6e 3e3c 2f78 733a 656e 756d  tation></xs:enum
-00006f30: 6572 6174 696f 6e3e 0a20 2020 2020 203c  eration>.      <
-00006f40: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
-00006f50: 616c 7565 3d22 3136 4122 3e3c 7873 3a61  alue="16A"><xs:a
-00006f60: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
-00006f70: 6375 6d65 6e74 6174 696f 6e3e 4162 7573  cumentation>Abus
-00006f80: 6520 6f72 206e 6567 6c65 6374 20e2 8093  e or neglect ...
-00006f90: 20e2 8098 4e45 474c 4543 54e2 8099 3a20   ...NEGLECT...: 
-00006fa0: 636f 6e63 6572 6e73 2074 6861 7420 7365  concerns that se
-00006fb0: 7276 6963 6573 206d 6179 2062 6520 7265  rvices may be re
-00006fc0: 7175 6972 6564 206f 7220 7468 6520 6368  quired or the ch
-00006fd0: 696c 6420 6d61 7920 6265 2073 7566 6665  ild may be suffe
-00006fe0: 7269 6e67 206f 7220 6c69 6b65 6c79 2074  ring or likely t
-00006ff0: 6f20 7375 6666 6572 2073 6967 6e69 6669  o suffer signifi
-00007000: 6361 6e74 2068 6172 6d20 6475 6520 746f  cant harm due to
-00007010: 2061 6275 7365 206f 7220 6e65 676c 6563   abuse or neglec
-00007020: 743c 2f78 733a 646f 6375 6d65 6e74 6174  t</xs:documentat
-00007030: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
-00007040: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
-00007050: 7469 6f6e 3e0a 2020 2020 2020 3c78 733a  tion>.      <xs:
-00007060: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
-00007070: 653d 2231 3741 223e 3c78 733a 616e 6e6f  e="17A"><xs:anno
-00007080: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
-00007090: 656e 7461 7469 6f6e 3e41 6275 7365 206f  entation>Abuse o
-000070a0: 7220 6e65 676c 6563 7420 e280 9320 e280  r neglect ... ..
-000070b0: 9845 4d4f 5449 4f4e 414c 2041 4255 5345  .EMOTIONAL ABUSE
-000070c0: e280 993a 2063 6f6e 6365 726e 7320 7468  ...: concerns th
-000070d0: 6174 2073 6572 7669 6365 7320 6d61 7920  at services may 
-000070e0: 6265 2072 6571 7569 7265 6420 6f72 2074  be required or t
-000070f0: 6865 2063 6869 6c64 206d 6179 2062 6520  he child may be 
-00007100: 7375 6666 6572 696e 6720 6f72 206c 696b  suffering or lik
-00007110: 656c 7920 746f 2073 7566 6665 7220 7369  ely to suffer si
-00007120: 676e 6966 6963 616e 7420 6861 726d 2064  gnificant harm d
-00007130: 7565 2074 6f20 6162 7573 6520 6f72 206e  ue to abuse or n
-00007140: 6567 6c65 6374 3c2f 7873 3a64 6f63 756d  eglect</xs:docum
-00007150: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
-00007160: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
-00007170: 756d 6572 6174 696f 6e3e 0a20 2020 2020  umeration>.     
-00007180: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
-00007190: 2076 616c 7565 3d22 3138 4222 3e3c 7873   value="18B"><xs
-000071a0: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
-000071b0: 646f 6375 6d65 6e74 6174 696f 6e3e 4162  documentation>Ab
-000071c0: 7573 6520 6f72 206e 6567 6c65 6374 20e2  use or neglect .
-000071d0: 8093 20e2 8098 5048 5953 4943 414c 2041  .. ...PHYSICAL A
-000071e0: 4255 5345 e280 9920 2863 6869 6c64 206f  BUSE... (child o
-000071f0: 6e20 6368 696c 6429 3a20 636f 6e63 6572  n child): concer
-00007200: 6e73 2074 6861 7420 7365 7276 6963 6573  ns that services
-00007210: 206d 6179 2062 6520 7265 7175 6972 6564   may be required
-00007220: 206f 7220 7468 6520 6368 696c 6420 6d61   or the child ma
-00007230: 7920 6265 2073 7566 6665 7269 6e67 206f  y be suffering o
-00007240: 7220 6c69 6b65 6c79 2074 6f20 7375 6666  r likely to suff
-00007250: 6572 2073 6967 6e69 6669 6361 6e74 2068  er significant h
-00007260: 6172 6d20 6475 6520 746f 2061 6275 7365  arm due to abuse
-00007270: 206f 7220 6e65 676c 6563 7420 6279 2061   or neglect by a
-00007280: 6e6f 7468 6572 2063 6869 6c64 3c2f 7873  nother child</xs
-00007290: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
-000072a0: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
-000072b0: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
-000072c0: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
-000072d0: 7261 7469 6f6e 2076 616c 7565 3d22 3138  ration value="18
-000072e0: 4322 3e3c 7873 3a61 6e6e 6f74 6174 696f  C"><xs:annotatio
-000072f0: 6e3e 3c78 733a 646f 6375 6d65 6e74 6174  n><xs:documentat
-00007300: 696f 6e3e 4162 7573 6520 6f72 206e 6567  ion>Abuse or neg
-00007310: 6c65 6374 20e2 8093 20e2 8098 5048 5953  lect ... ...PHYS
-00007320: 4943 414c 2041 4255 5345 e280 9920 2861  ICAL ABUSE... (a
-00007330: 6475 6c74 206f 6e20 6368 696c 6429 3a20  dult on child): 
-00007340: 636f 6e63 6572 6e73 2074 6861 7420 7365  concerns that se
-00007350: 7276 6963 6573 206d 6179 2062 6520 7265  rvices may be re
-00007360: 7175 6972 6564 206f 7220 7468 6520 6368  quired or the ch
-00007370: 696c 6420 6d61 7920 6265 2073 7566 6665  ild may be suffe
-00007380: 7269 6e67 206f 7220 6c69 6b65 6c79 2074  ring or likely t
-00007390: 6f20 7375 6666 6572 2073 6967 6e69 6669  o suffer signifi
-000073a0: 6361 6e74 2068 6172 6d20 6475 6520 746f  cant harm due to
-000073b0: 2061 6275 7365 206f 7220 6e65 676c 6563   abuse or neglec
-000073c0: 7420 6279 2061 6e20 6164 756c 743c 2f78  t by an adult</x
-000073d0: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
-000073e0: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
-000073f0: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
-00007400: 3e0a 2020 2020 2020 3c78 733a 656e 756d  >.      <xs:enum
-00007410: 6572 6174 696f 6e20 7661 6c75 653d 2231  eration value="1
-00007420: 3942 223e 3c78 733a 616e 6e6f 7461 7469  9B"><xs:annotati
-00007430: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
-00007440: 7469 6f6e 3e41 6275 7365 206f 7220 6e65  tion>Abuse or ne
-00007450: 676c 6563 7420 e280 9320 e280 9853 4558  glect ... ...SEX
-00007460: 5541 4c20 4142 5553 45e2 8099 2028 6368  UAL ABUSE... (ch
-00007470: 696c 6420 6f6e 2063 6869 6c64 293a 2063  ild on child): c
-00007480: 6f6e 6365 726e 7320 7468 6174 2073 6572  oncerns that ser
-00007490: 7669 6365 7320 6d61 7920 6265 2072 6571  vices may be req
-000074a0: 7569 7265 6420 6f72 2074 6865 2063 6869  uired or the chi
-000074b0: 6c64 206d 6179 2062 6520 7375 6666 6572  ld may be suffer
-000074c0: 696e 6720 6f72 206c 696b 656c 7920 746f  ing or likely to
-000074d0: 2073 7566 6665 7220 7369 676e 6966 6963   suffer signific
-000074e0: 616e 7420 6861 726d 2064 7565 2074 6f20  ant harm due to 
-000074f0: 6162 7573 6520 6f72 206e 6567 6c65 6374  abuse or neglect
-00007500: 2062 7920 616e 6f74 6865 7220 6368 696c   by another chil
-00007510: 643c 2f78 733a 646f 6375 6d65 6e74 6174  d</xs:documentat
-00007520: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
-00007530: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
-00007540: 7469 6f6e 3e0a 2020 2020 2020 3c78 733a  tion>.      <xs:
-00007550: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
-00007560: 653d 2231 3943 223e 3c78 733a 616e 6e6f  e="19C"><xs:anno
-00007570: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
-00007580: 656e 7461 7469 6f6e 3e41 6275 7365 206f  entation>Abuse o
-00007590: 7220 6e65 676c 6563 7420 e280 9320 e280  r neglect ... ..
-000075a0: 9853 4558 5541 4c20 4142 5553 45e2 8099  .SEXUAL ABUSE...
-000075b0: 2028 6164 756c 7420 6f6e 2063 6869 6c64   (adult on child
-000075c0: 293a 2063 6f6e 6365 726e 7320 7468 6174  ): concerns that
-000075d0: 2073 6572 7669 6365 7320 6d61 7920 6265   services may be
-000075e0: 2072 6571 7569 7265 6420 6f72 2074 6865   required or the
-000075f0: 2063 6869 6c64 206d 6179 2062 6520 7375   child may be su
-00007600: 6666 6572 696e 6720 6f72 206c 696b 656c  ffering or likel
-00007610: 7920 746f 2073 7566 6665 7220 7369 676e  y to suffer sign
-00007620: 6966 6963 616e 7420 6861 726d 2064 7565  ificant harm due
-00007630: 2074 6f20 6162 7573 6520 6f72 206e 6567   to abuse or neg
-00007640: 6c65 6374 2062 7920 616e 2061 6475 6c74  lect by an adult
-00007650: 3c2f 7873 3a64 6f63 756d 656e 7461 7469  </xs:documentati
-00007660: 6f6e 3e3c 2f78 733a 616e 6e6f 7461 7469  on></xs:annotati
-00007670: 6f6e 3e3c 2f78 733a 656e 756d 6572 6174  on></xs:enumerat
-00007680: 696f 6e3e 0a20 2020 2020 203c 7873 3a65  ion>.      <xs:e
-00007690: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
-000076a0: 3d22 3230 223e 3c78 733a 616e 6e6f 7461  ="20"><xs:annota
-000076b0: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
-000076c0: 7461 7469 6f6e 3e4f 7468 6572 3c2f 7873  tation>Other</xs
-000076d0: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
-000076e0: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
-000076f0: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
-00007700: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
-00007710: 7261 7469 6f6e 2076 616c 7565 3d22 3231  ration value="21
-00007720: 223e 3c78 733a 616e 6e6f 7461 7469 6f6e  "><xs:annotation
-00007730: 3e3c 7873 3a64 6f63 756d 656e 7461 7469  ><xs:documentati
-00007740: 6f6e 3e4e 6f20 6661 6374 6f72 7320 6964  on>No factors id
-00007750: 656e 7469 6669 6564 202d 206f 6e6c 7920  entified - only 
-00007760: 7573 6520 7468 6973 2069 6620 7468 6572  use this if ther
-00007770: 6520 6973 206e 6f20 6576 6964 656e 6365  e is no evidence
-00007780: 206f 6620 616e 7920 6f66 2074 6865 2066   of any of the f
-00007790: 6163 746f 7273 2061 626f 7665 2061 6e64  actors above and
-000077a0: 206e 6f20 6675 7274 6865 7220 6163 7469   no further acti
-000077b0: 6f6e 2069 7320 6265 696e 6720 7461 6b65  on is being take
-000077c0: 6e3c 2f78 733a 646f 6375 6d65 6e74 6174  n</xs:documentat
-000077d0: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
-000077e0: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
-000077f0: 7469 6f6e 3e0a 2020 2020 2020 3c78 733a  tion>.      <xs:
-00007800: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
-00007810: 653d 2232 3241 223e 3c78 733a 616e 6e6f  e="22A"><xs:anno
-00007820: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
-00007830: 656e 7461 7469 6f6e 3e46 656d 616c 6520  entation>Female 
-00007840: 6765 6e69 7461 6c20 6d75 7469 6c61 7469  genital mutilati
-00007850: 6f6e 2028 4647 4d29 202d 2063 6f6e 6365  on (FGM) - conce
-00007860: 726e 7320 7468 6174 2073 6572 7669 6365  rns that service
-00007870: 7320 6d61 7920 6265 2072 6571 7569 7265  s may be require
-00007880: 6420 6f72 2074 6865 2063 6869 6c64 206d  d or the child m
-00007890: 6179 2062 6520 6174 2072 6973 6b20 6475  ay be at risk du
-000078a0: 6520 746f 2066 656d 616c 6520 6765 6e69  e to female geni
-000078b0: 7461 6c20 6d75 7469 6c61 7469 6f6e 3c2f  tal mutilation</
-000078c0: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
-000078d0: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
-000078e0: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
-000078f0: 6e3e 0a20 2020 2020 203c 7873 3a65 6e75  n>.      <xs:enu
-00007900: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
-00007910: 3233 4122 3e3c 7873 3a61 6e6e 6f74 6174  23A"><xs:annotat
-00007920: 696f 6e3e 3c78 733a 646f 6375 6d65 6e74  ion><xs:document
-00007930: 6174 696f 6e3e 4162 7573 6520 6c69 6e6b  ation>Abuse link
-00007940: 6564 2074 6f20 6661 6974 6820 6f72 2062  ed to faith or b
-00007950: 656c 6965 6620 2d20 636f 6e63 6572 6e73  elief - concerns
-00007960: 2074 6861 7420 7365 7276 6963 6573 206d   that services m
-00007970: 6179 2062 6520 7265 7175 6972 6564 206f  ay be required o
-00007980: 7220 7468 6520 6368 696c 6420 6d61 7920  r the child may 
-00007990: 6265 2061 7420 7269 736b 2064 7565 2074  be at risk due t
-000079a0: 6f20 6162 7573 6520 6c69 6e6b 6564 2074  o abuse linked t
-000079b0: 6f20 6661 6974 6820 6f72 2062 656c 6965  o faith or belie
-000079c0: 663c 2f78 733a 646f 6375 6d65 6e74 6174  f</xs:documentat
-000079d0: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
-000079e0: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
-000079f0: 7469 6f6e 3e0a 2020 2020 2020 3c78 733a  tion>.      <xs:
-00007a00: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
-00007a10: 653d 2232 3441 223e 3c78 733a 616e 6e6f  e="24A"><xs:anno
-00007a20: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
-00007a30: 656e 7461 7469 6f6e 3e43 6869 6c64 2063  entation>Child c
-00007a40: 7269 6d69 6e61 6c20 6578 706c 6f69 7461  riminal exploita
-00007a50: 7469 6f6e 3a20 636f 6e63 6572 6e73 2074  tion: concerns t
-00007a60: 6861 7420 7365 7276 6963 6573 206d 6179  hat services may
-00007a70: 2062 6520 7265 7175 6972 6564 206f 7220   be required or 
-00007a80: 7468 6520 6368 696c 6420 6d61 7920 6265  the child may be
-00007a90: 2061 7420 7269 736b 206f 6620 6861 726d   at risk of harm
-00007aa0: 2064 7565 2074 6f20 6368 696c 6420 6372   due to child cr
-00007ab0: 696d 696e 616c 2065 7870 6c6f 6974 6174  iminal exploitat
-00007ac0: 696f 6e3c 2f78 733a 646f 6375 6d65 6e74  ion</xs:document
-00007ad0: 6174 696f 6e3e 3c2f 7873 3a61 6e6e 6f74  ation></xs:annot
-00007ae0: 6174 696f 6e3e 3c2f 7873 3a65 6e75 6d65  ation></xs:enume
-00007af0: 7261 7469 6f6e 3e0a 2020 2020 3c2f 7873  ration>.    </xs
-00007b00: 3a72 6573 7472 6963 7469 6f6e 3e0a 2020  :restriction>.  
-00007b10: 3c2f 7873 3a73 696d 706c 6554 7970 653e  </xs:simpleType>
-00007b20: 0a0a 3c2f 7873 3a73 6368 656d 613e       ..</xs:schema>
+00003570: 7461 7469 6f6e 3e56 6973 696f 6e3c 2f78  tation>Vision</x
+00003580: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00003590: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
+000035a0: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
+000035b0: 3e0d 0a20 2020 2020 203c 7873 3a65 6e75  >..      <xs:enu
+000035c0: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
+000035d0: 4245 4822 3e3c 7873 3a61 6e6e 6f74 6174  BEH"><xs:annotat
+000035e0: 696f 6e3e 3c78 733a 646f 6375 6d65 6e74  ion><xs:document
+000035f0: 6174 696f 6e3e 4265 6861 7669 6f75 723c  ation>Behaviour<
+00003600: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
+00003610: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
+00003620: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
+00003630: 6f6e 3e0d 0a20 2020 2020 203c 7873 3a65  on>..      <xs:e
+00003640: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+00003650: 3d22 434f 4e22 3e3c 7873 3a61 6e6e 6f74  ="CON"><xs:annot
+00003660: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
+00003670: 6e74 6174 696f 6e3e 436f 6e73 6369 6f75  ntation>Consciou
+00003680: 736e 6573 733c 2f78 733a 646f 6375 6d65  sness</xs:docume
+00003690: 6e74 6174 696f 6e3e 3c2f 7873 3a61 6e6e  ntation></xs:ann
+000036a0: 6f74 6174 696f 6e3e 3c2f 7873 3a65 6e75  otation></xs:enu
+000036b0: 6d65 7261 7469 6f6e 3e0d 0a20 2020 2020  meration>..     
+000036c0: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
+000036d0: 2076 616c 7565 3d22 4155 5422 3e3c 7873   value="AUT"><xs
+000036e0: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
+000036f0: 646f 6375 6d65 6e74 6174 696f 6e3e 4175  documentation>Au
+00003700: 7469 736d 3c2f 7873 3a64 6f63 756d 656e  tism</xs:documen
+00003710: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
+00003720: 7461 7469 6f6e 3e3c 2f78 733a 656e 756d  tation></xs:enum
+00003730: 6572 6174 696f 6e3e 0d0a 2020 2020 2020  eration>..      
+00003740: 3c78 733a 656e 756d 6572 6174 696f 6e20  <xs:enumeration 
+00003750: 7661 6c75 653d 2244 4441 223e 3c78 733a  value="DDA"><xs:
+00003760: 616e 6e6f 7461 7469 6f6e 3e3c 7873 3a64  annotation><xs:d
+00003770: 6f63 756d 656e 7461 7469 6f6e 3e4f 7468  ocumentation>Oth
+00003780: 6572 3c2f 7873 3a64 6f63 756d 656e 7461  er</xs:documenta
+00003790: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
+000037a0: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
+000037b0: 6174 696f 6e3e 0d0a 2020 2020 3c2f 7873  ation>..    </xs
+000037c0: 3a72 6573 7472 6963 7469 6f6e 3e0d 0a20  :restriction>.. 
+000037d0: 203c 2f78 733a 7369 6d70 6c65 5479 7065   </xs:simpleType
+000037e0: 3e0d 0a0d 0a20 203c 7873 3a73 696d 706c  >....  <xs:simpl
+000037f0: 6554 7970 6520 6e61 6d65 3d22 7265 6665  eType name="refe
+00003800: 7272 616c 736f 7572 6365 7479 7065 223e  rralsourcetype">
+00003810: 0d0a 2020 2020 3c78 733a 7265 7374 7269  ..    <xs:restri
+00003820: 6374 696f 6e20 6261 7365 3d22 6e6f 6e45  ction base="nonE
+00003830: 6d70 7479 5374 7269 6e67 223e 0d0a 2020  mptyString">..  
+00003840: 2020 2020 3c78 733a 656e 756d 6572 6174      <xs:enumerat
+00003850: 696f 6e20 7661 6c75 653d 2231 4122 3e3c  ion value="1A"><
+00003860: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
+00003870: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00003880: 494e 4449 5649 4455 414c 20e2 8093 2066  INDIVIDUAL ... f
+00003890: 616d 696c 7920 6d65 6d62 6572 2c20 7265  amily member, re
+000038a0: 6c61 7469 7665 206f 7220 6361 7265 723c  lative or carer<
+000038b0: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
+000038c0: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
+000038d0: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
+000038e0: 6f6e 3e0d 0a20 2020 2020 203c 7873 3a65  on>..      <xs:e
+000038f0: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+00003900: 3d22 3142 223e 3c78 733a 616e 6e6f 7461  ="1B"><xs:annota
+00003910: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
+00003920: 7461 7469 6f6e 3e49 4e44 4956 4944 5541  tation>INDIVIDUA
+00003930: 4c20 e280 9320 6163 7175 6169 6e74 616e  L ... acquaintan
+00003940: 6365 2028 696e 636c 7564 696e 6720 6e65  ce (including ne
+00003950: 6967 6862 6f75 7273 2061 6e64 2063 6869  ighbours and chi
+00003960: 6c64 206d 696e 6465 7273 293c 2f78 733a  ld minders)</xs:
+00003970: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
+00003980: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
+00003990: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0d  xs:enumeration>.
+000039a0: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
+000039b0: 7261 7469 6f6e 2076 616c 7565 3d22 3143  ration value="1C
+000039c0: 223e 3c78 733a 616e 6e6f 7461 7469 6f6e  "><xs:annotation
+000039d0: 3e3c 7873 3a64 6f63 756d 656e 7461 7469  ><xs:documentati
+000039e0: 6f6e 3e49 4e44 4956 4944 5541 4c20 e280  on>INDIVIDUAL ..
+000039f0: 9320 7365 6c66 3c2f 7873 3a64 6f63 756d  . self</xs:docum
+00003a00: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
+00003a10: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
+00003a20: 756d 6572 6174 696f 6e3e 0d0a 2020 2020  umeration>..    
+00003a30: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
+00003a40: 6e20 7661 6c75 653d 2231 4422 3e3c 7873  n value="1D"><xs
+00003a50: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
+00003a60: 646f 6375 6d65 6e74 6174 696f 6e3e 494e  documentation>IN
+00003a70: 4449 5649 4455 414c 20e2 8093 206f 7468  DIVIDUAL ... oth
+00003a80: 6572 2028 696e 636c 7564 696e 6720 7374  er (including st
+00003a90: 7261 6e67 6572 7329 3c2f 7873 3a64 6f63  rangers)</xs:doc
+00003aa0: 756d 656e 7461 7469 6f6e 3e3c 2f78 733a  umentation></xs:
+00003ab0: 616e 6e6f 7461 7469 6f6e 3e3c 2f78 733a  annotation></xs:
+00003ac0: 656e 756d 6572 6174 696f 6e3e 0d0a 2020  enumeration>..  
+00003ad0: 2020 2020 3c78 733a 656e 756d 6572 6174      <xs:enumerat
+00003ae0: 696f 6e20 7661 6c75 653d 2232 4122 3e3c  ion value="2A"><
+00003af0: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
+00003b00: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00003b10: 5343 484f 4f4c 533c 2f78 733a 646f 6375  SCHOOLS</xs:docu
+00003b20: 6d65 6e74 6174 696f 6e3e 3c2f 7873 3a61  mentation></xs:a
+00003b30: 6e6e 6f74 6174 696f 6e3e 3c2f 7873 3a65  nnotation></xs:e
+00003b40: 6e75 6d65 7261 7469 6f6e 3e0d 0a20 2020  numeration>..   
+00003b50: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
+00003b60: 6f6e 2076 616c 7565 3d22 3242 223e 3c78  on value="2B"><x
+00003b70: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
+00003b80: 3a64 6f63 756d 656e 7461 7469 6f6e 3e45  :documentation>E
+00003b90: 4455 4341 5449 4f4e 2053 4552 5649 4345  DUCATION SERVICE
+00003ba0: 533c 2f78 733a 646f 6375 6d65 6e74 6174  S</xs:documentat
+00003bb0: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
+00003bc0: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
+00003bd0: 7469 6f6e 3e0d 0a20 2020 2020 203c 7873  tion>..      <xs
+00003be0: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
+00003bf0: 7565 3d22 3341 223e 3c78 733a 616e 6e6f  ue="3A"><xs:anno
+00003c00: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
+00003c10: 656e 7461 7469 6f6e 3e48 4541 4c54 4820  entation>HEALTH 
+00003c20: 5345 5256 4943 4553 20e2 8093 2067 656e  SERVICES ... gen
+00003c30: 6572 616c 2070 7261 6374 6974 696f 6e65  eral practitione
+00003c40: 7220 2847 5029 3c2f 7873 3a64 6f63 756d  r (GP)</xs:docum
+00003c50: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
+00003c60: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
+00003c70: 756d 6572 6174 696f 6e3e 0d0a 2020 2020  umeration>..    
+00003c80: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
+00003c90: 6e20 7661 6c75 653d 2233 4222 3e3c 7873  n value="3B"><xs
+00003ca0: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
+00003cb0: 646f 6375 6d65 6e74 6174 696f 6e3e 4845  documentation>HE
+00003cc0: 414c 5448 2053 4552 5649 4345 5320 e280  ALTH SERVICES ..
+00003cd0: 9320 6865 616c 7468 2076 6973 6974 6f72  . health visitor
+00003ce0: 3c2f 7873 3a64 6f63 756d 656e 7461 7469  </xs:documentati
+00003cf0: 6f6e 3e3c 2f78 733a 616e 6e6f 7461 7469  on></xs:annotati
+00003d00: 6f6e 3e3c 2f78 733a 656e 756d 6572 6174  on></xs:enumerat
+00003d10: 696f 6e3e 0d0a 2020 2020 2020 3c78 733a  ion>..      <xs:
+00003d20: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
+00003d30: 653d 2233 4322 3e3c 7873 3a61 6e6e 6f74  e="3C"><xs:annot
+00003d40: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
+00003d50: 6e74 6174 696f 6e3e 4845 414c 5448 2053  ntation>HEALTH S
+00003d60: 4552 5649 4345 5320 e280 9320 7363 686f  ERVICES ... scho
+00003d70: 6f6c 206e 7572 7365 3c2f 7873 3a64 6f63  ol nurse</xs:doc
+00003d80: 756d 656e 7461 7469 6f6e 3e3c 2f78 733a  umentation></xs:
+00003d90: 616e 6e6f 7461 7469 6f6e 3e3c 2f78 733a  annotation></xs:
+00003da0: 656e 756d 6572 6174 696f 6e3e 0d0a 2020  enumeration>..  
+00003db0: 2020 2020 3c78 733a 656e 756d 6572 6174      <xs:enumerat
+00003dc0: 696f 6e20 7661 6c75 653d 2233 4422 3e3c  ion value="3D"><
+00003dd0: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
+00003de0: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00003df0: 4845 414c 5448 2053 4552 5649 4345 5320  HEALTH SERVICES 
+00003e00: e280 9320 6f74 6865 7220 7072 696d 6172  ... other primar
+00003e10: 7920 6865 616c 7468 2073 6572 7669 6365  y health service
+00003e20: 733c 2f78 733a 646f 6375 6d65 6e74 6174  s</xs:documentat
+00003e30: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
+00003e40: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
+00003e50: 7469 6f6e 3e0d 0a20 2020 2020 203c 7873  tion>..      <xs
+00003e60: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
+00003e70: 7565 3d22 3345 223e 3c78 733a 616e 6e6f  ue="3E"><xs:anno
+00003e80: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
+00003e90: 656e 7461 7469 6f6e 3e48 4541 4c54 4820  entation>HEALTH 
+00003ea0: 5345 5256 4943 4553 20e2 8093 2041 2661  SERVICES ... A&a
+00003eb0: 6d70 3b45 2028 6163 6369 6465 6e74 2061  mp;E (accident a
+00003ec0: 6e64 2065 6d65 7267 656e 6379 2064 6570  nd emergency dep
+00003ed0: 6172 746d 656e 7429 3c2f 7873 3a64 6f63  artment)</xs:doc
+00003ee0: 756d 656e 7461 7469 6f6e 3e3c 2f78 733a  umentation></xs:
+00003ef0: 616e 6e6f 7461 7469 6f6e 3e3c 2f78 733a  annotation></xs:
+00003f00: 656e 756d 6572 6174 696f 6e3e 0d0a 2020  enumeration>..  
+00003f10: 2020 2020 3c78 733a 656e 756d 6572 6174      <xs:enumerat
+00003f20: 696f 6e20 7661 6c75 653d 2233 4622 3e3c  ion value="3F"><
+00003f30: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
+00003f40: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00003f50: 4845 414c 5448 2053 4552 5649 4345 5320  HEALTH SERVICES 
+00003f60: e280 9320 6f74 6865 7220 2866 6f72 2065  ... other (for e
+00003f70: 7861 6d70 6c65 2068 6f73 7069 6365 2920  xample hospice) 
+00003f80: 3c2f 7873 3a64 6f63 756d 656e 7461 7469  </xs:documentati
+00003f90: 6f6e 3e3c 2f78 733a 616e 6e6f 7461 7469  on></xs:annotati
+00003fa0: 6f6e 3e3c 2f78 733a 656e 756d 6572 6174  on></xs:enumerat
+00003fb0: 696f 6e3e 0d0a 2020 2020 2020 3c78 733a  ion>..      <xs:
+00003fc0: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
+00003fd0: 653d 2234 223e 3c78 733a 616e 6e6f 7461  e="4"><xs:annota
+00003fe0: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
+00003ff0: 7461 7469 6f6e 3e48 4f55 5349 4e47 202d  tation>HOUSING -
+00004000: 206c 6f63 616c 2061 7574 686f 7269 7479   local authority
+00004010: 2068 6f75 7369 6e67 206f 7220 686f 7573   housing or hous
+00004020: 696e 6720 6173 736f 6369 6174 696f 6e3c  ing association<
+00004030: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
+00004040: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
+00004050: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
+00004060: 6f6e 3e0d 0a20 2020 2020 203c 7873 3a65  on>..      <xs:e
+00004070: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+00004080: 3d22 3541 223e 3c78 733a 616e 6e6f 7461  ="5A"><xs:annota
+00004090: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
+000040a0: 7461 7469 6f6e 3e4c 4120 5345 5256 4943  tation>LA SERVIC
+000040b0: 4553 20e2 8093 2073 6f63 6961 6c20 6361  ES ... social ca
+000040c0: 7265 2066 6f72 2065 7861 6d70 6c65 2061  re for example a
+000040d0: 6475 6c74 7320 736f 6369 616c 2063 6172  dults social car
+000040e0: 6520 7365 7276 6963 6573 3c2f 7873 3a64  e services</xs:d
+000040f0: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
+00004100: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
+00004110: 733a 656e 756d 6572 6174 696f 6e3e 0d0a  s:enumeration>..
+00004120: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
+00004130: 6174 696f 6e20 7661 6c75 653d 2235 4222  ation value="5B"
+00004140: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
+00004150: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
+00004160: 6e3e 4c41 2053 4552 5649 4345 5320 e280  n>LA SERVICES ..
+00004170: 9320 6f74 6865 7220 696e 7465 726e 616c  . other internal
+00004180: 2028 6465 7061 7274 6d65 6e74 206f 7468   (department oth
+00004190: 6572 2074 6861 6e20 736f 6369 616c 2063  er than social c
+000041a0: 6172 6520 696e 206c 6f63 616c 2061 7574  are in local aut
+000041b0: 686f 7269 7469 6573 2c20 666f 7220 6578  horities, for ex
+000041c0: 616d 706c 652c 2079 6f75 7468 206f 6666  ample, youth off
+000041d0: 656e 6469 6e67 2028 6578 636c 7564 696e  ending (excludin
+000041e0: 6720 686f 7573 696e 6729 293c 2f78 733a  g housing))</xs:
+000041f0: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
+00004200: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
+00004210: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0d  xs:enumeration>.
+00004220: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
+00004230: 7261 7469 6f6e 2076 616c 7565 3d22 3543  ration value="5C
+00004240: 223e 3c78 733a 616e 6e6f 7461 7469 6f6e  "><xs:annotation
+00004250: 3e3c 7873 3a64 6f63 756d 656e 7461 7469  ><xs:documentati
+00004260: 6f6e 3e4c 4120 5345 5256 4943 4553 20e2  on>LA SERVICES .
+00004270: 8093 2065 7874 6572 6e61 6c2c 2066 6f72  .. external, for
+00004280: 2065 7861 6d70 6c65 2c20 6672 6f6d 2061   example, from a
+00004290: 6e6f 7468 6572 206c 6f63 616c 2061 7574  nother local aut
+000042a0: 686f 7269 7479 e280 9973 2061 6475 6c74  hority...s adult
+000042b0: 7320 736f 6369 616c 2063 6172 6520 7365  s social care se
+000042c0: 7276 6963 6573 3c2f 7873 3a64 6f63 756d  rvices</xs:docum
+000042d0: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
+000042e0: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
+000042f0: 756d 6572 6174 696f 6e3e 0d0a 2020 2020  umeration>..    
+00004300: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
+00004310: 6e20 7661 6c75 653d 2236 223e 3c78 733a  n value="6"><xs:
+00004320: 616e 6e6f 7461 7469 6f6e 3e3c 7873 3a64  annotation><xs:d
+00004330: 6f63 756d 656e 7461 7469 6f6e 3e50 4f4c  ocumentation>POL
+00004340: 4943 453c 2f78 733a 646f 6375 6d65 6e74  ICE</xs:document
+00004350: 6174 696f 6e3e 3c2f 7873 3a61 6e6e 6f74  ation></xs:annot
+00004360: 6174 696f 6e3e 3c2f 7873 3a65 6e75 6d65  ation></xs:enume
+00004370: 7261 7469 6f6e 3e0d 0a20 2020 2020 203c  ration>..      <
+00004380: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
+00004390: 616c 7565 3d22 3722 3e3c 7873 3a61 6e6e  alue="7"><xs:ann
+000043a0: 6f74 6174 696f 6e3e 3c78 733a 646f 6375  otation><xs:docu
+000043b0: 6d65 6e74 6174 696f 6e3e 4f54 4845 5220  mentation>OTHER 
+000043c0: 4c45 4741 4c20 4147 454e 4359 20e2 8093  LEGAL AGENCY ...
+000043d0: 2069 6e63 6c75 6469 6e67 2063 6f75 7274   including court
+000043e0: 732c 2070 726f 6261 7469 6f6e 2c20 696d  s, probation, im
+000043f0: 6d69 6772 6174 696f 6e2c 2043 4146 4341  migration, CAFCA
+00004400: 5353 2028 4368 696c 6472 656e 2061 6e64  SS (Children and
+00004410: 2046 616d 696c 7920 436f 7572 7420 4164   Family Court Ad
+00004420: 7669 736f 7279 2061 6e64 2053 7570 706f  visory and Suppo
+00004430: 7274 2053 6572 7669 6365 2920 6f72 2070  rt Service) or p
+00004440: 7269 736f 6e3c 2f78 733a 646f 6375 6d65  rison</xs:docume
+00004450: 6e74 6174 696f 6e3e 3c2f 7873 3a61 6e6e  ntation></xs:ann
+00004460: 6f74 6174 696f 6e3e 3c2f 7873 3a65 6e75  otation></xs:enu
+00004470: 6d65 7261 7469 6f6e 3e0d 0a20 2020 2020  meration>..     
+00004480: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
+00004490: 2076 616c 7565 3d22 3822 3e3c 7873 3a61   value="8"><xs:a
+000044a0: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
+000044b0: 6375 6d65 6e74 6174 696f 6e3e 4f54 4845  cumentation>OTHE
+000044c0: 5220 e280 9320 696e 636c 7564 696e 6720  R ... including 
+000044d0: 6368 696c 6472 656e e280 9973 2063 656e  children...s cen
+000044e0: 7472 6573 2c20 696e 6465 7065 6e64 656e  tres, independen
+000044f0: 7420 6167 656e 6379 2070 726f 7669 6465  t agency provide
+00004500: 7273 206f 7220 766f 6c75 6e74 6172 7920  rs or voluntary 
+00004510: 6f72 6761 6e69 7361 7469 6f6e 733c 2f78  organisations</x
+00004520: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00004530: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
+00004540: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
+00004550: 3e0d 0a20 2020 2020 203c 7873 3a65 6e75  >..      <xs:enu
+00004560: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
+00004570: 3922 3e3c 7873 3a61 6e6e 6f74 6174 696f  9"><xs:annotatio
+00004580: 6e3e 3c78 733a 646f 6375 6d65 6e74 6174  n><xs:documentat
+00004590: 696f 6e3e 414e 4f4e 594d 4f55 533c 2f78  ion>ANONYMOUS</x
+000045a0: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+000045b0: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
+000045c0: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
+000045d0: 3e0d 0a20 2020 2020 203c 7873 3a65 6e75  >..      <xs:enu
+000045e0: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
+000045f0: 3130 223e 3c78 733a 616e 6e6f 7461 7469  10"><xs:annotati
+00004600: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
+00004610: 7469 6f6e 3e55 4e4b 4e4f 574e 3c2f 7873  tion>UNKNOWN</xs
+00004620: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
+00004630: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
+00004640: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
+00004650: 0d0a 2020 2020 3c2f 7873 3a72 6573 7472  ..    </xs:restr
+00004660: 6963 7469 6f6e 3e0d 0a20 203c 2f78 733a  iction>..  </xs:
+00004670: 7369 6d70 6c65 5479 7065 3e0d 0a0d 0a20  simpleType>.... 
+00004680: 203c 7873 3a73 696d 706c 6554 7970 6520   <xs:simpleType 
+00004690: 6e61 6d65 3d22 6361 7465 676f 7279 6f66  name="categoryof
+000046a0: 6162 7573 6522 3e0d 0a20 2020 203c 7873  abuse">..    <xs
+000046b0: 3a72 6573 7472 6963 7469 6f6e 2062 6173  :restriction bas
+000046c0: 653d 226e 6f6e 456d 7074 7953 7472 696e  e="nonEmptyStrin
+000046d0: 6722 3e0d 0a20 2020 2020 203c 7873 3a65  g">..      <xs:e
+000046e0: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+000046f0: 3d22 4e45 4722 3e3c 7873 3a61 6e6e 6f74  ="NEG"><xs:annot
+00004700: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
+00004710: 6e74 6174 696f 6e3e 4e65 676c 6563 743c  ntation>Neglect<
+00004720: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
+00004730: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
+00004740: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
+00004750: 6f6e 3e0d 0a20 2020 2020 203c 7873 3a65  on>..      <xs:e
+00004760: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+00004770: 3d22 5048 5922 3e3c 7873 3a61 6e6e 6f74  ="PHY"><xs:annot
+00004780: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
+00004790: 6e74 6174 696f 6e3e 5068 7973 6963 616c  ntation>Physical
+000047a0: 2061 6275 7365 3c2f 7873 3a64 6f63 756d   abuse</xs:docum
+000047b0: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
+000047c0: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
+000047d0: 756d 6572 6174 696f 6e3e 0d0a 2020 2020  umeration>..    
+000047e0: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
+000047f0: 6e20 7661 6c75 653d 2253 4142 223e 3c78  n value="SAB"><x
+00004800: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
+00004810: 3a64 6f63 756d 656e 7461 7469 6f6e 3e53  :documentation>S
+00004820: 6578 7561 6c20 6162 7573 653c 2f78 733a  exual abuse</xs:
+00004830: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
+00004840: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
+00004850: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0d  xs:enumeration>.
+00004860: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
+00004870: 7261 7469 6f6e 2076 616c 7565 3d22 454d  ration value="EM
+00004880: 4f22 3e3c 7873 3a61 6e6e 6f74 6174 696f  O"><xs:annotatio
+00004890: 6e3e 3c78 733a 646f 6375 6d65 6e74 6174  n><xs:documentat
+000048a0: 696f 6e3e 456d 6f74 696f 6e61 6c20 6162  ion>Emotional ab
+000048b0: 7573 653c 2f78 733a 646f 6375 6d65 6e74  use</xs:document
+000048c0: 6174 696f 6e3e 3c2f 7873 3a61 6e6e 6f74  ation></xs:annot
+000048d0: 6174 696f 6e3e 3c2f 7873 3a65 6e75 6d65  ation></xs:enume
+000048e0: 7261 7469 6f6e 3e0d 0a20 2020 2020 203c  ration>..      <
+000048f0: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
+00004900: 616c 7565 3d22 4d55 4c22 3e3c 7873 3a61  alue="MUL"><xs:a
+00004910: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
+00004920: 6375 6d65 6e74 6174 696f 6e3e 4d75 6c74  cumentation>Mult
+00004930: 6970 6c65 2f6e 6f74 2072 6563 6f6d 6d65  iple/not recomme
+00004940: 6e64 6564 3c2f 7873 3a64 6f63 756d 656e  nded</xs:documen
+00004950: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
+00004960: 7461 7469 6f6e 3e3c 2f78 733a 656e 756d  tation></xs:enum
+00004970: 6572 6174 696f 6e3e 0d0a 2020 2020 3c2f  eration>..    </
+00004980: 7873 3a72 6573 7472 6963 7469 6f6e 3e0d  xs:restriction>.
+00004990: 0a20 203c 2f78 733a 7369 6d70 6c65 5479  .  </xs:simpleTy
+000049a0: 7065 3e0d 0a0d 0a20 2020 203c 7873 3a73  pe>....    <xs:s
+000049b0: 696d 706c 6554 7970 6520 6e61 6d65 3d22  impleType name="
+000049c0: 7072 696d 6172 796e 6565 6463 6f64 6574  primaryneedcodet
+000049d0: 7970 6522 3e0d 0a20 2020 203c 7873 3a72  ype">..    <xs:r
+000049e0: 6573 7472 6963 7469 6f6e 2062 6173 653d  estriction base=
+000049f0: 2278 733a 7374 7269 6e67 223e 0d0a 2020  "xs:string">..  
+00004a00: 2020 2020 3c78 733a 656e 756d 6572 6174      <xs:enumerat
+00004a10: 696f 6e20 7661 6c75 653d 224e 3122 3e3c  ion value="N1"><
+00004a20: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
+00004a30: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00004a40: 4162 7573 6520 6f72 206e 6567 6c65 6374  Abuse or neglect
+00004a50: 3c2f 7873 3a64 6f63 756d 656e 7461 7469  </xs:documentati
+00004a60: 6f6e 3e3c 2f78 733a 616e 6e6f 7461 7469  on></xs:annotati
+00004a70: 6f6e 3e3c 2f78 733a 656e 756d 6572 6174  on></xs:enumerat
+00004a80: 696f 6e3e 0d0a 2020 2020 2020 3c78 733a  ion>..      <xs:
+00004a90: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
+00004aa0: 653d 224e 3222 3e3c 7873 3a61 6e6e 6f74  e="N2"><xs:annot
+00004ab0: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
+00004ac0: 6e74 6174 696f 6e3e 4368 696c 6427 7320  ntation>Child's 
+00004ad0: 6469 7361 6269 6c69 7479 3c2f 7873 3a64  disability</xs:d
+00004ae0: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
+00004af0: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
+00004b00: 733a 656e 756d 6572 6174 696f 6e3e 0d0a  s:enumeration>..
+00004b10: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
+00004b20: 6174 696f 6e20 7661 6c75 653d 224e 3322  ation value="N3"
+00004b30: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
+00004b40: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
+00004b50: 6e3e 5061 7265 6e74 616c 2064 6973 6162  n>Parental disab
+00004b60: 696c 6974 7920 6f72 2069 6c6c 6e65 7373  ility or illness
+00004b70: 3c2f 7873 3a64 6f63 756d 656e 7461 7469  </xs:documentati
+00004b80: 6f6e 3e3c 2f78 733a 616e 6e6f 7461 7469  on></xs:annotati
+00004b90: 6f6e 3e3c 2f78 733a 656e 756d 6572 6174  on></xs:enumerat
+00004ba0: 696f 6e3e 0d0a 2020 2020 2020 3c78 733a  ion>..      <xs:
+00004bb0: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
+00004bc0: 653d 224e 3422 3e3c 7873 3a61 6e6e 6f74  e="N4"><xs:annot
+00004bd0: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
+00004be0: 6e74 6174 696f 6e3e 4661 6d69 6c79 2069  ntation>Family i
+00004bf0: 6e20 6163 7574 6520 7374 7265 7373 3c2f  n acute stress</
+00004c00: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
+00004c10: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
+00004c20: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
+00004c30: 6e3e 0d0a 2020 2020 2020 3c78 733a 656e  n>..      <xs:en
+00004c40: 756d 6572 6174 696f 6e20 7661 6c75 653d  umeration value=
+00004c50: 224e 3522 3e3c 7873 3a61 6e6e 6f74 6174  "N5"><xs:annotat
+00004c60: 696f 6e3e 3c78 733a 646f 6375 6d65 6e74  ion><xs:document
+00004c70: 6174 696f 6e3e 4661 6d69 6c79 2064 7973  ation>Family dys
+00004c80: 6675 6e63 7469 6f6e 3c2f 7873 3a64 6f63  function</xs:doc
+00004c90: 756d 656e 7461 7469 6f6e 3e3c 2f78 733a  umentation></xs:
+00004ca0: 616e 6e6f 7461 7469 6f6e 3e3c 2f78 733a  annotation></xs:
+00004cb0: 656e 756d 6572 6174 696f 6e3e 0d0a 2020  enumeration>..  
+00004cc0: 2020 2020 3c78 733a 656e 756d 6572 6174      <xs:enumerat
+00004cd0: 696f 6e20 7661 6c75 653d 224e 3622 3e3c  ion value="N6"><
+00004ce0: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
+00004cf0: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00004d00: 536f 6369 616c 6c79 2075 6e61 6363 6570  Socially unaccep
+00004d10: 7461 626c 6520 6265 6861 7669 6f75 723c  table behaviour<
+00004d20: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
+00004d30: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
+00004d40: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
+00004d50: 6f6e 3e0d 0a20 2020 2020 203c 7873 3a65  on>..      <xs:e
+00004d60: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+00004d70: 3d22 4e37 223e 3c78 733a 616e 6e6f 7461  ="N7"><xs:annota
+00004d80: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
+00004d90: 7461 7469 6f6e 3e4c 6f77 2069 6e63 6f6d  tation>Low incom
+00004da0: 653c 2f78 733a 646f 6375 6d65 6e74 6174  e</xs:documentat
+00004db0: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
+00004dc0: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
+00004dd0: 7469 6f6e 3e0d 0a20 2020 2020 203c 7873  tion>..      <xs
+00004de0: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
+00004df0: 7565 3d22 4e38 223e 3c78 733a 616e 6e6f  ue="N8"><xs:anno
+00004e00: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
+00004e10: 656e 7461 7469 6f6e 3e41 6273 656e 7420  entation>Absent 
+00004e20: 7061 7265 6e74 696e 673c 2f78 733a 646f  parenting</xs:do
+00004e30: 6375 6d65 6e74 6174 696f 6e3e 3c2f 7873  cumentation></xs
+00004e40: 3a61 6e6e 6f74 6174 696f 6e3e 3c2f 7873  :annotation></xs
+00004e50: 3a65 6e75 6d65 7261 7469 6f6e 3e0d 0a20  :enumeration>.. 
+00004e60: 2020 2020 203c 7873 3a65 6e75 6d65 7261       <xs:enumera
+00004e70: 7469 6f6e 2076 616c 7565 3d22 4e39 223e  tion value="N9">
+00004e80: 3c78 733a 616e 6e6f 7461 7469 6f6e 3e3c  <xs:annotation><
+00004e90: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
+00004ea0: 3e43 6173 6573 206f 7468 6572 2074 6861  >Cases other tha
+00004eb0: 6e20 6368 696c 6472 656e 2069 6e20 6e65  n children in ne
+00004ec0: 6564 3c2f 7873 3a64 6f63 756d 656e 7461  ed</xs:documenta
+00004ed0: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
+00004ee0: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
+00004ef0: 6174 696f 6e3e 0d0a 2020 2020 2020 3c78  ation>..      <x
+00004f00: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
+00004f10: 6c75 653d 224e 3022 3e3c 7873 3a61 6e6e  lue="N0"><xs:ann
+00004f20: 6f74 6174 696f 6e3e 3c78 733a 646f 6375  otation><xs:docu
+00004f30: 6d65 6e74 6174 696f 6e3e 4e6f 7420 7374  mentation>Not st
+00004f40: 6174 6564 3c2f 7873 3a64 6f63 756d 656e  ated</xs:documen
+00004f50: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
+00004f60: 7461 7469 6f6e 3e3c 2f78 733a 656e 756d  tation></xs:enum
+00004f70: 6572 6174 696f 6e3e 0d0a 2020 2020 3c2f  eration>..    </
+00004f80: 7873 3a72 6573 7472 6963 7469 6f6e 3e0d  xs:restriction>.
+00004f90: 0a20 203c 2f78 733a 7369 6d70 6c65 5479  .  </xs:simpleTy
+00004fa0: 7065 3e0d 0a0d 0a0d 0a20 203c 7873 3a73  pe>......  <xs:s
+00004fb0: 696d 706c 6554 7970 6520 6e61 6d65 3d22  impleType name="
+00004fc0: 7265 6173 6f6e 666f 7263 6c6f 7375 7265  reasonforclosure
+00004fd0: 7479 7065 223e 0d0a 2020 2020 3c78 733a  type">..    <xs:
+00004fe0: 7265 7374 7269 6374 696f 6e20 6261 7365  restriction base
+00004ff0: 3d22 7873 3a73 7472 696e 6722 3e0d 0a20  ="xs:string">.. 
+00005000: 2020 2020 203c 7873 3a65 6e75 6d65 7261       <xs:enumera
+00005010: 7469 6f6e 2076 616c 7565 3d22 5243 3122  tion value="RC1"
+00005020: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
+00005030: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
+00005040: 6e3e 4164 6f70 7465 643c 2f78 733a 646f  n>Adopted</xs:do
+00005050: 6375 6d65 6e74 6174 696f 6e3e 3c2f 7873  cumentation></xs
+00005060: 3a61 6e6e 6f74 6174 696f 6e3e 3c2f 7873  :annotation></xs
+00005070: 3a65 6e75 6d65 7261 7469 6f6e 3e0d 0a20  :enumeration>.. 
+00005080: 2020 2020 203c 7873 3a65 6e75 6d65 7261       <xs:enumera
+00005090: 7469 6f6e 2076 616c 7565 3d22 5243 3222  tion value="RC2"
+000050a0: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
+000050b0: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
+000050c0: 6e3e 4469 6564 3c2f 7873 3a64 6f63 756d  n>Died</xs:docum
+000050d0: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
+000050e0: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
+000050f0: 756d 6572 6174 696f 6e3e 0d0a 2020 2020  umeration>..    
+00005100: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
+00005110: 6e20 7661 6c75 653d 2252 4333 223e 3c78  n value="RC3"><x
+00005120: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
+00005130: 3a64 6f63 756d 656e 7461 7469 6f6e 3e43  :documentation>C
+00005140: 6869 6c64 2061 7272 616e 6765 6d65 6e74  hild arrangement
+00005150: 7320 6f72 6465 723c 2f78 733a 646f 6375  s order</xs:docu
+00005160: 6d65 6e74 6174 696f 6e3e 3c2f 7873 3a61  mentation></xs:a
+00005170: 6e6e 6f74 6174 696f 6e3e 3c2f 7873 3a65  nnotation></xs:e
+00005180: 6e75 6d65 7261 7469 6f6e 3e0d 0a20 2020  numeration>..   
+00005190: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
+000051a0: 6f6e 2076 616c 7565 3d22 5243 3422 3e3c  on value="RC4"><
+000051b0: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
+000051c0: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+000051d0: 5370 6563 6961 6c20 6775 6172 6469 616e  Special guardian
+000051e0: 7368 6970 206f 7264 6572 3c2f 7873 3a64  ship order</xs:d
+000051f0: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
+00005200: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
+00005210: 733a 656e 756d 6572 6174 696f 6e3e 0d0a  s:enumeration>..
+00005220: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
+00005230: 6174 696f 6e20 7661 6c75 653d 2252 4335  ation value="RC5
+00005240: 223e 3c78 733a 616e 6e6f 7461 7469 6f6e  "><xs:annotation
+00005250: 3e3c 7873 3a64 6f63 756d 656e 7461 7469  ><xs:documentati
+00005260: 6f6e 3e54 7261 6e73 6665 7272 6564 2074  on>Transferred t
+00005270: 6f20 7365 7276 6963 6573 206f 6620 616e  o services of an
+00005280: 6f74 6865 7220 6c6f 6361 6c20 6175 7468  other local auth
+00005290: 6f72 6974 793c 2f78 733a 646f 6375 6d65  ority</xs:docume
+000052a0: 6e74 6174 696f 6e3e 3c2f 7873 3a61 6e6e  ntation></xs:ann
+000052b0: 6f74 6174 696f 6e3e 3c2f 7873 3a65 6e75  otation></xs:enu
+000052c0: 6d65 7261 7469 6f6e 3e0d 0a20 2020 2020  meration>..     
+000052d0: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
+000052e0: 2076 616c 7565 3d22 5243 3622 3e3c 7873   value="RC6"><xs
+000052f0: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
+00005300: 646f 6375 6d65 6e74 6174 696f 6e3e 5472  documentation>Tr
+00005310: 616e 7366 6572 7265 6420 746f 2061 6475  ansferred to adu
+00005320: 6c74 2073 6f63 6961 6c20 6361 7265 2073  lt social care s
+00005330: 6572 7669 6365 733c 2f78 733a 646f 6375  ervices</xs:docu
+00005340: 6d65 6e74 6174 696f 6e3e 3c2f 7873 3a61  mentation></xs:a
+00005350: 6e6e 6f74 6174 696f 6e3e 3c2f 7873 3a65  nnotation></xs:e
+00005360: 6e75 6d65 7261 7469 6f6e 3e0d 0a20 2020  numeration>..   
+00005370: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
+00005380: 6f6e 2076 616c 7565 3d22 5243 3722 3e3c  on value="RC7"><
+00005390: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
+000053a0: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+000053b0: 5365 7276 6963 6573 2063 6561 7365 6420  Services ceased 
+000053c0: 666f 7220 616e 7920 6f74 6865 7220 7265  for any other re
+000053d0: 6173 6f6e 2c20 696e 636c 7564 696e 6720  ason, including 
+000053e0: 6368 696c 6420 6e6f 206c 6f6e 6765 7220  child no longer 
+000053f0: 696e 206e 6565 643c 2f78 733a 646f 6375  in need</xs:docu
+00005400: 6d65 6e74 6174 696f 6e3e 3c2f 7873 3a61  mentation></xs:a
+00005410: 6e6e 6f74 6174 696f 6e3e 3c2f 7873 3a65  nnotation></xs:e
+00005420: 6e75 6d65 7261 7469 6f6e 3e0d 0a20 2020  numeration>..   
+00005430: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
+00005440: 6f6e 2076 616c 7565 3d22 5243 3822 3e3c  on value="RC8"><
+00005450: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
+00005460: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00005470: 4361 7365 2063 6c6f 7365 6420 6166 7465  Case closed afte
+00005480: 7220 6173 7365 7373 6d65 6e74 2c20 6e6f  r assessment, no
+00005490: 2066 7572 7468 6572 2061 6374 696f 6e3c   further action<
+000054a0: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
+000054b0: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
+000054c0: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
+000054d0: 6f6e 3e0d 0a20 2020 203c 2f78 733a 7265  on>..    </xs:re
+000054e0: 7374 7269 6374 696f 6e3e 0d0a 2020 3c2f  striction>..  </
+000054f0: 7873 3a73 696d 706c 6554 7970 653e 0d0a  xs:simpleType>..
+00005500: 0d0a 2020 2020 3c78 733a 7369 6d70 6c65  ..    <xs:simple
+00005510: 5479 7065 206e 616d 653d 2261 7373 6573  Type name="asses
+00005520: 736d 656e 7466 6163 746f 7273 7479 7065  smentfactorstype
+00005530: 223e 0d0a 2020 2020 3c78 733a 7265 7374  ">..    <xs:rest
+00005540: 7269 6374 696f 6e20 6261 7365 3d22 6e6f  riction base="no
+00005550: 6e45 6d70 7479 5374 7269 6e67 223e 0d0a  nEmptyString">..
+00005560: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
+00005570: 6174 696f 6e20 7661 6c75 653d 2231 4122  ation value="1A"
+00005580: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
+00005590: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
+000055a0: 6e3e 416c 636f 686f 6c20 6d69 7375 7365  n>Alcohol misuse
+000055b0: 3a20 636f 6e63 6572 6e73 2061 626f 7574  : concerns about
+000055c0: 2061 6c63 6f68 6f6c 206d 6973 7573 6520   alcohol misuse 
+000055d0: 6279 2074 6865 2063 6869 6c64 3c2f 7873  by the child</xs
+000055e0: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
+000055f0: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
+00005600: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
+00005610: 0d0a 2020 2020 2020 3c78 733a 656e 756d  ..      <xs:enum
+00005620: 6572 6174 696f 6e20 7661 6c75 653d 2231  eration value="1
+00005630: 4222 3e3c 7873 3a61 6e6e 6f74 6174 696f  B"><xs:annotatio
+00005640: 6e3e 3c78 733a 646f 6375 6d65 6e74 6174  n><xs:documentat
+00005650: 696f 6e3e 416c 636f 686f 6c20 6d69 7375  ion>Alcohol misu
+00005660: 7365 3a20 636f 6e63 6572 6e73 2061 626f  se: concerns abo
+00005670: 7574 2061 6c63 6f68 6f6c 206d 6973 7573  ut alcohol misus
+00005680: 6520 6279 2074 6865 2070 6172 656e 7428  e by the parent(
+00005690: 7329 2f63 6172 6572 2873 293c 2f78 733a  s)/carer(s)</xs:
+000056a0: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
+000056b0: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
+000056c0: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0d  xs:enumeration>.
+000056d0: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
+000056e0: 7261 7469 6f6e 2076 616c 7565 3d22 3143  ration value="1C
+000056f0: 223e 3c78 733a 616e 6e6f 7461 7469 6f6e  "><xs:annotation
+00005700: 3e3c 7873 3a64 6f63 756d 656e 7461 7469  ><xs:documentati
+00005710: 6f6e 3e41 6c63 6f68 6f6c 206d 6973 7573  on>Alcohol misus
+00005720: 653a 2063 6f6e 6365 726e 7320 6162 6f75  e: concerns abou
+00005730: 7420 616c 636f 686f 6c20 6d69 7375 7365  t alcohol misuse
+00005740: 2062 7920 616e 6f74 6865 7220 7065 7273   by another pers
+00005750: 6f6e 206c 6976 696e 6720 696e 2074 6865  on living in the
+00005760: 2068 6f75 7365 686f 6c64 3c2f 7873 3a64   household</xs:d
+00005770: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
+00005780: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
+00005790: 733a 656e 756d 6572 6174 696f 6e3e 0d0a  s:enumeration>..
+000057a0: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
+000057b0: 6174 696f 6e20 7661 6c75 653d 2232 4122  ation value="2A"
+000057c0: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
+000057d0: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
+000057e0: 6e3e 4472 7567 206d 6973 7573 653a 2063  n>Drug misuse: c
+000057f0: 6f6e 6365 726e 7320 6162 6f75 7420 6472  oncerns about dr
+00005800: 7567 206d 6973 7573 6520 6279 2074 6865  ug misuse by the
+00005810: 2063 6869 6c64 3c2f 7873 3a64 6f63 756d   child</xs:docum
+00005820: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
+00005830: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
+00005840: 756d 6572 6174 696f 6e3e 0d0a 2020 2020  umeration>..    
+00005850: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
+00005860: 6e20 7661 6c75 653d 2232 4222 3e3c 7873  n value="2B"><xs
+00005870: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
+00005880: 646f 6375 6d65 6e74 6174 696f 6e3e 4472  documentation>Dr
+00005890: 7567 206d 6973 7573 653a 2063 6f6e 6365  ug misuse: conce
+000058a0: 726e 7320 6162 6f75 7420 6472 7567 206d  rns about drug m
+000058b0: 6973 7573 6520 6279 2074 6865 2070 6172  isuse by the par
+000058c0: 656e 7428 7329 2f63 6172 6572 2873 293c  ent(s)/carer(s)<
+000058d0: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
+000058e0: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
+000058f0: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
+00005900: 6f6e 3e0d 0a20 2020 2020 203c 7873 3a65  on>..      <xs:e
+00005910: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+00005920: 3d22 3243 223e 3c78 733a 616e 6e6f 7461  ="2C"><xs:annota
+00005930: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
+00005940: 7461 7469 6f6e 3e44 7275 6720 6d69 7375  tation>Drug misu
+00005950: 7365 3a20 636f 6e63 6572 6e73 2061 626f  se: concerns abo
+00005960: 7574 2064 7275 6720 6d69 7375 7365 2062  ut drug misuse b
+00005970: 7920 616e 6f74 6865 7220 7065 7273 6f6e  y another person
+00005980: 206c 6976 696e 6720 696e 2074 6865 2068   living in the h
+00005990: 6f75 7365 686f 6c64 3c2f 7873 3a64 6f63  ousehold</xs:doc
+000059a0: 756d 656e 7461 7469 6f6e 3e3c 2f78 733a  umentation></xs:
+000059b0: 616e 6e6f 7461 7469 6f6e 3e3c 2f78 733a  annotation></xs:
+000059c0: 656e 756d 6572 6174 696f 6e3e 0d0a 2020  enumeration>..  
+000059d0: 2020 2020 3c78 733a 656e 756d 6572 6174      <xs:enumerat
+000059e0: 696f 6e20 7661 6c75 653d 2233 4122 3e3c  ion value="3A"><
+000059f0: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
+00005a00: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00005a10: 446f 6d65 7374 6963 2076 696f 6c65 6e63  Domestic violenc
+00005a20: 653a 2063 6f6e 6365 726e 7320 6162 6f75  e: concerns abou
+00005a30: 7420 7468 6520 6368 696c 6420 6265 696e  t the child bein
+00005a40: 6720 7468 6520 7375 626a 6563 7420 6f66  g the subject of
+00005a50: 2064 6f6d 6573 7469 6320 7669 6f6c 656e   domestic violen
+00005a60: 6365 3c2f 7873 3a64 6f63 756d 656e 7461  ce</xs:documenta
+00005a70: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
+00005a80: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
+00005a90: 6174 696f 6e3e 0d0a 2020 2020 2020 3c78  ation>..      <x
+00005aa0: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
+00005ab0: 6c75 653d 2233 4222 3e3c 7873 3a61 6e6e  lue="3B"><xs:ann
+00005ac0: 6f74 6174 696f 6e3e 3c78 733a 646f 6375  otation><xs:docu
+00005ad0: 6d65 6e74 6174 696f 6e3e 446f 6d65 7374  mentation>Domest
+00005ae0: 6963 2076 696f 6c65 6e63 653a 2063 6f6e  ic violence: con
+00005af0: 6365 726e 7320 6162 6f75 7420 7468 6520  cerns about the 
+00005b00: 6368 696c 64e2 8099 7320 7061 7265 6e74  child...s parent
+00005b10: 2873 292f 6361 7265 7228 7329 2062 6569  (s)/carer(s) bei
+00005b20: 6e67 2074 6865 2073 7562 6a65 6374 206f  ng the subject o
+00005b30: 6620 646f 6d65 7374 6963 2076 696f 6c65  f domestic viole
+00005b40: 6e63 653c 2f78 733a 646f 6375 6d65 6e74  nce</xs:document
+00005b50: 6174 696f 6e3e 3c2f 7873 3a61 6e6e 6f74  ation></xs:annot
+00005b60: 6174 696f 6e3e 3c2f 7873 3a65 6e75 6d65  ation></xs:enume
+00005b70: 7261 7469 6f6e 3e0d 0a20 2020 2020 203c  ration>..      <
+00005b80: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
+00005b90: 616c 7565 3d22 3343 223e 3c78 733a 616e  alue="3C"><xs:an
+00005ba0: 6e6f 7461 7469 6f6e 3e3c 7873 3a64 6f63  notation><xs:doc
+00005bb0: 756d 656e 7461 7469 6f6e 3e44 6f6d 6573  umentation>Domes
+00005bc0: 7469 6320 7669 6f6c 656e 6365 3a20 636f  tic violence: co
+00005bd0: 6e63 6572 6e73 2061 626f 7574 2061 6e6f  ncerns about ano
+00005be0: 7468 6572 2070 6572 736f 6e20 6c69 7669  ther person livi
+00005bf0: 6e67 2069 6e20 7468 6520 686f 7573 6568  ng in the househ
+00005c00: 6f6c 6420 6265 696e 6720 7468 6520 7375  old being the su
+00005c10: 626a 6563 7420 6f66 2064 6f6d 6573 7469  bject of domesti
+00005c20: 6320 7669 6f6c 656e 6365 3c2f 7873 3a64  c violence</xs:d
+00005c30: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
+00005c40: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
+00005c50: 733a 656e 756d 6572 6174 696f 6e3e 0d0a  s:enumeration>..
+00005c60: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
+00005c70: 6174 696f 6e20 7661 6c75 653d 2234 4122  ation value="4A"
+00005c80: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
+00005c90: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
+00005ca0: 6e3e 4d65 6e74 616c 2068 6561 6c74 683a  n>Mental health:
+00005cb0: 2063 6f6e 6365 726e 7320 6162 6f75 7420   concerns about 
+00005cc0: 7468 6520 6d65 6e74 616c 2068 6561 6c74  the mental healt
+00005cd0: 6820 6f66 2074 6865 2063 6869 6c64 3c2f  h of the child</
+00005ce0: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
+00005cf0: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
+00005d00: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
+00005d10: 6e3e 0d0a 2020 2020 2020 3c78 733a 656e  n>..      <xs:en
+00005d20: 756d 6572 6174 696f 6e20 7661 6c75 653d  umeration value=
+00005d30: 2234 4222 3e3c 7873 3a61 6e6e 6f74 6174  "4B"><xs:annotat
+00005d40: 696f 6e3e 3c78 733a 646f 6375 6d65 6e74  ion><xs:document
+00005d50: 6174 696f 6e3e 4d65 6e74 616c 2068 6561  ation>Mental hea
+00005d60: 6c74 683a 2063 6f6e 6365 726e 7320 6162  lth: concerns ab
+00005d70: 6f75 7420 7468 6520 6d65 6e74 616c 2068  out the mental h
+00005d80: 6561 6c74 6820 6f66 2074 6865 2070 6172  ealth of the par
+00005d90: 656e 7428 7329 2f63 6172 6572 2873 293c  ent(s)/carer(s)<
+00005da0: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
+00005db0: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
+00005dc0: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
+00005dd0: 6f6e 3e0d 0a20 2020 2020 203c 7873 3a65  on>..      <xs:e
+00005de0: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+00005df0: 3d22 3443 223e 3c78 733a 616e 6e6f 7461  ="4C"><xs:annota
+00005e00: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
+00005e10: 7461 7469 6f6e 3e4d 656e 7461 6c20 6865  tation>Mental he
+00005e20: 616c 7468 3a20 636f 6e63 6572 6e73 2061  alth: concerns a
+00005e30: 626f 7574 2074 6865 206d 656e 7461 6c20  bout the mental 
+00005e40: 6865 616c 7468 206f 6620 616e 6f74 6865  health of anothe
+00005e50: 7220 7065 7273 6f6e 2069 6e20 7468 6520  r person in the 
+00005e60: 6661 6d69 6c79 2f68 6f75 7365 686f 6c64  family/household
+00005e70: 3c2f 7873 3a64 6f63 756d 656e 7461 7469  </xs:documentati
+00005e80: 6f6e 3e3c 2f78 733a 616e 6e6f 7461 7469  on></xs:annotati
+00005e90: 6f6e 3e3c 2f78 733a 656e 756d 6572 6174  on></xs:enumerat
+00005ea0: 696f 6e3e 0d0a 2020 2020 2020 3c78 733a  ion>..      <xs:
+00005eb0: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
+00005ec0: 653d 2235 4122 3e3c 7873 3a61 6e6e 6f74  e="5A"><xs:annot
+00005ed0: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
+00005ee0: 6e74 6174 696f 6e3e 4c65 6172 6e69 6e67  ntation>Learning
+00005ef0: 2064 6973 6162 696c 6974 793a 2063 6f6e   disability: con
+00005f00: 6365 726e 7320 6162 6f75 7420 7468 6520  cerns about the 
+00005f10: 6368 696c 64e2 8099 7320 6c65 6172 6e69  child...s learni
+00005f20: 6e67 2064 6973 6162 696c 6974 793c 2f78  ng disability</x
+00005f30: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00005f40: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
+00005f50: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
+00005f60: 3e0d 0a20 2020 2020 203c 7873 3a65 6e75  >..      <xs:enu
+00005f70: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
+00005f80: 3542 223e 3c78 733a 616e 6e6f 7461 7469  5B"><xs:annotati
+00005f90: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
+00005fa0: 7469 6f6e 3e4c 6561 726e 696e 6720 6469  tion>Learning di
+00005fb0: 7361 6269 6c69 7479 3a20 636f 6e63 6572  sability: concer
+00005fc0: 6e73 2061 626f 7574 2074 6865 2070 6172  ns about the par
+00005fd0: 656e 7428 7329 2f63 6172 6572 2873 2920  ent(s)/carer(s) 
+00005fe0: 6c65 6172 6e69 6e67 2064 6973 6162 696c  learning disabil
+00005ff0: 6974 793c 2f78 733a 646f 6375 6d65 6e74  ity</xs:document
+00006000: 6174 696f 6e3e 3c2f 7873 3a61 6e6e 6f74  ation></xs:annot
+00006010: 6174 696f 6e3e 3c2f 7873 3a65 6e75 6d65  ation></xs:enume
+00006020: 7261 7469 6f6e 3e0d 0a20 2020 2020 203c  ration>..      <
+00006030: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
+00006040: 616c 7565 3d22 3543 223e 3c78 733a 616e  alue="5C"><xs:an
+00006050: 6e6f 7461 7469 6f6e 3e3c 7873 3a64 6f63  notation><xs:doc
+00006060: 756d 656e 7461 7469 6f6e 3e4c 6561 726e  umentation>Learn
+00006070: 696e 6720 6469 7361 6269 6c69 7479 3a20  ing disability: 
+00006080: 636f 6e63 6572 6e73 2061 626f 7574 2061  concerns about a
+00006090: 6e6f 7468 6572 2070 6572 736f 6e20 696e  nother person in
+000060a0: 2074 6865 2066 616d 696c 792f 686f 7573   the family/hous
+000060b0: 6568 6f6c 64e2 8099 7320 6c65 6172 6e69  ehold...s learni
+000060c0: 6e67 2064 6973 6162 696c 6974 793c 2f78  ng disability</x
+000060d0: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+000060e0: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
+000060f0: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
+00006100: 3e0d 0a20 2020 2020 203c 7873 3a65 6e75  >..      <xs:enu
+00006110: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
+00006120: 3641 223e 3c78 733a 616e 6e6f 7461 7469  6A"><xs:annotati
+00006130: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
+00006140: 7469 6f6e 3e50 6879 7369 6361 6c20 6469  tion>Physical di
+00006150: 7361 6269 6c69 7479 206f 7220 696c 6c6e  sability or illn
+00006160: 6573 733a 2063 6f6e 6365 726e 7320 6162  ess: concerns ab
+00006170: 6f75 7420 6120 7068 7973 6963 616c 2064  out a physical d
+00006180: 6973 6162 696c 6974 7920 6f72 2069 6c6c  isability or ill
+00006190: 6e65 7373 206f 6620 7468 6520 6368 696c  ness of the chil
+000061a0: 643c 2f78 733a 646f 6375 6d65 6e74 6174  d</xs:documentat
+000061b0: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
+000061c0: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
+000061d0: 7469 6f6e 3e0d 0a20 2020 2020 203c 7873  tion>..      <xs
+000061e0: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
+000061f0: 7565 3d22 3642 223e 3c78 733a 616e 6e6f  ue="6B"><xs:anno
+00006200: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
+00006210: 656e 7461 7469 6f6e 3e50 6879 7369 6361  entation>Physica
+00006220: 6c20 6469 7361 6269 6c69 7479 206f 7220  l disability or 
+00006230: 696c 6c6e 6573 733a 2063 6f6e 6365 726e  illness: concern
+00006240: 7320 6162 6f75 7420 6120 7068 7973 6963  s about a physic
+00006250: 616c 2064 6973 6162 696c 6974 7920 6f72  al disability or
+00006260: 2069 6c6c 6e65 7373 206f 6620 7468 6520   illness of the 
+00006270: 7061 7265 6e74 2873 292f 6361 7265 7228  parent(s)/carer(
+00006280: 7329 3c2f 7873 3a64 6f63 756d 656e 7461  s)</xs:documenta
+00006290: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
+000062a0: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
+000062b0: 6174 696f 6e3e 0d0a 2020 2020 2020 3c78  ation>..      <x
+000062c0: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
+000062d0: 6c75 653d 2236 4322 3e3c 7873 3a61 6e6e  lue="6C"><xs:ann
+000062e0: 6f74 6174 696f 6e3e 3c78 733a 646f 6375  otation><xs:docu
+000062f0: 6d65 6e74 6174 696f 6e3e 5068 7973 6963  mentation>Physic
+00006300: 616c 2064 6973 6162 696c 6974 7920 6f72  al disability or
+00006310: 2069 6c6c 6e65 7373 3a20 636f 6e63 6572   illness: concer
+00006320: 6e73 2061 626f 7574 2061 2070 6879 7369  ns about a physi
+00006330: 6361 6c20 6469 7361 6269 6c69 7479 206f  cal disability o
+00006340: 7220 696c 6c6e 6573 7320 6f66 2061 6e6f  r illness of ano
+00006350: 7468 6572 2070 6572 736f 6e20 696e 2074  ther person in t
+00006360: 6865 2066 616d 696c 792f 686f 7573 6568  he family/househ
+00006370: 6f6c 643c 2f78 733a 646f 6375 6d65 6e74  old</xs:document
+00006380: 6174 696f 6e3e 3c2f 7873 3a61 6e6e 6f74  ation></xs:annot
+00006390: 6174 696f 6e3e 3c2f 7873 3a65 6e75 6d65  ation></xs:enume
+000063a0: 7261 7469 6f6e 3e0d 0a20 2020 2020 203c  ration>..      <
+000063b0: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
+000063c0: 616c 7565 3d22 3741 223e 3c78 733a 616e  alue="7A"><xs:an
+000063d0: 6e6f 7461 7469 6f6e 3e3c 7873 3a64 6f63  notation><xs:doc
+000063e0: 756d 656e 7461 7469 6f6e 3e59 6f75 6e67  umentation>Young
+000063f0: 2063 6172 6572 3a20 636f 6e63 6572 6e73   carer: concerns
+00006400: 2074 6861 7420 7365 7276 6963 6573 206d   that services m
+00006410: 6179 2062 6520 7265 7175 6972 6564 206f  ay be required o
+00006420: 7220 7468 6520 6368 696c 64e2 8099 7320  r the child...s 
+00006430: 6865 616c 7468 206f 7220 6465 7665 6c6f  health or develo
+00006440: 706d 656e 7420 6d61 7920 6265 2069 6d70  pment may be imp
+00006450: 6169 7265 6420 6475 6520 746f 2074 6865  aired due to the
+00006460: 6972 2063 6172 696e 6720 7265 7370 6f6e  ir caring respon
+00006470: 7369 6269 6c69 7469 6573 3c2f 7873 3a64  sibilities</xs:d
+00006480: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
+00006490: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
+000064a0: 733a 656e 756d 6572 6174 696f 6e3e 0d0a  s:enumeration>..
+000064b0: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
+000064c0: 6174 696f 6e20 7661 6c75 653d 2238 4222  ation value="8B"
+000064d0: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
+000064e0: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
+000064f0: 6e3e 5072 6976 6174 656c 7920 666f 7374  n>Privately fost
+00006500: 6572 6564 3a20 636f 6e63 6572 6e73 2074  ered: concerns t
+00006510: 6861 7420 7365 7276 6963 6573 206d 6179  hat services may
+00006520: 2062 6520 7265 7175 6972 6564 206f 7220   be required or 
+00006530: 7468 6520 6368 696c 6420 6d61 7920 6265  the child may be
+00006540: 2061 7420 7269 736b 2061 7320 6120 7072   at risk as a pr
+00006550: 6976 6174 656c 7920 666f 7374 6572 6564  ivately fostered
+00006560: 2063 6869 6c64 202d 206f 7665 7273 6561   child - oversea
+00006570: 7320 6368 696c 6472 656e 2077 686f 2069  s children who i
+00006580: 6e74 656e 6420 746f 2072 6574 7572 6e3c  ntend to return<
+00006590: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
+000065a0: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
+000065b0: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
+000065c0: 6f6e 3e0d 0a20 2020 2020 203c 7873 3a65  on>..      <xs:e
+000065d0: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+000065e0: 3d22 3843 223e 3c78 733a 616e 6e6f 7461  ="8C"><xs:annota
+000065f0: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
+00006600: 7461 7469 6f6e 3e50 7269 7661 7465 6c79  tation>Privately
+00006610: 2066 6f73 7465 7265 643a 2063 6f6e 6365   fostered: conce
+00006620: 726e 7320 7468 6174 2073 6572 7669 6365  rns that service
+00006630: 7320 6d61 7920 6265 2072 6571 7569 7265  s may be require
+00006640: 6420 6f72 2074 6865 2063 6869 6c64 206d  d or the child m
+00006650: 6179 2062 6520 6174 2072 6973 6b20 6173  ay be at risk as
+00006660: 2061 2070 7269 7661 7465 6c79 2066 6f73   a privately fos
+00006670: 7465 7265 6420 6368 696c 6420 2d20 6f76  tered child - ov
+00006680: 6572 7365 6173 2063 6869 6c64 7265 6e20  erseas children 
+00006690: 7768 6f20 696e 7465 6e64 2074 6f20 7374  who intend to st
+000066a0: 6179 3c2f 7873 3a64 6f63 756d 656e 7461  ay</xs:documenta
+000066b0: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
+000066c0: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
+000066d0: 6174 696f 6e3e 0d0a 2020 2020 2020 3c78  ation>..      <x
+000066e0: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
+000066f0: 6c75 653d 2238 4422 3e3c 7873 3a61 6e6e  lue="8D"><xs:ann
+00006700: 6f74 6174 696f 6e3e 3c78 733a 646f 6375  otation><xs:docu
+00006710: 6d65 6e74 6174 696f 6e3e 5072 6976 6174  mentation>Privat
+00006720: 656c 7920 666f 7374 6572 6564 3a20 636f  ely fostered: co
+00006730: 6e63 6572 6e73 2074 6861 7420 7365 7276  ncerns that serv
+00006740: 6963 6573 206d 6179 2062 6520 7265 7175  ices may be requ
+00006750: 6972 6564 206f 7220 7468 6520 6368 696c  ired or the chil
+00006760: 6420 6d61 7920 6265 2061 7420 7269 736b  d may be at risk
+00006770: 2061 7320 6120 7072 6976 6174 656c 7920   as a privately 
+00006780: 666f 7374 6572 6564 2063 6869 6c64 202d  fostered child -
+00006790: 2055 4b20 6368 696c 6472 656e 2069 6e20   UK children in 
+000067a0: 6564 7563 6174 696f 6e61 6c20 706c 6163  educational plac
+000067b0: 656d 656e 7473 3c2f 7873 3a64 6f63 756d  ements</xs:docum
+000067c0: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
+000067d0: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
+000067e0: 756d 6572 6174 696f 6e3e 0d0a 2020 2020  umeration>..    
+000067f0: 2020 3c78 733a 656e 756d 6572 6174 696f    <xs:enumeratio
+00006800: 6e20 7661 6c75 653d 2238 4522 3e3c 7873  n value="8E"><xs
+00006810: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
+00006820: 646f 6375 6d65 6e74 6174 696f 6e3e 5072  documentation>Pr
+00006830: 6976 6174 656c 7920 666f 7374 6572 6564  ivately fostered
+00006840: 3a20 636f 6e63 6572 6e73 2074 6861 7420  : concerns that 
+00006850: 7365 7276 6963 6573 206d 6179 2062 6520  services may be 
+00006860: 7265 7175 6972 6564 206f 7220 7468 6520  required or the 
+00006870: 6368 696c 6420 6d61 7920 6265 2061 7420  child may be at 
+00006880: 7269 736b 2061 7320 6120 7072 6976 6174  risk as a privat
+00006890: 656c 7920 666f 7374 6572 6564 2063 6869  ely fostered chi
+000068a0: 6c64 202d 2055 4b20 6368 696c 6472 656e  ld - UK children
+000068b0: 206d 616b 696e 6720 616c 7465 726e 6174   making alternat
+000068c0: 6976 6520 6661 6d69 6c79 2061 7272 616e  ive family arran
+000068d0: 6765 6d65 6e74 733c 2f78 733a 646f 6375  gements</xs:docu
+000068e0: 6d65 6e74 6174 696f 6e3e 3c2f 7873 3a61  mentation></xs:a
+000068f0: 6e6e 6f74 6174 696f 6e3e 3c2f 7873 3a65  nnotation></xs:e
+00006900: 6e75 6d65 7261 7469 6f6e 3e0d 0a20 2020  numeration>..   
+00006910: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
+00006920: 6f6e 2076 616c 7565 3d22 3846 223e 3c78  on value="8F"><x
+00006930: 733a 616e 6e6f 7461 7469 6f6e 3e3c 7873  s:annotation><xs
+00006940: 3a64 6f63 756d 656e 7461 7469 6f6e 3e50  :documentation>P
+00006950: 7269 7661 7465 6c79 2066 6f73 7465 7265  rivately fostere
+00006960: 643a 2063 6f6e 6365 726e 7320 7468 6174  d: concerns that
+00006970: 2073 6572 7669 6365 7320 6d61 7920 6265   services may be
+00006980: 2072 6571 7569 7265 6420 6f72 2074 6865   required or the
+00006990: 2063 6869 6c64 206d 6179 2062 6520 6174   child may be at
+000069a0: 2072 6973 6b20 6173 2061 2070 7269 7661   risk as a priva
+000069b0: 7465 6c79 2066 6f73 7465 7265 6420 6368  tely fostered ch
+000069c0: 696c 6420 2d20 6f74 6865 723c 2f78 733a  ild - other</xs:
+000069d0: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
+000069e0: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
+000069f0: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0d  xs:enumeration>.
+00006a00: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
+00006a10: 7261 7469 6f6e 2076 616c 7565 3d22 3941  ration value="9A
+00006a20: 223e 3c78 733a 616e 6e6f 7461 7469 6f6e  "><xs:annotation
+00006a30: 3e3c 7873 3a64 6f63 756d 656e 7461 7469  ><xs:documentati
+00006a40: 6f6e 3e55 4153 433a 2063 6f6e 6365 726e  on>UASC: concern
+00006a50: 7320 7468 6174 2073 6572 7669 6365 7320  s that services 
+00006a60: 6d61 7920 6265 2072 6571 7569 7265 6420  may be required 
+00006a70: 6f72 2074 6865 2063 6869 6c64 206d 6179  or the child may
+00006a80: 2062 6520 6174 2072 6973 6b20 6f66 2068   be at risk of h
+00006a90: 6172 6d20 6173 2061 6e20 756e 6163 636f  arm as an unacco
+00006aa0: 6d70 616e 6965 6420 6173 796c 756d 2d73  mpanied asylum-s
+00006ab0: 6565 6b69 6e67 2063 6869 6c64 3c2f 7873  eeking child</xs
+00006ac0: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
+00006ad0: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
+00006ae0: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
+00006af0: 0d0a 2020 2020 2020 3c78 733a 656e 756d  ..      <xs:enum
+00006b00: 6572 6174 696f 6e20 7661 6c75 653d 2231  eration value="1
+00006b10: 3041 223e 3c78 733a 616e 6e6f 7461 7469  0A"><xs:annotati
+00006b20: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
+00006b30: 7469 6f6e 3e4d 6973 7369 6e67 3a20 636f  tion>Missing: co
+00006b40: 6e63 6572 6e73 2074 6861 7420 7365 7276  ncerns that serv
+00006b50: 6963 6573 206d 6179 2062 6520 7265 7175  ices may be requ
+00006b60: 6972 6564 206f 7220 7468 6520 6368 696c  ired or the chil
+00006b70: 6420 6d61 7920 6265 2061 7420 7269 736b  d may be at risk
+00006b80: 206f 6620 6861 726d 2064 7565 2074 6f20   of harm due to 
+00006b90: 676f 696e 672f 6265 696e 6720 6d69 7373  going/being miss
+00006ba0: 696e 673c 2f78 733a 646f 6375 6d65 6e74  ing</xs:document
+00006bb0: 6174 696f 6e3e 3c2f 7873 3a61 6e6e 6f74  ation></xs:annot
+00006bc0: 6174 696f 6e3e 3c2f 7873 3a65 6e75 6d65  ation></xs:enume
+00006bd0: 7261 7469 6f6e 3e0d 0a20 2020 2020 203c  ration>..      <
+00006be0: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
+00006bf0: 616c 7565 3d22 3131 4122 3e3c 7873 3a61  alue="11A"><xs:a
+00006c00: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
+00006c10: 6375 6d65 6e74 6174 696f 6e3e 4368 696c  cumentation>Chil
+00006c20: 6420 7365 7875 616c 2065 7870 6c6f 6974  d sexual exploit
+00006c30: 6174 696f 6e3a 2063 6f6e 6365 726e 7320  ation: concerns 
+00006c40: 7468 6174 2073 6572 7669 6365 7320 6d61  that services ma
+00006c50: 7920 6265 2072 6571 7569 7265 6420 6f72  y be required or
+00006c60: 2074 6865 2063 6869 6c64 206d 6179 2062   the child may b
+00006c70: 6520 6174 2072 6973 6b20 6f66 2068 6172  e at risk of har
+00006c80: 6d20 6475 6520 746f 2063 6869 6c64 2073  m due to child s
+00006c90: 6578 7561 6c20 6578 706c 6f69 7461 7469  exual exploitati
+00006ca0: 6f6e 3c2f 7873 3a64 6f63 756d 656e 7461  on</xs:documenta
+00006cb0: 7469 6f6e 3e3c 2f78 733a 616e 6e6f 7461  tion></xs:annota
+00006cc0: 7469 6f6e 3e3c 2f78 733a 656e 756d 6572  tion></xs:enumer
+00006cd0: 6174 696f 6e3e 0d0a 2020 2020 2020 3c78  ation>..      <x
+00006ce0: 733a 656e 756d 6572 6174 696f 6e20 7661  s:enumeration va
+00006cf0: 6c75 653d 2231 3241 223e 3c78 733a 616e  lue="12A"><xs:an
+00006d00: 6e6f 7461 7469 6f6e 3e3c 7873 3a64 6f63  notation><xs:doc
+00006d10: 756d 656e 7461 7469 6f6e 3e54 7261 6666  umentation>Traff
+00006d20: 6963 6b69 6e67 3a20 636f 6e63 6572 6e73  icking: concerns
+00006d30: 2074 6861 7420 7365 7276 6963 6573 206d   that services m
+00006d40: 6179 2062 6520 7265 7175 6972 6564 206f  ay be required o
+00006d50: 7220 7468 6520 6368 696c 6420 6d61 7920  r the child may 
+00006d60: 6265 2061 7420 7269 736b 206f 6620 6861  be at risk of ha
+00006d70: 726d 2064 7565 2074 6f20 7472 6166 6669  rm due to traffi
+00006d80: 636b 696e 673c 2f78 733a 646f 6375 6d65  cking</xs:docume
+00006d90: 6e74 6174 696f 6e3e 3c2f 7873 3a61 6e6e  ntation></xs:ann
+00006da0: 6f74 6174 696f 6e3e 3c2f 7873 3a65 6e75  otation></xs:enu
+00006db0: 6d65 7261 7469 6f6e 3e0d 0a20 2020 2020  meration>..     
+00006dc0: 203c 7873 3a65 6e75 6d65 7261 7469 6f6e   <xs:enumeration
+00006dd0: 2076 616c 7565 3d22 3133 4122 3e3c 7873   value="13A"><xs
+00006de0: 3a61 6e6e 6f74 6174 696f 6e3e 3c78 733a  :annotation><xs:
+00006df0: 646f 6375 6d65 6e74 6174 696f 6e3e 4761  documentation>Ga
+00006e00: 6e67 733a 2063 6f6e 6365 726e 7320 7468  ngs: concerns th
+00006e10: 6174 2073 6572 7669 6365 7320 6d61 7920  at services may 
+00006e20: 6265 2072 6571 7569 7265 6420 6f72 2074  be required or t
+00006e30: 6865 2063 6869 6c64 206d 6179 2062 6520  he child may be 
+00006e40: 6174 2072 6973 6b20 6f66 2068 6172 6d20  at risk of harm 
+00006e50: 6265 6361 7573 6520 6f66 2069 6e76 6f6c  because of invol
+00006e60: 7665 6d65 6e74 2069 6e2f 7769 7468 2067  vement in/with g
+00006e70: 616e 6773 3c2f 7873 3a64 6f63 756d 656e  angs</xs:documen
+00006e80: 7461 7469 6f6e 3e3c 2f78 733a 616e 6e6f  tation></xs:anno
+00006e90: 7461 7469 6f6e 3e3c 2f78 733a 656e 756d  tation></xs:enum
+00006ea0: 6572 6174 696f 6e3e 0d0a 2020 2020 2020  eration>..      
+00006eb0: 3c78 733a 656e 756d 6572 6174 696f 6e20  <xs:enumeration 
+00006ec0: 7661 6c75 653d 2231 3441 223e 3c78 733a  value="14A"><xs:
+00006ed0: 616e 6e6f 7461 7469 6f6e 3e3c 7873 3a64  annotation><xs:d
+00006ee0: 6f63 756d 656e 7461 7469 6f6e 3e53 6f63  ocumentation>Soc
+00006ef0: 6961 6c6c 7920 756e 6163 6365 7074 6162  ially unacceptab
+00006f00: 6c65 2062 6568 6176 696f 7572 3a20 636f  le behaviour: co
+00006f10: 6e63 6572 6e73 2074 6861 7420 7365 7276  ncerns that serv
+00006f20: 6963 6573 206d 6179 2062 6520 7265 7175  ices may be requ
+00006f30: 6972 6564 206f 7220 7468 6520 6368 696c  ired or the chil
+00006f40: 6420 6d61 7920 6265 2061 7420 7269 736b  d may be at risk
+00006f50: 2064 7565 2074 6f20 7468 6569 7220 736f   due to their so
+00006f60: 6369 616c 6c79 2075 6e61 6363 6570 7461  cially unaccepta
+00006f70: 626c 6520 6265 6861 7669 6f75 723c 2f78  ble behaviour</x
+00006f80: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00006f90: 3c2f 7873 3a61 6e6e 6f74 6174 696f 6e3e  </xs:annotation>
+00006fa0: 3c2f 7873 3a65 6e75 6d65 7261 7469 6f6e  </xs:enumeration
+00006fb0: 3e0d 0a20 2020 2020 203c 7873 3a65 6e75  >..      <xs:enu
+00006fc0: 6d65 7261 7469 6f6e 2076 616c 7565 3d22  meration value="
+00006fd0: 3135 4122 3e3c 7873 3a61 6e6e 6f74 6174  15A"><xs:annotat
+00006fe0: 696f 6e3e 3c78 733a 646f 6375 6d65 6e74  ion><xs:document
+00006ff0: 6174 696f 6e3e 5365 6c66 2d68 6172 6d3a  ation>Self-harm:
+00007000: 2063 6f6e 6365 726e 7320 7468 6174 2073   concerns that s
+00007010: 6572 7669 6365 7320 6d61 7920 6265 2072  ervices may be r
+00007020: 6571 7569 7265 6420 6f72 2064 7565 2074  equired or due t
+00007030: 6f20 7375 7370 6563 7465 642f 6163 7475  o suspected/actu
+00007040: 616c 2073 656c 662d 6861 726d 696e 6720  al self-harming 
+00007050: 6368 696c 6420 6d61 7920 6265 2061 7420  child may be at 
+00007060: 7269 736b 206f 6620 6861 726d 3c2f 7873  risk of harm</xs
+00007070: 3a64 6f63 756d 656e 7461 7469 6f6e 3e3c  :documentation><
+00007080: 2f78 733a 616e 6e6f 7461 7469 6f6e 3e3c  /xs:annotation><
+00007090: 2f78 733a 656e 756d 6572 6174 696f 6e3e  /xs:enumeration>
+000070a0: 0d0a 2020 2020 2020 3c78 733a 656e 756d  ..      <xs:enum
+000070b0: 6572 6174 696f 6e20 7661 6c75 653d 2231  eration value="1
+000070c0: 3641 223e 3c78 733a 616e 6e6f 7461 7469  6A"><xs:annotati
+000070d0: 6f6e 3e3c 7873 3a64 6f63 756d 656e 7461  on><xs:documenta
+000070e0: 7469 6f6e 3e41 6275 7365 206f 7220 6e65  tion>Abuse or ne
+000070f0: 676c 6563 7420 e280 9320 e280 984e 4547  glect ... ...NEG
+00007100: 4c45 4354 e280 993a 2063 6f6e 6365 726e  LECT...: concern
+00007110: 7320 7468 6174 2073 6572 7669 6365 7320  s that services 
+00007120: 6d61 7920 6265 2072 6571 7569 7265 6420  may be required 
+00007130: 6f72 2074 6865 2063 6869 6c64 206d 6179  or the child may
+00007140: 2062 6520 7375 6666 6572 696e 6720 6f72   be suffering or
+00007150: 206c 696b 656c 7920 746f 2073 7566 6665   likely to suffe
+00007160: 7220 7369 676e 6966 6963 616e 7420 6861  r significant ha
+00007170: 726d 2064 7565 2074 6f20 6162 7573 6520  rm due to abuse 
+00007180: 6f72 206e 6567 6c65 6374 3c2f 7873 3a64  or neglect</xs:d
+00007190: 6f63 756d 656e 7461 7469 6f6e 3e3c 2f78  ocumentation></x
+000071a0: 733a 616e 6e6f 7461 7469 6f6e 3e3c 2f78  s:annotation></x
+000071b0: 733a 656e 756d 6572 6174 696f 6e3e 0d0a  s:enumeration>..
+000071c0: 2020 2020 2020 3c78 733a 656e 756d 6572        <xs:enumer
+000071d0: 6174 696f 6e20 7661 6c75 653d 2231 3741  ation value="17A
+000071e0: 223e 3c78 733a 616e 6e6f 7461 7469 6f6e  "><xs:annotation
+000071f0: 3e3c 7873 3a64 6f63 756d 656e 7461 7469  ><xs:documentati
+00007200: 6f6e 3e41 6275 7365 206f 7220 6e65 676c  on>Abuse or negl
+00007210: 6563 7420 e280 9320 e280 9845 4d4f 5449  ect ... ...EMOTI
+00007220: 4f4e 414c 2041 4255 5345 e280 993a 2063  ONAL ABUSE...: c
+00007230: 6f6e 6365 726e 7320 7468 6174 2073 6572  oncerns that ser
+00007240: 7669 6365 7320 6d61 7920 6265 2072 6571  vices may be req
+00007250: 7569 7265 6420 6f72 2074 6865 2063 6869  uired or the chi
+00007260: 6c64 206d 6179 2062 6520 7375 6666 6572  ld may be suffer
+00007270: 696e 6720 6f72 206c 696b 656c 7920 746f  ing or likely to
+00007280: 2073 7566 6665 7220 7369 676e 6966 6963   suffer signific
+00007290: 616e 7420 6861 726d 2064 7565 2074 6f20  ant harm due to 
+000072a0: 6162 7573 6520 6f72 206e 6567 6c65 6374  abuse or neglect
+000072b0: 3c2f 7873 3a64 6f63 756d 656e 7461 7469  </xs:documentati
+000072c0: 6f6e 3e3c 2f78 733a 616e 6e6f 7461 7469  on></xs:annotati
+000072d0: 6f6e 3e3c 2f78 733a 656e 756d 6572 6174  on></xs:enumerat
+000072e0: 696f 6e3e 0d0a 2020 2020 2020 3c78 733a  ion>..      <xs:
+000072f0: 656e 756d 6572 6174 696f 6e20 7661 6c75  enumeration valu
+00007300: 653d 2231 3842 223e 3c78 733a 616e 6e6f  e="18B"><xs:anno
+00007310: 7461 7469 6f6e 3e3c 7873 3a64 6f63 756d  tation><xs:docum
+00007320: 656e 7461 7469 6f6e 3e41 6275 7365 206f  entation>Abuse o
+00007330: 7220 6e65 676c 6563 7420 e280 9320 e280  r neglect ... ..
+00007340: 9850 4859 5349 4341 4c20 4142 5553 45e2  .PHYSICAL ABUSE.
+00007350: 8099 2028 6368 696c 6420 6f6e 2063 6869  .. (child on chi
+00007360: 6c64 293a 2063 6f6e 6365 726e 7320 7468  ld): concerns th
+00007370: 6174 2073 6572 7669 6365 7320 6d61 7920  at services may 
+00007380: 6265 2072 6571 7569 7265 6420 6f72 2074  be required or t
+00007390: 6865 2063 6869 6c64 206d 6179 2062 6520  he child may be 
+000073a0: 7375 6666 6572 696e 6720 6f72 206c 696b  suffering or lik
+000073b0: 656c 7920 746f 2073 7566 6665 7220 7369  ely to suffer si
+000073c0: 676e 6966 6963 616e 7420 6861 726d 2064  gnificant harm d
+000073d0: 7565 2074 6f20 6162 7573 6520 6f72 206e  ue to abuse or n
+000073e0: 6567 6c65 6374 2062 7920 616e 6f74 6865  eglect by anothe
+000073f0: 7220 6368 696c 643c 2f78 733a 646f 6375  r child</xs:docu
+00007400: 6d65 6e74 6174 696f 6e3e 3c2f 7873 3a61  mentation></xs:a
+00007410: 6e6e 6f74 6174 696f 6e3e 3c2f 7873 3a65  nnotation></xs:e
+00007420: 6e75 6d65 7261 7469 6f6e 3e0d 0a20 2020  numeration>..   
+00007430: 2020 203c 7873 3a65 6e75 6d65 7261 7469     <xs:enumerati
+00007440: 6f6e 2076 616c 7565 3d22 3138 4322 3e3c  on value="18C"><
+00007450: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c78  xs:annotation><x
+00007460: 733a 646f 6375 6d65 6e74 6174 696f 6e3e  s:documentation>
+00007470: 4162 7573 6520 6f72 206e 6567 6c65 6374  Abuse or neglect
+00007480: 20e2 8093 20e2 8098 5048 5953 4943 414c   ... ...PHYSICAL
+00007490: 2041 4255 5345 e280 9920 2861 6475 6c74   ABUSE... (adult
+000074a0: 206f 6e20 6368 696c 6429 3a20 636f 6e63   on child): conc
+000074b0: 6572 6e73 2074 6861 7420 7365 7276 6963  erns that servic
+000074c0: 6573 206d 6179 2062 6520 7265 7175 6972  es may be requir
+000074d0: 6564 206f 7220 7468 6520 6368 696c 6420  ed or the child 
+000074e0: 6d61 7920 6265 2073 7566 6665 7269 6e67  may be suffering
+000074f0: 206f 7220 6c69 6b65 6c79 2074 6f20 7375   or likely to su
+00007500: 6666 6572 2073 6967 6e69 6669 6361 6e74  ffer significant
+00007510: 2068 6172 6d20 6475 6520 746f 2061 6275   harm due to abu
+00007520: 7365 206f 7220 6e65 676c 6563 7420 6279  se or neglect by
+00007530: 2061 6e20 6164 756c 743c 2f78 733a 646f   an adult</xs:do
+00007540: 6375 6d65 6e74 6174 696f 6e3e 3c2f 7873  cumentation></xs
+00007550: 3a61 6e6e 6f74 6174 696f 6e3e 3c2f 7873  :annotation></xs
+00007560: 3a65 6e75 6d65 7261 7469 6f6e 3e0d 0a20  :enumeration>.. 
+00007570: 2020 2020 203c 7873 3a65 6e75 6d65 7261       <xs:enumera
+00007580: 7469 6f6e 2076 616c 7565 3d22 3139 4222  tion value="19B"
+00007590: 3e3c 7873 3a61 6e6e 6f74 6174 696f 6e3e  ><xs:annotation>
+000075a0: 3c78 733a 646f 6375 6d65 6e74 6174 696f  <xs:documentatio
+000075b0: 6e3e 4162 7573 6520 6f72 206e 6567 6c65  n>Abuse or negle
+000075c0: 6374 20e2 8093 20e2 8098 5345 5855 414c  ct ... ...SEXUAL
+000075d0: 2041 4255 5345 e280 9920 2863 6869 6c64   ABUSE... (child
+000075e0: 206f 6e20 6368 696c 6429 3a20 636f 6e63   on child): conc
+000075f0: 6572 6e73 2074 6861 7420 7365 7276 6963  erns that servic
+00007600: 6573 206d 6179 2062 6520 7265 7175 6972  es may be requir
+00007610: 6564 206f 7220 7468 6520 6368 696c 6420  ed or the child 
+00007620: 6d61 7920 6265 2073 7566 6665 7269 6e67  may be suffering
+00007630: 206f 7220 6c69 6b65 6c79 2074 6f20 7375   or likely to su
+00007640: 6666 6572 2073 6967 6e69 6669 6361 6e74  ffer significant
+00007650: 2068 6172 6d20 6475 6520 746f 2061 6275   harm due to abu
+00007660: 7365 206f 7220 6e65 676c 6563 7420 6279  se or neglect by
+00007670: 2061 6e6f 7468 6572 2063 6869 6c64 3c2f   another child</
+00007680: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
+00007690: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
+000076a0: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
+000076b0: 6e3e 0d0a 2020 2020 2020 3c78 733a 656e  n>..      <xs:en
+000076c0: 756d 6572 6174 696f 6e20 7661 6c75 653d  umeration value=
+000076d0: 2231 3943 223e 3c78 733a 616e 6e6f 7461  "19C"><xs:annota
+000076e0: 7469 6f6e 3e3c 7873 3a64 6f63 756d 656e  tion><xs:documen
+000076f0: 7461 7469 6f6e 3e41 6275 7365 206f 7220  tation>Abuse or 
+00007700: 6e65 676c 6563 7420 e280 9320 e280 9853  neglect ... ...S
+00007710: 4558 5541 4c20 4142 5553 45e2 8099 2028  EXUAL ABUSE... (
+00007720: 6164 756c 7420 6f6e 2063 6869 6c64 293a  adult on child):
+00007730: 2063 6f6e 6365 726e 7320 7468 6174 2073   concerns that s
+00007740: 6572 7669 6365 7320 6d61 7920 6265 2072  ervices may be r
+00007750: 6571 7569 7265 6420 6f72 2074 6865 2063  equired or the c
+00007760: 6869 6c64 206d 6179 2062 6520 7375 6666  hild may be suff
+00007770: 6572 696e 6720 6f72 206c 696b 656c 7920  ering or likely 
+00007780: 746f 2073 7566 6665 7220 7369 676e 6966  to suffer signif
+00007790: 6963 616e 7420 6861 726d 2064 7565 2074  icant harm due t
+000077a0: 6f20 6162 7573 6520 6f72 206e 6567 6c65  o abuse or negle
+000077b0: 6374 2062 7920 616e 2061 6475 6c74 3c2f  ct by an adult</
+000077c0: 7873 3a64 6f63 756d 656e 7461 7469 6f6e  xs:documentation
+000077d0: 3e3c 2f78 733a 616e 6e6f 7461 7469 6f6e  ></xs:annotation
+000077e0: 3e3c 2f78 733a 656e 756d 6572 6174 696f  ></xs:enumeratio
+000077f0: 6e3e 0d0a 2020 2020 2020 3c78 733a 656e  n>..      <xs:en
+00007800: 756d 6572 6174 696f 6e20 7661 6c75 653d  umeration value=
+00007810: 2232 3022 3e3c 7873 3a61 6e6e 6f74 6174  "20"><xs:annotat
+00007820: 696f 6e3e 3c78 733a 646f 6375 6d65 6e74  ion><xs:document
+00007830: 6174 696f 6e3e 4f74 6865 723c 2f78 733a  ation>Other</xs:
+00007840: 646f 6375 6d65 6e74 6174 696f 6e3e 3c2f  documentation></
+00007850: 7873 3a61 6e6e 6f74 6174 696f 6e3e 3c2f  xs:annotation></
+00007860: 7873 3a65 6e75 6d65 7261 7469 6f6e 3e0d  xs:enumeration>.
+00007870: 0a20 2020 2020 203c 7873 3a65 6e75 6d65  .      <xs:enume
+00007880: 7261 7469 6f6e 2076 616c 7565 3d22 3231  ration value="21
+00007890: 223e 3c78 733a 616e 6e6f 7461 7469 6f6e  "><xs:annotation
+000078a0: 3e3c 7873 3a64 6f63 756d 656e 7461 7469  ><xs:documentati
+000078b0: 6f6e 3e4e 6f20 6661 6374 6f72 7320 6964  on>No factors id
+000078c0: 656e 7469 6669 6564 202d 206f 6e6c 7920  entified - only 
+000078d0: 7573 6520 7468 6973 2069 6620 7468 6572  use this if ther
+000078e0: 6520 6973 206e 6f20 6576 6964 656e 6365  e is no evidence
+000078f0: 206f 6620 616e 7920 6f66 2074 6865 2066   of any of the f
+00007900: 6163 746f 7273 2061 626f 7665 2061 6e64  actors above and
+00007910: 206e 6f20 6675 7274 6865 7220 6163 7469   no further acti
+00007920: 6f6e 2069 7320 6265 696e 6720 7461 6b65  on is being take
+00007930: 6e3c 2f78 733a 646f 6375 6d65 6e74 6174  n</xs:documentat
+00007940: 696f 6e3e 3c2f 7873 3a61 6e6e 6f74 6174  ion></xs:annotat
+00007950: 696f 6e3e 3c2f 7873 3a65 6e75 6d65 7261  ion></xs:enumera
+00007960: 7469 6f6e 3e0d 0a20 2020 2020 203c 7873  tion>..      <xs
+00007970: 3a65 6e75 6d65 7261 7469 6f6e 2076 616c  :enumeration val
+00007980: 7565 3d22 3232 4122 3e3c 7873 3a61 6e6e  ue="22A"><xs:ann
+00007990: 6f74 6174 696f 6e3e 3c78 733a 646f 6375  otation><xs:docu
+000079a0: 6d65 6e74 6174 696f 6e3e 4665 6d61 6c65  mentation>Female
+000079b0: 2067 656e 6974 616c 206d 7574 696c 6174   genital mutilat
+000079c0: 696f 6e20 2846 474d 2920 2d20 636f 6e63  ion (FGM) - conc
+000079d0: 6572 6e73 2074 6861 7420 7365 7276 6963  erns that servic
+000079e0: 6573 206d 6179 2062 6520 7265 7175 6972  es may be requir
+000079f0: 6564 206f 7220 7468 6520 6368 696c 6420  ed or the child 
+00007a00: 6d61 7920 6265 2061 7420 7269 736b 2064  may be at risk d
+00007a10: 7565 2074 6f20 6665 6d61 6c65 2067 656e  ue to female gen
+00007a20: 6974 616c 206d 7574 696c 6174 696f 6e3c  ital mutilation<
+00007a30: 2f78 733a 646f 6375 6d65 6e74 6174 696f  /xs:documentatio
+00007a40: 6e3e 3c2f 7873 3a61 6e6e 6f74 6174 696f  n></xs:annotatio
+00007a50: 6e3e 3c2f 7873 3a65 6e75 6d65 7261 7469  n></xs:enumerati
+00007a60: 6f6e 3e0d 0a20 2020 2020 203c 7873 3a65  on>..      <xs:e
+00007a70: 6e75 6d65 7261 7469 6f6e 2076 616c 7565  numeration value
+00007a80: 3d22 3233 4122 3e3c 7873 3a61 6e6e 6f74  ="23A"><xs:annot
+00007a90: 6174 696f 6e3e 3c78 733a 646f 6375 6d65  ation><xs:docume
+00007aa0: 6e74 6174 696f 6e3e 4162 7573 6520 6c69  ntation>Abuse li
+00007ab0: 6e6b 6564 2074 6f20 6661 6974 6820 6f72  nked to faith or
+00007ac0: 2062 656c 6965 6620 2d20 636f 6e63 6572   belief - concer
+00007ad0: 6e73 2074 6861 7420 7365 7276 6963 6573  ns that services
+00007ae0: 206d 6179 2062 6520 7265 7175 6972 6564   may be required
+00007af0: 206f 7220 7468 6520 6368 696c 6420 6d61   or the child ma
+00007b00: 7920 6265 2061 7420 7269 736b 2064 7565  y be at risk due
+00007b10: 2074 6f20 6162 7573 6520 6c69 6e6b 6564   to abuse linked
+00007b20: 2074 6f20 6661 6974 6820 6f72 2062 656c   to faith or bel
+00007b30: 6965 663c 2f78 733a 646f 6375 6d65 6e74  ief</xs:document
+00007b40: 6174 696f 6e3e 3c2f 7873 3a61 6e6e 6f74  ation></xs:annot
+00007b50: 6174 696f 6e3e 3c2f 7873 3a65 6e75 6d65  ation></xs:enume
+00007b60: 7261 7469 6f6e 3e0d 0a20 2020 2020 203c  ration>..      <
+00007b70: 7873 3a65 6e75 6d65 7261 7469 6f6e 2076  xs:enumeration v
+00007b80: 616c 7565 3d22 3234 4122 3e3c 7873 3a61  alue="24A"><xs:a
+00007b90: 6e6e 6f74 6174 696f 6e3e 3c78 733a 646f  nnotation><xs:do
+00007ba0: 6375 6d65 6e74 6174 696f 6e3e 4368 696c  cumentation>Chil
+00007bb0: 6420 6372 696d 696e 616c 2065 7870 6c6f  d criminal explo
+00007bc0: 6974 6174 696f 6e3a 2063 6f6e 6365 726e  itation: concern
+00007bd0: 7320 7468 6174 2073 6572 7669 6365 7320  s that services 
+00007be0: 6d61 7920 6265 2072 6571 7569 7265 6420  may be required 
+00007bf0: 6f72 2074 6865 2063 6869 6c64 206d 6179  or the child may
+00007c00: 2062 6520 6174 2072 6973 6b20 6f66 2068   be at risk of h
+00007c10: 6172 6d20 6475 6520 746f 2063 6869 6c64  arm due to child
+00007c20: 2063 7269 6d69 6e61 6c20 6578 706c 6f69   criminal exploi
+00007c30: 7461 7469 6f6e 3c2f 7873 3a64 6f63 756d  tation</xs:docum
+00007c40: 656e 7461 7469 6f6e 3e3c 2f78 733a 616e  entation></xs:an
+00007c50: 6e6f 7461 7469 6f6e 3e3c 2f78 733a 656e  notation></xs:en
+00007c60: 756d 6572 6174 696f 6e3e 0d0a 2020 2020  umeration>..    
+00007c70: 3c2f 7873 3a72 6573 7472 6963 7469 6f6e  </xs:restriction
+00007c80: 3e0d 0a20 203c 2f78 733a 7369 6d70 6c65  >..  </xs:simple
+00007c90: 5479 7065 3e0d 0a0d 0a3c 2f78 733a 7363  Type>....</xs:sc
+00007ca0: 6865 6d61 3e                             hema>
```

### Comparing `liiatools-0.1.5.1/liiatools/spec/cin_census/samples/cin-2022.xml` & `liiatools-0.1.5.2/liiatools/spec/cin_census/samples/cin-2022.xml`

 * *Files 3% similar despite different names*

#### Comparing `liiatools-0.1.5.1/liiatools/spec/cin_census/samples/cin-2022.xml` & `liiatools-0.1.5.2/liiatools/spec/cin_census/samples/cin-2022.xml`

```diff
@@ -1,22 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <Message>
   <Header>
     <CollectionDetails>
       <Collection>CIN</Collection>
-      <Year>2023</Year>
-      <ReferenceDate>2023-03-31</ReferenceDate>
+      <Year>2022</Year>
+      <ReferenceDate>2022-03-31</ReferenceDate>
     </CollectionDetails>
     <Source>
       <SourceLevel>L</SourceLevel>
       <LEA>201</LEA>
       <SoftwareCode>Local Authority</SoftwareCode>
       <Release>ver 3.1.21</Release>
       <SerialNo>001</SerialNo>
-      <DateTime>2023-05-23T11:14:05</DateTime>
+      <DateTime>2022-05-23T11:14:05</DateTime>
     </Source>
   </Header>
   <Children>
     <Child>
       <ChildIdentifiers>
         <LAchildID>DfEX0000001</LAchildID>
         <UPN>A123456789123</UPN>
```

### Comparing `liiatools-0.1.5.1/liiatools/spec/common/LA-codes.yml` & `liiatools-0.1.5.2/liiatools/spec/common/LA-codes.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/spec/s903/la-agg.yml` & `liiatools-0.1.5.2/liiatools/spec/s903/la-agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/spec/s903/pan-agg.yml` & `liiatools-0.1.5.2/liiatools/spec/s903/pan-agg.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/spec/s903/sufficiency.yml` & `liiatools-0.1.5.2/liiatools/spec/s903/sufficiency.yml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/spec/social_work_workforce/samples/social_work_workforce_2022.xml` & `liiatools-0.1.5.2/liiatools/spec/social_work_workforce/samples/social_work_workforce_2022.xml`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/liiatools/spec/social_work_workforce/social_work_workforce_2022.xsd` & `liiatools-0.1.5.2/liiatools/spec/social_work_workforce/social_work_workforce_2022.xsd`

 * *Files identical despite different names*

### Comparing `liiatools-0.1.5.1/pyproject.toml` & `liiatools-0.1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liiatools"
-version = "0.1.5.1"
+version = "0.1.5.2"
 description = "Children's Services Data Tools - Utilities for cleaning and normalising CS data by Social Finance"
 authors = [
     "Michael Hanks <michael.hanks@socialfinance.org.uk>",
     "Patrick Troy <patrick.troy@socialfinance.org.uk>",
     "Céline Gross <celine.m.gross@gmail.com>",
     "Kaj Siebert <kaj@k-si.com>",
     "Matthew Pugh <matthew.pugh@socialfinance.org.uk>"
```

### Comparing `liiatools-0.1.5.1/PKG-INFO` & `liiatools-0.1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liiatools
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: Children's Services Data Tools - Utilities for cleaning and normalising CS data by Social Finance
 License: MIT
 Author: Michael Hanks
 Author-email: michael.hanks@socialfinance.org.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

