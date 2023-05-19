# Comparing `tmp/geneparse-0.8.1.tar.gz` & `tmp/geneparse-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/geneparse-0.8.1.tar", last modified: Fri Aug 21 20:22:58 2020, max compression
+gzip compressed data, was "geneparse-0.8.2.tar", last modified: Fri May 19 18:14:02 2023, max compression
```

## Comparing `geneparse-0.8.1.tar` & `geneparse-0.8.2.tar`

### file list

```diff
@@ -1,86 +1,93 @@
-drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2020-08-21 20:22:58.334112 geneparse-0.8.1/
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     1090 2018-04-04 14:57:22.000000 geneparse-0.8.1/LICENSE
--rw-r-----   0 lemieuxl (12551) pgx      (35376)       34 2018-04-04 14:57:22.000000 geneparse-0.8.1/MANIFEST.in
--rw-r-----   0 lemieuxl (12551) pgx      (35376)      861 2020-08-21 20:22:58.334112 geneparse-0.8.1/PKG-INFO
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     4112 2020-06-19 18:52:37.000000 geneparse-0.8.1/README.md
-drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2020-08-21 20:22:58.329112 geneparse-0.8.1/geneparse/
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     3704 2018-12-06 15:40:26.000000 geneparse-0.8.1/geneparse/__init__.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     1361 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/config.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)    15807 2018-07-24 17:21:08.000000 geneparse-0.8.1/geneparse/core.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     1249 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/exceptions.py
-drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2020-08-21 20:22:58.330112 geneparse-0.8.1/geneparse/extract/
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     1208 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/extract/__init__.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)    13166 2020-06-19 18:52:37.000000 geneparse-0.8.1/geneparse/extract/__main__.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     3542 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/extract/extractor.py
-drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2020-08-21 20:22:58.330112 geneparse-0.8.1/geneparse/index/
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     1206 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/index/__init__.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     3837 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/index/__main__.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     6287 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/index/impute2.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     2305 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/logging.py
-drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2020-08-21 20:22:58.330112 geneparse-0.8.1/geneparse/readers/
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     1189 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/readers/__init__.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     9082 2020-08-21 20:21:32.000000 geneparse-0.8.1/geneparse/readers/bgen.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     3713 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/readers/dataframe.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     3388 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/readers/dict_based.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)    16488 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/readers/impute2.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     9608 2020-06-19 18:52:37.000000 geneparse-0.8.1/geneparse/readers/plink.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     5188 2020-08-21 20:14:28.000000 geneparse-0.8.1/geneparse/readers/vcf.py
-drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2020-08-21 20:22:58.331112 geneparse-0.8.1/geneparse/testing/
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     1242 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/testing/__init__.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     2335 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/testing/simulation.py
-drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2020-08-21 20:22:58.332112 geneparse-0.8.1/geneparse/tests/
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     1244 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/__init__.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     1264 2020-08-21 20:15:09.000000 geneparse-0.8.1/geneparse/tests/__main__.py
-drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2020-08-21 20:22:58.328112 geneparse-0.8.1/geneparse/tests/data/
-drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2020-08-21 20:22:58.332112 geneparse-0.8.1/geneparse/tests/data/impute2/
--rwxr-x---   0 lemieuxl (12551) pgx      (35376)     1499 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/data/impute2/generate_impute2_from_plink.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)      174 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/data/impute2/impute2_test.impute2.gz
--rw-r-----   0 lemieuxl (12551) pgx      (35376)      120 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/data/impute2/impute2_test.impute2.gz.idx
--rw-r-----   0 lemieuxl (12551) pgx      (35376)      197 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/data/impute2/impute2_test.sample
-drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2020-08-21 20:22:58.333112 geneparse-0.8.1/geneparse/tests/data/ld/
--rw-r-----   0 lemieuxl (12551) pgx      (35376)    61995 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/tests/data/ld/common_extracted_1kg.bed
--rw-r-----   0 lemieuxl (12551) pgx      (35376)    13928 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/tests/data/ld/common_extracted_1kg.bim
--rw-r-----   0 lemieuxl (12551) pgx      (35376)    12575 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/tests/data/ld/common_extracted_1kg.fam
--rw-r-----   0 lemieuxl (12551) pgx      (35376)    61995 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/tests/data/ld/common_extracted_1kg.missing.bed
--rw-r-----   0 lemieuxl (12551) pgx      (35376)    13928 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/tests/data/ld/common_extracted_1kg.missing.bim
--rw-r-----   0 lemieuxl (12551) pgx      (35376)    12575 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/tests/data/ld/common_extracted_1kg.missing.fam
--rw-r-----   0 lemieuxl (12551) pgx      (35376)    38454 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/tests/data/ld/plink_rs1800775_pairs.ld
--rw-r-----   0 lemieuxl (12551) pgx      (35376)    38454 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/tests/data/ld/plink_rs1800775_pairs.missing.ld
-drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2020-08-21 20:22:58.333112 geneparse-0.8.1/geneparse/tests/data/plink/
--rw-r-----   0 lemieuxl (12551) pgx      (35376)       13 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/data/plink/btest.bed
--rw-r-----   0 lemieuxl (12551) pgx      (35376)      144 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/data/plink/btest.bim
--rw-r-----   0 lemieuxl (12551) pgx      (35376)      125 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/data/plink/btest.fam
--rw-r-----   0 lemieuxl (12551) pgx      (35376)      121 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/data/plink/test.map
--rw-r-----   0 lemieuxl (12551) pgx      (35376)      246 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/data/plink/test.ped
-drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2020-08-21 20:22:58.333112 geneparse-0.8.1/geneparse/tests/data/vcf/
--rw-r-----   0 lemieuxl (12551) pgx      (35376)      526 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/tests/data/vcf/test.vcf.gz
--rw-r-----   0 lemieuxl (12551) pgx      (35376)      443 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/tests/data/vcf/test.vcf.gz.tbi
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     7197 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/generic_tests.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)    11429 2018-05-10 17:40:22.000000 geneparse-0.8.1/geneparse/tests/test_bgen.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     1207 2018-04-12 18:37:46.000000 geneparse-0.8.1/geneparse/tests/test_core.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     4053 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/test_dataframe.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     3514 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/test_dict_based_reader.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     6180 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/tests/test_extractor.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     5564 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/tests/test_genotypes.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     1945 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/test_impute2.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     1657 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/test_plink.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     3052 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/test_serialization.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     2008 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tests/test_testing.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     7568 2018-05-25 14:23:52.000000 geneparse-0.8.1/geneparse/tests/test_utils.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     4304 2018-04-13 13:43:47.000000 geneparse-0.8.1/geneparse/tests/test_variants.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     4294 2018-12-06 15:40:26.000000 geneparse-0.8.1/geneparse/tests/test_vcf.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     4255 2018-04-10 16:18:48.000000 geneparse-0.8.1/geneparse/tests/truth.py
-drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2020-08-21 20:22:58.333112 geneparse-0.8.1/geneparse/tools/
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     1165 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tools/__init__.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     4116 2018-04-04 14:57:22.000000 geneparse-0.8.1/geneparse/tools/compare_calls.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     9341 2020-06-19 18:52:37.000000 geneparse-0.8.1/geneparse/utils.py
--rw-r-----   0 lemieuxl (12551) pgx      (35376)       69 2020-08-21 20:22:58.000000 geneparse-0.8.1/geneparse/version.py
-drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2020-08-21 20:22:58.329112 geneparse-0.8.1/geneparse.egg-info/
--rw-r-----   0 lemieuxl (12551) pgx      (35376)      861 2020-08-21 20:22:58.000000 geneparse-0.8.1/geneparse.egg-info/PKG-INFO
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     2319 2020-08-21 20:22:58.000000 geneparse-0.8.1/geneparse.egg-info/SOURCES.txt
--rw-r-----   0 lemieuxl (12551) pgx      (35376)        1 2020-08-21 20:22:58.000000 geneparse-0.8.1/geneparse.egg-info/dependency_links.txt
--rw-r-----   0 lemieuxl (12551) pgx      (35376)        1 2018-05-10 16:38:41.000000 geneparse-0.8.1/geneparse.egg-info/not-zip-safe
--rw-r-----   0 lemieuxl (12551) pgx      (35376)       93 2020-08-21 20:22:58.000000 geneparse-0.8.1/geneparse.egg-info/requires.txt
--rw-r-----   0 lemieuxl (12551) pgx      (35376)       10 2020-08-21 20:22:58.000000 geneparse-0.8.1/geneparse.egg-info/top_level.txt
--rw-r-----   0 lemieuxl (12551) pgx      (35376)       38 2020-08-21 20:22:58.334112 geneparse-0.8.1/setup.cfg
--rw-r-----   0 lemieuxl (12551) pgx      (35376)     2687 2020-08-21 20:21:32.000000 geneparse-0.8.1/setup.py
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.750891 geneparse-0.8.2/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      130 2023-05-19 18:10:20.000000 geneparse-0.8.2/.coveragerc
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.745891 geneparse-0.8.2/.github/
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.746891 geneparse-0.8.2/.github/workflows/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      800 2023-05-19 18:10:20.000000 geneparse-0.8.2/.github/workflows/python-app.yml
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)       92 2020-08-21 20:21:32.000000 geneparse-0.8.2/.gitignore
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1090 2018-04-04 14:57:22.000000 geneparse-0.8.2/LICENSE
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)       34 2018-04-04 14:57:22.000000 geneparse-0.8.2/MANIFEST.in
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      806 2023-05-19 18:14:02.750891 geneparse-0.8.2/PKG-INFO
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     4153 2022-02-28 14:07:23.000000 geneparse-0.8.2/README.md
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.747891 geneparse-0.8.2/geneparse/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     3704 2018-12-06 15:40:26.000000 geneparse-0.8.2/geneparse/__init__.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1361 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/config.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    15807 2018-07-24 17:21:08.000000 geneparse-0.8.2/geneparse/core.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1249 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/exceptions.py
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.747891 geneparse-0.8.2/geneparse/extract/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1208 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/extract/__init__.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    13166 2020-06-19 18:52:37.000000 geneparse-0.8.2/geneparse/extract/__main__.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     3542 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/extract/extractor.py
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.747891 geneparse-0.8.2/geneparse/index/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1206 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/index/__init__.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     3837 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/index/__main__.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     6287 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/index/impute2.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     2305 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/logging.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     2876 2022-02-28 14:07:23.000000 geneparse-0.8.2/geneparse/match_genotype_iterators.py
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.748891 geneparse-0.8.2/geneparse/readers/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1189 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/readers/__init__.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     9082 2020-08-21 20:21:32.000000 geneparse-0.8.2/geneparse/readers/bgen.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     3713 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/readers/dataframe.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     3388 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/readers/dict_based.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    16480 2023-05-19 18:10:20.000000 geneparse-0.8.2/geneparse/readers/impute2.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     9608 2023-05-19 18:08:37.000000 geneparse-0.8.2/geneparse/readers/plink.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     5188 2023-05-19 18:08:37.000000 geneparse-0.8.2/geneparse/readers/vcf.py
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.748891 geneparse-0.8.2/geneparse/testing/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1242 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/testing/__init__.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     2335 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/testing/simulation.py
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.748891 geneparse-0.8.2/geneparse/tests/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1244 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/__init__.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1264 2020-08-21 20:15:09.000000 geneparse-0.8.2/geneparse/tests/__main__.py
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.746891 geneparse-0.8.2/geneparse/tests/data/
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.749891 geneparse-0.8.2/geneparse/tests/data/impute2/
+-rwxr-x---   0 lemieuxl (12551) pgx      (35376)     1499 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/data/impute2/generate_impute2_from_plink.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      174 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/data/impute2/impute2_test.impute2.gz
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      120 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/data/impute2/impute2_test.impute2.gz.idx
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      197 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/data/impute2/impute2_test.sample
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.749891 geneparse-0.8.2/geneparse/tests/data/ld/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    61995 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/tests/data/ld/common_extracted_1kg.bed
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    13928 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/tests/data/ld/common_extracted_1kg.bim
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    12575 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/tests/data/ld/common_extracted_1kg.fam
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    61995 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/tests/data/ld/common_extracted_1kg.missing.bed
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    13928 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/tests/data/ld/common_extracted_1kg.missing.bim
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    12575 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/tests/data/ld/common_extracted_1kg.missing.fam
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    38454 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/tests/data/ld/plink_rs1800775_pairs.ld
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    38454 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/tests/data/ld/plink_rs1800775_pairs.missing.ld
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.749891 geneparse-0.8.2/geneparse/tests/data/plink/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)       13 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/data/plink/btest.bed
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      144 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/data/plink/btest.bim
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      125 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/data/plink/btest.fam
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      121 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/data/plink/test.map
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      246 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/data/plink/test.ped
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.750891 geneparse-0.8.2/geneparse/tests/data/vcf/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      526 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/tests/data/vcf/test.vcf.gz
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      443 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/tests/data/vcf/test.vcf.gz.tbi
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     7197 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/generic_tests.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)    11429 2018-05-10 17:40:22.000000 geneparse-0.8.2/geneparse/tests/test_bgen.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1207 2018-04-12 18:37:46.000000 geneparse-0.8.2/geneparse/tests/test_core.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     4053 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/test_dataframe.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     3514 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/test_dict_based_reader.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     6180 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/tests/test_extractor.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     5564 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/tests/test_genotypes.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1945 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/test_impute2.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1657 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/test_plink.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     3052 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/test_serialization.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     2008 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tests/test_testing.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     7568 2018-05-25 14:23:52.000000 geneparse-0.8.2/geneparse/tests/test_utils.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     4304 2018-04-13 13:43:47.000000 geneparse-0.8.2/geneparse/tests/test_variants.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     4294 2018-12-06 15:40:26.000000 geneparse-0.8.2/geneparse/tests/test_vcf.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     4255 2018-04-10 16:18:48.000000 geneparse-0.8.2/geneparse/tests/truth.py
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.750891 geneparse-0.8.2/geneparse/tools/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     1165 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tools/__init__.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     4116 2018-04-04 14:57:22.000000 geneparse-0.8.2/geneparse/tools/compare_calls.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     9935 2022-02-28 14:07:23.000000 geneparse-0.8.2/geneparse/utils.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)       69 2023-05-19 18:14:02.000000 geneparse-0.8.2/geneparse/version.py
+drwxr-x---   0 lemieuxl (12551) pgx      (35376)        0 2023-05-19 18:14:02.747891 geneparse-0.8.2/geneparse.egg-info/
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      806 2023-05-19 18:14:02.000000 geneparse-0.8.2/geneparse.egg-info/PKG-INFO
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     2421 2023-05-19 18:14:02.000000 geneparse-0.8.2/geneparse.egg-info/SOURCES.txt
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)        1 2023-05-19 18:14:02.000000 geneparse-0.8.2/geneparse.egg-info/dependency_links.txt
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)        1 2018-05-10 16:38:41.000000 geneparse-0.8.2/geneparse.egg-info/not-zip-safe
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)       93 2023-05-19 18:14:02.000000 geneparse-0.8.2/geneparse.egg-info/requires.txt
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)       10 2023-05-19 18:14:02.000000 geneparse-0.8.2/geneparse.egg-info/top_level.txt
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)       38 2023-05-19 18:14:02.750891 geneparse-0.8.2/setup.cfg
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)     2687 2023-05-19 18:10:20.000000 geneparse-0.8.2/setup.py
+-rw-r-----   0 lemieuxl (12551) pgx      (35376)      270 2023-05-19 18:10:20.000000 geneparse-0.8.2/tox.ini
```

### Comparing `geneparse-0.8.1/LICENSE` & `geneparse-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/PKG-INFO` & `geneparse-0.8.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: geneparse
-Version: 0.8.1
+Version: 0.8.2
 Summary: A suite of parse for genotype formats.
 Home-page: https://github.com/pgxcentre/geneparse
-Author: UNKNOWN
-Author-email: UNKNOWN
 License: MIT
-Description: UNKNOWN
 Keywords: bioinformatics genetics statistics
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+License-File: LICENSE
```

### Comparing `geneparse-0.8.1/README.md` & `geneparse-0.8.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![PyPI version](https://badge.fury.io/py/geneparse.svg)](http://badge.fury.io/py/geneparse)
-[![Build Status](https://travis-ci.org/pgxcentre/geneparse.svg?branch=master)](https://travis-ci.org/pgxcentre/geneparse)
+[![Build Status](https://github.com/pgxcentre/geneparse/actions/workflows/python-app.yml/badge.svg?branch=master)](https://github.com/pgxcentre/geneparse/actions)
 
 
 # geneparse - Module to parse genetics data file
 
 `geneparse` is a module that helps developers to parse multiple genetics file
 format (*e.g.* Plink binary files, IMPUTE2 files, BGEN and VCF).
```

### Comparing `geneparse-0.8.1/geneparse/__init__.py` & `geneparse-0.8.2/geneparse/__init__.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/config.py` & `geneparse-0.8.2/geneparse/config.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/core.py` & `geneparse-0.8.2/geneparse/core.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/exceptions.py` & `geneparse-0.8.2/geneparse/exceptions.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/extract/__init__.py` & `geneparse-0.8.2/geneparse/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/extract/__main__.py` & `geneparse-0.8.2/geneparse/extract/__main__.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/extract/extractor.py` & `geneparse-0.8.2/geneparse/extract/extractor.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/index/__init__.py` & `geneparse-0.8.2/geneparse/index/__init__.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/index/__main__.py` & `geneparse-0.8.2/geneparse/index/__main__.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/index/impute2.py` & `geneparse-0.8.2/geneparse/index/impute2.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/logging.py` & `geneparse-0.8.2/geneparse/logging.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/readers/__init__.py` & `geneparse-0.8.2/geneparse/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/readers/bgen.py` & `geneparse-0.8.2/geneparse/readers/bgen.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/readers/dataframe.py` & `geneparse-0.8.2/geneparse/readers/dataframe.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/readers/dict_based.py` & `geneparse-0.8.2/geneparse/readers/dict_based.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/readers/impute2.py` & `geneparse-0.8.2/geneparse/readers/impute2.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,19 +127,19 @@
                 # The dictionary that will contain information about the
                 # duplicated markers
                 self._dup_markers = {
                     m: [] for m in duplicated_marker_counts.index
                 }
 
                 # Logging a warning
-                logging.found_duplicates(duplicated_marker_counts.iteritems())
+                logging.found_duplicates(duplicated_marker_counts.items())
 
                 # Renaming the markers
                 counter = Counter()
-                for i, marker in duplicated_markers.iteritems():
+                for i, marker in duplicated_markers.items():
                     counter[marker] += 1
                     new_name = "{}:dup{}".format(marker, counter[marker])
                     self._impute2_index.loc[i, "name"] = new_name
 
                     # Updating the dictionary containing the duplicated markers
                     self._dup_markers[marker].append(new_name)
```

### Comparing `geneparse-0.8.1/geneparse/readers/plink.py` & `geneparse-0.8.2/geneparse/readers/plink.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/readers/vcf.py` & `geneparse-0.8.2/geneparse/readers/vcf.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/testing/__init__.py` & `geneparse-0.8.2/geneparse/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/testing/simulation.py` & `geneparse-0.8.2/geneparse/testing/simulation.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/__init__.py` & `geneparse-0.8.2/geneparse/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/__main__.py` & `geneparse-0.8.2/geneparse/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/data/impute2/generate_impute2_from_plink.py` & `geneparse-0.8.2/geneparse/tests/data/impute2/generate_impute2_from_plink.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/data/ld/common_extracted_1kg.bed` & `geneparse-0.8.2/geneparse/tests/data/ld/common_extracted_1kg.bed`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/data/ld/common_extracted_1kg.bim` & `geneparse-0.8.2/geneparse/tests/data/ld/common_extracted_1kg.bim`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/data/ld/common_extracted_1kg.fam` & `geneparse-0.8.2/geneparse/tests/data/ld/common_extracted_1kg.fam`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/data/ld/common_extracted_1kg.missing.bed` & `geneparse-0.8.2/geneparse/tests/data/ld/common_extracted_1kg.missing.bed`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/data/ld/common_extracted_1kg.missing.bim` & `geneparse-0.8.2/geneparse/tests/data/ld/common_extracted_1kg.missing.bim`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/data/ld/common_extracted_1kg.missing.fam` & `geneparse-0.8.2/geneparse/tests/data/ld/common_extracted_1kg.missing.fam`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/data/ld/plink_rs1800775_pairs.ld` & `geneparse-0.8.2/geneparse/tests/data/ld/plink_rs1800775_pairs.ld`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/data/ld/plink_rs1800775_pairs.missing.ld` & `geneparse-0.8.2/geneparse/tests/data/ld/plink_rs1800775_pairs.missing.ld`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/data/vcf/test.vcf.gz` & `geneparse-0.8.2/geneparse/tests/data/vcf/test.vcf.gz`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/generic_tests.py` & `geneparse-0.8.2/geneparse/tests/generic_tests.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/test_bgen.py` & `geneparse-0.8.2/geneparse/tests/test_bgen.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/test_core.py` & `geneparse-0.8.2/geneparse/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/test_dataframe.py` & `geneparse-0.8.2/geneparse/tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/test_dict_based_reader.py` & `geneparse-0.8.2/geneparse/tests/test_dict_based_reader.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/test_extractor.py` & `geneparse-0.8.2/geneparse/tests/test_extractor.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/test_genotypes.py` & `geneparse-0.8.2/geneparse/tests/test_genotypes.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/test_impute2.py` & `geneparse-0.8.2/geneparse/tests/test_impute2.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/test_plink.py` & `geneparse-0.8.2/geneparse/tests/test_plink.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/test_serialization.py` & `geneparse-0.8.2/geneparse/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/test_testing.py` & `geneparse-0.8.2/geneparse/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/test_utils.py` & `geneparse-0.8.2/geneparse/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/test_variants.py` & `geneparse-0.8.2/geneparse/tests/test_variants.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/test_vcf.py` & `geneparse-0.8.2/geneparse/tests/test_vcf.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tests/truth.py` & `geneparse-0.8.2/geneparse/tests/truth.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tools/__init__.py` & `geneparse-0.8.2/geneparse/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/tools/compare_calls.py` & `geneparse-0.8.2/geneparse/tools/compare_calls.py`

 * *Files identical despite different names*

### Comparing `geneparse-0.8.1/geneparse/utils.py` & `geneparse-0.8.2/geneparse/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # THE SOFTWARE.
 
 
 import urllib
 import json
 import logging
 import warnings
+from typing import List
 
 import numpy as np
 import pandas as pd
 
 from .core import Variant
 from . import parsers
 
@@ -81,14 +82,33 @@
     if maf > 0.5:
         maf = 1 - maf
         return maf, False
 
     return maf, True
 
 
+def variants_to_df(variants: List[Variant],
+                   make_id: bool = False) -> pd.DataFrame:
+    """Create a pandas dataframe from a list of variants."""
+    df = pd.DataFrame.from_records(
+        [
+            (v.name, v.chrom, v.pos, v.alleles[0], v.alleles[1])
+            for v in variants
+        ],
+        columns=["name", "chrom", "pos", "allele1", "allele2"]
+    )
+
+    # ID that can be used for fast joining.
+    if make_id:
+        meta = df.drop(columns="name").astype(str)
+        df["geneparse_id"] = meta.agg("-".join, axis=1)
+
+    return df
+
+
 def rsids_to_variants(li):
     url = "http://grch37.rest.ensembl.org/variation/homo_sapiens"
 
     req = urllib.request.Request(
         url=url,
         data=json.dumps({"ids": li}).encode("utf-8"),
         headers={
```

### Comparing `geneparse-0.8.1/geneparse.egg-info/PKG-INFO` & `geneparse-0.8.2/geneparse.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: geneparse
-Version: 0.8.1
+Version: 0.8.2
 Summary: A suite of parse for genotype formats.
 Home-page: https://github.com/pgxcentre/geneparse
-Author: UNKNOWN
-Author-email: UNKNOWN
 License: MIT
-Description: UNKNOWN
 Keywords: bioinformatics genetics statistics
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+License-File: LICENSE
```

### Comparing `geneparse-0.8.1/geneparse.egg-info/SOURCES.txt` & `geneparse-0.8.2/geneparse.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+.coveragerc
+.gitignore
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+tox.ini
+.github/workflows/python-app.yml
 geneparse/__init__.py
 geneparse/config.py
 geneparse/core.py
 geneparse/exceptions.py
 geneparse/logging.py
+geneparse/match_genotype_iterators.py
 geneparse/utils.py
 geneparse/version.py
 geneparse.egg-info/PKG-INFO
 geneparse.egg-info/SOURCES.txt
 geneparse.egg-info/dependency_links.txt
 geneparse.egg-info/not-zip-safe
 geneparse.egg-info/requires.txt
```

### Comparing `geneparse-0.8.1/setup.py` & `geneparse-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import sys
 
 from setuptools import setup, find_packages
 
 
 MAJOR = 0
 MINOR = 8
-MICRO = 1
+MICRO = 2
 VERSION = "{0}.{1}.{2}".format(MAJOR, MINOR, MICRO)
 
 
 def check_python_version():
     """Checks the python version, exits if < 3.4."""
     python_major, python_minor = sys.version_info[:2]
```

