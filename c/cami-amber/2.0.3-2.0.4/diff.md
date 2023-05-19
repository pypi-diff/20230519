# Comparing `tmp/cami-amber-2.0.3.tar.gz` & `tmp/cami-amber-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cami-amber-2.0.3.tar", last modified: Tue Nov 23 15:50:47 2021, max compression
+gzip compressed data, was "cami-amber-2.0.4.tar", last modified: Fri May 19 14:06:21 2023, max compression
```

## Comparing `cami-amber-2.0.3.tar` & `cami-amber-2.0.4.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2021-11-23 15:50:47.000000 cami-amber-2.0.3/
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    35155 2021-11-23 15:49:19.000000 cami-amber-2.0.3/LICENSE
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       39 2021-11-23 15:49:19.000000 cami-amber-2.0.3/MANIFEST.in
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      672 2021-11-23 15:50:47.000000 cami-amber-2.0.3/PKG-INFO
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    11631 2021-11-23 15:49:19.000000 cami-amber-2.0.3/README.md
--rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)    15947 2021-11-23 15:49:19.000000 cami-amber-2.0.3/amber.py
-drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2021-11-23 15:50:47.000000 cami-amber-2.0.3/cami_amber.egg-info/
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      672 2021-11-23 15:50:47.000000 cami-amber-2.0.3/cami_amber.egg-info/PKG-INFO
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      697 2021-11-23 15:50:47.000000 cami-amber-2.0.3/cami_amber.egg-info/SOURCES.txt
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)        1 2021-11-23 15:50:47.000000 cami-amber-2.0.3/cami_amber.egg-info/dependency_links.txt
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       94 2021-11-23 15:50:47.000000 cami-amber-2.0.3/cami_amber.egg-info/requires.txt
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)        4 2021-11-23 15:50:47.000000 cami-amber-2.0.3/cami_amber.egg-info/top_level.txt
-drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2021-11-23 15:50:47.000000 cami-amber-2.0.3/requirements/
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       93 2021-11-23 15:49:19.000000 cami-amber-2.0.3/requirements/default.txt
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       50 2021-11-23 15:49:19.000000 cami-amber-2.0.3/requirements/development.txt
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       71 2021-11-23 15:50:47.000000 cami-amber-2.0.3/setup.cfg
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     1221 2021-11-23 15:49:19.000000 cami-amber-2.0.3/setup.py
-drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2021-11-23 15:50:47.000000 cami-amber-2.0.3/src/
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)        0 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/__init__.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    48567 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/amber_html.py
--rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)    46063 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/binning_classes.py
--rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)     4366 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/plot_by_genome.py
--rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)    26475 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/plots.py
--rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)     4916 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/precision_recall_per_bin.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     2948 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/unifrac_distance.py
-drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2021-11-23 15:50:47.000000 cami-amber-2.0.3/src/utils/
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     2251 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/utils/EMDUnifrac.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    20779 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/utils/ProfilingTools.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)        0 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/utils/__init__.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     3357 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/utils/add_length_column.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     2594 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/utils/argparse_parents.py
--rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)     2042 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/utils/convert_fasta_bins_to_biobox_format.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     9949 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/utils/labels.py
--rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)    12204 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/utils/load_data.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     6110 2021-11-23 15:49:19.000000 cami-amber-2.0.3/src/utils/load_ncbi_taxinfo.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       22 2021-11-23 15:49:19.000000 cami-amber-2.0.3/version.py
+drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2023-05-19 14:06:21.515985 cami-amber-2.0.4/
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    35155 2020-05-09 22:29:05.000000 cami-amber-2.0.4/LICENSE
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       41 2023-05-19 13:51:18.000000 cami-amber-2.0.4/MANIFEST.in
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      645 2023-05-19 14:06:21.515985 cami-amber-2.0.4/PKG-INFO
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    12157 2023-05-19 13:51:18.000000 cami-amber-2.0.4/README.md
+-rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)    15885 2023-05-19 13:51:18.000000 cami-amber-2.0.4/amber.py
+drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2023-05-19 14:06:21.515985 cami-amber-2.0.4/cami_amber.egg-info/
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      645 2023-05-19 14:06:21.000000 cami-amber-2.0.4/cami_amber.egg-info/PKG-INFO
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      660 2023-05-19 14:06:21.000000 cami-amber-2.0.4/cami_amber.egg-info/SOURCES.txt
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)        1 2023-05-19 14:06:21.000000 cami-amber-2.0.4/cami_amber.egg-info/dependency_links.txt
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      123 2023-05-19 14:06:21.000000 cami-amber-2.0.4/cami_amber.egg-info/requires.txt
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)        4 2023-05-19 14:06:21.000000 cami-amber-2.0.4/cami_amber.egg-info/top_level.txt
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      123 2023-05-19 13:51:18.000000 cami-amber-2.0.4/requirements.txt
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       72 2023-05-19 14:06:21.515985 cami-amber-2.0.4/setup.cfg
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     1073 2023-05-19 14:06:19.000000 cami-amber-2.0.4/setup.py
+drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2023-05-19 14:06:21.515985 cami-amber-2.0.4/src/
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)        0 2020-05-05 20:32:20.000000 cami-amber-2.0.4/src/__init__.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    45549 2023-05-19 13:51:18.000000 cami-amber-2.0.4/src/amber_html.py
+-rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)    43580 2023-05-19 13:51:18.000000 cami-amber-2.0.4/src/binning_classes.py
+-rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)     4496 2023-05-19 13:51:18.000000 cami-amber-2.0.4/src/plot_by_genome.py
+-rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)    27102 2023-05-19 13:51:18.000000 cami-amber-2.0.4/src/plots.py
+-rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)     4976 2023-05-19 13:51:18.000000 cami-amber-2.0.4/src/precision_recall_per_bin.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     2948 2020-05-09 22:29:05.000000 cami-amber-2.0.4/src/unifrac_distance.py
+drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2023-05-19 14:06:21.515985 cami-amber-2.0.4/src/utils/
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     2251 2020-05-05 20:32:20.000000 cami-amber-2.0.4/src/utils/EMDUnifrac.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    20779 2023-05-19 13:51:18.000000 cami-amber-2.0.4/src/utils/ProfilingTools.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)        0 2020-05-05 20:32:20.000000 cami-amber-2.0.4/src/utils/__init__.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     3357 2020-05-05 20:32:20.000000 cami-amber-2.0.4/src/utils/add_length_column.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     2594 2020-05-05 20:32:20.000000 cami-amber-2.0.4/src/utils/argparse_parents.py
+-rwxrwxrwx   0 fmeyer    (1000) fmeyer    (1000)     2042 2022-10-10 08:10:38.000000 cami-amber-2.0.4/src/utils/convert_fasta_bins_to_biobox_format.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    14571 2023-05-19 13:51:18.000000 cami-amber-2.0.4/src/utils/labels.py
+-rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)    12257 2023-05-19 13:51:18.000000 cami-amber-2.0.4/src/utils/load_data.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     6110 2023-03-31 21:37:00.000000 cami-amber-2.0.4/src/utils/load_ncbi_taxinfo.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       22 2023-05-19 13:51:18.000000 cami-amber-2.0.4/version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cami-amber-2.0.3/LICENSE` & `cami-amber-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cami-amber-2.0.3/PKG-INFO` & `cami-amber-2.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: cami-amber
-Version: 2.0.3
+Version: 2.0.4
 Summary: AMBER: Assessment of Metagenome BinnERs
 Home-page: http://cami-challenge.org
 Author: CAMI
 Author-email: support@cami-challenge.org
 License: GNU General Public License v3 or later (GPLv3+)
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `cami-amber-2.0.3/README.md` & `cami-amber-2.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -28,47 +28,92 @@
 * [CAMI II mouse gut toy dataset](https://cami-challenge.github.io/AMBER/cami_ii_mouse_gut/)
 * [CAMI II mouse gut toy dataset (using option --filter 1)](https://cami-challenge.github.io/AMBER/cami_ii_mouse_gut_filter1/)
 
 # Installation
 
 ## Requirements
 
-AMBER requires Python 3.7.
+AMBER 2.0.4 has been tested with Python 3.11.
 
-See [default.txt](requirements/default.txt) for all dependencies.
+See [requirements.txt](requirements.txt) for all dependencies.
 
-## Steps
+## Installation options
 
-You can run [AMBER using Docker (see below)](#running-amberpy-using-docker) or install it as follows.
+There are several options to install AMBER:
 
-Install pip if not already installed (tested on Linux Ubuntu 18.04):
+* [Bioconda](#bioconda)
+* [Python pip](#python-pip)
+* [Docker](#docker)
+
+## Bioconda
+
+Install and configure [Bioconda](https://bioconda.github.io/index.html) if not already installed. Then use the following command to create a Conda environment and install AMBER:
+
+~~~BASH
+conda create --name amber cami-amber
+~~~
+
+Activate the Conda environment with:
+
+~~~BASH
+conda activate amber
+~~~
+
+## Python pip
+
+Install pip if not already installed (tested on Linux Ubuntu 22.04):
 
 ~~~BASH
 sudo apt install python3-pip
 ~~~
 Should you receive the message `Unable to locate package python3-pip`, enter the following commands and repeat the previous step.
 
 ~~~BASH
 sudo add-apt-repository universe
 sudo apt update
 ~~~
 
 Then run:
 
 ~~~BASH
-pip3 install cami-amber 
+pip install cami-amber 
 ~~~
 
 Make sure to add AMBER to your PATH:
 
 ~~~BASH
 echo 'PATH=$PATH:${HOME}/.local/bin' >> ~/.bashrc
 source ~/.bashrc
 ~~~
 
+Alternatively, download or git-clone AMBER from GitHub. In AMBER's directory, install all requirements with the command:
+
+~~~BASH
+pip install -r requirements.txt 
+~~~
+
+# Docker
+
+You can pull a pre-built [AMBER Docker BioContainer](https://bioconda.github.io/recipes/cami-amber/README.html) as follows:
+
+~~~BASH
+docker pull quay.io/biocontainers/cami-amber:<tag>
+~~~
+
+See [valid values for &lt;tag&gt;](https://quay.io/repository/biocontainers/cami-amber?tab=tags).
+
+Alternatively, download or git-clone AMBER from GitHub. In AMBER's directory, build the Docker image with the command:
+
+~~~BASH
+docker build -t amber .
+~~~
+
+See bellow an example of how to [run AMBER using Docker](#running-amberpy-using-docker).
+
+
 # User guide
 
 ## Input
 As input, AMBER uses three files and an additional file for assessing taxonomic binning:
 1. A gold standard mapping of contigs or read IDs to genomes and/or taxon IDs in the [CAMI binning Bioboxes format](https://github.com/bioboxes/rfc/tree/master/data-format). Columns are tab separated. Example:
 ~~~BASH
 @Version:0.9.1
@@ -80,45 +125,40 @@
 RH|P|C26099  1053046    765201 689201
 RH|P|C35075  1053046    765201 173282
 RH|P|C20873  1053046    765201 339258
 ~~~
 See [here](./test/gsa_mapping.binning) another example. Observations:
 * The value of the SampleID header tag must uniquely identify a sample and be the same in the gold standard and the predictions (input 2 below).
 * Column BINID (TAXID) is required to assess genome (taxonomic) binning.
-* Column _LENGTH can be added to a mapping file using tool [_src/utils/add_length_column.py_](#srcutilsadd_length_columnpy).
+* Column LENGTH can be added to a mapping file using tool [_src/utils/add_length_column.py_](#srcutilsadd_length_columnpy).
 
-2. One or more files, each containing the bin assignments from a binning program, also in the [CAMI binning Bioboxes format](https://github.com/bioboxes/rfc/tree/master/data-format). Column _LENGTH is not required  (_LENGTH is only required in the gold standard).
+2. One or more files, each containing the bin assignments from a binning program, also in the [CAMI binning Bioboxes format](https://github.com/bioboxes/rfc/tree/master/data-format). Column LENGTH is not required  (LENGTH is only required in the gold standard).
 
 Note: a tool for converting FASTA files, such that each file represents a bin, is available (see [_src/utils/convert_fasta_bins_to_biobox_format.py_](#srcutilsconvert_fasta_bins_to_biobox_formatpy)).
 
-3. For assessing **taxonomic binning**, AMBER also requires the file **nodes.dmp** from NCBI. Download taxdump.tar.gz from [ftp://ftp.ncbi.nih.gov/pub/taxonomy/taxdump.tar.gz](ftp://ftp.ncbi.nih.gov/pub/taxonomy/taxdump.tar.gz), extract nodes.tmp, and provide it to AMBER with option `--ncbi_nodes_file`.
+3. For assessing **taxonomic binning**, AMBER also requires the file **nodes.dmp** from NCBI. Download taxdump.tar.gz from [ftp://ftp.ncbi.nih.gov/pub/taxonomy/taxdump.tar.gz](ftp://ftp.ncbi.nih.gov/pub/taxonomy/taxdump.tar.gz), extract nodes.tmp, and provide it to AMBER with option `--ncbi_dir`.
 
 ## Input format for multiple samples
 
 Binnings of datasets with multiple samples are supported by AMBER. For each binning program, simply concatenate the binnings of the different samples into a single file to obtain one binning file per program. The gold standard must also consist in one file for all samples. Remember: binnings for the same sample must have the same SampleID.
 
 
 ## Running _amber.py_
 
 ~~~BASH
-usage: AMBER [-h] -g GOLD_STANDARD_FILE [-l LABELS] [-p FILTER]
-             [-n MIN_LENGTH] -o OUTPUT_DIR [--stdout] [-d DESC] [--silent]
-             [-v] [-m] [-x MIN_COMPLETENESS] [-y MAX_CONTAMINATION] [-c]
-             [-r REMOVE_GENOMES] [-k KEYWORD]
-             [--ncbi_nodes_file NCBI_NODES_FILE]
-             [--ncbi_names_file NCBI_NAMES_FILE]
-             [--rank_as_genome_binning RANK_AS_GENOME_BINNING]
+usage: AMBER [-h] -g GOLD_STANDARD_FILE [-l LABELS] [-p FILTER] [-n MIN_LENGTH] -o OUTPUT_DIR [--stdout] [-d DESC] [--colors COLORS] [--silent] [-v] [-x MIN_COMPLETENESS]
+             [-y MAX_CONTAMINATION] [-r REMOVE_GENOMES] [-k KEYWORD] [--genome_coverage GENOME_COVERAGE] [--ncbi_dir NCBI_DIR]
              bin_files [bin_files ...]
 
 AMBER: Assessment of Metagenome BinnERs
 
 positional arguments:
   bin_files             Binning files
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -g GOLD_STANDARD_FILE, --gold_standard_file GOLD_STANDARD_FILE
                         Gold standard - ground truth - file
   -l LABELS, --labels LABELS
                         Comma-separated binning names
   -p FILTER, --filter FILTER
                         Filter out [FILTER]% smallest genome bins (default: 0)
@@ -128,40 +168,27 @@
                         Directory to write the results to
   --stdout              Print summary to stdout
   -d DESC, --desc DESC  Description for HTML page
   --silent              Silent mode
   -v, --version         show program's version number and exit
 
 genome binning-specific arguments:
-  -m, --map_by_completeness
-                        Map genomes to bins by maximizing completeness
   -x MIN_COMPLETENESS, --min_completeness MIN_COMPLETENESS
-                        Comma-separated list of min. completeness thresholds
-                        (default %: 50,70,90)
+                        Comma-separated list of min. completeness thresholds (default %: 50,70,90)
   -y MAX_CONTAMINATION, --max_contamination MAX_CONTAMINATION
-                        Comma-separated list of max. contamination thresholds
-                        (default %: 10,5)
-  -c, --plot_heatmaps   Plot heatmaps of confusion matrices (can take some
-                        minutes)
+                        Comma-separated list of max. contamination thresholds (default %: 10,5)
   -r REMOVE_GENOMES, --remove_genomes REMOVE_GENOMES
                         File with list of genomes to be removed
   -k KEYWORD, --keyword KEYWORD
-                        Keyword in the second column of file with list of
-                        genomes to be removed (no keyword=remove all genomes
-                        in list)
+                        Keyword in the second column of file with list of genomes to be removed (no keyword=remove all genomes in list)
+  --genome_coverage GENOME_COVERAGE
+                        genome coverages
 
 taxonomic binning-specific arguments:
-  --ncbi_nodes_file NCBI_NODES_FILE
-                        NCBI nodes file
-  --ncbi_names_file NCBI_NAMES_FILE
-                        NCBI names file
-  --rank_as_genome_binning RANK_AS_GENOME_BINNING
-                        Assess taxonomic binning at a rank also as genome
-                        binning. Valid ranks: superkingdom, phylum, class,
-                        order, family, genus, species, strain
+  --ncbi_dir NCBI_DIR   Directory containing the NCBI taxonomy database dump files nodes.dmp, merged.dmp, and names.dmp
 ~~~
 **Example:**
 ~~~BASH
 amber.py -g test/gsa_mapping.binning \
 -l "MaxBin 2.0, CONCOCT, MetaBAT" \
 -p 1 \
 -r test/unique_common.tsv \
@@ -170,32 +197,26 @@
 test/goofy_hypatia_2 \
 test/elated_franklin_0 \
 -o output_dir/
 ~~~
 
 ## Running _amber.py_ using Docker
 
-Download or git-clone AMBER from GitHub. In AMBER's directory, build the Docker image with the command:
-
-~~~BASH
-docker build -t amber:latest .
-~~~
-
-_amber.py_ can then be run with the `docker run` command. Example:
+_amber.py_ can be run with the `docker run` command. Example:
 
 ~~~BASH
-docker run -v /path/to/AMBER/test:/host amber:latest \
+docker run -v $(pwd):/host amber \
 amber.py \
 -l "CONCOCT (CAMI), MaxBin 2.0.2 (CAMI)" \
 -p 1 \
--r /host/unique_common.tsv \
+-r /host/test/unique_common.tsv \
 -k "circular element" \
--g /host/gsa_mapping.binning \
-/host/goofy_hypatia_2 \
-/host/naughty_carson_2 \
+-g /host/test/gsa_mapping.binning \
+/host/test/goofy_hypatia_2 \
+/host/test/naughty_carson_2 \
 -o /host/output_dir
 ~~~
 
 # Utilities
 
 ### src/utils/add_length_column.py
 Adds column _LENGTH to the gold standard mapping file, eliminating the need to provide a FASTA or FASTQ file to amber.py.
@@ -275,15 +296,15 @@
 ~~~BASH
 tox
 ~~~
 
 You can use all libraries that AMBER depends on by activating tox's virtual environment with the command: 
 
 ~~~BASH
-source  <project_directory>/.tox/py37/bin/activate
+source  <project_directory>/.tox/py311/bin/activate
 ~~~
 
 ### Update GitHub page
 
 In order to update *https://cami-challenge.github.io/AMBER*, modify file index.html.
 
 ### Make a release
@@ -302,15 +323,19 @@
 python3 setup.py sdist bdist_wheel
 twine upload dist/*
 ~~~
 
 # Citation
 
 Please cite AMBER as:
-* Fernando Meyer, Peter Hofmann, Peter Belmann, Ruben Garrido-Oter, Adrian Fritz, Alexander Sczyrba, and Alice C. McHardy. (2018). **AMBER: Assessment of Metagenome BinnERs.** *GigaScience*, giy069. doi:[10.1093/gigascience/giy069](https://doi.org/10.1093/gigascience/giy069)
+* Meyer, F., Hofmann, P., Belmann, P., Garrido-Oter, R., Fritz, A., Sczyrba, A., McHardy, A.C., **AMBER: Assessment of Metagenome BinnERs**, GigaScience 7, giy069 (2018). [https://doi.org/10.1093/gigascience/giy069](https://doi.org/10.1093/gigascience/giy069)
 
 The metrics implemented in AMBER were used and described in the CAMI manuscript, thus you may also cite:
-* Sczyrba, Hofmann, Belmann, et al. (2017). **Critical Assessment of Metagenome Interpretation—a benchmark of metagenomics software.** *Nature Methods*, 14, 11:1063–1071. doi:[10.1038/nmeth.4458](https://doi.org/10.1038/nmeth.4458)
+* Sczyrba, A., Hofmann, P., Belmann, P. et al. **Critical Assessment of Metagenome Interpretation—a benchmark of metagenomics software.** Nat Methods 14, 1063–1071 (2017). [https://doi.org/10.1038/nmeth.4458](https://doi.org/10.1038/nmeth.4458)
+
+or
+
+* Meyer, F., Fritz, A., Deng, ZL. et al. **Critical Assessment of Metagenome Interpretation: the second round of challenges.** Nat Methods 19, 429–440 (2022). [https://doi.org/10.1038/s41592-022-01431-4](https://doi.org/10.1038/s41592-022-01431-4)
 
 # License
 
 AMBER 2 is licensed under GPL v3.
```

### Comparing `cami-amber-2.0.3/amber.py` & `cami-amber-2.0.4/amber.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright 2020 Department of Computational Biology for Infection Research - Helmholtz Centre for Infection Research
+# Copyright 2023 Department of Computational Biology for Infection Research - Helmholtz Centre for Infection Research
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -16,24 +16,21 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import argparse
 import errno
 import logging
 import os
 import sys
-
+import pandas as pd
 import matplotlib
-
+matplotlib.use('Agg')
 from src import amber_html
 from src import plot_by_genome
 from src import plots
 from version import __version__
-
-matplotlib.use('Agg')
-import pandas as pd
 from src.utils import load_data
 from src.utils import argparse_parents
 from src.utils import labels as utils_labels
 from src import binning_classes
 from src.utils import load_ncbi_taxinfo
 
 
@@ -205,22 +202,21 @@
 
 
 def save_metrics(sample_id_to_queries_list, df_summary, pd_bins, output_dir, stdout):
     logging.getLogger('amber').info('Saving computed metrics')
     df_summary.to_csv(os.path.join(output_dir, 'results.tsv'), sep='\t', index=False)
     pd_bins.to_csv(os.path.join(output_dir, 'bin_metrics.tsv'), index=False, sep='\t')
     if stdout:
-        summary_columns = [utils_labels.TOOL] + [col for col in df_summary if col != utils_labels.TOOL]
-        print(df_summary[summary_columns].to_string(index=False))
+        print(df_summary[utils_labels.LABELS1].rename(columns=utils_labels.LABELS).to_string(index=False))
     for tool, pd_group in pd_bins[pd_bins['rank'] == 'NA'].groupby(utils_labels.TOOL):
-        bins_columns = amber_html.get_genome_bins_columns()
+        bins_columns = utils_labels.get_genome_bins_columns()
         table = pd_group[['sample_id'] + list(bins_columns.keys())].rename(columns=dict(bins_columns))
         table.to_csv(os.path.join(output_dir, 'genome', tool, 'metrics_per_bin.tsv'), sep='\t', index=False)
     for tool, pd_group in pd_bins[pd_bins['rank'] != 'NA'].groupby(utils_labels.TOOL):
-        bins_columns = amber_html.get_tax_bins_columns()
+        bins_columns = utils_labels.get_tax_bins_columns()
         if 'name' not in pd_bins.columns or pd_group['name'].isnull().any():
             del bins_columns['name']
         table = pd_group[['sample_id'] + list(bins_columns.keys())].rename(columns=dict(bins_columns))
         table.to_csv(os.path.join(output_dir, 'taxonomic', tool, 'metrics_per_bin.tsv'), sep='\t', index=False)
 
     pd_genomes_all = pd.DataFrame()
     for sample_id in sample_id_to_queries_list:
```

### Comparing `cami-amber-2.0.3/cami_amber.egg-info/PKG-INFO` & `cami-amber-2.0.4/cami_amber.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: cami-amber
-Version: 2.0.3
+Version: 2.0.4
 Summary: AMBER: Assessment of Metagenome BinnERs
 Home-page: http://cami-challenge.org
 Author: CAMI
 Author-email: support@cami-challenge.org
 License: GNU General Public License v3 or later (GPLv3+)
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `cami-amber-2.0.3/cami_amber.egg-info/SOURCES.txt` & `cami-amber-2.0.4/cami_amber.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 LICENSE
 MANIFEST.in
 README.md
 amber.py
+requirements.txt
 setup.cfg
 setup.py
 version.py
 cami_amber.egg-info/PKG-INFO
 cami_amber.egg-info/SOURCES.txt
 cami_amber.egg-info/dependency_links.txt
 cami_amber.egg-info/requires.txt
 cami_amber.egg-info/top_level.txt
-requirements/default.txt
-requirements/development.txt
 src/__init__.py
 src/amber_html.py
 src/binning_classes.py
 src/plot_by_genome.py
 src/plots.py
 src/precision_recall_per_bin.py
 src/unifrac_distance.py
```

### Comparing `cami-amber-2.0.3/setup.py` & `cami-amber-2.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import pkg_resources, os, pkgutil
+import os
 from setuptools import setup, find_packages
 from version import __version__
 import glob
 
 
 def dependencies():
-    file_ = pkg_resources.resource_filename(__name__, os.path.join('requirements', 'default.txt'))
-    with open(file_, 'r') as f:
+    with open('requirements.txt', 'r') as f:
         return f.read().splitlines()
 
+
 setup(
-    name                 = 'cami-amber',
-    version              = __version__,
-    description          = 'AMBER: Assessment of Metagenome BinnERs',
-    author               = 'CAMI',
-    author_email         = 'support@cami-challenge.org',
-    url                  = 'http://cami-challenge.org',
-    license              = 'GNU General Public License v3 or later (GPLv3+)',
-    scripts              = glob.glob('*.py'),
-    install_requires     = dependencies(),
-    packages             = find_packages(),
+    name             = 'cami-amber',
+    version          = __version__,
+    description      = 'AMBER: Assessment of Metagenome BinnERs',
+    author           = 'CAMI',
+    author_email     = 'support@cami-challenge.org',
+    url              = 'http://cami-challenge.org',
+    license          = 'GNU General Public License v3 or later (GPLv3+)',
+    scripts          = glob.glob('*.py'),
+    install_requires = dependencies(),
+    packages         = find_packages(),
     classifiers = [
         'Natural Language :: English',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Intended Audience :: Science/Research',
         'Operating System :: POSIX'
     ]
 )
```

### Comparing `cami-amber-2.0.3/src/amber_html.py` & `cami-amber-2.0.4/src/amber_html.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright 2020 Department of Computational Biology for Infection Research - Helmholtz Centre for Infection Research
+# Copyright 2023 Department of Computational Biology for Infection Research - Helmholtz Centre for Infection Research
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
+import io
 import os
 from collections import OrderedDict
 from collections import defaultdict
 import datetime
 import numpy as np
 import pandas as pd
 import math
@@ -35,110 +35,96 @@
 import matplotlib.pyplot as pltx
 from matplotlib.colors import rgb2hex
 from matplotlib.colors import Normalize
 
 from version import __version__
 
 from bokeh.plotting import figure
-from bokeh.layouts import column, row, widgetbox
-from bokeh.models.widgets import TableColumn, Div, Select, Panel, Tabs
+from bokeh.layouts import column, row
+from bokeh.models.widgets import TableColumn, Div, Select
+from bokeh.models import TabPanel, Tabs
 from bokeh.models import (DataTable,
                           CustomJS,
                           Legend, LegendItem,
                           Band,
-                          FuncTickFormatter,
+                          CustomJSTickFormatter,
                           HoverTool)
 from bokeh.models.tickers import FixedTicker
-from bokeh.embed import components
 from bokeh.resources import INLINE
+from bokeh.embed import file_html
 from bokeh.plotting import ColumnDataSource
 
 
 AVG_OVER_SAMPLES = '[average over samples]'
 CLICK_ON_LEGENDS_DIV = '<div>' + AVG_OVER_SAMPLES + '</div><div style="padding-top: 10px;">Click on the legends to enable/disable the results for a tool.</div>'
 
-
-TEMPLATE = Template('''<!DOCTYPE html>
-    <html lang="en">
-        <head>
-            <meta charset="utf-8">
-            <title>AMBER: Assessment of Metagenome BinnERs</title>
-            {{ js_resources }}
-            {{ css_resources }}
-            <style>.bk-fit-content {width: fit-content; width: -moz-fit-content;}
-            .bk-width-auto {width: auto !important; height: auto !important;}
-            .bk-display-block {display: block !important;}
-            .bk-float-left {float: left;}
-            .bk-width-auto-main>div {width: -webkit-fill-available !important;}
-            div.bk-width-auto-main {width: -webkit-fill-available !important;}
-            .bk-tabs-margin{margin-top: 20px !important;}
-            .bk-tabs-margin-lr{margin-left: 10px; margin-right: 10px}
-            .bk-root {display: flex; justify-content: center;}
-            .bk-padding-top {padding-top: 10px;}
-            .bk-padding-top2 {padding-top: 20px;}
-            .bk-combo-box > div:first-child {
-                width: auto !important;
-                padding-right: 40px;
-            }
-            tr:hover {outline: 1px solid black;}
-            html {overflow: -moz-scrollbars-vertical; overflow-y: scroll;}
-            .tooltip {
-                position: relative;
-                display: inline-block;
-                border-bottom: 1px dashed lightgray;
-                cursor: help;
-            }
-            .tooltip-sem {
-                border-bottom: 1px dotted black;
-            }
-            .tooltip .tooltiptext {
-                visibility: hidden;
-                width: 280px;
-                background-color: #555;
-                color: #fff;
-                text-align: center;
-                border-radius: 6px;
-                padding: 5px 0;
-                position: absolute;
-                z-index: 1;
-                bottom: 125%;
-                left: 50%;
-                margin-left: -60px;
-                opacity: 0;
-            }
-            .tooltip .tooltiptext::after {
-                content: "";
-                position: absolute;
-                top: 100%;
-                left: 50%;
-                margin-left: -5px;
-                border-width: 5px;
-                border-style: solid;
-                border-color: #555 transparent transparent transparent;
-            }
-            .tooltip:hover .tooltiptext {
-                visibility: visible;
-                opacity: 1;
-            }
-            .proportions {
-                cursor: pointer;
-            }
-            .legend {
-                position:absolute;
-                cursor: move;
-                z-index: 1;
-            }
-            </style>
-        </head>
-        <body>
-            {{ div }}
-            {{ script }}
-        </body>
-    </html>
-    ''')
+TEMPLATE = Template('''
+{% from macros import embed %}
+<!DOCTYPE html>
+<html lang="en">
+  {% block head %}
+  <head>
+  {% block inner_head %}
+    <meta charset="utf-8">
+    <title>{% block title %}{{ title | e if title else "Bokeh Plot" }}{% endblock %}</title>
+  {%  block preamble -%}{%- endblock %}
+  {%  block resources %}
+    <style>
+      html, body {
+        box-sizing: border-box;
+        height: 100%;
+        margin: 8px;
+        padding: 0;
+      }
+      .bk-fit-content {width: fit-content; width: -moz-fit-content;}
+      .bk-width-auto {width: auto !important; height: auto !important;}
+      .bk-display-block {display: block !important;}
+      .bk-float-left {float: left;}
+      bk-width-auto-main>div {width: -webkit-fill-available !important;}
+      div.bk-width-auto-main {width: -webkit-fill-available !important;}
+      .bk-tabs-margin{margin-top: 20px !important;}
+      .bk-tabs-margin-lr{margin-left: 10px; margin-right: 10px}
+      .bk-root {display: flex; justify-content: center;}
+      .bk-padding-top {padding-top: 10px;}
+      .bk-padding-top2 {padding-top: 20px;}
+      .bk-combo-box > div:first-child {
+        width: auto !important;
+        padding-right: 40px;
+      }
+    </style>
+  {%   block css_resources -%}
+    {{- bokeh_css if bokeh_css }}
+  {%-  endblock css_resources %}
+  {%   block js_resources -%}
+    {{  bokeh_js if bokeh_js }}
+  {%-  endblock js_resources %}
+  {%  endblock resources %}
+  {%  block postamble %}{% endblock %}
+  {% endblock inner_head %}
+  </head>
+  {% endblock head%}
+  {% block body %}
+  <body>
+  {%  block inner_body %}
+  {%    block contents %}
+  {%      for doc in docs %}
+  {{        embed(doc) if doc.elementid }}
+  {%-       for root in doc.roots %}
+  {%          block root scoped %}
+  {{            embed(root) }}
+  {%          endblock %}
+  {%        endfor %}
+  {%      endfor %}
+  {%    endblock contents %}
+  {{ plot_script | indent(4) }}
+  {%  endblock inner_body %}
+  </body>
+  {% endblock body%}
+</html>
+''')
 
 
 def create_heatmap_bar(output_dir):
     fig = pltx.figure(figsize=(2, 2))
     x = np.arange(25).reshape(5, 5)
     cm = sns.diverging_palette(12, 250, sep=30, l=50, n=15, s=90, as_cmap=True)
     ax = sns.heatmap(x, cmap=cm, cbar=False)
@@ -163,39 +149,35 @@
         Normalize.__init__(self, vmin, vmax, clip)
 
     def __call__(self, value, clip=None):
         x, y = [self.vmin, self.midpoint, self.vmax], [0, 0.5, 1]
         return np.ma.masked_array(np.interp(value, x, y))
 
 
-def upper1(x):
-        return x[:1].upper() + x[1:]
-
-
 def get_colors_and_ranges(name, all_values):
     color1 = 'dodgerblue'
     color2 = 'red'
     hue1 = 12
     hue2 = 240
 
     metrics = [utils_labels.MISCLASSIFICATION_PER_BP, utils_labels.MISCLASSIFICATION_PER_SEQ]
-    if name in map(upper1, metrics + [x + utils_labels.UNFILTERED for x in metrics]):
+    if name in metrics + [x + utils_labels.UNFILTERED for x in metrics]:
         return color2, color1, hue2, hue1, 0, 1
     metrics = [utils_labels.UNIFRAC_BP, utils_labels.UNIFRAC_SEQ]
-    if name in map(upper1, metrics + [x + utils_labels.UNFILTERED for x in metrics]):
+    if name in metrics + [x + utils_labels.UNFILTERED for x in metrics]:
         return color2, color1, hue2, hue1, 0, max(all_values)
     return color1, color2, hue1, hue2, 0, 1
 
 
 def get_heatmap_colors(pd_series, **args):
     values = pd_series.tolist()
 
     metrics = [utils_labels.AVG_PRECISION_BP_SEM, utils_labels.AVG_RECALL_BP_SEM, utils_labels.AVG_PRECISION_SEQ_SEM,
                utils_labels.AVG_RECALL_SEQ_SEM, utils_labels.AVG_RECALL_BP_SEM_CAMI1, utils_labels.AVG_RECALL_SEQ_SEM_CAMI1]
-    if pd_series.name in map(upper1, metrics + [x + utils_labels.UNFILTERED for x in metrics]):
+    if pd_series.name in metrics + [x + utils_labels.UNFILTERED for x in metrics]:
         return ['background-color: white' for x in values]
 
     dropped_gs = False
     if pd_series.index[0] == utils_labels.GS:
         values = values[1:]
         dropped_gs = True
     if len(values) == 0:
@@ -227,15 +209,21 @@
     if dropped_gs:
         return [''] + return_colors
     else:
         return return_colors
 
 
 def create_title_div(id, name, info):
-    div = Div(text="""<div style="text-align:left;font-size: 20pt;font-weight: bold;">{1}<span style="float: right;font-size: 10pt;font-weight:normal;">{2}</span>""".format(id, name, info), css_classes=['bk-width-auto']) # width=DIV_WIDTH, height=DIV_HEIGHT)
+    div = Div(text="""<div style="text-align:left;font-size: 20pt;font-weight: bold;">{1}<span style="float: right;font-size: 10pt;font-weight:normal;">{2}</span>""".format(id, name, info), styles={'width': 'auto'})
+    div.stylesheets = ["""
+    .bk-clearfix {
+      width: -webkit-fill-available;
+      width: -moz-available;
+    }
+    """]
     return div
 
 
 def create_metrics_per_bin_panel(pd_bins, bins_columns, sample_ids_list, output_dir, binning_type):
     styles = [{'selector': 'td', 'props': [('width', '92pt')]},
               {'selector': 'th', 'props': [('width', '92pt'), ('text-align', 'left')]},
               {'selector': 'expand-toggle:checked ~ * .data', 'props': [('background-color', 'white !important')]}]
@@ -250,48 +238,48 @@
             if sample_id not in available_samples:
                 tool_to_sample_to_html[tool].append('')
                 continue
             pd_tool_sample = pd_tool_sample_groupby.get_group(sample_id)
             pd_tool_sample = pd_tool_sample[list(bins_columns.keys())].rename(columns=dict(bins_columns))
             if binning_type == 'taxonomic':
                 pd_tool_sample['Taxon ID'] = pd_tool_sample['Taxon ID'].astype('Int64')
-            tool_sample_html = pd_tool_sample.head(500).style.set_table_styles(styles).set_precision(3).hide_index().render()
+            tool_sample_html = pd_tool_sample.head(500).style.set_table_styles(styles).format(precision=3).hide(axis='index').to_html()
             tool_sample_html += '<div style="padding-top: 20px; padding-bottom: 20px;">{}</div>'.format('Complete table available in: ' + os.path.join(output_dir, binning_type, tool, 'metrics_per_bin.tsv'))
             tool_to_sample_to_html[tool].append(tool_sample_html)
     tool_to_sample_to_html['all_samples'] = sample_ids_list
 
-    table_div = Div(text="""<div>{}</div>""".format(tool_to_sample_to_html[tools[0]][0]), css_classes=['bk-width-auto'])
+    table_div = Div(text="""<div>{}</div>""".format(tool_to_sample_to_html[tools[0]][0]))
 
     source = ColumnDataSource(data=tool_to_sample_to_html)
 
-    select_tool = Select(title="Binner:", value=tools[0], options=tools, css_classes=['bk-fit-content'])
-    select_sample = Select(title="Sample:", value='0', options=list(zip(map(str, range(len(sample_ids_list))), sample_ids_list)), css_classes=['bk-fit-content'])
+    select_tool = Select(title="Binner:", value=tools[0], options=tools)
+    select_sample = Select(title="Sample:", value='0', options=list(zip(map(str, range(len(sample_ids_list))), sample_ids_list)))
     select_tool_sample_callback = CustomJS(args=dict(source=source), code="""
-        select_sample.options = []
-        options_array = []
-        for (index in source.data[select_tool.value]) {
+        select_sample.options = [];
+        const options_array = [];
+        for (let index in source.data[select_tool.value]) {
             if (source.data[select_tool.value][index] != "") {
                 options_array.push([index, source.data["all_samples"][index]])
             }
         }
-        select_sample.options = options_array
+        select_sample.options = options_array;
         if (source.data[select_tool.value][select_sample.value] != "") {
             mytable.text = source.data[select_tool.value][select_sample.value];
         } else {
             mytable.text = source.data[select_tool.value][options_array[0][0]];
         }
     """)
     select_tool.js_on_change('value', select_tool_sample_callback)
     select_sample.js_on_change('value', select_tool_sample_callback)
     select_tool_sample_callback.args["mytable"] = table_div
     select_tool_sample_callback.args["select_tool"] = select_tool
     select_tool_sample_callback.args["select_sample"] = select_sample
 
-    table_column = row(column(row(select_tool, select_sample, css_classes=['bk-width-auto', 'bk-combo-box']), table_div, sizing_mode='scale_width', css_classes=['bk-width-auto']), css_classes=['bk-width-auto'], sizing_mode='scale_width') # column(table_div, sizing_mode='scale_width', css_classes=['bk-width-auto', 'bk-width-auto-main'])
-    metrics_bins_panel = Panel(child=table_column, title="Metrics per bin")
+    table_column = row(column(row(select_tool, select_sample), table_div, sizing_mode='scale_width'), sizing_mode='scale_width')
+    metrics_bins_panel = TabPanel(child=table_column, title="Metrics per bin")
     return metrics_bins_panel
 
 
 def create_contamination_completeness_table(pd_bins, min_completeness, max_contamination):
     df = binning_classes.GenomeQuery.calc_num_recovered_genomes(pd_bins, min_completeness, max_contamination)
 
     def create_table_column(field):
@@ -299,21 +287,21 @@
 
     dt = DataTable(source=ColumnDataSource(df),
                    columns=list(map(lambda x: create_table_column(x), df.columns.values)),
                    width=800,
                    height=1000,
                    reorderable=True,
                    selectable=True)
-    return [widgetbox(dt)]
+    return [column(dt)]
 
 
 def create_heatmap_div():
     heatmap_legend = '<img src="heatmap_bar.png" /><div style="text-align:left;font-size: 11px;">Worst<span style="float:right;">Best</span><span style="margin-right: 36px;float:right;">Median</span></div>'
-    heatmap_legend_div = Div(text=heatmap_legend, style={"width": "155px", "margin-bottom": "-10px"})
-    return  heatmap_legend_div
+    heatmap_legend_div = Div(text=heatmap_legend, styles={"width": "155px", "margin-bottom": "-10px"})
+    return heatmap_legend_div
 
 
 def get_labels_genome():
     return ([(utils_labels.ACCURACY_PER_BP, utils_labels.TOOLTIP_ACCURACY_PER_BP),
              (utils_labels.ACCURACY_PER_SEQ, utils_labels.TOOLTIP_ACCURACY_PER_SEQ),
              (utils_labels.MISCLASSIFICATION_PER_BP, utils_labels.TOOLTIP_MISCLASSIFICATION_PER_BP),
              (utils_labels.MISCLASSIFICATION_PER_SEQ, utils_labels.TOOLTIP_MISCLASSIFICATION_PER_SEQ),
@@ -438,59 +426,104 @@
               {'selector': '', 'props': [('width', 'max-content'), ('width', '-moz-max-content'), ('border-top', '1px solid lightgray'), ('border-spacing', '0px')]},
               {'selector': 'expand-toggle:checked ~ * .data', 'props': [('background-color', 'white !important')]}]
     styles_hidden_thead = styles + [{'selector': 'thead', 'props': [('display', 'none')]}]
 
     def get_html_dict(metrics):
         d_dict = {}
         for tuple in metrics:
-            d_dict[tuple[0]] = '<div class="tooltip">{}<span class="tooltiptext">{}: {}</span></div>'.format(tuple[0], tuple[0], tuple[1])
+            d_dict[tuple[0] + '<'] = '<div class="tooltip">{}<span class="tooltiptext">{}: {}</span></div><'.format(utils_labels.LABELS[tuple[0]], utils_labels.LABELS[tuple[0]], tuple[1])
+            d_dict[tuple[0] + utils_labels.UNFILTERED + '<'] = '<div class="tooltip">{}<span class="tooltiptext">{}: {}</span></div><'.format(utils_labels.LABELS[tuple[0]] + utils_labels.UNFILTERED, utils_labels.LABELS[tuple[0]], tuple[1])
         return d_dict
 
     d = get_html_dict(get_labels_taxonomic() if is_taxonomic else get_labels_genome())
 
     pattern = re.compile('|'.join(map(re.escape, d)))
 
     def translate(match):
         return d[match.group(0)]
 
     df_summary.index.name = None
 
-    html = ''
+    html = io.StringIO()
     first_metrics = True
     for metrics, metrics_label in zip(all_metrics, all_metrics_labels):
-        html += '<p style="margin-bottom: auto"><b>{}</b></p>'.format(metrics_label)
+        html.write('<p style="margin-bottom: auto"><b>{}</b></p>'.format(metrics_label))
         df_metrics = df_summary.loc[metrics]
         sorted_columns = df_metrics.columns.tolist()
         df_metrics = df_metrics.loc[:, sorted_columns]
 
         if first_metrics:
             this_style = styles
             first_metrics = False
         else:
             this_style = styles_hidden_thead
-        html += df_metrics.style.apply(get_heatmap_colors, df_metrics=df_metrics, axis=1).set_precision(3).set_table_styles(this_style).render()
+        html.write(df_metrics.style.apply(get_heatmap_colors, df_metrics=df_metrics, axis=1).format(
+            precision=3).set_table_styles(this_style).to_html())
+    html = html.getvalue()
     html = pattern.sub(translate, html)
 
-    return '<div style="margin-bottom:10pt;">{}</div>'.format(html)
+    tooltips = """
+    <style>
+        .tooltip {
+            position: relative;
+            display: inline-block;
+            border-bottom: 1px dashed lightgray;
+            cursor: help;
+        }
+        div.tooltip span.tooltiptext {
+            visibility: hidden;
+            width: 280px;
+            background-color: #555;
+            color: #fff;
+            text-align: center;
+            border-radius: 6px;
+            padding: 5px 0;
+            position: absolute;
+            z-index: 1;
+            bottom: 125%;
+            left: 50%;
+            margin-left: -60px;
+            opacity: 0;
+        }
+        div.tooltip span.tooltiptext::after {
+            content: "";
+            position: absolute;
+            top: 100%;
+            left: 50%;
+            margin-left: -5px;
+            border-width: 5px;
+            border-style: solid;
+            border-color: #555 transparent transparent transparent;
+        }
+        div.tooltip:hover span.tooltiptext {
+            visibility: visible;
+            opacity: 1;
+        }
+        tr:hover {
+            outline: 1px solid black;
+        }
+    </style>"""
+
+    return '{}<div style="margin-bottom:10pt;">{}</div>'.format(tooltips, html)
 
 
 def create_precision_recall_figure(df_summary, xname1, yname1, xname2, yname2, title):
     colors_list = plots.create_colors_list()
     bokeh_colors = [matplotlib.colors.to_hex(c) for c in colors_list]
 
     legend_it = []
     tooltips1 = [(utils_labels.TOOL, '@index'),
                  (xname1, '@{' + xname1 + '}'),
                  (yname1, '@{' + yname1 + '}')]
     tooltips2 = [(utils_labels.TOOL, '@index'),
                  (xname2, '@{' + xname2 + '}'),
                  (yname2, '@{' + yname2 + '}')]
-    p = figure(title=title, plot_width=580, plot_height=400, x_range=(0, 1), y_range=(0, 1), toolbar_location="below")
-    p.xaxis.axis_label = upper1(xname1.split('(')[0])
-    p.yaxis.axis_label = upper1(yname1.split('(')[0])
+    p = figure(title=title, width=580, height=400, x_range=(0, 1), y_range=(0, 1), toolbar_location="below")
+    p.xaxis.axis_label = utils_labels.LABELS[xname1]
+    p.yaxis.axis_label = utils_labels.LABELS[yname1]
     p.xaxis.axis_label_text_font_style = 'normal'
     p.yaxis.axis_label_text_font_style = 'normal'
     for color, (index, row) in zip(bokeh_colors, df_summary.iterrows()):
         tool = index
         source = ColumnDataSource(data=row.to_frame().T)
         pcircle = p.circle(xname1, yname1, source=source, color=color, fill_alpha=0.2, size=10)
         px = p.x(xname2, yname2, source=source, color=color, size=10)
@@ -507,15 +540,15 @@
     return p
 
 
 def create_precision_recall_all_genomes_scatter(pd_genome_bins, tools):
     colors_list = plots.create_colors_list()
     bokeh_colors = [matplotlib.colors.to_hex(c) for c in colors_list]
 
-    p = figure(title='Quality per bin', plot_width=580, plot_height=400, x_range=(0, 1), y_range=(0, 1), toolbar_location="below")
+    p = figure(title='Quality per bin', width=580, height=400, x_range=(0, 1), y_range=(0, 1), toolbar_location="below")
     p.add_tools(HoverTool(tooltips=[('Sample', '@sample_id'),
                                     ('Genome', '@mapping_id'),
                                     ('Purity of bin (bp)', '@precision_bp'),
                                     ('Completeness of bin (bp)', '@recall_bp')], toggleable=False))
 
     legend_it = []
     for color, tool in zip(bokeh_colors, tools):
@@ -534,15 +567,15 @@
 def create_contamination_plot(pd_bins, tools, title, xlabel, ylabel, create_column_function):
     pd_bins_copy = pd_bins[[utils_labels.TOOL, 'precision_bp', 'recall_bp']].copy().dropna(subset=['precision_bp'])
     create_column_function(pd_bins_copy)
 
     colors_list = plots.create_colors_list()
     bokeh_colors = [matplotlib.colors.to_hex(c) for c in colors_list]
 
-    p = figure(title=title, plot_width=580, plot_height=400, toolbar_location="below")
+    p = figure(title=title, width=580, height=400, toolbar_location="below")
     p.x_range.start = 0
     # p.y_range.start = pd_bins_copy['newcolumn'].min()
     p.y_range.end = 1
     legend_it = []
     for color, tool in zip(bokeh_colors, tools):
         pd_tool_bins = pd_bins_copy[pd_bins_copy[utils_labels.TOOL] == tool]
         pd_tool_bins = pd_tool_bins.sort_values(by='newcolumn', ascending=False).reset_index()
@@ -568,20 +601,20 @@
     df["x"] = rank_indices
     for metric, error in zip(metrics_list, errors_list):
         if error:
             df[metric + "upper"] = df[metric] + df[error]
             df[metric + "lower"] = df[metric] - df[error]
     source = ColumnDataSource(df.reset_index())
 
-    p = figure(plot_width=500, plot_height=550, x_range=(0, 7), y_range=(0, 1))
+    p = figure(width=500, height=550, x_range=(0, 7), y_range=(0, 1))
     line_colors = ["#006cba", "#008000", "#ba9e00", "red"]
     legend_it = []
     for i, (metric, error, color) in enumerate(zip(metrics_list, errors_list, line_colors)):
         pline = p.line(x='x', y=metric, line_color=color, source=source, line_width=2)
-        legend_it.append(LegendItem(label=metric, renderers=[pline]))
+        legend_it.append(LegendItem(label=utils_labels.LABELS[metric], renderers=[pline]))
         if error:
             band = Band(base='x', lower=metric + "lower", upper=metric + "upper", source=source, level='underlay',
                               fill_alpha=.3, line_width=1, line_color='black', fill_color=color)
             p.add_layout(band)
             callback = CustomJS(args = dict(band=band), code="""
                 if (band.visible == false)
                     band.visible = true;
@@ -589,79 +622,65 @@
                     band.visible = false; """)
             pline.js_on_change('visible', callback)
             if i > 1:
                 pline.visible = False
                 band.visible = False
 
     p.xaxis.ticker = FixedTicker(ticks=rank_indices)
-    p.xaxis.formatter = FuncTickFormatter(code="""
+    p.xaxis.formatter = CustomJSTickFormatter(code="""
         var mapping = {0: "superkingdom", 1: "phylum", 2: "class", 3: "order", 4: "family", 5: "genus", 6: "species", 7: "strain"};
         return mapping[tick];
     """)
     p.xaxis.major_label_orientation = 1.2
     p.add_layout(Legend(items=legend_it, location=(10, 10)), 'above')
     p.xgrid[0].grid_line_color=None
     p.ygrid[0].grid_line_alpha=0.5
     p.title.text = tool
     p.legend.click_policy = 'hide'
     return p
 
 
 def create_rankings_table(df_summary, show_rank=False):
-    columns= [utils_labels.AVG_PRECISION_BP,
-              utils_labels.AVG_RECALL_BP,
-              utils_labels.PRECISION_PER_BP,
-              utils_labels.RECALL_PER_BP,
-              utils_labels.ARI_BY_SEQ,
-              utils_labels.ARI_BY_BP,
-              utils_labels.PERCENTAGE_ASSIGNED_BPS,
-              utils_labels.ACCURACY_PER_BP]
+    columns = [utils_labels.AVG_PRECISION_BP,
+               utils_labels.AVG_RECALL_BP,
+               utils_labels.PRECISION_PER_BP,
+               utils_labels.RECALL_PER_BP,
+               utils_labels.ARI_BY_SEQ,
+               utils_labels.ARI_BY_BP,
+               utils_labels.PERCENTAGE_ASSIGNED_BPS,
+               utils_labels.ACCURACY_PER_BP]
     if show_rank:
         columns.insert(0, utils_labels.RANK)
-    pd_rankings = df_summary[columns].rename(columns={utils_labels.RANK: 'Taxonomic rank'}).round(decimals=5).reset_index()
-    pd_rankings.columns = list(map(upper1, pd_rankings.columns))
+    labels_dict = utils_labels.LABELS.copy()
+    labels_dict[utils_labels.RANK] = 'Taxonomic rank'
+    pd_rankings = df_summary[columns].rename(columns=labels_dict).round(decimals=5).reset_index()
 
     def create_table_column(field):
         return TableColumn(title=field, field=field, width=100)
 
     dt = DataTable(source=ColumnDataSource(pd_rankings),
                    columns=list(map(lambda x: create_table_column(x), pd_rankings.columns.values)),
                    width=1500,
                    height=1000,
                    reorderable=True,
                    selectable=True)
-    return [widgetbox(dt)]
-
-
-def get_genome_bins_columns():
-    return OrderedDict([('BINID', 'Bin ID'),
-                        ('genome_id', 'Most abundant genome'),
-                        ('precision_bp', utils_labels.PRECISION_PER_BP),
-                        ('recall_bp', utils_labels.RECALL_PER_BP),
-                        ('total_length', 'Bin size (bp)'),
-                        ('tp_length', 'True positives (bp)'),
-                        ('length_gs', 'True size of most abundant genome (bp)'),
-                        ('precision_seq', utils_labels.PRECISION_PER_SEQ),
-                        ('recall_seq', utils_labels.RECALL_PER_SEQ),
-                        ('total_seq_counts', 'Bin size (seq)'),
-                        ('tp_seq_counts', 'True positives (seq)'),
-                        ('seq_counts_gs', 'True size of most abundant genome (seq)')])
+    return [column(dt)]
 
 
 def create_genome_binning_plots_panel(pd_bins, pd_mean):
-    click_div = Div(text=CLICK_ON_LEGENDS_DIV, css_classes=['bk-width-auto'], style={"width": "500px", "margin-top": "15px; margin-bottom:5px;"})
-    purity_completeness_plot = column(create_precision_recall_figure(pd_mean, utils_labels.AVG_PRECISION_BP, utils_labels.AVG_RECALL_BP, utils_labels.AVG_PRECISION_SEQ, utils_labels.AVG_RECALL_SEQ, utils_labels.QUALITY_OF_BINS), css_classes=['bk-width-auto', 'bk-float-left'])
-    purity_recall_bp_plot = column(create_precision_recall_figure(pd_mean, utils_labels.PRECISION_PER_BP, utils_labels.RECALL_PER_BP, utils_labels.PRECISION_PER_SEQ, utils_labels.RECALL_PER_SEQ, utils_labels.QUALITY_OF_SAMPLE), css_classes=['bk-width-auto', 'bk-float-left'])
-
-    all_samples_div = Div(text='<div style="padding-top: 20px;">All samples</div>', css_classes=['bk-width-auto'], style={"width": "500px", "margin-top": "15px; margin-bottom:5px;"})
-    all_bins_plot = column(create_precision_recall_all_genomes_scatter(pd_bins, pd_mean.index.tolist()), css_classes=['bk-width-auto', 'bk-float-left'])
-    completeness_contamination_plot = column(create_contamination_plot(pd_bins, pd_mean.index.tolist(), 'Completeness - contamination', 'Index of bin (sorted by completeness - contamination (bp))', 'Completeness - contamination (bp)', plots.create_completeness_minus_contamination_column), css_classes=['bk-width-auto', 'bk-float-left'])
-    contamination_plot = column(create_contamination_plot(pd_bins, pd_mean.index.tolist(), 'Contamination', 'Index of bin (sorted by contamination (bp))', 'Contamination (bp)', plots.create_contamination_column), css_classes=['bk-width-auto', 'bk-float-left'])
+    click_div = Div(text=CLICK_ON_LEGENDS_DIV, styles={"width": "500px", "margin-top": "15px; margin-bottom:5px;"})
+    purity_completeness_plot = column(create_precision_recall_figure(pd_mean, utils_labels.AVG_PRECISION_BP, utils_labels.AVG_RECALL_BP, utils_labels.AVG_PRECISION_SEQ, utils_labels.AVG_RECALL_SEQ, utils_labels.QUALITY_OF_BINS))
+    purity_recall_bp_plot = column(create_precision_recall_figure(pd_mean, utils_labels.PRECISION_PER_BP, utils_labels.RECALL_PER_BP, utils_labels.PRECISION_PER_SEQ, utils_labels.RECALL_PER_SEQ, utils_labels.QUALITY_OF_SAMPLE))
+
+    all_samples_div = Div(text='<div style="padding-top: 20px;">All samples</div>', styles={"width": "500px", "margin-top": "15px; margin-bottom:5px;"})
+    all_bins_plot = column(create_precision_recall_all_genomes_scatter(pd_bins, pd_mean.index.tolist()))
+    completeness_contamination_plot = column(create_contamination_plot(pd_bins, pd_mean.index.tolist(), 'Completeness - contamination', 'Index of bin (sorted by completeness - contamination (bp))', 'Completeness - contamination (bp)', plots.create_completeness_minus_contamination_column))
+    contamination_plot = column(create_contamination_plot(pd_bins, pd_mean.index.tolist(), 'Contamination', 'Index of bin (sorted by contamination (bp))', 'Contamination (bp)', plots.create_contamination_column))
 
-    return Panel(child=column([click_div, purity_completeness_plot, purity_recall_bp_plot, all_samples_div, all_bins_plot, completeness_contamination_plot, contamination_plot], sizing_mode='scale_width', css_classes=['bk-width-auto', 'bk-display-block']), title='Plots')
+    return TabPanel(child=column([click_div, purity_completeness_plot, purity_recall_bp_plot, all_samples_div, all_bins_plot, completeness_contamination_plot, contamination_plot], sizing_mode='scale_width'), title='Plots')
 
 
 def create_genome_binning_html(df_summary, pd_bins, labels, sample_ids_list, options):
     if pd_bins.empty:
         return None
     df_summary_g = df_summary[df_summary[utils_labels.BINNING_TYPE] == 'genome']
     if df_summary_g.empty:
@@ -669,135 +688,118 @@
 
     sample_to_html = {}
     available_samples = list(df_summary_g[utils_labels.SAMPLE].unique())
     available_samples = [sample_id for sample_id in sample_ids_list if sample_id in available_samples]
     available_tools = list(df_summary_g[utils_labels.TOOL].unique())
     available_tools = [tool for tool in labels if tool in available_tools]
 
-    pd_mean = df_summary_g.groupby(utils_labels.TOOL).mean().reindex(available_tools)
+    pd_mean = df_summary_g.groupby(utils_labels.TOOL).mean(numeric_only=True).reindex(available_tools)
     pd_mean[utils_labels.SAMPLE] = AVG_OVER_SAMPLES
     sample_to_html[AVG_OVER_SAMPLES] = [create_table_html(pd_mean.T, include_cami1=True)]
 
     for sample_id, pd_sample in df_summary_g.groupby(utils_labels.SAMPLE):
         sample_to_html[sample_id] = [create_table_html(pd_sample.set_index(utils_labels.TOOL).T, include_cami1=True)]
 
     sample_ids_list_combo = [AVG_OVER_SAMPLES] + available_samples
 
-    genome_div = Div(text="""<div style="margin-bottom:10pt;">{}</div>""".format(sample_to_html[sample_ids_list_combo[0]][0]), css_classes=['bk-width-auto'])
+    genome_div = Div(text="""<div style="margin-bottom:10pt;">{}</div>""".format(sample_to_html[sample_ids_list_combo[0]][0]))
     source = ColumnDataSource(data=sample_to_html)
 
-    select_sample = Select(title="Sample:", value=sample_ids_list_combo[0], options=sample_ids_list_combo, css_classes=['bk-fit-content'])
+    select_sample = Select(title="Sample:", value=sample_ids_list_combo[0], options=sample_ids_list_combo)
     select_sample_callback = CustomJS(args=dict(source=source), code="""
         mytable.text = source.data[select_sample.value][0];
     """)
     select_sample.js_on_change('value', select_sample_callback)
     select_sample_callback.args["mytable"] = genome_div
     select_sample_callback.args["select_sample"] = select_sample
 
-    metrics_column = column(column(select_sample, create_heatmap_div(), genome_div, sizing_mode='scale_width', css_classes=['bk-width-auto']), css_classes=['bk-width-auto'], sizing_mode='scale_width')
-    metrics_panel = Panel(child=metrics_column, title="Metrics")
+    metrics_column = column(column(select_sample, create_heatmap_div(), genome_div, sizing_mode='scale_width'), sizing_mode='scale_width')
+    metrics_panel = TabPanel(child=metrics_column, title="Metrics")
 
     plots_panel = create_genome_binning_plots_panel(pd_bins, pd_mean)
 
-    bins_columns = get_genome_bins_columns()
+    bins_columns = utils_labels.get_genome_bins_columns()
     metrics_bins_panel = create_metrics_per_bin_panel(pd_bins, bins_columns, sample_ids_list, options.output_dir, 'genome')
 
     cc_table = create_contamination_completeness_table(pd_bins, options.min_completeness, options.max_contamination)
-    cc_panel = Panel(child=row(cc_table), title="#Recovered genomes")
+    cc_panel = TabPanel(child=row(cc_table), title="#Recovered genomes")
 
-    rankings_panel = Panel(child=column([Div(text="Click on the columns header for sorting.", style={"width": "500px", "margin-top": "20px"}),
+    rankings_panel = TabPanel(child=column([Div(text="Click on the columns header for sorting.", styles={"width": "500px", "margin-top": "20px"}),
                                         row(create_rankings_table(pd_mean.reset_index().set_index([utils_labels.SAMPLE, utils_labels.TOOL])))]), title="Rankings")
 
-    tabs = Tabs(tabs=[metrics_panel, plots_panel, metrics_bins_panel, rankings_panel, cc_panel], css_classes=['bk-tabs-margin', 'bk-tabs-margin-lr'])
+    tabs = Tabs(tabs=[metrics_panel, plots_panel, metrics_bins_panel, rankings_panel, cc_panel])
 
     return tabs
 
 
 def create_plots_per_binner(df_summary_t):
     tools = df_summary_t[utils_labels.TOOL].unique().tolist()
-    sample_div = Div(text=AVG_OVER_SAMPLES, css_classes=['bk-width-auto'], style={"margin-top": "15px; margin-bottom:5px;"})
+    sample_div = Div(text=AVG_OVER_SAMPLES, styles={"margin-top": "15px; margin-bottom:5px;"})
     # using the same div breaks the layout
-    sample_div2 = Div(text=AVG_OVER_SAMPLES, css_classes=['bk-width-auto'], style={"margin-top": "15px; margin-bottom:5px;"})
+    sample_div2 = Div(text=AVG_OVER_SAMPLES, styles={"margin-top": "15px; margin-bottom:5px;"})
 
     metrics_list = [utils_labels.AVG_PRECISION_BP, utils_labels.AVG_RECALL_BP, utils_labels.AVG_PRECISION_SEQ, utils_labels.AVG_RECALL_SEQ]
     errors_list = [utils_labels.AVG_PRECISION_BP_SEM, utils_labels.AVG_RECALL_BP_SEM, utils_labels.AVG_PRECISION_SEQ_SEM, utils_labels.AVG_RECALL_SEQ_SEM]
     tools_figures = [create_tax_figure(tool, df_summary_t[df_summary_t[utils_labels.TOOL] == tool], metrics_list, errors_list) for tool in tools]
-    tools_figures_columns = [column(x, css_classes=['bk-width-auto', 'bk-float-left']) for x in tools_figures]
-    tools_column_unweighted = column([sample_div] + tools_figures_columns, sizing_mode='scale_width', css_classes=['bk-width-auto', 'bk-display-block'])
+    tools_figures_columns = [column(x) for x in tools_figures]
+    tools_column_unweighted = column([sample_div] + tools_figures_columns, sizing_mode='scale_width')
 
     metrics_list = [utils_labels.PRECISION_PER_BP, utils_labels.RECALL_PER_BP, utils_labels.PRECISION_PER_SEQ, utils_labels.RECALL_PER_SEQ]
     errors_list = ['', '', '', '']
     tools_figures_weighted = [create_tax_figure(tool, df_summary_t[df_summary_t[utils_labels.TOOL] == tool], metrics_list, errors_list) for tool in tools]
-    tools_figures_columns = [column(x, css_classes=['bk-width-auto', 'bk-float-left']) for x in tools_figures_weighted]
-    tools_column_weighted = column([sample_div2] + tools_figures_columns, sizing_mode='scale_width', css_classes=['bk-width-auto', 'bk-display-block'])
+    tools_figures_columns = [column(x) for x in tools_figures_weighted]
+    tools_column_weighted = column([sample_div2] + tools_figures_columns, sizing_mode='scale_width')
 
-    tools_unweighted_panel = Panel(child=tools_column_unweighted, title=utils_labels.QUALITY_OF_BINS)
-    tools_weighted_panel = Panel(child=tools_column_weighted, title=utils_labels.QUALITY_OF_SAMPLE)
-    tools_tabs = Tabs(tabs=[tools_unweighted_panel, tools_weighted_panel], css_classes=['bk-tabs-margin', 'bk-tabs-margin-lr'])
+    tools_unweighted_panel = TabPanel(child=tools_column_unweighted, title=utils_labels.QUALITY_OF_BINS)
+    tools_weighted_panel = TabPanel(child=tools_column_weighted, title=utils_labels.QUALITY_OF_SAMPLE)
+    tools_tabs = Tabs(tabs=[tools_unweighted_panel, tools_weighted_panel])
     return tools_tabs
 
 
-def get_tax_bins_columns():
-    return OrderedDict([('TAXID', 'Taxon ID'),
-                        ('name', 'Scientific name'),
-                        ('rank', 'Taxonomic rank'),
-                        ('precision_bp', utils_labels.PRECISION_PER_BP),
-                        ('recall_bp', utils_labels.RECALL_PER_BP),
-                        ('total_length', 'Bin size (bp)'),
-                        ('tp_length', 'True positives (bp)'),
-                        ('length_gs', 'True size (bp)'),
-                        ('precision_seq', utils_labels.PRECISION_PER_SEQ),
-                        ('recall_seq', utils_labels.RECALL_PER_SEQ),
-                        ('total_seq_counts', 'Bin size (seq)'),
-                        ('tp_seq_counts', 'True positives (seq)'),
-                        ('seq_counts_gs', 'True size (seq)'),
-                        ('filtered', 'Filtered')])
-
-
 def create_tax_ranks_panel(qbins_plots_list, qsamples_plots_list, cc_plots_dict_list, contamination_plots_list):
-    sample_div = Div(text=CLICK_ON_LEGENDS_DIV, css_classes=['bk-width-auto'], style={"width": "500px", "margin-top": "20px"})
-    all_samples_div = Div(text='<div style="padding-top: 20px;">All samples</div>', css_classes=['bk-width-auto'], style={"width": "500px", "margin-top": "15px; margin-bottom:5px;"})
-    all_samples_div2 = Div(text='<div style="padding-top: 20px;">All samples</div>', css_classes=['bk-width-auto'], style={"width": "500px", "margin-top": "15px; margin-bottom:5px;"})
-    unweighted_panel = Panel(child=column([sample_div] + qbins_plots_list + [all_samples_div] + cc_plots_dict_list + [all_samples_div2] + contamination_plots_list, sizing_mode='scale_width', css_classes=['bk-width-auto', 'bk-display-block']), title=utils_labels.QUALITY_OF_BINS)
-
-    sample_div2 = Div(text=CLICK_ON_LEGENDS_DIV, css_classes=['bk-width-auto'], style={"width": "500px", "margin-top": "20px"})
-    weighted_panel = Panel(child=column([sample_div2] + qsamples_plots_list, sizing_mode='scale_width', css_classes=['bk-width-auto', 'bk-display-block']), title=utils_labels.QUALITY_OF_SAMPLE)
-    tax_ranks_tabs = Tabs(tabs=[unweighted_panel, weighted_panel], css_classes=['bk-tabs-margin', 'bk-tabs-margin-lr'])
-    return Panel(child=tax_ranks_tabs, title="Plots per taxonomic rank")
+    sample_div = Div(text=CLICK_ON_LEGENDS_DIV, styles={"width": "500px", "margin-top": "20px"})
+    all_samples_div = Div(text='<div style="padding-top: 20px;">All samples</div>', styles={"width": "500px", "margin-top": "15px; margin-bottom:5px;"})
+    all_samples_div2 = Div(text='<div style="padding-top: 20px;">All samples</div>', styles={"width": "500px", "margin-top": "15px; margin-bottom:5px;"})
+    unweighted_panel = TabPanel(child=column([sample_div] + qbins_plots_list + [all_samples_div] + cc_plots_dict_list + [all_samples_div2] + contamination_plots_list, sizing_mode='scale_width'), title=utils_labels.QUALITY_OF_BINS)
+
+    sample_div2 = Div(text=CLICK_ON_LEGENDS_DIV, styles={"width": "500px", "margin-top": "20px"})
+    weighted_panel = TabPanel(child=column([sample_div2] + qsamples_plots_list, sizing_mode='scale_width'), title=utils_labels.QUALITY_OF_SAMPLE)
+    tax_ranks_tabs = Tabs(tabs=[unweighted_panel, weighted_panel])
+    return TabPanel(child=tax_ranks_tabs, title="Plots per taxonomic rank")
 
 
 def create_taxonomic_binning_html(df_summary, pd_bins, labels, sample_ids_list, options):
     if pd_bins.empty:
         return None
     df_summary_t = df_summary[df_summary[utils_labels.BINNING_TYPE] == 'taxonomic'].copy()
     df_summary_t[[utils_labels.UNIFRAC_BP, utils_labels.UNIFRAC_SEQ]] = df_summary_t[[utils_labels.UNIFRAC_BP, utils_labels.UNIFRAC_SEQ]].apply(pd.to_numeric)
 
     rank_to_sample_to_html = defaultdict(list)
     qbins_plots_dict = OrderedDict([(rank, '') for rank in load_ncbi_taxinfo.RANKS])
     qsamples_plots_dict = OrderedDict([(rank, '') for rank in load_ncbi_taxinfo.RANKS])
     cc_plots_dict = OrderedDict([(rank, '') for rank in load_ncbi_taxinfo.RANKS])
     contamination_plots_dict = OrderedDict([(rank, '') for rank in load_ncbi_taxinfo.RANKS])
 
-    pd_mean = df_summary_t.groupby([utils_labels.RANK, utils_labels.TOOL]).mean().reset_index()
+    pd_mean = df_summary_t.groupby([utils_labels.RANK, utils_labels.TOOL]).mean(numeric_only=True).reset_index()
     pd_mean[utils_labels.SAMPLE] = AVG_OVER_SAMPLES
     for rank, pd_mean_rank in pd_mean.groupby(utils_labels.RANK):
         available_tools = list(pd_mean_rank[utils_labels.TOOL].unique())
         available_tools = [tool for tool in labels if tool in available_tools]
         pd_mean_rank = pd_mean_rank.set_index(utils_labels.TOOL).reindex(available_tools)
 
         purity_completeness_plot = create_precision_recall_figure(pd_mean_rank, utils_labels.AVG_PRECISION_BP, utils_labels.AVG_RECALL_BP, utils_labels.AVG_PRECISION_SEQ, utils_labels.AVG_RECALL_SEQ, rank)
         purity_recall_bp_plot = create_precision_recall_figure(pd_mean_rank, utils_labels.PRECISION_PER_BP, utils_labels.RECALL_PER_BP, utils_labels.PRECISION_PER_SEQ, utils_labels.RECALL_PER_SEQ, rank)
-        qbins_plots_dict[rank] = column(purity_completeness_plot, css_classes=['bk-width-auto', 'bk-float-left'])
-        qsamples_plots_dict[rank] = column(purity_recall_bp_plot, css_classes=['bk-width-auto', 'bk-float-left'])
+        qbins_plots_dict[rank] = column(purity_completeness_plot)
+        qsamples_plots_dict[rank] = column(purity_recall_bp_plot)
 
         pd_bins_rank = pd_bins[pd_bins['rank'] == rank]
         completeness_minus_contamination_plot = create_contamination_plot(pd_bins_rank, available_tools, rank + ' | Completeness - contamination', 'Index of bin (sorted by completeness - contamination (bp))', 'Completeness - contamination (bp)', plots.create_completeness_minus_contamination_column)
         contamination_plot = create_contamination_plot(pd_bins_rank, available_tools, rank + ' | Contamination', 'Index of bin (sorted by contamination (bp))', 'Contamination (bp)', plots.create_contamination_column)
-        cc_plots_dict[rank] = column(completeness_minus_contamination_plot, css_classes=['bk-width-auto', 'bk-float-left'])
-        contamination_plots_dict[rank] = column(contamination_plot, css_classes=['bk-width-auto', 'bk-float-left'])
+        cc_plots_dict[rank] = column(completeness_minus_contamination_plot)
+        contamination_plots_dict[rank] = column(contamination_plot)
 
         rank_to_sample_to_html[rank].append(create_table_html(pd_mean_rank.T, is_taxonomic=True))
 
     qbins_plots_list = [v for k, v in qbins_plots_dict.items() if v]
     qsamples_plots_list = [v for k, v in qsamples_plots_dict.items() if v]
     cc_plots_dict_list = [v for k, v in cc_plots_dict.items() if v]
     contamination_plots_list = [v for k, v in contamination_plots_dict.items() if v]
@@ -815,79 +817,73 @@
             rank_to_sample_to_html[rank].append(create_table_html(pd_rank_sample, is_taxonomic=True))
 
     if not rank_to_sample_to_html:
         return None
 
     sample_ids_list_combo = [AVG_OVER_SAMPLES] + sample_ids_list
 
-    taxonomic_div = Div(text="""<div style="margin-bottom:10pt;">{}</div>""".format(rank_to_sample_to_html[load_ncbi_taxinfo.RANKS[0]][0]), css_classes=['bk-width-auto'])
+    taxonomic_div = Div(text="""<div style="margin-bottom:10pt;">{}</div>""".format(rank_to_sample_to_html[load_ncbi_taxinfo.RANKS[0]][0]))
     source = ColumnDataSource(data=rank_to_sample_to_html)
 
     available_ranks = list(pd_groupby_rank.groups.keys())
     available_ranks_sorted = [rank for rank in load_ncbi_taxinfo.RANKS if rank in available_ranks]
 
-    select_rank = Select(title="Taxonomic rank:", value=load_ncbi_taxinfo.RANKS[0], options=available_ranks_sorted, css_classes=['bk-fit-content'])
-    select_sample = Select(title="Sample:", value='0', options=list(zip(map(str, range(len(sample_ids_list_combo))), sample_ids_list_combo)), css_classes=['bk-fit-content'])
+    select_rank = Select(title="Taxonomic rank:", value=load_ncbi_taxinfo.RANKS[0], options=available_ranks_sorted)
+    select_sample = Select(title="Sample:", value='0', options=list(zip(map(str, range(len(sample_ids_list_combo))), sample_ids_list_combo)))
     select_rank_sample_callback = CustomJS(args=dict(source=source), code="""
         mytable.text = source.data[select_rank.value][select_sample.value];
     """)
     select_rank.js_on_change('value', select_rank_sample_callback)
     select_sample.js_on_change('value', select_rank_sample_callback)
     select_rank_sample_callback.args["mytable"] = taxonomic_div
     select_rank_sample_callback.args["select_rank"] = select_rank
     select_rank_sample_callback.args["select_sample"] = select_sample
 
-    metrics_column = column(column(row(select_sample, select_rank, css_classes=['bk-width-auto', 'bk-combo-box']), create_heatmap_div(), taxonomic_div, sizing_mode='scale_width', css_classes=['bk-width-auto']), css_classes=['bk-width-auto'], sizing_mode='scale_width')
-    metrics_panel = Panel(child=metrics_column, title="Metrics")
+    metrics_column = column(column(row(select_sample, select_rank), create_heatmap_div(), taxonomic_div, sizing_mode='scale_width'), sizing_mode='scale_width')
+    metrics_panel = TabPanel(child=metrics_column, title="Metrics")
 
-    bins_columns = get_tax_bins_columns()
+    bins_columns = utils_labels.get_tax_bins_columns()
     if 'name' not in pd_bins.columns or pd_bins['name'].isnull().any():
         del bins_columns['name']
 
     metrics_bins_panel = create_metrics_per_bin_panel(pd_bins, bins_columns, sample_ids_list, options.output_dir, 'taxonomic')
 
-    rankings_panel = Panel(child=column([Div(text="Click on the columns header for sorting.", style={"width": "500px", "margin-top": "20px"}),
+    rankings_panel = TabPanel(child=column([Div(text="Click on the columns header for sorting.", styles={"width": "500px", "margin-top": "20px"}),
                                         row(create_rankings_table(pd_mean.reset_index().set_index([utils_labels.SAMPLE, utils_labels.TOOL]), True))]), title="Rankings")
 
     tax_ranks_panel = create_tax_ranks_panel(qbins_plots_list, qsamples_plots_list, cc_plots_dict_list, contamination_plots_list)
 
-    tools_panel = Panel(child=create_plots_per_binner(pd_mean), title="Plots per binner")
+    tools_panel = TabPanel(child=create_plots_per_binner(pd_mean), title="Plots per binner")
 
-    tabs = Tabs(tabs=[metrics_panel, tax_ranks_panel, tools_panel, metrics_bins_panel, rankings_panel], css_classes=['bk-tabs-margin', 'bk-tabs-margin-lr'])
+    tabs = Tabs(tabs=[metrics_panel, tax_ranks_panel, tools_panel, metrics_bins_panel, rankings_panel])
 
     return tabs
 
 
 def create_html(df_summary, pd_bins, labels, sample_ids_list, options, desc_text):
     logging.getLogger('amber').info('Creating HTML page')
     create_heatmap_bar(options.output_dir)
     tabs_list = []
 
     metrics_row_g = create_genome_binning_html(df_summary, pd_bins[pd_bins['rank'] == 'NA'], labels, sample_ids_list, options)
     if metrics_row_g:
-        tabs_list.append(Panel(child=metrics_row_g, title="Genome binning"))
+        tabs_list.append(TabPanel(child=metrics_row_g, title="Genome binning"))
 
     metrics_row_t = create_taxonomic_binning_html(df_summary, pd_bins[pd_bins['rank'] != 'NA'], labels, sample_ids_list, options)
     if metrics_row_t:
-        tabs_list.append(Panel(child=metrics_row_t, title="Taxonomic binning"))
+        tabs_list.append(TabPanel(child=metrics_row_t, title="Taxonomic binning"))
 
-    tabs = Tabs(tabs=tabs_list, css_classes=['bk-tabs-margin'])
+    tabs = Tabs(tabs=tabs_list)
 
     title = create_title_div("main", "AMBER: Assessment of Metagenome BinnERs", " produced on {0} with AMBER version {1} ".format(
             datetime.datetime.now().strftime("%Y-%m-%d %H:%M"), __version__))
 
     if desc_text:
-        data_desc_div = Div(text="""<div style="text-align:left;font-size: 11pt;font-weight: bold;">{}""".format(desc_text), css_classes=['bk-width-auto'])
-        html_columns = column(title, data_desc_div, tabs, sizing_mode='scale_width', css_classes=['bk-width-auto-main'])
+        data_desc_div = Div(text="""<div style="text-align:left;font-size: 11pt;font-weight: bold;">{}""".format(desc_text))
+        html_columns = column(title, data_desc_div, tabs, sizing_mode='scale_width')
     else:
-        html_columns = column(title, tabs, sizing_mode='scale_width', css_classes=['bk-width-auto-main'])
-    script, div = components(html_columns)
-    js_resources = INLINE.render_js()
-    css_resources = INLINE.render_css()
-
-    html = TEMPLATE.render(js_resources=js_resources,
-            css_resources=css_resources,
-            script=script,
-            div=div)
+        html_columns = column(title, tabs, sizing_mode='scale_width')
+
+    html = file_html(models=html_columns, resources=INLINE, title='AMBER: Assessment of Metagenome BinnERs', template=TEMPLATE)
 
     with open(os.path.join(options.output_dir, "index.html"), 'w') as f:
         f.write(html)
```

### Comparing `cami-amber-2.0.3/src/binning_classes.py` & `cami-amber-2.0.4/src/binning_classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Department of Computational Biology for Infection Research - Helmholtz Centre for Infection Research
+# Copyright 2023 Department of Computational Biology for Infection Research - Helmholtz Centre for Infection Research
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -17,26 +17,27 @@
 import logging
 import itertools
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 matplotlib.use('Agg')
 import os
+import math
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from collections import OrderedDict
 from src.utils import labels as utils_labels
 from src.utils import load_ncbi_taxinfo
 from src.utils import ProfilingTools as pf
 from src import unifrac_distance as uf
 from src import precision_recall_per_bin
 from src import plots
 
 
-class Metrics():
+class Metrics:
     def __init__(self):
         self.__percentage_of_assigned_bps = .0
         self.__percentage_of_assigned_seqs = .0
         self.__accuracy_bp = .0
         self.__accuracy_seq = .0
         self.__rand_index_bp = .0
         self.__adjusted_rand_index_bp = .0
@@ -299,92 +300,52 @@
     @unifrac_seq.setter
     def unifrac_seq(self, unifrac_seq):
         self.__unifrac_seq = unifrac_seq
 
     @staticmethod
     def compute_rand_index(confusion_df, col_name, gs_col_name, field):
         def choose2(n):
-            return (n * (n - 1)) / 2.0
+            return math.comb(n, 2)
 
-        bin_mapping_comb = confusion_df[field].apply(choose2).sum()
-        bin_comb = confusion_df.groupby(col_name).agg({field: 'sum'})[field].apply(choose2).sum()
-        mapping_comb = confusion_df.groupby(gs_col_name).agg({field: 'sum'})[field].apply(choose2).sum()
-        num_bp_comb = choose2(confusion_df[field].sum())
+        bin_mapping_comb = sum(confusion_df[field].apply(choose2))
+        bin_comb = sum(confusion_df.groupby(col_name).agg({field: 'sum'})[field].apply(choose2))
+        mapping_comb = sum(confusion_df.groupby(gs_col_name).agg({field: 'sum'})[field].apply(choose2))
+        num_bp_comb = choose2(sum(confusion_df[field]))
 
         rand_index = ((num_bp_comb - bin_comb - mapping_comb + 2 * bin_mapping_comb) / num_bp_comb) if num_bp_comb != 0 else .0
 
-        temp = (bin_comb * mapping_comb / num_bp_comb) if num_bp_comb != 0 else .0
+        temp = (bin_comb * (mapping_comb / num_bp_comb)) if num_bp_comb != 0 else .0
         ret = bin_mapping_comb - temp
         denominator = (((bin_comb + mapping_comb) / 2.0) - temp)
         adjusted_rand_index = (ret / denominator) if denominator != 0 else .0
 
         return rand_index, adjusted_rand_index
 
     def get_ordered_dict(self):
         def f1_score(metric1, metric2):
             if metric1 + metric2 > 0:
                 return 2 * metric1 * metric2 / (metric1 + metric2)
             else:
                 return np.nan
 
-        f1_score_bp = f1_score(self.__precision_avg_bp, self.__recall_avg_bp)
-        f1_score_seq = f1_score(self.__precision_avg_seq, self.__recall_avg_seq)
-        f1_score_bp_cami1 = f1_score(self.__precision_avg_bp, self.__recall_avg_bp_cami1)
-        f1_score_seq_cami1 = f1_score(self.__precision_avg_seq, self.__recall_avg_seq_cami1)
-        f1_score_per_bp = f1_score(self.__precision_weighted_bp, self.__recall_weighted_bp)
-        f1_score_per_seq = f1_score(self.__precision_weighted_seq, self.__recall_weighted_seq)
+        metrics_dict = {metric.split("__")[1]: value for metric, value in self.__dict__.items()}
+        metrics_dict['f1_score_bp'] = f1_score(self.__precision_avg_bp, self.__recall_avg_bp)
+        metrics_dict['f1_score_seq'] = f1_score(self.__precision_avg_seq, self.__recall_avg_seq)
+        metrics_dict['f1_score_bp_cami1'] = f1_score(self.__precision_avg_bp, self.__recall_avg_bp_cami1)
+        metrics_dict['f1_score_seq_cami1'] = f1_score(self.__precision_avg_seq, self.__recall_avg_seq_cami1)
+        metrics_dict['f1_score_per_bp'] = f1_score(self.__precision_weighted_bp, self.__recall_weighted_bp)
+        metrics_dict['f1_score_per_seq'] = f1_score(self.__precision_weighted_seq, self.__recall_weighted_seq)
+        metrics_dict['misclassification_bp'] = 1 - self.__precision_weighted_bp
+        metrics_dict['misclassification_seq'] = 1 - self.__precision_weighted_seq
 
         return OrderedDict([(utils_labels.TOOL, None),
                             (utils_labels.BINNING_TYPE, None),
                             (utils_labels.SAMPLE, None),
-                            (utils_labels.RANK, None),
-                            (utils_labels.AVG_PRECISION_BP, [self.__precision_avg_bp]),
-                            (utils_labels.AVG_PRECISION_BP_SEM, [self.__precision_avg_bp_sem]),
-
-                            ('avg_precision_bp_var', [self.__precision_avg_bp_var]),
-                            (utils_labels.AVG_RECALL_BP, [self.__recall_avg_bp]),
-                            (utils_labels.AVG_RECALL_BP_CAMI1, [self.__recall_avg_bp_cami1]),
-                            (utils_labels.AVG_RECALL_BP_SEM, [self.__recall_avg_bp_sem]),
-                            (utils_labels.AVG_RECALL_BP_SEM_CAMI1, [self.__recall_avg_bp_sem_cami1]),
-                            ('avg_recall_bp_var', [self.__recall_avg_bp_var]),
-                            ('avg_recall_bp_var_cami1', [self.__recall_avg_bp_var_cami1]),
-                            (utils_labels.F1_SCORE_BP, [f1_score_bp]),
-                            (utils_labels.F1_SCORE_BP_CAMI1, [f1_score_bp_cami1]),
-
-                            (utils_labels.AVG_PRECISION_SEQ, [self.__precision_avg_seq]),
-                            (utils_labels.AVG_PRECISION_SEQ_SEM, [self.__precision_avg_seq_sem]),
-                            (utils_labels.AVG_RECALL_SEQ, [self.__recall_avg_seq]),
-                            (utils_labels.AVG_RECALL_SEQ_CAMI1, [self.__recall_avg_seq_cami1]),
-                            (utils_labels.AVG_RECALL_SEQ_SEM, [self.__recall_avg_seq_sem]),
-                            (utils_labels.AVG_RECALL_SEQ_SEM_CAMI1, [self.__recall_avg_seq_sem_cami1]),
-                            (utils_labels.F1_SCORE_SEQ, [f1_score_seq]),
-                            (utils_labels.F1_SCORE_SEQ_CAMI1, [f1_score_seq_cami1]),
-
-                            (utils_labels.PRECISION_PER_BP, [self.__precision_weighted_bp]),
-                            (utils_labels.PRECISION_PER_SEQ, [self.__precision_weighted_seq]),
-                            (utils_labels.RECALL_PER_BP, [self.__recall_weighted_bp]),
-                            (utils_labels.RECALL_PER_SEQ, [self.__recall_weighted_seq]),
-                            (utils_labels.F1_SCORE_PER_BP, [f1_score_per_bp]),
-                            (utils_labels.F1_SCORE_PER_SEQ, [f1_score_per_seq]),
-
-                            (utils_labels.ACCURACY_PER_BP, [self.__accuracy_bp]),
-                            (utils_labels.ACCURACY_PER_SEQ, [self.__accuracy_seq]),
-
-                            (utils_labels.PERCENTAGE_ASSIGNED_BPS, [self.__percentage_of_assigned_bps]),
-                            (utils_labels.PERCENTAGE_ASSIGNED_SEQS, [self.__percentage_of_assigned_seqs]),
-                            (utils_labels.RI_BY_BP, [self.__rand_index_bp]),
-                            (utils_labels.RI_BY_SEQ, [self.__rand_index_seq]),
-                            (utils_labels.ARI_BY_BP, [self.__adjusted_rand_index_bp]),
-                            (utils_labels.ARI_BY_SEQ, [self.__adjusted_rand_index_seq]),
-
-                            (utils_labels.UNIFRAC_BP, self.__unifrac_bp),
-                            (utils_labels.UNIFRAC_SEQ, self.__unifrac_seq),
-
-                            (utils_labels.MISCLASSIFICATION_PER_BP, [1 - self.__precision_weighted_bp]),
-                            (utils_labels.MISCLASSIFICATION_PER_SEQ, [1 - self.__precision_weighted_seq])])
+                            (utils_labels.RANK, None)] +
+                            [(k, [v]) for k, v in metrics_dict.items()])
 
 
 class Query(ABC):
     def __init__(self, label, sample_id, options):
         self.__label = label
         self.__sample_id = sample_id
         self.__gold_standard = None
@@ -513,15 +474,15 @@
         metrics_dict = self.metrics.get_ordered_dict()
         metrics_dict[utils_labels.TOOL] = self.label
         metrics_dict[utils_labels.BINNING_TYPE] = self.binning_type
         metrics_dict[utils_labels.RANK] = 'NA'
         return pd.DataFrame(metrics_dict)
 
     def compute_metrics(self):
-        if self.label == utils_labels.GS and self.options.only_taxonomic_queries:
+        if self.label == utils_labels.GS and (self.options.only_taxonomic_queries or self.options.skip_gs):
             return False
         logging.getLogger('amber').info('Evaluating {} (sample {}, genome binning)'.format(self.label, self.sample_id))
         gs_df = self.gold_standard_df
         gs_df = gs_df[['SEQUENCEID', 'BINID', 'LENGTH']].rename(columns={'LENGTH': 'seq_length', 'BINID': 'genome_id'})
 
         query_df = self.df
         query_df = query_df[['SEQUENCEID', 'BINID']]
@@ -590,16 +551,20 @@
             precision_df = precision_df[~precision_df['genome_id'].isin(self.options.genome_to_unique_common)]
 
         self.metrics.precision_avg_bp = precision_df['precision_bp'].mean()
         self.metrics.precision_avg_bp_sem = precision_df['precision_bp'].sem()
         self.metrics.precision_avg_bp_var = precision_df['precision_bp'].var()
         self.metrics.precision_avg_seq = precision_df['precision_seq'].mean()
         self.metrics.precision_avg_seq_sem = precision_df['precision_seq'].sem()
-        self.metrics.precision_weighted_bp = precision_df['tp_length'].sum() / precision_df['total_length'].sum()
-        self.metrics.precision_weighted_seq = precision_df['tp_seq_counts'].sum() / precision_df['total_seq_counts'].sum()
+
+        def safe_divide(x, y):
+            return x / y if y else np.nan
+
+        self.metrics.precision_weighted_bp = safe_divide(precision_df['tp_length'].sum(), precision_df['total_length'].sum())
+        self.metrics.precision_weighted_seq = safe_divide(precision_df['tp_seq_counts'].sum(), precision_df['total_seq_counts'].sum())
 
         genome_sizes_df = gs_df.groupby('genome_id', sort=False).agg({'seq_length': 'sum', 'SEQUENCEID': 'count'}).rename(columns={'seq_length': 'length_gs', 'SEQUENCEID': 'seq_counts_gs'})
         precision_df = precision_df.reset_index().join(genome_sizes_df, on='genome_id', how='left', sort=False).set_index('BINID')
         precision_df['recall_bp'] = precision_df['tp_length'] / precision_df['length_gs']
         precision_df['recall_seq'] = precision_df['tp_seq_counts'] / precision_df['seq_counts_gs']
         precision_df['rank'] = 'NA'
 
@@ -899,15 +864,15 @@
         self.precision_df = pd.concat([self.precision_df, tp_fp_fn_df.reset_index().sort_values(
             by='recall_bp', axis=0, ascending=False)], ignore_index=True, sort=True)
         self.recall_df = self.precision_df
 
         self.recall_df['name'] = self.recall_df['TAXID'].apply(lambda x: TaxonomicQuery.taxonomy_df.loc[x]['name'])
 
     def compute_metrics(self):
-        if self.label == utils_labels.GS and self.options.only_genome_queries:
+        if self.label == utils_labels.GS and (self.options.only_genome_queries or self.options.skip_gs):
             return False
         logging.getLogger('amber').info('Evaluating {} (sample {}, taxonomic binning)'.format(self.label, self.sample_id))
         for rank in self.rank_to_df:
             self.compute_metrics_per_rank(rank)
 
         unifrac_bp, unifrac_seq = self.compute_unifrac(all_bins=True)
         for rank in self.metrics:
@@ -920,15 +885,16 @@
                 self.metrics_filtered[rank].unifrac_seq = unifrac_seq
 
         return True
 
 
 class Options:
     def __init__(self, filter_tail_percentage, genome_to_unique_common, filter_keyword, min_length,
-                 rank_as_genome_binning, output_dir, min_completeness=None, max_contamination=None):
+                 rank_as_genome_binning, output_dir, min_completeness=None, max_contamination=None,
+                 skip_gs=False):
         self.__filter_tail_percentage = float(filter_tail_percentage) if filter_tail_percentage else .0
         self.__genome_to_unique_common = genome_to_unique_common
         self.__filter_keyword = filter_keyword
         self.__min_length = int(min_length) if min_length else 0
         if rank_as_genome_binning and rank_as_genome_binning not in load_ncbi_taxinfo.RANKS:
             exit("Not a valid rank to assess taxonomic binning as genome binning (option --rank_as_genome_binning): " + rank_as_genome_binning)
         self.__rank_as_genome_binning = rank_as_genome_binning
@@ -939,14 +905,15 @@
             self.__min_completeness = [int(x.strip()) / 100.0 for x in min_completeness.split(',')]
         else:
             self.__min_completeness = [.5, .7, .9]
         if max_contamination:
             self.__max_contamination = [int(x.strip()) / 100.0 for x in max_contamination.split(',')]
         else:
             self.__max_contamination = [.1, .05]
+        self.__skip_gs = skip_gs
 
     @property
     def filter_tail_percentage(self):
         return self.__filter_tail_percentage
 
     @property
     def genome_to_unique_common(self):
@@ -980,14 +947,18 @@
     def min_completeness(self):
         return self.__min_completeness
 
     @property
     def max_contamination(self):
         return self.__max_contamination
 
+    @property
+    def skip_gs(self):
+        return self.__skip_gs
+
     @filter_tail_percentage.setter
     def filter_tail_percentage(self, filter_tail_percentage):
         self.__filter_tail_percentage = filter_tail_percentage
 
     @genome_to_unique_common.setter
     def genome_to_unique_common(self, genome_to_unique_common):
         self.__genome_to_unique_common = genome_to_unique_common
@@ -1019,7 +990,11 @@
     @min_completeness.setter
     def min_completeness(self, min_completeness):
         self.__min_completeness = min_completeness
 
     @max_contamination.setter
     def max_contamination(self, max_contamination):
         self.__max_contamination = max_contamination
+
+    @skip_gs.setter
+    def skip_gs(self, skip_gs):
+        self.__skip_gs = skip_gs
```

### Comparing `cami-amber-2.0.3/src/plot_by_genome.py` & `cami-amber-2.0.4/src/plot_by_genome.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-#!/usr/bin/env python
-
-# Copyright 2020 Department of Computational Biology for Infection Research - Helmholtz Centre for Infection Research
+# Copyright 2023 Department of Computational Biology for Infection Research - Helmholtz Centre for Infection Research
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -16,14 +14,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import matplotlib
 import numpy as np
 
 matplotlib.use('Agg')
 import matplotlib.pyplot as plt
+import matplotlib.ticker as ticker
 import os, sys, inspect
 currentdir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 parentdir = os.path.dirname(currentdir)
 sys.path.insert(0, parentdir)
 from src import plots
 from src.utils import labels as utils_labels
 
@@ -82,16 +81,18 @@
     # turn on grid
     axs.minorticks_on()
     axs.grid(which='major', linestyle='-', linewidth='0.5')
     axs.grid(which='minor', linestyle=':', linewidth='0.5')
 
     # transform plot_labels to percentages
     vals = axs.get_xticks()
+    axs.xaxis.set_major_locator(ticker.FixedLocator(vals))
     axs.set_xticklabels(['{:3.0f}%'.format(x * 100) for x in vals])
     vals = axs.get_yticks()
+    axs.yaxis.set_major_locator(ticker.FixedLocator(vals))
     axs.set_yticklabels(['{:3.0f}%'.format(x * 100) for x in vals])
 
     plt.xlabel('Purity per bin')
     plt.ylabel('Completeness per genome')
     plt.tight_layout()
     fig.savefig(os.path.join(output_dir, 'genome', 'purity_completeness_per_bin.eps'), dpi=100, format='eps', bbox_inches='tight')
```

### Comparing `cami-amber-2.0.3/src/plots.py` & `cami-amber-2.0.4/src/plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,16 +87,21 @@
         axs.scatter(pd_tool['genome_coverage'], pd_tool[pd_target_column], marker='o', color=colors_list[i], s=[3] * pd_tool.shape[0])
         window = 50
         rolling_mean = pd_tool[pd_target_column].rolling(window=window, min_periods=10).mean()
         axs.plot(pd_tool['genome_coverage'], rolling_mean, color=colors_list[i])
 
     axs.set_ylim([-0.01, 1.01])
 
-    axs.set_xticklabels(['{:,.1f}'.format(np.exp(x)) for x in axs.get_xticks()], fontsize=12)
-    axs.set_yticklabels(['{:3.0f}'.format(x * 100) for x in axs.get_yticks()], fontsize=12)
+    vals = axs.get_xticks()
+    axs.xaxis.set_major_locator(ticker.FixedLocator(vals))
+    axs.set_xticklabels(['{:,.1f}'.format(np.exp(x)) for x in vals], fontsize=12)
+
+    vals = axs.get_yticks()
+    axs.yaxis.set_major_locator(ticker.FixedLocator(vals))
+    axs.set_yticklabels(['{:3.0f}'.format(x * 100) for x in vals], fontsize=12)
 
     axs.tick_params(axis='x', labelsize=12)
 
     if pd_target_column == 'precision_bp':
         ylabel = 'Purity per bin (%)'
         file_name = 'purity_by_genome_coverage'
     else:
@@ -128,15 +133,15 @@
             recall_df = recall_df.reset_index().set_index(['sample_id', utils_labels.TOOL])
             pd_genomes_recall = pd.concat([pd_genomes_recall, recall_df])
     return pd_genomes_recall
 
 
 def plot_precision_recall_by_coverage(sample_id_to_queries_list, pd_bins_g, coverages_pd, available_tools, output_dir):
     # compute average genome coverage if coverages for multiple samples were provided
-    coverages_pd = coverages_pd.groupby(['GENOMEID']).mean()
+    coverages_pd = coverages_pd.groupby(['GENOMEID']).mean(numeric_only=True)
     coverages_pd.rename(columns={'GENOMEID': 'genome_id'})
     coverages_pd = coverages_pd.sort_values(by=['COVERAGE'])
     coverages_pd['rank'] = coverages_pd['COVERAGE'].rank()
 
     pd_genomes_recall = get_pd_genomes_recall(sample_id_to_queries_list)
     pd_genomes_recall['genome_index'] = pd_genomes_recall['genome_id'].map(coverages_pd['rank'].to_dict())
     pd_genomes_recall = pd_genomes_recall.reset_index()
@@ -247,14 +252,15 @@
     axs.grid(which='major', linestyle=':', linewidth='0.5', color='lightgrey')
 
     # force axes to be from 0 to 100%
     axs.set_xlim([-0.01, 1.01])
 
     # transform plot_labels to percentages
     vals = axs.get_xticks()
+    axs.xaxis.set_major_locator(ticker.FixedLocator(vals))
     axs.set_xticklabels(['{:3.0f}'.format(x * 100) for x in vals])
 
     # enable code to rotate labels
     tick_labels = axs.get_yticklabels()
     plt.setp(tick_labels, fontsize=13) ## rotation=55
 
     for box in bplot['boxes']:
@@ -285,67 +291,71 @@
 def plot_summary(color_indices, df_results, labels, output_dir, rank, plot_type, file_name, xlabel, ylabel):
     available_tools = df_results[utils_labels.TOOL].unique()
     tools = [tool for tool in labels if tool in available_tools]
 
     colors_list = create_colors_list()
     if color_indices:
         colors_list = [colors_list[i] for i in color_indices]
-    df_mean = df_results.groupby(utils_labels.TOOL).mean().reindex(tools)
+    df_mean = df_results.groupby(utils_labels.TOOL).mean(numeric_only=True).reindex(tools)
 
     binning_type = df_results[utils_labels.BINNING_TYPE].iloc[0]
 
     if len(df_mean) > len(colors_list):
         raise RuntimeError("Plot only supports 29 colors")
 
     fig, axs = plt.subplots(figsize=(5, 4.5))
 
     # force axes to be from 0 to 100%
     axs.set_xlim([0.0, 1.0])
     axs.set_ylim([0.0, 1.0])
 
     if plot_type == 'e':
         for i, (tool, df_row) in enumerate(df_mean.iterrows()):
-            axs.errorbar(df_row[utils_labels.AVG_PRECISION_BP], df_row[utils_labels.AVG_RECALL_BP], xerr=df_row['avg_precision_bp_var'], yerr=df_row['avg_recall_bp_var'],
+            axs.errorbar(df_row['precision_avg_bp'], df_row['recall_avg_bp_cami1'], xerr=df_row['precision_avg_bp_var'], yerr=df_row['recall_avg_bp_var_cami1'],
                          fmt='o',
                          ecolor=colors_list[i],
                          mec=colors_list[i],
                          mfc=colors_list[i],
                          capsize=3,
                          markersize=8)
     if plot_type == 'f':
         for i, (tool, df_row) in enumerate(df_mean.iterrows()):
-            axs.errorbar(df_row[utils_labels.AVG_PRECISION_SEQ], df_row[utils_labels.AVG_RECALL_SEQ], xerr=df_row[utils_labels.AVG_PRECISION_SEQ_SEM], yerr=df_row[utils_labels.AVG_RECALL_SEQ_SEM],
+            axs.errorbar(df_row['precision_avg_seq'], df_row['recall_avg_seq_cami1'],
+                         xerr=df_row['precision_avg_seq_sem'] if not np.isnan(df_row['precision_avg_seq_sem']) else 0,
+                         yerr=df_row['recall_avg_seq_sem_cami1'] if not np.isnan(df_row['recall_avg_seq_sem_cami1']) else 0,
                          fmt='o',
                          ecolor=colors_list[i],
                          mec=colors_list[i],
                          mfc=colors_list[i],
                          capsize=3,
                          markersize=8)
     if plot_type == 'w':
         for i, (tool, df_row) in enumerate(df_mean.iterrows()):
-            axs.plot(df_row[utils_labels.PRECISION_PER_BP], df_row[utils_labels.RECALL_PER_BP], marker='o', color=colors_list[i], markersize=10)
+            axs.plot(df_row['precision_weighted_bp'], df_row['recall_weighted_bp'], marker='o', color=colors_list[i], markersize=10)
     if plot_type == 'x':
         for i, (tool, df_row) in enumerate(df_mean.iterrows()):
-            axs.plot(df_row[utils_labels.PRECISION_PER_SEQ], df_row[utils_labels.RECALL_PER_SEQ], marker='o', color=colors_list[i], markersize=10)
+            axs.plot(df_row['precision_weighted_seq'], df_row['recall_weighted_seq'], marker='o', color=colors_list[i], markersize=10)
     elif plot_type == 'p':
         for i, (tool, df_row) in enumerate(df_mean.iterrows()):
-            axs.plot(df_row[utils_labels.ARI_BY_BP], df_row[utils_labels.PERCENTAGE_ASSIGNED_BPS], marker='o', color=colors_list[i], markersize=10)
+            axs.plot(df_row['adjusted_rand_index_bp'], df_row['percentage_of_assigned_bps'], marker='o', color=colors_list[i], markersize=10)
 
     # turn on grid
     # axs.minorticks_on()
     axs.grid(which='major', linestyle=':', linewidth='0.5')
     # axs.grid(which='minor', linestyle=':', linewidth='0.5')
 
     # transform plot_labels to percentages
     if plot_type != 'p':
         vals = axs.get_xticks()
+        axs.xaxis.set_major_locator(ticker.FixedLocator(vals))
         axs.set_xticklabels(['{:3.0f}'.format(x * 100) for x in vals], fontsize=11)
     else:
         axs.tick_params(axis='x', labelsize=12)
     vals = axs.get_yticks()
+    axs.yaxis.set_major_locator(ticker.FixedLocator(vals))
     axs.set_yticklabels(['{:3.0f}'.format(x * 100) for x in vals], fontsize=11)
 
     if rank:
         file_name = rank + '_' + file_name
         plt.title(rank)
         ylabel = ylabel.replace('genome', 'taxon')
 
@@ -454,17 +464,18 @@
         for rank_to_metric_error, y_values, color in zip(dict_error_list, y_values_list, colors_list):
             sem = list(rank_to_metric_error.values())
             plt.fill_between(x_values, np.subtract(y_values, sem).tolist(), np.add(y_values, sem).tolist(), color=color, alpha=0.5)
 
         plt.xticks(x_values, load_ncbi_taxinfo.RANKS, rotation='vertical')
 
         vals = axs.get_yticks()
+        axs.yaxis.set_major_locator(ticker.FixedLocator(vals))
         axs.set_yticklabels(['{:3.0f}%'.format(x * 100) for x in vals])
 
-        lgd = plt.legend(metrics_list, loc=1, borderaxespad=0., handlelength=2, frameon=False)
+        lgd = plt.legend([utils_labels.LABELS[x] for x in metrics_list], loc=1, borderaxespad=0., handlelength=2, frameon=False)
 
         plt.tight_layout()
         fig.savefig(os.path.join(output_dir, 'taxonomic', tool, file_name + '.png'), dpi=100, format='png', bbox_extra_artists=(lgd,), bbox_inches='tight')
         fig.savefig(os.path.join(output_dir, 'taxonomic', tool, file_name + '.pdf'), dpi=100, format='pdf', bbox_extra_artists=(lgd,), bbox_inches='tight')
         plt.close(fig)
 
 
@@ -499,14 +510,15 @@
     min_value = pd_bins_copy['newcolumn'].min()
     axs.set_ylim(min_value if min_value < 1.0 else .9, 1.0)
     axs.set_xlim(1, None)
     axs.grid(which='major', linestyle='-', linewidth='0.5', color='lightgrey')
 
     # transform plot_labels to percentages
     vals = axs.get_yticks()
+    axs.yaxis.set_major_locator(ticker.FixedLocator(vals))
     axs.set_yticklabels(['{:3.0f}'.format(y * 100) for y in vals])
 
     plt.xlabel(xlabel, fontsize=14)
     plt.ylabel(ylabel + ' [%]', fontsize=14)
 
     lgd = plt.legend(tools, bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0., handlelength=1, frameon=False, fontsize=12)
 
@@ -523,15 +535,15 @@
     pd_bins_copy = pd_bins[[utils_labels.TOOL, 'precision_bp', 'recall_bp']].copy().dropna(subset=['precision_bp'])
     for tool in tools:
         pd_tool_bins = pd_bins_copy[pd_bins_copy[utils_labels.TOOL] == tool]
         x50 = pd_tool_bins[(pd_tool_bins['recall_bp'] > .5) & (pd_tool_bins['precision_bp'] > .9)].shape[0]
         x70 = pd_tool_bins[(pd_tool_bins['recall_bp'] > .7) & (pd_tool_bins['precision_bp'] > .9)].shape[0]
         x90 = pd_tool_bins[(pd_tool_bins['recall_bp'] > .9) & (pd_tool_bins['precision_bp'] > .9)].shape[0]
         pd_tool_counts = pd.DataFrame([[x90, x70, x50]], columns=['>90%', '>70%', '>50%'], index=[tool])
-        pd_counts = pd_counts.append(pd_tool_counts)
+        pd_counts = pd.concat([pd_counts, pd_tool_counts])
     return pd_counts
 
 
 def get_number_of_hq_bins_by_score(tools, pd_bins):
     pd_counts = pd.DataFrame()
     pd_bins_copy = pd_bins[[utils_labels.TOOL, 'precision_bp', 'recall_bp']].copy().dropna(subset=['precision_bp'])
     pd_bins_copy['newcolumn'] = pd_bins_copy['recall_bp'] + 5 * (pd_bins_copy['precision_bp'] - 1)
@@ -539,15 +551,15 @@
         pd_tool_bins = pd_bins_copy[pd_bins_copy[utils_labels.TOOL] == tool]
         x50 = pd_tool_bins[pd_tool_bins['newcolumn'] > .5].shape[0]
         x70 = pd_tool_bins[pd_tool_bins['newcolumn'] > .7].shape[0]
         x90 = pd_tool_bins[pd_tool_bins['newcolumn'] > .9].shape[0]
         x50 -= x70
         x70 -= x90
         pd_tool_counts = pd.DataFrame([[x90, x70, x50]], columns=['>90', '>70', '>50'], index=[tool])
-        pd_counts = pd_counts.append(pd_tool_counts)
+        pd_counts = pd.concat([pd_counts, pd_tool_counts])
     return pd_counts
 
 
 def plot_counts(pd_bins, tools, output_dir, output_file, get_bin_counts_function):
     pd_counts = get_bin_counts_function(tools, pd_bins)
     fig, axs = plt.subplots(figsize=(11, 5))
     if output_file == 'bin_counts':
```

### Comparing `cami-amber-2.0.3/src/precision_recall_per_bin.py` & `cami-amber-2.0.4/src/precision_recall_per_bin.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,24 +31,24 @@
 
     genomes_sorted_list = precision_df[['genome_id', 'tp_length']].sort_values(by='tp_length', ascending=False).groupby(['genome_id'], sort=False).first().index.tolist()
     unmapped_genomes = set(genomes_df['genome_id']) - set(genomes_sorted_list)
     unmapped_genomes = [genome_id for genome_id in all_genomes_sorted_by_size if genome_id in unmapped_genomes]
     genomes_sorted_list += unmapped_genomes
 
     unbinned_genomes_df = genomes_df[~genomes_df['genome_id'].isin(confusion_df.reset_index()['genome_id'])]
-    heatmap_df = confusion_df.reset_index().append(unbinned_genomes_df, sort=True).fillna({'genome_length': 0, 'genome_seq_counts': 0})
+    heatmap_df = pd.concat([confusion_df.reset_index(), unbinned_genomes_df], sort=True).fillna({'genome_length': 0, 'genome_seq_counts': 0})
     heatmap_df = heatmap_df.pivot(index='BINID', columns='genome_id', values='genome_length')
     heatmap_df = heatmap_df.merge(precision_df['tp_length'], on='BINID', sort=False).sort_values(by='tp_length', axis=0, ascending=False)
 
     gs_df = gs_df.set_index(['SEQUENCEID', 'genome_id'])
     query_df = query.df.set_index(['SEQUENCEID', 'genome_id'])
     difference_df = gs_df.index.difference(query_df.index)
     unassigned_sequences = gs_df.loc[difference_df].groupby('genome_id', sort=False).agg({'seq_length': 'sum'})
 
-    heatmap_df = heatmap_df.append(unassigned_sequences.T, sort=True)
+    heatmap_df = pd.concat([heatmap_df, unassigned_sequences.T], sort=True)
     heatmap_df = heatmap_df[genomes_sorted_list].fillna(0)
 
     return heatmap_df
 
 
 def transform_confusion_matrix(query):
     gold_standard = query.gold_standard
@@ -62,15 +62,15 @@
     gs_sequence_ids = set(gold_standard.sequence_id_to_bin_id.keys())
     genome_id_to_unassigned_bps = collections.Counter()
     for unassigned_seq_id in gs_sequence_ids - query_sequence_ids:
         genome_id = gold_standard.sequence_id_to_bin_id[unassigned_seq_id]
         genome_id_to_unassigned_bps[genome_id] += gold_standard.sequence_id_to_length[unassigned_seq_id]
 
     df_unassigned = pd.DataFrame.from_dict(genome_id_to_unassigned_bps, orient='index').rename(columns={0: 'unassigned'}).T
-    table = df_confusion.append(df_unassigned, sort=False)
+    table = pd.concat([df_confusion, df_unassigned], sort=False)
     table.fillna(0, inplace=True)
     # use log scale
     # table = table.applymap(np.log).fillna(0)
 
     bin_id_to_mapped_genome = {}
     for bin in query.bins:
         bin_id_to_mapped_genome[bin.id] = bin.most_abundant_genome
@@ -79,19 +79,19 @@
     bin_id_to_mapped_genome_by_length = collections.OrderedDict(sorted(bin_id_to_mapped_genome.items(), key=lambda t: bin_id_to_genome_id_to_length[t[0]][t[1]], reverse=True))
 
     # sort genomes
     genome_order = []
     for bin_id in bin_id_to_mapped_genome_by_length:
         mapped_genome = bin_id_to_mapped_genome_by_length[bin_id]
         if mapped_genome not in genome_order:
-            genome_order.append(mapped_genome)
+            genome_order = pd.concat([genome_order, mapped_genome])
     genome_order += list(set(table.columns.values.tolist()) - set(genome_order))
     for genome_id in genome_id_to_unassigned_bps.keys():
         if genome_id not in genome_order:
-            genome_order.append(genome_id)
+            genome_order = pd.concat([genome_order, genome_id])
 
     table = table.loc[list(bin_id_to_mapped_genome_by_length.keys()) + ['unassigned'], genome_order]
 
     for genome_id in gold_standard.get_bin_ids():
         if genome_id not in table.columns.values.tolist():
             table[genome_id] = 0
```

### Comparing `cami-amber-2.0.3/src/unifrac_distance.py` & `cami-amber-2.0.4/src/unifrac_distance.py`

 * *Files identical despite different names*

### Comparing `cami-amber-2.0.3/src/utils/EMDUnifrac.py` & `cami-amber-2.0.4/src/utils/EMDUnifrac.py`

 * *Files identical despite different names*

### Comparing `cami-amber-2.0.3/src/utils/ProfilingTools.py` & `cami-amber-2.0.4/src/utils/ProfilingTools.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 _data[tax_id]["ancestor"] = "-1"  # no ancestor, it's a root
                 _data[tax_id]["branch_length"] = 1
                 ancestor = "-1"
             else:
                 ancestor = tax_path[-2]
                 _data[tax_id]["branch_length"] = 1
                 i = -3
-                while ancestor is "" or ancestor == tax_id:  # if it's a blank or repeated, go up until finding ancestor
+                while ancestor == "" or ancestor == tax_id:  # if it's a blank or repeated, go up until finding ancestor
                     ancestor = tax_path[i]
                     _data[tax_id]["branch_length"] += 1
                     i -= 1
                     if i + len(tax_path) < 0:  # no ancestor available, manually set to -1 (the root)
                         ancestor = "-1"
                 _data[tax_id]["ancestor"] = ancestor
 
@@ -123,15 +123,15 @@
             for index in bad_indicies:
                 tax_path[index] = ''  # remove the bad tax_ids
             # fix the branch lengths and find the ancestors
             if len(tax_path) >= 2:
                 ancestor = tax_path[-2]
                 _data[key]["branch_length"] = 1
                 i = -3
-                while ancestor is "" or ancestor == key:  # if it's a blank or repeated, go up until finding ancestor
+                while ancestor == "" or ancestor == key:  # if it's a blank or repeated, go up until finding ancestor
                     if i < -len(tax_path):  # Path is all the way full with bad tax_ids, connect to root
                         _data[key]["branch_length"] += 1
                         ancestor = "-1"
                         _data["-1"]["descendants"].append(key)  # note this is now a descendant of the root
                         break
                     else:
                         ancestor = tax_path[i]
```

### Comparing `cami-amber-2.0.3/src/utils/add_length_column.py` & `cami-amber-2.0.4/src/utils/add_length_column.py`

 * *Files identical despite different names*

### Comparing `cami-amber-2.0.3/src/utils/argparse_parents.py` & `cami-amber-2.0.4/src/utils/argparse_parents.py`

 * *Files identical despite different names*

### Comparing `cami-amber-2.0.3/src/utils/convert_fasta_bins_to_biobox_format.py` & `cami-amber-2.0.4/src/utils/convert_fasta_bins_to_biobox_format.py`

 * *Files identical despite different names*

### Comparing `cami-amber-2.0.3/src/utils/load_data.py` & `cami-amber-2.0.4/src/utils/load_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,16 @@
 
 
 def load_ncbi_info(ncbi_dir):
     if ncbi_dir:
         logging.getLogger('amber').info('Loading NCBI taxonomy')
         try:
             binning_classes.TaxonomicQuery.taxonomy_df = pd.read_feather(os.path.join(ncbi_dir, 'nodes.amber.ft')).set_index('TAXID')
-        except:
+        except BaseException as e:
+            traceback.print_exc()
             logging.getLogger('amber').info('Preprocessed NCBI taxonomy file not found. Creating file {}'.format(os.path.join(ncbi_dir, 'nodes.amber.ft')))
             binning_classes.TaxonomicQuery.taxonomy_df = load_ncbi_taxinfo.preprocess_ncbi_tax(ncbi_dir)
 
 
 def read_metadata(file_path_query):
     header = {}
     index_to_column_name = {}
```

### Comparing `cami-amber-2.0.3/src/utils/load_ncbi_taxinfo.py` & `cami-amber-2.0.4/src/utils/load_ncbi_taxinfo.py`

 * *Files identical despite different names*

