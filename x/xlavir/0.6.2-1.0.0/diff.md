# Comparing `tmp/xlavir-0.6.2.tar.gz` & `tmp/xlavir-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlavir-0.6.2.tar", last modified: Fri Mar 18 15:36:04 2022, max compression
+gzip compressed data, was "xlavir-1.0.0.tar", last modified: Fri May 19 16:57:41 2023, max compression
```

## Comparing `xlavir-0.6.2.tar` & `xlavir-1.0.0.tar`

### file list

```diff
@@ -1,97 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.013614 xlavir-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-03-18 15:35:53.000000 xlavir-0.6.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3496 2022-03-18 15:35:53.000000 xlavir-0.6.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6535 2022-03-18 15:35:53.000000 xlavir-0.6.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-03-18 15:35:53.000000 xlavir-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-03-18 15:35:53.000000 xlavir-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9529 2022-03-18 15:36:04.013614 xlavir-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2205 2022-03-18 15:35:53.000000 xlavir-0.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.005613 xlavir-0.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-03-18 15:35:53.000000 xlavir-0.6.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-18 15:35:53.000000 xlavir-0.6.2/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     4781 2022-03-18 15:35:53.000000 xlavir-0.6.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-03-18 15:35:53.000000 xlavir-0.6.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-03-18 15:35:53.000000 xlavir-0.6.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-03-18 15:35:53.000000 xlavir-0.6.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-03-18 15:35:53.000000 xlavir-0.6.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-03-18 15:35:53.000000 xlavir-0.6.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-03-18 15:35:53.000000 xlavir-0.6.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-03-18 15:35:53.000000 xlavir-0.6.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-03-18 15:36:04.013614 xlavir-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-03-18 15:35:53.000000 xlavir-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.005613 xlavir-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.001613 xlavir-0.6.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.005613 xlavir-0.6.2/tests/data/images/
--rw-r--r--   0 runner    (1001) docker     (121)    23422 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/images/190px-Arthur-Pyle_Excalibur_the_Sword.JPG
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.005613 xlavir-0.6.2/tests/data/io/
--rw-r--r--   0 runner    (1001) docker     (121)     8116 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/io/ct.ods
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/io/ct.tsv
--rw-r--r--   0 runner    (1001) docker     (121)     4778 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/io/ct.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.001613 xlavir-0.6.2/tests/data/tools/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.005613 xlavir-0.6.2/tests/data/tools/consensus/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/consensus/Sample1.consensus.fa
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/consensus/Sample2.consensus.fa
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/consensus/Sample3.consensus.fa
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.005613 xlavir-0.6.2/tests/data/tools/fastp/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/fastp/Sample1.fastp.json
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/fastp/Sample2.fastp.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.005613 xlavir-0.6.2/tests/data/tools/mosdepth/
--rw-r--r--   0 runner    (1001) docker     (121)    75574 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/mosdepth/Sample1.per-base.bed.gz
--rw-r--r--   0 runner    (1001) docker     (121)   107366 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/mosdepth/Sample2.per-base.bed.gz
--rw-r--r--   0 runner    (1001) docker     (121)   104812 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/mosdepth/Sample3.per-base.bed.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.005613 xlavir-0.6.2/tests/data/tools/nextflow/
--rw-r--r--   0 runner    (1001) docker     (121)  3051711 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/nextflow/execution_report.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.009614 xlavir-0.6.2/tests/data/tools/pangolin/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/pangolin/pangolin.lineage_report.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.009614 xlavir-0.6.2/tests/data/tools/samtools/
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/samtools/Sample1.flagstat
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/samtools/Sample2.flagstat
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/samtools/Sample3.flagstat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.001613 xlavir-0.6.2/tests/data/tools/variants/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.009614 xlavir-0.6.2/tests/data/tools/variants/ivar/
--rwxr-xr-x   0 runner    (1001) docker     (121)     7170 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/variants/ivar/Sample3.snpsift.txt
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/variants/ivar/Sample3.vcf.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.009614 xlavir-0.6.2/tests/data/tools/variants/nanopolish/
--rwxr-xr-x   0 runner    (1001) docker     (121)      887 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/variants/nanopolish/Sample1.pass.vcf.gz
--rwxr-xr-x   0 runner    (1001) docker     (121)     1568 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/variants/nanopolish/Sample1.snpsift.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     2195 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/variants/nanopolish/Sample2.pass.vcf.gz
--rwxr-xr-x   0 runner    (1001) docker     (121)    21406 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/data/tools/variants/nanopolish/Sample2.snpsift.txt
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/test_io_ct.py
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/test_tools_fastp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/test_tools_nextflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-03-18 15:35:53.000000 xlavir-0.6.2/tests/test_xlavir.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.009614 xlavir-0.6.2/xlavir/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5722 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/images.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.013614 xlavir-0.6.2/xlavir/io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/io/ct.py
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/io/excel_sheet_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (121)    21566 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/io/xl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.013614 xlavir-0.6.2/xlavir/qc/
--rw-r--r--   0 runner    (1001) docker     (121)     4993 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/qc/quality_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.013614 xlavir-0.6.2/xlavir/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/tools/consensus.py
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/tools/fastp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3466 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/tools/mosdepth.py
--rw-r--r--   0 runner    (1001) docker     (121)     7352 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/tools/nextclade.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.013614 xlavir-0.6.2/xlavir/tools/nextflow/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/tools/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/tools/nextflow/exec_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     3506 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/tools/pangolin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/tools/samtools.py
--rw-r--r--   0 runner    (1001) docker     (121)    24747 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/tools/variants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4023 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     6683 2022-03-18 15:35:53.000000 xlavir-0.6.2/xlavir/xlavir.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 15:36:04.013614 xlavir-0.6.2/xlavir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9529 2022-03-18 15:36:03.000000 xlavir-0.6.2/xlavir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-03-18 15:36:03.000000 xlavir-0.6.2/xlavir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-18 15:36:03.000000 xlavir-0.6.2/xlavir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-03-18 15:36:03.000000 xlavir-0.6.2/xlavir.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-18 15:36:03.000000 xlavir-0.6.2/xlavir.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-03-18 15:36:03.000000 xlavir-0.6.2/xlavir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-18 15:36:03.000000 xlavir-0.6.2/xlavir.egg-info/top_level.txt
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.353814 xlavir-1.0.0/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     1077 2021-02-16 18:28:39.000000 xlavir-1.0.0/LICENSE
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)      242 2023-05-19 15:00:54.000000 xlavir-1.0.0/MANIFEST.in
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     5897 2023-05-19 16:57:41.353814 xlavir-1.0.0/PKG-INFO
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     3347 2023-05-19 15:48:16.000000 xlavir-1.0.0/README.md
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     2091 2023-05-19 15:53:53.000000 xlavir-1.0.0/pyproject.toml
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)       38 2023-05-19 16:57:41.353814 xlavir-1.0.0/setup.cfg
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.340481 xlavir-1.0.0/tests/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)      123 2021-07-30 18:52:06.000000 xlavir-1.0.0/tests/.~lock.xlavir-report.xlsx#
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)       36 2021-02-16 18:28:39.000000 xlavir-1.0.0/tests/__init__.py
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.333814 xlavir-1.0.0/tests/data/
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.340481 xlavir-1.0.0/tests/data/images/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)    23422 2018-07-21 18:09:10.000000 xlavir-1.0.0/tests/data/images/190px-Arthur-Pyle_Excalibur_the_Sword.JPG
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.340481 xlavir-1.0.0/tests/data/io/
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.340481 xlavir-1.0.0/tests/data/io/.ipynb_checkpoints/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)       72 2021-04-23 14:04:25.000000 xlavir-1.0.0/tests/data/io/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)    78325 2021-04-23 17:50:32.000000 xlavir-1.0.0/tests/data/io/Untitled.ipynb
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     8116 2021-04-23 16:08:06.000000 xlavir-1.0.0/tests/data/io/ct.ods
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)       47 2021-04-23 16:08:06.000000 xlavir-1.0.0/tests/data/io/ct.tsv
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     4778 2021-04-23 16:08:06.000000 xlavir-1.0.0/tests/data/io/ct.xlsx
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.333814 xlavir-1.0.0/tests/data/tools/
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.343814 xlavir-1.0.0/tests/data/tools/consensus/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)       16 2021-02-19 22:27:43.000000 xlavir-1.0.0/tests/data/tools/consensus/Sample1.consensus.fa
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)       16 2021-02-19 22:27:43.000000 xlavir-1.0.0/tests/data/tools/consensus/Sample2.consensus.fa
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)       16 2021-02-19 22:27:43.000000 xlavir-1.0.0/tests/data/tools/consensus/Sample3.consensus.fa
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.343814 xlavir-1.0.0/tests/data/tools/fastp/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)       96 2021-10-29 12:45:30.000000 xlavir-1.0.0/tests/data/tools/fastp/Sample1.fastp.json
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)       93 2021-10-29 12:45:30.000000 xlavir-1.0.0/tests/data/tools/fastp/Sample2.fastp.json
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.343814 xlavir-1.0.0/tests/data/tools/mosdepth/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)    75574 2021-02-17 22:20:17.000000 xlavir-1.0.0/tests/data/tools/mosdepth/Sample1.per-base.bed.gz
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)   107366 2021-02-17 22:22:51.000000 xlavir-1.0.0/tests/data/tools/mosdepth/Sample2.per-base.bed.gz
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)   104812 2021-02-17 22:22:47.000000 xlavir-1.0.0/tests/data/tools/mosdepth/Sample3.per-base.bed.gz
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.343814 xlavir-1.0.0/tests/data/tools/nextflow/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)  3051711 2021-02-19 21:16:11.000000 xlavir-1.0.0/tests/data/tools/nextflow/execution_report.html
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.347147 xlavir-1.0.0/tests/data/tools/pangolin/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)      177 2021-02-19 21:27:17.000000 xlavir-1.0.0/tests/data/tools/pangolin/pangolin.lineage_report.csv
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.347147 xlavir-1.0.0/tests/data/tools/samtools/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)      387 2021-02-19 21:30:02.000000 xlavir-1.0.0/tests/data/tools/samtools/Sample1.flagstat
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)      388 2021-02-19 21:30:02.000000 xlavir-1.0.0/tests/data/tools/samtools/Sample2.flagstat
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)      388 2021-02-19 21:30:02.000000 xlavir-1.0.0/tests/data/tools/samtools/Sample3.flagstat
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.333814 xlavir-1.0.0/tests/data/tools/variants/
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.347147 xlavir-1.0.0/tests/data/tools/variants/ivar/
+-rwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)     7170 2021-10-29 12:45:30.000000 xlavir-1.0.0/tests/data/tools/variants/ivar/Sample3.snpsift.txt
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)      873 2021-10-29 12:45:30.000000 xlavir-1.0.0/tests/data/tools/variants/ivar/Sample3.vcf.gz
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.350481 xlavir-1.0.0/tests/data/tools/variants/nanopolish/
+-rwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)      887 2021-08-03 15:14:34.000000 xlavir-1.0.0/tests/data/tools/variants/nanopolish/Sample1.pass.vcf.gz
+-rwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)     1568 2021-08-03 15:14:34.000000 xlavir-1.0.0/tests/data/tools/variants/nanopolish/Sample1.snpsift.txt
+-rwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)     2195 2021-08-03 15:14:34.000000 xlavir-1.0.0/tests/data/tools/variants/nanopolish/Sample2.pass.vcf.gz
+-rwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)    21406 2021-08-03 15:14:34.000000 xlavir-1.0.0/tests/data/tools/variants/nanopolish/Sample2.snpsift.txt
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.337147 xlavir-1.0.0/tests/data/vcfs/
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.350481 xlavir-1.0.0/tests/data/vcfs/bcftools/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)    19434 2023-05-18 19:24:49.000000 xlavir-1.0.0/tests/data/vcfs/bcftools/Sample1.vcf
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.350481 xlavir-1.0.0/tests/data/vcfs/clair3/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)    15237 2023-05-11 17:14:30.000000 xlavir-1.0.0/tests/data/vcfs/clair3/Sample1.clair3.vcf
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.350481 xlavir-1.0.0/tests/data/vcfs/ivar/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)    10492 2023-05-18 19:28:41.000000 xlavir-1.0.0/tests/data/vcfs/ivar/Sample1.vcf
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)      469 2021-04-23 16:08:06.000000 xlavir-1.0.0/tests/test_io_ct.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)      421 2021-10-29 12:45:30.000000 xlavir-1.0.0/tests/test_tools_fastp.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     1381 2021-02-19 21:25:20.000000 xlavir-1.0.0/tests/test_tools_nextflow.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     1453 2023-05-18 19:29:14.000000 xlavir-1.0.0/tests/test_vcf_parsing.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     1041 2023-05-16 20:06:46.000000 xlavir-1.0.0/tests/test_xlavir.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)    33315 2021-07-30 18:51:51.000000 xlavir-1.0.0/tests/xlavir-report.xlsx
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.350481 xlavir-1.0.0/xlavir/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)      130 2023-05-18 22:33:21.000000 xlavir-1.0.0/xlavir/__init__.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     5661 2023-05-10 21:22:55.000000 xlavir-1.0.0/xlavir/cli.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)      954 2021-02-19 22:06:49.000000 xlavir-1.0.0/xlavir/images.py
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.350481 xlavir-1.0.0/xlavir/io/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)        0 2021-02-19 22:43:25.000000 xlavir-1.0.0/xlavir/io/__init__.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     1575 2023-05-18 18:58:02.000000 xlavir-1.0.0/xlavir/io/ct.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     1107 2023-05-18 19:43:02.000000 xlavir-1.0.0/xlavir/io/excel_sheet_dataframe.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)    21781 2023-05-19 15:44:46.000000 xlavir-1.0.0/xlavir/io/xl.py
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.350481 xlavir-1.0.0/xlavir/qc/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     5195 2023-05-19 16:07:37.000000 xlavir-1.0.0/xlavir/qc/__init__.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)      213 2021-02-20 04:51:07.000000 xlavir-1.0.0/xlavir/qc/quality_requirements.py
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.353814 xlavir-1.0.0/xlavir/tools/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)        0 2021-02-16 20:52:31.000000 xlavir-1.0.0/xlavir/tools/__init__.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     2027 2023-05-10 21:36:24.000000 xlavir-1.0.0/xlavir/tools/consensus.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     1077 2023-05-18 19:00:01.000000 xlavir-1.0.0/xlavir/tools/fastp.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     5658 2023-05-18 22:24:55.000000 xlavir-1.0.0/xlavir/tools/mosdepth.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     7518 2023-05-10 21:25:43.000000 xlavir-1.0.0/xlavir/tools/nextclade.py
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.353814 xlavir-1.0.0/xlavir/tools/nextflow/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)        0 2021-02-16 21:43:52.000000 xlavir-1.0.0/xlavir/tools/nextflow/__init__.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     4141 2023-01-24 22:29:30.000000 xlavir-1.0.0/xlavir/tools/nextflow/exec_report.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     3511 2023-01-24 22:36:40.000000 xlavir-1.0.0/xlavir/tools/pangolin.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     1821 2023-01-24 20:24:10.000000 xlavir-1.0.0/xlavir/tools/samtools.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)    28761 2023-05-18 19:17:54.000000 xlavir-1.0.0/xlavir/tools/variants.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     4142 2023-05-19 16:27:46.000000 xlavir-1.0.0/xlavir/util.py
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     6710 2023-05-18 18:59:25.000000 xlavir-1.0.0/xlavir/xlavir.py
+drwxr-xr-x   0 pkruczkiewicz  (1001) users      (985)        0 2023-05-19 16:57:41.350481 xlavir-1.0.0/xlavir.egg-info/
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     5897 2023-05-19 16:57:41.000000 xlavir-1.0.0/xlavir.egg-info/PKG-INFO
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)     2179 2023-05-19 16:57:41.000000 xlavir-1.0.0/xlavir.egg-info/SOURCES.txt
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)        1 2023-05-19 16:57:41.000000 xlavir-1.0.0/xlavir.egg-info/dependency_links.txt
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)       42 2023-05-19 16:57:41.000000 xlavir-1.0.0/xlavir.egg-info/entry_points.txt
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)      167 2023-05-19 16:57:41.000000 xlavir-1.0.0/xlavir.egg-info/requires.txt
+-rw-r--r--   0 pkruczkiewicz  (1001) users      (985)        7 2023-05-19 16:57:41.000000 xlavir-1.0.0/xlavir.egg-info/top_level.txt
```

### Comparing `xlavir-0.6.2/LICENSE` & `xlavir-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/setup.py` & `xlavir-1.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,95 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-from setuptools import setup, find_packages
-
-with open('README.rst') as readme_file:
-    readme = readme_file.read()
-
-with open('HISTORY.rst') as history_file:
-    history = history_file.read()
+[project]
+name = "xlavir"
+version = "1.0.0"
+description = "Excel report from viral sequencing analysis output"
+authors = [
+    { name = "Peter Kruczkiewicz", email = "peter.kruczkiewicz@gmail.com" }
+]
+keywords = [
+    "bioinformatics",
+    "nextflow",
+    "virus sequencing",
+    "excel report",
+]
+license = { file = "LICENSE" }
+readme = { file = "README.md", content-type = "text/markdown"}
+requires-python = ">=3.8"
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Console",
+    "Intended Audience :: Science/Research",
+    'License :: OSI Approved :: MIT License',
+    'Natural Language :: English',
+    'Programming Language :: Python :: 3',
+    "Programming Language :: Python :: 3 :: Only",
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Unix Shell',
+    'Topic :: Scientific/Engineering :: Bio-Informatics',
+    'Topic :: Utilities',
+    "Operating System :: POSIX :: Linux",
+]
 
-requirements = [
+dependencies = [
     'typer',
     'rich',
     'pandas',
     'numpy>=1.20.0',
     'xlsxwriter',
     'pydantic',
     'beautifulsoup4',
     'biopython',
     'openpyxl',
     'imageio',
     'odfpy',
+    'pysam',
+]
+
+[project.optional-dependencies]
+dev = [
+    "twine",
+    "wheel",
+    "ruff",
+    "mypy"
+]
+
+test = [
+    "pytest>=3",
+    "pytest-runner",
+]
+
+[tool.setuptools]
+py-modules = ["xlavir"]
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+filterwarnings = [
+    "ignore:.*PytestConfigWarning.*Unknown config option.*",
+    "ignore::UserWarning",
+]
+
+[tool.ruff]
+line-length = 120
+
+[tool.mypy]
+files = ["xlavir", "tests"]
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = [
+    "openpyxl",
+    "pandas",
 ]
 
-setup_requirements = ['pytest-runner', ]
+[project.scripts]
+xlavir = "xlavir.cli:app"
 
-test_requirements = ['pytest>=3', ]
+[project.urls]
+"Homepage" = "https://github.com/CFIA-NCFAD/xlavir"
+"Repository" = "https://github.com/CFIA-NCFAD/xlavir.git"
+"Bug Tracker" = "https://github.com/CFIA-NCFAD/xlavir/issues"
 
-setup(
-    author="Peter Kruczkiewicz",
-    author_email='peter.kruczkiewicz@gmail.com',
-    python_requires='>=3.5',
-    classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-    ],
-    description="Excel report from viral sequencing analysis output",
-    entry_points={
-        'console_scripts': [
-            'xlavir=xlavir.cli:app',
-        ],
-    },
-    install_requires=requirements,
-    license="MIT license",
-    long_description=readme + '\n\n' + history,
-    include_package_data=True,
-    keywords='xlavir',
-    name='xlavir',
-    packages=find_packages(include=['xlavir', 'xlavir.*']),
-    setup_requires=setup_requirements,
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/peterk87/xlavir',
-    version='0.6.2',
-    zip_safe=False,
-)
+[build-system]
+requires = ["setuptools", "wheel"]
```

### Comparing `xlavir-0.6.2/tests/data/images/190px-Arthur-Pyle_Excalibur_the_Sword.JPG` & `xlavir-1.0.0/tests/data/images/190px-Arthur-Pyle_Excalibur_the_Sword.JPG`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/tests/data/io/ct.ods` & `xlavir-1.0.0/tests/data/io/ct.ods`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/tests/data/io/ct.xlsx` & `xlavir-1.0.0/tests/data/io/ct.xlsx`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/tests/data/tools/mosdepth/Sample1.per-base.bed.gz` & `xlavir-1.0.0/tests/data/tools/mosdepth/Sample1.per-base.bed.gz`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/tests/data/tools/mosdepth/Sample2.per-base.bed.gz` & `xlavir-1.0.0/tests/data/tools/mosdepth/Sample2.per-base.bed.gz`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/tests/data/tools/mosdepth/Sample3.per-base.bed.gz` & `xlavir-1.0.0/tests/data/tools/mosdepth/Sample3.per-base.bed.gz`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/tests/data/tools/nextflow/execution_report.html` & `xlavir-1.0.0/tests/data/tools/nextflow/execution_report.html`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/tests/data/tools/variants/ivar/Sample3.snpsift.txt` & `xlavir-1.0.0/tests/data/tools/variants/ivar/Sample3.snpsift.txt`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/tests/data/tools/variants/ivar/Sample3.vcf.gz` & `xlavir-1.0.0/tests/data/tools/variants/ivar/Sample3.vcf.gz`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/tests/data/tools/variants/nanopolish/Sample1.pass.vcf.gz` & `xlavir-1.0.0/tests/data/tools/variants/nanopolish/Sample1.pass.vcf.gz`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/tests/data/tools/variants/nanopolish/Sample1.snpsift.txt` & `xlavir-1.0.0/tests/data/tools/variants/nanopolish/Sample1.snpsift.txt`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/tests/data/tools/variants/nanopolish/Sample2.pass.vcf.gz` & `xlavir-1.0.0/tests/data/tools/variants/nanopolish/Sample2.pass.vcf.gz`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/tests/data/tools/variants/nanopolish/Sample2.snpsift.txt` & `xlavir-1.0.0/tests/data/tools/variants/nanopolish/Sample2.snpsift.txt`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/tests/test_tools_nextflow.py` & `xlavir-1.0.0/tests/test_tools_nextflow.py`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/tests/test_xlavir.py` & `xlavir-1.0.0/tests/test_xlavir.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 test_image = dirpath / 'data/images/190px-Arthur-Pyle_Excalibur_the_Sword.JPG'
 
 
 def test_command_line_interface():
     """Test the CLI."""
     result = runner.invoke(app)
     assert result.exit_code != 0
-    assert 'Error: Missing argument' in result.output
+    assert 'Missing argument' in result.output
     help_result = runner.invoke(app, ['--help'])
     assert help_result.exit_code == 0
-    assert 'Show this message and exit.' in help_result.output
+    assert 'Usage: ' in help_result.output
     with runner.isolated_filesystem():
         out_report = 'report.xlsx'
         result = runner.invoke(app, [str((dirpath / 'data').resolve().absolute()), out_report])
         if result.exception:
             raise result.exception
         assert result.exit_code == 0
         assert Path(out_report).exists()
```

### Comparing `xlavir-0.6.2/xlavir/cli.py` & `xlavir-1.0.0/xlavir/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,21 +86,24 @@
 
     Specify report output filename:
 
     $ xlavir /path/to/viralrecon-or-virontus-results xlavir-run-XXXX.xlsx
 
     """
     from rich.traceback import install
-    install(show_locals=True, width=120, word_wrap=True)
+    install(show_locals=True, width=240, word_wrap=True)
 
-    logging.basicConfig(format='%(message)s',
-                        datefmt='[%Y-%m-%d %X]',
-                        level=logging.INFO if not verbose else logging.DEBUG,
-                        handlers=[RichHandler(rich_tracebacks=True,
-                                              tracebacks_show_locals=True)])
+    logging.basicConfig(
+        format='%(message)s',
+        datefmt='[%Y-%m-%d %X]',
+        level=logging.DEBUG if verbose else logging.INFO,
+        handlers=[
+            RichHandler(rich_tracebacks=True, tracebacks_show_locals=True)
+        ],
+    )
 
     images_for_sheets = None
     if image:
         images_for_sheets = get_images_for_sheets(image, image_title, image_description)
 
     quality_reqs = qc_presets[QCPresets.default.value]
     if qc_preset:
```

### Comparing `xlavir-0.6.2/xlavir/images.py` & `xlavir-1.0.0/xlavir/images.py`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/xlavir/io/ct.py` & `xlavir-1.0.0/xlavir/io/ct.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def validate_ct_table(df: pd.DataFrame) -> bool:
     if df.empty:
-        logger.error(f'Ct values table is empty! No Ct values present!')
+        logger.error('Ct values table is empty! No Ct values present!')
         return False
     n_rows, n_cols = df.shape
     if n_cols != 2:
         logger.error(
-            f'Ct values table expected to only have 2 columns, but {n_cols} were found with names: {", ".join(df.columns)}')
+            f'Ct values table expected to only have 2 columns, but {n_cols} '
+            f'were found with names: {", ".join(df.columns)}'
+        )
         return False
     return True
 
 
 def read_ct_table(ct_path: Path) -> Dict[str, float]:
     suffix = ct_path.suffix.lower()
     if suffix == '.txt':
```

### Comparing `xlavir-0.6.2/xlavir/io/excel_sheet_dataframe.py` & `xlavir-1.0.0/xlavir/io/excel_sheet_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     varmat = 'Variant Matrix'
     nextclade = 'Nextclade'
     xlavir_info = 'xlavir info'
 
 
 class ExcelSheetDataFrame:
     def __init__(self,
-                 sheet_name: SheetName,
+                 sheet_name: str,
                  df: pd.DataFrame,
                  pd_to_excel_kwargs: dict = None,
                  autofit: bool = True,
                  column_widths: Optional[Iterable[Union[int, float]]] = None,
                  include_header_width: bool = True,
                  header_comments: Optional[Mapping[str, str]] = None):
         self.include_header_width = include_header_width
```

### Comparing `xlavir-0.6.2/xlavir/io/xl.py` & `xlavir-1.0.0/xlavir/io/xl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Excel spreadsheet IO functions"""
+
+import contextlib
 import logging
 from copy import copy
 from pathlib import Path
 from typing import List, Optional, Set, Tuple, Dict, Union
 
 import openpyxl
 import pandas as pd
@@ -21,15 +23,15 @@
 def copy_spreadsheet(src_path: Path,
                      dest_path: Path,
                      source_sheet_index: int = 0) -> None:
     """Copy a spreadsheet from a source Excel spreadsheet to a destination spreadsheet.
 
     All cell values and styles are copied over as well as row heights, column widths, merged cells.
 
-    By default the 1st worksheet is copied over.
+    By default, the 1st worksheet is copied over.
 
     Args:
         src_path (Path): Source Excel spreadsheet path
         dest_path (Path): Destination Excel spreadsheet path
         source_sheet_index (int): Source spreadsheet worksheet index to copy to destination spreadsheet
     """
     from openpyxl.cell.cell import Cell
@@ -60,17 +62,21 @@
     dest_book.save(filename=dest_path)
 
 
 def write_xlsx_report(dfs: List[ExcelSheetDataFrame],
                       output_xlsx: Path,
                       quality_reqs: QualityRequirements,
                       images_for_sheets: Optional[List[SheetImage]] = None):
-    """Write the output Excel XLSX file
-
+    """Write the output Excel XLSX file using the given dataframes.
 
+    Args:
+        dfs (List[ExcelSheetDataFrame]): List of ExcelSheetDataFrame objects to write to the output XLSX file
+        output_xlsx (Path): Path to the output XLSX file
+        quality_reqs (QualityRequirements): Quality requirements for the run
+        images_for_sheets (Optional[List[SheetImage]]): List of SheetImage objects to add to the output XLSX file
     """
     with pd.ExcelWriter(output_xlsx, engine='xlsxwriter') as writer:
         monospace = dict(font_name='Courier New')
         text_wrap = dict(text_wrap=True)
         float_1dec = dict(num_format='0.0')
         perc_1dec = dict(num_format='0.0%')
         perc_2dec = dict(num_format='0.00%')
@@ -143,15 +149,15 @@
                         sheet.write_string(0, i, string=col_name, cell_format=header_with_wrap_fmt)
 
             elif esdf.column_widths:
                 for i, (width, col_name) in enumerate(zip(esdf.column_widths, idx_and_cols)):
                     logger.debug(f'{esdf.sheet_name}|Column {col_name} ({i}) width = {width}')
                     sheet.set_column(i, i, width, monospace_wrap_fmt)
 
-                for i, idx in enumerate(esdf.df.index, 1):
+                for i, idx in enumerate(esdf.df.index, start=1):
                     sheet.set_row(i, get_row_heights(esdf.df, idx), monospace_wrap_fmt)
 
             if esdf.sheet_name == SheetName.varmat.value:
                 sheet.write_comment(row=0,
                                     col=0,
                                     comment=f'This sheet contains a matrix of alternate allele variant observation'
                                             f' frequency values for samples and variants. '
@@ -305,16 +311,16 @@
     from openpyxl.comments import Comment
     from openpyxl.styles import PatternFill, Font
     from openpyxl.worksheet.worksheet import Worksheet
     from openpyxl.worksheet.dimensions import ColumnDimension
     logger.info(f'Loading workbook "{xlsx_path.name}" with openpyxl '
                 f'to highlight {len(failed_samples)} samples that have failed QC')
     book = openpyxl.load_workbook(xlsx_path)
-    logger.info(f'Loaded "{xlsx_path.name}" using openpyxl. Sheets: {book.get_sheet_names()}')
-    logger.info(f'Adjusting comment textbox sizes to fit text')
+    logger.info(f'Loaded "{xlsx_path.name}" using openpyxl. Sheets: {book.sheetnames}')
+    logger.info('Adjusting comment textbox sizes to fit text')
     for sheetname in book.sheetnames:
         for row in book[sheetname]:
             for cell in row:
                 if cell.comment:
                     comment: Comment = cell.comment
                     comment.width = 300
                     comment.height = max((100, len(comment.text) / 3 * 2))
@@ -323,105 +329,93 @@
     sheet_names = [
         SheetName.pangolin.value,
         SheetName.variants.value,
         SheetName.varmat.value,
     ]
     light_red = 'FC9295'
     for sheet_name in sheet_names:
-        try:
+        with contextlib.suppress(KeyError):
             sheet: Worksheet = book[sheet_name]
             logger.info(f'Highlighting failed samples in sheet "{sheet_name}".')
             for i, row in enumerate(sheet.rows):
                 if i == 0:
                     continue
                 cell = row[0]
                 if cell.value in failed_samples:
                     cell.comment = Comment(f'Warning: Sample "{cell.value}" has failed general NGS QC',
                                            author='xlavir')
                     cell.fill = PatternFill(fill_type='solid',
                                             fgColor=light_red)
-        except KeyError:
-            pass
-
     esd_varmat = get_excel_sheet_df(esdfs, SheetName.varmat.value)
     esd_variants = get_excel_sheet_df(esdfs, SheetName.variants.value)
     if esd_varmat and esd_variants:
-        try:
+        with contextlib.suppress(KeyError):
             sheet: Worksheet = book[SheetName.varmat.value]
-            logger.info(f'Adding additional comments to variant matrix values')
+            logger.info('Adding additional comments to variant matrix values')
             df_varmat = esd_varmat.df
             variants: Dict[Tuple[str, str], Dict[str, Union[str, float, int]]] = esd_variants \
                 .df.reset_index() \
                 .set_index(['Sample', 'Mutation']) \
                 .to_dict(orient='index')
 
             for i, row in enumerate(sheet.rows):
                 if i == 0:
                     continue
                 sample = df_varmat.index.values[i - 1]
                 for j, cell in enumerate(row):
                     if j == 0:
                         continue
                     mutation = df_varmat.columns.values[j - 1]
-                    variant = variants.get((sample, mutation), None)
-                    if variant:
+                    if variant := variants.get((sample, mutation), None):
                         variant_str = '\n'.join(f'{k}: {v}' for k, v in variant.items())
                         comment_text = f'Sample: {sample}\nMutation: {mutation}\n{variant_str}'
                     else:
                         comment_text = f'Mutation "{mutation}" not found in sample "{sample}"'
                     cell.comment = Comment(comment_text,
                                            author=f'xlavir version {__version__}',
                                            width=300,
                                            height=len(comment_text))
-        except KeyError:
-            pass
-
-    try:
+    with contextlib.suppress(KeyError):
         sheet: Worksheet = book[SheetName.consensus.value]
 
         sheet.column_dimensions['A'] = ColumnDimension(worksheet=sheet,
                                                        index='A',
                                                        width=100)
 
         logger.info(f'Highlighting consensus sequences of failed '
                     f'samples in sheet "{SheetName.consensus.value}".')
         highlight_seq = False
         sample_name = ''
         dark_red = '260000'
-        for i, row in enumerate(sheet.rows):
+        for row in sheet.rows:
             cell = row[0]
+            font: Font = cell.font
             if cell.value[0] == '>':
                 sample_name = cell.value[1:]
                 if sample_name in failed_samples:
                     highlight_seq = True
                     # only add comment to cell containing failing sample fasta header
                     cell.comment = Comment(f'Warning: Sample "{sample_name}" has failed general NGS QC',
                                            author='xlavir')
                     cell.fill = PatternFill(fill_type='solid', fgColor=light_red)
-                    font: Font = cell.font
                     cell.font = Font(name='Courier New',
                                      color=dark_red,
                                      size=font.size,
                                      family=font.family)
                 else:
                     highlight_seq = False
-                    font: Font = cell.font
                     cell.font = Font(name='Courier New',
                                      color='000000',
                                      size=font.size,
                                      family=font.family)
             elif cell.value and highlight_seq:
                 cell.fill = PatternFill(fill_type='solid', fgColor=light_red)
-                font: Font = cell.font
                 cell.font = Font(name='Courier New',
                                  color=dark_red,
                                  size=font.size,
                                  family=font.family)
             else:
-                font: Font = cell.font
                 cell.font = Font(name='Courier New',
                                  color='000000',
                                  size=font.size,
                                  family=font.family)
-    except KeyError:
-        pass
     book.save(xlsx_path)
```

### Comparing `xlavir-0.6.2/xlavir/qc/__init__.py` & `xlavir-1.0.0/xlavir/qc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 from xlavir.qc.quality_requirements import QualityRequirements
 from xlavir.tools import mosdepth, samtools
 
 logger = logging.getLogger(__name__)
 
 
-def columns(low_coverage_threshold: int = 5) -> List[Tuple[str, str]]:
-    return [
+def columns(low_coverage_threshold: int = 5, has_ct = False) -> List[Tuple[str, str, str]]:
+    cols = [
         ('sample', 'Sample', 'Sample name'),
-        ('ct_value', 'Ct Value', 'Real-time PCR Ct value'),
+        ('ct_value', 'Ct Value', 'Real-time PCR Ct value') if has_ct else None,
         (
             'qc_status',
             'QC Status',
             'Quality control status, i.e. PASS or FAIL based on QC criteria '
             'such as minimum mean read depth '
             'or percent of reference genome covered by sequencing'
         ),
@@ -75,14 +75,15 @@
         (
             'low_coverage_coords',
             f'<{low_coverage_threshold}X Coverage Regions',
             f'A list of reference sequence 1-based regions with less than {low_coverage_threshold}'
             f' coverage depth.'
         ),
     ]
+    return [x for x in cols if x is not None]
 
 
 def report_format(df: pd.DataFrame, low_coverage_threshold: int = 5) -> pd.DataFrame:
     output_cols = columns(low_coverage_threshold)
     df.rename(columns={x: y for x, y, _ in output_cols}, inplace=True)
     df.set_index('Sample', inplace=True)
     return df
@@ -95,16 +96,18 @@
     sample_names = set(sample_depth_info.keys()) | set(sample_mapping_info.keys())
     logger.info(f'N samples: {len(sample_names)}')
     merged_stats_info = {}
     for sample in sample_names:
         depth_info = sample_depth_info[sample].dict() if sample in sample_depth_info else {}
         mapping_info = sample_mapping_info[sample].dict() if sample in sample_mapping_info else {}
         merged_stats_info[sample] = {**depth_info, **mapping_info}
-        merged_stats_info[sample]['ct_value'] = sample_cts.get(sample, None)
-    df_stats = pd.DataFrame(merged_stats_info.values())
+        sample_ct = sample_cts.get(sample)
+        if sample_ct is not None:
+            merged_stats_info[sample]['ct_value'] = sample_ct
+    df_stats = pd.DataFrame(list(merged_stats_info.values()))
     mask_pass_depth = (df_stats.median_coverage >= quality_reqs.min_median_depth)
     mask_pass_breadth = (df_stats.genome_coverage >= quality_reqs.min_genome_coverage)
     qc_pass_mask = mask_pass_depth & mask_pass_breadth
     df_stats['qc_status'] = 'FAIL'
     df_stats.loc[qc_pass_mask, 'qc_status'] = 'PASS'
     qc_comments = []
     for i, (pass_depth, pass_breadth) in enumerate(zip(mask_pass_depth, mask_pass_breadth)):
@@ -115,12 +118,15 @@
             comments += [f'Genome coverage below {quality_reqs.min_genome_coverage:.0%}']
         qc_comments.append('; '.join(comments))
     df_stats['qc_comment'] = qc_comments
     df_stats.loc[qc_pass_mask, 'qc_comment'] = ''
     df_stats.sort_values('sample', inplace=True)
 
     present_cols = set(df_stats.columns)
-    output_cols = columns(quality_reqs.low_coverage_threshold)
+    output_cols = columns(
+        quality_reqs.low_coverage_threshold,
+        has_ct=bool(sample_cts)
+    )
     df_stats = df_stats.loc[:, [x for x, y, _ in output_cols if x in present_cols]]
 
     logger.debug(df_stats)
     return df_stats
```

### Comparing `xlavir-0.6.2/xlavir/tools/consensus.py` & `xlavir-1.0.0/xlavir/tools/consensus.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,19 @@
     >>> chunk('x', 80)
     ['x']
     """
     return [s[i:i + n] for i in range(0, len(s), n)]
 
 
 def read_fasta(sample: str, path: Path) -> List[str]:
+    """Read consensus FASTA file into list of strings.
+
+    If consensus sequence is longer than Excel cell character limit (32,767)
+    then split the sequence into 80 character chunks.
+    """
     out = []
     rec: SeqRecord
     for idx, rec in enumerate(SeqIO.parse(path, format='fasta')):
         out.append(f'>{sample}' if idx == 0 else f'>{sample}-{idx}')
         seq = str(rec.seq)
         # if length of seq is over Excel cell character limit (32,767)
         # then chunk seq up into 80 character chunks
@@ -57,8 +62,9 @@
     return df
 
 
 def get_info(basedir: Path) -> pd.DataFrame:
     sample_fasta = find_file_for_each_sample(basedir,
                                              glob_patterns=GLOB_PATTERNS,
                                              sample_name_cleanup=SAMPLE_NAME_CLEANUP)
+    logger.info(f'Found {len(sample_fasta)} consensus FASTA files')
     return fasta_dataframe(sample_fasta)
```

### Comparing `xlavir-0.6.2/xlavir/tools/fastp.py` & `xlavir-1.0.0/xlavir/tools/fastp.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """Parse total number of reads from fastp JSON file"""
     total = 0
     try:
         with open(p) as fh:
             j = json.load(fh)
             total = j['summary']['before_filtering']['total_reads']
     except KeyError as ex:
-        logger.error(f'')
+        logger.error(f'Could not parse total number of reads from "{p}". Error: {ex}')
     return total
 
 
 def get_info(basedir: Path) -> Dict[str, int]:
     out = {}
     sample_fastp = find_file_for_each_sample(basedir,
                                              glob_patterns=GLOB_PATTERNS,
```

### Comparing `xlavir-0.6.2/xlavir/tools/nextclade.py` & `xlavir-1.0.0/xlavir/tools/nextclade.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,15 +243,18 @@
     sample_nextclade = find_file_for_each_sample(basedir=basedir,
                                                  glob_patterns=NEXTCLADE_GLOB_PATTERNS,
                                                  sample_name_cleanup=NEXTCLADE_SAMPLE_NAME_CLEANUP)
     logger.info(f'Found {len(sample_nextclade)} Nextclade CSV files. Parsing...')
     out = {}
     for sample, nextclade_path in sample_nextclade.items():
         out[sample] = read_nextclade_csv(nextclade_path, sample)
+        logger.info(f'Columns: {out[sample].columns}')
     return out
 
 
 def to_dataframe(sample_nextclade: Dict[str, pd.DataFrame]) -> pd.DataFrame:
     df = pd.concat(list(sample_nextclade.values()))
     df.sort_values('Sample', inplace=True)
     df.set_index('Sample', inplace=True)
-    return df[[x for _,x,_ in nextclade_cols if x in df.columns]]
+    ordered_cols = [x for _, x, _ in nextclade_cols if x in df.columns]
+    rest_cols = [x for x in df.columns if x not in ordered_cols]
+    return df[ordered_cols + rest_cols]
```

### Comparing `xlavir-0.6.2/xlavir/tools/pangolin.py` & `xlavir-1.0.0/xlavir/tools/pangolin.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,18 @@
     df.rename(columns={x: y for x, y, _ in pangolin_cols}, inplace=True)
     if sample_name:
         df['Sample'] = sample_name
     df.set_index('Sample', inplace=True)
     return df
 
 
-def get_info(basedir: Path,
-             pangolin_lineage_csv: Optional[Path] = None) -> Optional[pd.DataFrame]:
+def get_info(
+        basedir: Path,
+        pangolin_lineage_csv: Optional[Path] = None
+) -> Optional[pd.DataFrame]:
     if pangolin_lineage_csv:
         return read_pangolin_csv(pangolin_lineage_csv)
     else:
         path = find_pangolin_lineage_csv(basedir)
         if path:
             return read_pangolin_csv(path)
         else:
```

### Comparing `xlavir-0.6.2/xlavir/tools/samtools.py` & `xlavir-1.0.0/xlavir/tools/samtools.py`

 * *Files identical despite different names*

### Comparing `xlavir-0.6.2/xlavir/tools/variants.py` & `xlavir-1.0.0/xlavir/tools/variants.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """VCF and SnpEff/SnpSift parsing functions"""
 import logging
 import os
 import re
-from enum import Enum
+from dataclasses import dataclass
 from operator import itemgetter
 from pathlib import Path
 from typing import Dict, Tuple, List, Optional, Iterable, Union
 
 import pandas as pd
 from pydantic import BaseModel
 
@@ -159,38 +159,45 @@
 class VariantStats(BaseModel):
     sample: str
     n_snp: int
     n_mnp: int
     n_indel: int
 
 
-class VariantCaller(Enum):
+@dataclass
+class VariantCaller:
     iVar = 'iVar'
     Longshot = 'Longshot'
     Nanopolish = 'nanopolish'
     Medaka = 'medaka'
+    Clair3 = 'clair3'
+    Bcftools = 'bcftools'
 
 
 VCF_GLOB_PATTERNS = [
     '**/nanopolish/*.pass.vcf.gz',
     '**/ivar/*.vcf.gz',
+    '**/bcftools/*.vcf.gz',
     '**/*.filt.no_fs.vcf',
     '**/*.longshot.vcf',
     '**/*.vcf',
+    '**/*.vcf.gz',
 ]
 
 VCF_SAMPLE_NAME_CLEANUP = [
     re.compile(r'(\.pass)?\.vcf(\.gz)?$'),
     re.compile(r'\.AF0\.\d+(\.filt)?'),
     re.compile(r'\.0\.\d+AF(\.filt)?'),
     re.compile(r'\.medaka'),
     re.compile(r'\.longshot'),
+    re.compile(r'\.clair3'),
     re.compile(r'\.snpeff'),
     re.compile(r'\.no_fs'),
     re.compile(r'\.merged'),
+    re.compile(r'\.filtered'),
 ]
 
 SNPSIFT_GLOB_PATTERNS = [
     '**/ivar/**/*.snpSift.table.txt',
     '**/ivar/**/*.snpsift.table.txt',
     '**/ivar/**/*.snpsift.txt',
     '**/*.snpSift.table.txt',
@@ -199,14 +206,15 @@
 ]
 
 SNPSIFT_SAMPLE_NAME_CLEANUP = [
     re.compile(r'\.snp[sS]ift\.table\.txt$'),
     re.compile(r'\.snp[sS]ift\.txt$'),
     re.compile(r'\.AF0\.\d+(\.filt)?'),
     re.compile(r'\.0\.\d+AF(\.filt)?'),
+    re.compile(r'\.filtered'),
 ]
 
 
 def vcf_selector(paths: List[Path]) -> Optional[Path]:
     xs = []
     for path in paths:
         variant_caller, df = read_vcf(path)
@@ -235,26 +243,33 @@
     gzipped = vcf_file.name.endswith('.gz')
     with os.popen(f'zcat < {vcf_file.absolute()}') if gzipped else open(vcf_file) as fh:
         vcf_cols = []
         variant_caller = ''
         for line in fh:
             if line.startswith('##source='):
                 variant_caller = line.strip().replace('##source=', '')
+            if line.startswith('##bcftools_callVersion'):
+                variant_caller = 'bcftools'
             if line.startswith('##nanopolish'):
                 variant_caller = 'nanopolish'
             if line.startswith('##medaka_version'):
                 variant_caller = 'medaka'
             if line.startswith('#CHROM'):
                 vcf_cols = line[1:].strip().split('\t')
                 break
-        df = pd.read_table(fh,
-                           comment='#',
-                           header=None,
-                           names=vcf_cols)
-        df = df[~df.duplicated(['CHROM', 'POS', 'ID', 'REF', 'ALT', 'FILTER'], keep='first')]
+        try:
+
+            df = pd.read_table(vcf_file,
+                               sep='\t',
+                               comment='#',
+                               header=None,
+                               names=vcf_cols)
+            df = df[~df.duplicated(['CHROM', 'POS', 'ID', 'REF', 'ALT', 'FILTER'], keep='first')]
+        except pd.errors.EmptyDataError:
+            return variant_caller, pd.DataFrame()
     return variant_caller, df
 
 
 def parse_aa(gene: str,
              ref: str,
              alt: str,
              nt_pos: int,
@@ -342,24 +357,26 @@
             else:
                 new_series = dfc.astype('str')
             new_series.name = new_series_name
             series.append(new_series)
         else:
             series.append(df[c])
     df_out = pd.concat(series, axis=1)
-    mutation_desc = []
-    for row in df_out.itertuples():
-        mutation_desc.append(parse_aa(gene=row.gene,
-                                      ref=row.REF,
-                                      alt=row.ALT,
-                                      nt_pos=row.POS,
-                                      aa_pos=row.aa_pos,
-                                      snpeff_aa=row.aa,
-                                      effect=row.effect))
-
+    mutation_desc = [
+        parse_aa(
+            gene=row.gene,
+            ref=row.REF,
+            alt=row.ALT,
+            nt_pos=row.POS,
+            aa_pos=row.aa_pos,
+            snpeff_aa=row.aa,
+            effect=row.effect,
+        )
+        for row in df_out.itertuples()
+    ]
     df_out['mutation'] = mutation_desc
     df_out['sample'] = sample_name
     return df_out
 
 
 def parse_ivar_vcf(df: pd.DataFrame, sample_name: str = None) -> Optional[pd.DataFrame]:
     if df.empty:
@@ -438,15 +455,19 @@
     df_merge['sample'] = sample_name
     df_merge = df_merge[df_merge.DP > 0]
     df_merge['ALT_FREQ'] = df_merge.ALT_DP / df_merge.DP
     cols_to_keep = list({col for col, _, _ in variants_cols} & set(df_merge.columns))
     return df_merge.loc[:, cols_to_keep]
 
 
-def parse_medaka_vcf(df: pd.DataFrame, sample_name: str = None, qc_reqs: QualityRequirements = None) -> Optional[pd.DataFrame]:
+def parse_medaka_vcf(
+        df: pd.DataFrame,
+        sample_name: str = None,
+        qc_reqs: QualityRequirements = None
+) -> Optional[pd.DataFrame]:
     if df.empty:
         return None
     if not sample_name:
         sample_name = df.columns[-1] if df.columns[-1] != 'SAMPLE' else None
         if sample_name is None:
             raise ValueError(f'Sample name is not defined for VCF: shape={df.shape}; columns={df.columns}')
     pos_info_val = {}
@@ -475,88 +496,182 @@
     df_merge['sample'] = sample_name
     df_merge = df_merge[df_merge.DP > 0]
     df_merge['ALT_FREQ'] = df_merge.ALT_DP / (df_merge.ALT_DP + df_merge.REF_DP)
     cols_to_keep = list({col for col, _, _ in variants_cols} & set(df_merge.columns))
     return df_merge.loc[:, cols_to_keep]
 
 
-def parse_nanopolish_vcf(df: pd.DataFrame, sample_name: str = None) -> Optional[pd.DataFrame]:
+def parse_nanopolish_vcf(
+        df: pd.DataFrame,
+        sample_name: str = None
+) -> Optional[pd.DataFrame]:
     if df.empty:
         return None
     if not sample_name:
         sample_name = df.columns[-1] if df.columns[-1] != 'sample' else None
         if sample_name is None:
-            raise ValueError(f'Sample name is not defined for VCF: shape={df.shape}; columns={df.columns}')
+            raise ValueError(
+                f'Sample name is not defined for VCF: shape={df.shape}; '
+                f'columns={df.columns}'
+            )
     pos_info_val = {}
     for row in df.itertuples():
         infos = parse_vcf_info(row.INFO)
         fwd_ref, rev_ref, fwd_alt, rev_alt = infos['StrandSupport']
         allele_count = infos['AlleleCount']
         if allele_count > 1:
-            raise NotImplementedError(f'Handling of allele count of {allele_count} is not supported. '
-                                      f'Only allele counts of 1 are supported.')
+            raise NotImplementedError(
+                f'Handling of allele count of {allele_count} is not supported. '
+                f'Only allele counts of 1 are supported.'
+            )
         infos['DP'] = fwd_ref + fwd_alt + rev_ref + rev_alt
         infos['REF_DP'] = fwd_ref + rev_ref
         infos['ALT_DP'] = fwd_alt + rev_alt
         pos_info_val[row.POS] = infos
     df_nanopolish_info = pd.DataFrame(pos_info_val).transpose()
     df_nanopolish_info.index.name = 'POS'
     df_nanopolish_info.reset_index(inplace=True)
     df_merge = pd.merge(df, df_nanopolish_info, on='POS')
     df_merge['sample'] = sample_name
     df_merge = df_merge[df_merge.DP > 0]
     df_merge['ALT_FREQ'] = df_merge.ALT_DP / df_merge.DP
     cols_to_keep = list({col for col, _, _ in variants_cols} & set(df_merge.columns))
     return df_merge.loc[:, cols_to_keep]
 
+def parse_bcftools_vcf(df: pd.DataFrame, sample_name: str = None) -> Optional[pd.DataFrame]:
+    if df.empty:
+        return None
+    if not sample_name:
+        sample_name = df.columns[-1] if df.columns[-1] != 'sample' else None
+        if sample_name is None:
+            raise ValueError(f'Sample name is not defined for VCF: shape={df.shape}; columns={df.columns}')
+    pos_info_val = {}
+    for row in df.itertuples():
+        infos = parse_vcf_info(row.INFO)
+        allele_count = infos['AC']
+        if allele_count > 1:
+            raise NotImplementedError(f'Handling of allele count of {allele_count} is not supported. '
+                                      f'Only allele counts of 1 are supported.')
+        ref_dp, alt_dp = infos['AD']
+        infos['REF_DP'] = ref_dp
+        infos['ALT_DP'] = alt_dp
+        pos_info_val[row.POS] = infos
+    df_bcftools_info = pd.DataFrame(pos_info_val).transpose()
+    df_bcftools_info.index.name = 'POS'
+    df_bcftools_info.reset_index(inplace=True)
+    df_merge = pd.merge(df, df_bcftools_info, on='POS')
+    df_merge['sample'] = sample_name
+    df_merge = df_merge[df_merge.DP > 0]
+    df_merge['ALT_FREQ'] = df_merge.ALT_DP / df_merge.DP
+    cols_to_keep = list({col for col, _, _ in variants_cols} & set(df_merge.columns))
+    return df_merge.loc[:, cols_to_keep]
+
 
 def parse_vcf_info(s: str) -> dict:
     out = {}
     for x in s.split(';'):
         if not x:
             continue
+        if '=' not in x:
+            continue
         key, val_str = x.split('=', maxsplit=1)
         out[key] = try_parse_number(val_str)
     return out
 
 
+def parse_clair3_vcf(
+        df: pd.DataFrame,
+        sample_name: str,
+        qc_reqs: QualityRequirements
+) -> Optional[pd.DataFrame]:
+    if df.empty:
+        return None
+    if not sample_name:
+        sample_name = df.columns[-1] if df.columns[-1] != 'SAMPLE' else None
+        if sample_name is None:
+            raise ValueError(f'Sample name is not defined for VCF: shape={df.shape}; columns={df.columns}')
+    pos_info_val = {}
+    for row in df.itertuples():
+        infos = parse_vcf_info(row.INFO)
+        # no DP INFO? skip this file
+        if 'DP' not in infos:
+            return None
+        depth = infos['DP']
+        if depth < qc_reqs.low_coverage_threshold:
+            continue
+        allele_fraction = infos['AF']
+        alt_dp = int(depth * allele_fraction)
+        ref_dp = depth - alt_dp
+        infos['ALT_DP'] = alt_dp
+        infos['REF_DP'] = ref_dp
+        if infos['REF_DP'] + infos['ALT_DP'] < qc_reqs.low_coverage_threshold:
+            continue
+        pos_info_val[row.POS] = infos
+    if pos_info_val == {}:
+        return None
+    df_clair3_info = pd.DataFrame(pos_info_val).transpose()
+    df_clair3_info.index.name = 'POS'
+    df_clair3_info.reset_index(inplace=True)
+    df_merge = pd.merge(df, df_clair3_info, on='POS')
+    df_merge['sample'] = sample_name
+    df_merge = df_merge[df_merge.DP > 0]
+    df_merge['ALT_FREQ'] = df_merge.AF
+    cols_to_keep = list({col for col, _, _ in variants_cols} & set(df_merge.columns))
+    return df_merge.loc[:, cols_to_keep]
+
+
 def get_info(basedir: Path, qc_reqs: QualityRequirements) -> Dict[str, pd.DataFrame]:
     sample_vcf = find_file_for_each_sample(basedir=basedir,
                                            glob_patterns=VCF_GLOB_PATTERNS,
                                            sample_name_cleanup=VCF_SAMPLE_NAME_CLEANUP,
                                            single_entry_selector_func=vcf_selector)
     sample_dfvcf = {}
     for sample, vcf_path in sample_vcf.items():
         variant_caller, df_vcf = read_vcf(vcf_path)
-        if variant_caller.startswith(VariantCaller.iVar.value):
+        if variant_caller.startswith(VariantCaller.iVar):
             df_parsed_ivar_vcf = parse_ivar_vcf(df_vcf, sample)
             if df_parsed_ivar_vcf is not None:
                 sample_dfvcf[sample] = df_parsed_ivar_vcf
             else:
                 logger.warning(f'Sample "{sample}" has no entries in VCF "{vcf_path}"')
-        elif variant_caller.startswith(VariantCaller.Medaka.value):
+        elif variant_caller.startswith(VariantCaller.Bcftools):
+            df_bcftools_vcf = parse_bcftools_vcf(df_vcf, sample)
+            if df_bcftools_vcf is not None:
+                sample_dfvcf[sample] = df_bcftools_vcf
+            else:
+                logger.warning(f'Sample "{sample}" has no entries in VCF "{vcf_path}"')
+        elif variant_caller.startswith(VariantCaller.Clair3):
+            df_clair3_vcf = parse_clair3_vcf(df_vcf, sample, qc_reqs)
+            if df_clair3_vcf is not None:
+                sample_dfvcf[sample] = df_clair3_vcf
+            else:
+                logger.warning(f'Sample "{sample}" has no entries in Clair3 VCF "{vcf_path}"')
+        elif variant_caller.startswith(VariantCaller.Medaka):
             df_medaka_vcf = parse_medaka_vcf(df_vcf, sample, qc_reqs)
             if df_medaka_vcf is not None:
                 sample_dfvcf[sample] = df_medaka_vcf
             else:
                 logger.warning(f'Sample "{sample}" has no entries in VCF "{vcf_path}"')
-        elif variant_caller.startswith(VariantCaller.Longshot.value):
+        elif variant_caller.startswith(VariantCaller.Longshot):
             df_longshot_vcf = parse_longshot_vcf(df_vcf, sample)
             if df_longshot_vcf is not None:
                 sample_dfvcf[sample] = df_longshot_vcf
             else:
                 logger.warning(f'Sample "{sample}" has no entries in VCF "{vcf_path}"')
-        elif variant_caller.startswith(VariantCaller.Nanopolish.value):
+        elif variant_caller.startswith(VariantCaller.Nanopolish):
             df_nanopolish_vcf = parse_nanopolish_vcf(df_vcf, sample)
             if df_nanopolish_vcf is not None:
                 sample_dfvcf[sample] = df_nanopolish_vcf
             else:
                 logger.warning(f'Sample "{sample}" has no entries in VCF "{vcf_path}"')
         else:
-            logger.warning(f'Sample "{sample}" VCF file "{vcf_path}" with variant_caller={variant_caller} not supported. Skipping...')
+            logger.warning(
+                f'Sample "{sample}" VCF file "{vcf_path}" with '
+                f'variant_caller={variant_caller} not supported. Skipping...'
+            )
 
     sample_snpsift = find_file_for_each_sample(basedir=basedir,
                                                glob_patterns=SNPSIFT_GLOB_PATTERNS,
                                                sample_name_cleanup=SNPSIFT_SAMPLE_NAME_CLEANUP,
                                                single_entry_selector_func=snpsift_selector)
     if not sample_snpsift:
         logger.warning(f'No SnpSift tables found in "{basedir}" using glob patterns "{SNPSIFT_GLOB_PATTERNS}"')
```

### Comparing `xlavir-0.6.2/xlavir/util.py` & `xlavir-1.0.0/xlavir/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,45 @@
+import contextlib
 import logging
 import re
 from collections import defaultdict
 from pathlib import Path
-from typing import Union, List, Optional, Mapping, Callable
+from typing import Union, List, Optional, Mapping, Callable, Iterator
 
 import numpy as np
+import pandas as pd
+
 
 logger = logging.getLogger(__name__)
 
 
-def find_file_for_each_sample(basedir: Path,
-                              glob_patterns: List[str],
-                              sample_name_cleanup: Optional[List[Union[str, re.Pattern]]] = None,
-                              single_entry_selector_func: Optional[Callable] = None) -> Mapping[str, Path]:
+def find_file_for_each_sample(
+        basedir: Path,
+        glob_patterns: List[str],
+        sample_name_cleanup: Optional[List[Union[str, re.Pattern]]] = None,
+        single_entry_selector_func: Optional[Callable] = None
+) -> Mapping[str, Path]:
     sample_files = defaultdict(list)
     for glob_pattern in glob_patterns:
         for p in basedir.glob(glob_pattern):
             sample = extract_sample_name(p.name,
                                          remove=sample_name_cleanup)
             sample_files[sample].append(p)
-    sample_file = {}
-    for sample, files in sample_files.items():
-        if single_entry_selector_func:
-            sample_file[sample] = single_entry_selector_func(files)
-        else:
-            # select first file if no selector func specified
-            sample_file[sample] = files[0]
-    return sample_file
+    return {
+        sample: single_entry_selector_func(files)
+        if single_entry_selector_func
+        else files[0]
+        for sample, files in sample_files.items()
+    }
 
 
-def extract_sample_name(filename: str,
-                        remove: List[Union[str, re.Pattern]] = None) -> str:
+def extract_sample_name(
+        filename: str,
+        remove: Optional[List[Union[str, re.Pattern]]] = None
+) -> str:
     if not remove:
         remove = [
             '.pass',
             '.mapped',
             '.trim',
             '.ivar_trim',
             '.mkD',
@@ -60,63 +65,74 @@
             out = x.sub('', out)
         else:
             logger.warning(f'Not sure how to use "{x}" (type={type(x)}) for removing '
                            f'non-sample name text from "{filename}". Skipping "{x}". Output="{out}".')
     return out
 
 
-def get_col_widths(df, index=False, offset=2, max_width: int = None, include_header=True):
+def get_col_widths(
+        df: pd.DataFrame,
+        index=False,
+        offset=2,
+        max_width: Optional[int] = None,
+        include_header=True
+) -> Iterator[int]:
     """Calculate column widths based on column headers and contents"""
     if index:
         idx_max = max([len(str(s)) for s in df.index.values] + [len(str(df.index.name))]) + offset
         if max_width:
             idx_max = min(idx_max, max_width)
         yield idx_max
     for c in df.columns:
         # get max length of column contents and length of column header
         max_width_cells = df[c].astype(str).str.len().max() + 1
         if include_header:
             width = np.max([max_width_cells, len(c) + 1]) + offset
+        elif isinstance(c, str):
+            col_words = c.split()
+            col_words.sort(key=len, reverse=True)
+            max_word_size = int(len(col_words[-1]) * 1.25 + 1)
+            width = np.max([max_width_cells, max_word_size]) + offset
         else:
-            if isinstance(c, str):
-                col_words = c.split()
-                col_words.sort(key=len, reverse=True)
-                max_word_size = int(len(col_words[-1]) * 1.25 + 1)
-                width = np.max([max_width_cells, max_word_size]) + offset
-            else:
-                width = max_width_cells + offset
+            width = max_width_cells + offset
         if max_width:
             width = min(width, max_width)
         yield width
 
 
-def get_row_heights(df, idx, offset=0, multiplier=15):
+def get_row_heights(
+        df: pd.DataFrame,
+        idx: Union[str, int],
+        offset=0,
+        multiplier=15
+) -> int:
     """Calculate row heights"""
     # get max number of newlines in the row
     newline_count = np.max(df.loc[idx, :].astype(str).str.count('\n').max())
-    if newline_count < 1:
-        newline_count = 1
+    newline_count = max(newline_count, 1)
     height = newline_count * multiplier + offset
     logger.debug(f'idx="{idx}" height={height} newline_count={newline_count}')
     return height
 
 
-def list_get(xs: Optional[List], idx: int, default=None):
+def list_get(
+        xs: Optional[List],
+        idx: int,
+        default=None
+) -> Optional[Union[str, int, float, List[Union[str, int, float]]]]:
+    if xs is None:
+        return default
     try:
         return xs[idx]
     except (TypeError, IndexError):
         return default
 
 
-def try_parse_number(s: str) -> Union[int, float, List[float], List[int], str]:
+def try_parse_number(s: str) -> Union[int, float, str, List[Union[float, int, str]]]:
     if ',' in s:
         xs = s.split(',')
-        return [try_parse_number(x) for x in xs]
-    try:
+        return [try_parse_number(x) for x in xs] # type: ignore[misc]
+    with contextlib.suppress(ValueError):
         return int(s)
-    except ValueError:
-        pass
-    try:
+    with contextlib.suppress(ValueError):
         return float(s)
-    except ValueError:
-        pass
     return s
```

### Comparing `xlavir-0.6.2/xlavir/xlavir.py` & `xlavir-1.0.0/xlavir/xlavir.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 from xlavir.tools import mosdepth, samtools, consensus, pangolin, variants, nextclade, fastp
 from xlavir.tools.nextflow import exec_report
 from xlavir.tools.nextflow.exec_report import to_dataframe
 
 logger = logging.getLogger(__name__)
 
 
-def run(input_dir: Path,
+def run(
+        input_dir: Path,
         quality_reqs: Optional[qc.QualityRequirements],
         pangolin_lineage_csv: Optional[Path] = None,
-        ct_values_table: Optional[Path] = None) -> List[ExcelSheetDataFrame]:
+        ct_values_table: Optional[Path] = None
+) -> List[ExcelSheetDataFrame]:
     if quality_reqs is None:
         quality_reqs = qc.QualityRequirements()
     nf_exec_info = exec_report.get_info(input_dir)
     sample_depth_info = mosdepth.get_info(input_dir, low_coverage_threshold=quality_reqs.low_coverage_threshold)
     if logger.level == logging.DEBUG:
         for sample, info in sample_depth_info.items():
             logger.debug(info.dict())
@@ -93,16 +95,18 @@
             dfs.append(ExcelSheetDataFrame(sheet_name=SheetName.varmat.value,
                                            df=df_varmap,
                                            pd_to_excel_kwargs=dict(freeze_panes=(1, 1), na_rep=0.0),
                                            autofit=False,
                                            column_widths=[max_index_length + 2] + [3 for _ in
                                                                                    range(df_varmap.columns.size)]))
         else:
-            logger.warning(f'No column "Mutation" found in variant info dataframe. SnpEff/SnpSift table may not have '
-                           f'been found or parsed correctly.')
+            logger.warning(
+                'No column "Mutation" found in variant info dataframe. '
+                'SnpEff/SnpSift table may not have been found or parsed correctly.'
+            )
 
     dfs.append(ExcelSheetDataFrame(sheet_name=SheetName.consensus.value,
                                    df=consensus.get_info(basedir=input_dir),
                                    autofit=False,
                                    pd_to_excel_kwargs=dict(index=None, header=None)))
     if nf_exec_info:
         df_exec_info = to_dataframe(nf_exec_info)
```

