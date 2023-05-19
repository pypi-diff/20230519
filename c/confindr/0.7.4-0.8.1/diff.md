# Comparing `tmp/confindr-0.7.4.tar.gz` & `tmp/confindr-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/confindr-0.7.4.tar", last modified: Thu Aug 20 17:13:50 2020, max compression
+gzip compressed data, was "confindr-0.8.1.tar", last modified: Fri May 19 17:53:56 2023, max compression
```

## Comparing `confindr-0.7.4.tar` & `confindr-0.8.1.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2020-08-20 17:13:50.000000 confindr-0.7.4/
--rwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)      760 2020-08-20 16:46:07.000000 confindr-0.7.4/setup.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      239 2020-08-20 17:13:50.000000 confindr-0.7.4/PKG-INFO
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2020-08-20 17:13:50.000000 confindr-0.7.4/confindr.egg-info/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      431 2020-08-20 17:13:50.000000 confindr-0.7.4/confindr.egg-info/SOURCES.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       13 2020-08-20 17:13:50.000000 confindr-0.7.4/confindr.egg-info/top_level.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      239 2020-08-20 17:13:50.000000 confindr-0.7.4/confindr.egg-info/PKG-INFO
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       35 2020-08-20 17:13:50.000000 confindr-0.7.4/confindr.egg-info/requires.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        1 2020-08-20 17:13:50.000000 confindr-0.7.4/confindr.egg-info/dependency_links.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      221 2020-08-20 17:13:50.000000 confindr-0.7.4/confindr.egg-info/entry_points.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3209 2020-07-15 13:15:32.000000 confindr-0.7.4/README.md
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2020-08-20 17:13:50.000000 confindr-0.7.4/confindr_src/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    13016 2020-07-15 13:15:32.000000 confindr-0.7.4/confindr_src/create_genus_specific_db.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2020-07-15 13:15:32.000000 confindr-0.7.4/confindr_src/__init__.py
--rwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)    67456 2020-08-20 16:46:07.000000 confindr-0.7.4/confindr_src/confindr.py
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2020-08-20 17:13:50.000000 confindr-0.7.4/confindr_src/wrappers/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    25103 2020-07-15 13:15:32.000000 confindr-0.7.4/confindr_src/wrappers/bbtools.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     5348 2020-07-15 13:15:32.000000 confindr-0.7.4/confindr_src/wrappers/mash.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2020-07-15 13:15:32.000000 confindr-0.7.4/confindr_src/wrappers/__init__.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    13568 2020-07-15 13:15:32.000000 confindr-0.7.4/confindr_src/database_setup.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       38 2020-08-20 17:13:50.000000 confindr-0.7.4/setup.cfg
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-19 17:53:56.547115 confindr-0.8.1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1088 2023-05-19 17:52:34.000000 confindr-0.8.1/LICENSE
+-rw-rw-r--   0 liam      (1000) liam      (1000)      195 2023-05-19 17:53:56.547115 confindr-0.8.1/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4178 2023-05-19 17:52:34.000000 confindr-0.8.1/README.md
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-19 17:53:56.547115 confindr-0.8.1/confindr.egg-info/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      195 2023-05-19 17:53:56.000000 confindr-0.8.1/confindr.egg-info/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)      486 2023-05-19 17:53:56.000000 confindr-0.8.1/confindr.egg-info/SOURCES.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-05-19 17:53:56.000000 confindr-0.8.1/confindr.egg-info/dependency_links.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      220 2023-05-19 17:53:56.000000 confindr-0.8.1/confindr.egg-info/entry_points.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       35 2023-05-19 17:53:56.000000 confindr-0.8.1/confindr.egg-info/requires.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       13 2023-05-19 17:53:56.000000 confindr-0.8.1/confindr.egg-info/top_level.txt
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-19 17:53:56.547115 confindr-0.8.1/confindr_src/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-05-19 17:52:34.000000 confindr-0.8.1/confindr_src/__init__.py
+-rwxrwxr-x   0 liam      (1000) liam      (1000)    13601 2023-05-19 17:52:34.000000 confindr-0.8.1/confindr_src/confindr.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13016 2023-05-19 17:52:34.000000 confindr-0.8.1/confindr_src/create_genus_specific_db.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15715 2023-05-19 17:52:34.000000 confindr-0.8.1/confindr_src/database_setup.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    92070 2023-05-19 17:52:34.000000 confindr-0.8.1/confindr_src/methods.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-19 17:53:56.547115 confindr-0.8.1/confindr_src/wrappers/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-05-19 17:52:34.000000 confindr-0.8.1/confindr_src/wrappers/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    25166 2023-05-19 17:52:34.000000 confindr-0.8.1/confindr_src/wrappers/bbtools.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5348 2023-05-19 17:52:34.000000 confindr-0.8.1/confindr_src/wrappers/mash.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)       38 2023-05-19 17:53:56.547115 confindr-0.8.1/setup.cfg
+-rwxrwxr-x   0 liam      (1000) liam      (1000)      767 2023-05-19 17:52:34.000000 confindr-0.8.1/setup.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-05-19 17:53:56.547115 confindr-0.8.1/tests/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8409 2023-05-19 17:52:34.000000 confindr-0.8.1/tests/test_confindr.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `confindr-0.7.4/setup.py` & `confindr-0.8.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name="confindr",
-    version="0.7.4",
+    version="0.8.1",
     packages=find_packages(),
     entry_points={
        'console_scripts': [
             'confindr.py = confindr_src.confindr:main',
             'confindr = confindr_src.confindr:main',
             'confindr_database_setup = confindr_src.database_setup:main',
             'confindr_create_db = confindr_src.create_genus_specific_db:main'
        ],
     },
     author="Adam Koziol",
-    author_email="adam.koziol@canada.ca",
+    author_email="adam.koziol@inspection.gc.ca",
     url="https://github.com/OLC-Bioinformatics/ConFindr",
     install_requires=['biopython',
                       'pysam',
                       'pytest',
                       'numpy',
                       'rauth']
 )
```

### Comparing `confindr-0.7.4/README.md` & `confindr-0.8.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,62 @@
-[![Build status](https://travis-ci.org/OLC-Bioinformatics/ConFindr.svg?master)](https://travis-ci.org/OLC-Bioinformatics)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/OLC-Bioinformatics/ConFindr/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/OLC-Bioinformatics/ConFindr/tree/main)
 [![PyPI version](https://badge.fury.io/py/confindr.svg)](https://badge.fury.io/py/confindr)
 [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat-square)](http://bioconda.github.io/recipes/confindr/README.html)
 
+
 # ConFindr
 
 This program is designed to find bacterial intra-species contamination in raw Illumina data. It does this
  by looking for multiple alleles of core, single copy genes.
 
-For complete instructions on installation and usage, please visit [the ConFindr github pages site](https://olc-bioinformatics.github.io/ConFindr/).
+For **complete instructions on installation and usage**, please visit [the ConFindr GitHub Pages site](https://olc-bioinformatics.github.io/ConFindr/).
+
+## Important Note
+
+ConFindr has only been validated using rMLST databases. **Please use them if possible** (`--rmlst`). Complete installation instructions can be found [here](https://olc-bioinformatics.github.io/ConFindr/install/#downloading-confindr-databases).
 
 ## Quickstart
 
-To install ConFindr, use conda (see [here](https://bioconda.github.io/) for instructions on getting bioconda set up): 
+### Installing ConFindr
+
+1. Follow the instructions [here](https://bioconda.github.io/) to add the Bioconda channel to your list of conda channels, if it hasn't already been added.
+
+2. Install ConFindr into a new conda environment named 'confindr':
+
+`conda create -n confindr -c bioconda confindr=0.8.1`
+
+3. Activate the new conda environment:
+
+`conda activate confindr`
 
-`conda install -c bioconda confindr`
+### Downloading and setting up the rMLST databases
 
-To get an example dataset, use this command, which will create a folder called `example-data` in your current working directory: 
+Instructions for downloading and setting up the rMLST databases can be found [here](https://olc-bioinformatics.github.io/ConFindr/install/#downloading-confindr-databases).
+
+### Testing ConFindr
+
+1. To obtain an example dataset, run the following command, which will create a folder named `example-data` in your current working directory: 
 
 `wget https://ndownloader.figshare.com/files/9972709 && tar xf 9972709 && rm 9972709`
 
-As of version `0.7.0` ConFindr can run automatically on _Escherichia_, _Salmonella_, and _Listeria_ with no further 
-work on your part - just run:
+2. As of version `0.7.0` ConFindr can be run automatically on _Escherichia_, _Salmonella_, and _Listeria_ with no further 
+work on your part, using core-gene databases (*experimental*). Simply run:
+
+`confindr -i example-data -o example-out`
+
+3. To use the *recommended* rMLST database (after installation):
 
-`confindr.py -i example-data -o example-out`
+`confindr -i example-data -o example-out --rmlst`
 
-Once ConFindr finishes running, take a look at the `confindr_report.csv` file found in `example-out` - it shows that multiple
+Once ConFindr finishes running, take a look at the `confindr_report.csv` file found in `example-out`—it shows that multiple
 alleles were found for many sites within the genes that ConFindr examines, meaning that this sample is quite contaminated!
 
-If you want to run ConFindr on genera other than the 3 listed above, you'll need to get access to and download rMLST databases. 
-[You can find instructions on how to do that here](https://olc-bioinformatics.github.io/ConFindr/install/#downloading-confindr-databases).
+If you want to run ConFindr on genera other than the 3 listed above, you'll need to get access to and download the rMLST databases by following the instructions [here](https://olc-bioinformatics.github.io/ConFindr/install/#downloading-confindr-databases).
 
-### Running ConFindr in a Python Script
+## Running ConFindr in a Python Script
 
 If you want to run ConFindr from within a script instead of running from the command line, here's how:
 
 ```python
 from confindr_src import confindr
 
 # Find read files.
@@ -46,22 +68,19 @@
                                 forward_id='_R1', # change if yours is different
                                 threads=4, 
                                 output_folder='path/to/output',
                                 databases_folder='path/to/databases')
                                 
 ```
 
-
 ## Reporting Issues
 
 If you have any problems installing or running ConFindr, or have feature request,
 please open an issue here on GitHub.
 
-
 ## Citing ConFindr
 
-ConFindr has been published in PeerJ - if you use it in your work, please cite the following:
+ConFindr has been published in PeerJ—if you use it in your work, please cite the following:
 
 ```
 Low AJ, Koziol AG, Manninger PA, Blais B, Carrillo CD. 2019. ConFindr: rapid detection of intraspecies and cross-species contamination in bacterial whole-genome sequence data. PeerJ 7:e6995 https://doi.org/10.7717/peerj.6995
-```
-
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `confindr-0.7.4/confindr_src/create_genus_specific_db.py` & `confindr-0.8.1/confindr_src/create_genus_specific_db.py`

 * *Files identical despite different names*

### Comparing `confindr-0.7.4/confindr_src/confindr.py` & `confindr-0.8.1/confindr_src/methods.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,83 @@
 #!/usr/bin/env python
+from confindr_src.wrappers import bbtools, mash
+from Bio import SeqIO
 from pysam.utils import SamtoolsError
+from itertools import chain
+from statistics import mean
 import multiprocessing
+import urllib.request
 import pkg_resources
 import numpy as np
 import subprocess
-import traceback
-import argparse
 import logging
 import shutil
+import tarfile
+import pysam
 import glob
+import gzip
+import math
 import csv
 import os
-import pysam
-from Bio import SeqIO
-from confindr_src.database_setup import download_cgmlst_derived_data, download_mash_sketch
-from confindr_src.wrappers import mash
-from confindr_src.wrappers import bbtools
+
+
+def download_mash_sketch(output_folder):
+    logging.info('Downloading mash refseq sketch...')
+    urllib.request.urlretrieve('https://github.com/OLC-Bioinformatics/ConFindr/raw/master/refseq_sketch/refseq.msh',
+                               os.path.join(output_folder, 'refseq.msh'))
+
+
+def download_cgmlst_derived_data(output_folder):
+    logging.info('Downloading cgMLST-derived data for Escherichia, Salmonella, and Listeria...')
+    urllib.request.urlretrieve('https://ndownloader.figshare.com/files/14771267',
+                               os.path.join(output_folder, 'confindr_db.tar.gz'))
+    confindr_tar = os.path.join(output_folder, 'confindr_db.tar.gz')
+    tar = tarfile.open(confindr_tar)
+    tar.extractall(path=output_folder)
+    tar.close()
+    os.remove(confindr_tar)
+    index(output_folder=output_folder,
+          genera=['Escherichia', 'Listeria', 'Salmonella'],
+          cgderived=True)
+
+
+def index(output_folder, genera, cgderived=False):
+    """
+
+    :param output_folder:
+    :param genera:
+    :param cgderived:
+    :return:
+    """
+    for predominant_genus in genera:
+        if cgderived:
+            sample_database = os.path.join(output_folder, '{pg}_db_cgderived.fasta'.format(pg=predominant_genus))
+        else:
+            sample_database = os.path.join(output_folder, '{pg}_db.fasta'.format(pg=predominant_genus))
+
+        if not os.path.isfile(sample_database):
+
+            if os.path.isfile(os.path.join(output_folder, 'gene_allele.txt')) and \
+                    os.path.isfile(os.path.join(output_folder, 'rMLST_combined.fasta')):
+                logging.info('Setting up rMLST genus-specific database for genus {pg}...'
+                             .format(pg=predominant_genus))
+                allele_list = find_genus_specific_allele_list(os.path.join(output_folder, 'gene_allele.txt'),
+                                                              predominant_genus)
+                # Create the allele-specific database
+                setup_allelespecific_database(fasta_file=sample_database,
+                                              database_folder=output_folder,
+                                              allele_list=allele_list)
+        # Perform the necessary samtools and KMA indexing
+        index_databases(sample_database=sample_database)
 
 
 def run_cmd(cmd):
     """
     Runs a command using subprocess, and returns both the stdout and stderr from that command
-    If exit code from command is non-zero, raises subproess.CalledProcessError
+    If exit code from command is non-zero, raises subprocess.CalledProcessError
     :param cmd: command to run as a string, as it would be called on the command line
     :return: out, err: Strings that are the stdout and stderr from the command called.
     """
     p = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     out, err = p.communicate()
     out = out.decode('utf-8')
     err = err.decode('utf-8')
@@ -102,15 +154,15 @@
         elif forward_id in name and not os.path.isfile(name.replace(forward_id, reverse_id)):
             read_list.append([name])
         elif reverse_id in name and not os.path.isfile(name.replace(reverse_id, forward_id)):
             read_list.append([name])
     return read_list
 
 
-def find_genusspecific_allele_list(profiles_file, target_genus):
+def find_genus_specific_allele_list(profiles_file, target_genus):
     """
     A new way of making our specific databases: Make our profiles file have lists of every gene/allele present for
     each genus instead of just excluding a few genes for each. This way, should have much smaller databases
     while managing to make ConFindr a decent bit faster (maybe)
     :param profiles_file: Path to profiles file.
     :param target_genus: Genus you want to make a custom database for (STR)
     :return: List of gene/allele combinations that should be part of species-specific database.
@@ -128,81 +180,71 @@
 
 def setup_allelespecific_database(fasta_file, database_folder, allele_list):
     """
     Since some genera have some rMLST genes missing, or two copies of some genes, genus-specific databases are needed.
     This will take only the alleles known to be part of each genus and write them to a genus-specific file.
     :param database_folder: Path to folder where rMLST_combined is stored.
     :param fasta_file: Path to fasta file to write allele-specific database to.
-    :param allele_list: allele list generated by find_genusspecific_allele_list
+    :param allele_list: allele list generated by find_genus_specific_allele_list
     """
-    index = SeqIO.index(os.path.join(database_folder, 'rMLST_combined.fasta'), 'fasta')
+    rmlst_index = SeqIO.index(os.path.join(database_folder, 'rMLST_combined.fasta'), 'fasta')
     seqs = list()
     for s in allele_list:
         try:
-            seqs.append(index[s])
+            seqs.append(rmlst_index[s])
         except KeyError:
             logging.warning('Tried to add {} to allele-specific database, but could not find it.'.format(s))
-    SeqIO.write(seqs, fasta_file, 'fasta')
-
-
-def extract_rmlst_genes(pair, database, forward_out, reverse_out, threads=12, logfile=None):
-    """
-    Given a pair of reads and an rMLST database, will extract reads that contain sequence from the database.
-    :param pair: List containing path to forward reads at index 0 and path to reverse reads at index 1.
-    :param database: Path to rMLST database, in FASTA format.
-    :param forward_out: Filepath to write forward reads to (STR)
-    :param reverse_out: Filepath to write reverse reads to (STR)
-    :param threads: Number of threads to use (INT)
-    :param logfile: Logfile to write command/stdout/stderr to. If None, nothing will be written.
-    """
-    out, err, cmd = bbtools.bbduk_bait(database, pair[0], forward_out, reverse_in=pair[1],
-                                       reverse_out=reverse_out, threads=str(threads), returncmd=True)
-    if logfile:
-        write_to_logfile(logfile, out, err, cmd)
+    try:
+        SeqIO.write(seqs, fasta_file, 'fasta')
+    except FileNotFoundError:
+        pass
 
 
-def find_cross_contamination(databases, reads, tmpdir='tmp', log='log.txt', threads=1, min_matching_hashes=40):
+def find_cross_contamination(databases, reads, sample_name, tmpdir='tmp', log='log.txt', threads=1,
+                             min_matching_hashes=40):
     """
     Uses mash to find out whether or not a sample has more than one genus present, indicating cross-contamination.
     :param databases: A databases folder, which must contain refseq.msh, a mash sketch that has one representative
     per genus from refseq.
     :param reads: Relative path(s) to either unpaired (type STR) or paired (type LIST) FASTQ reads
+    :param sample_name:
     :param tmpdir: Temporary directory to store mash result files in.
     :param log: Logfile to write to.
     :param threads: Number of threads to run mash with.
     :param min_matching_hashes: Minimum number of matching hashes in a MASH screen in order for a genus to be
     considered present in a sample. Default is 40
     :return: cross_contam: a bool that is True if more than one genus is found, and False otherwise.
     :return: genera_present: A string. If only one genus is found, string is NA. If more than one genus is found,
     the string is a list of genera present, separated by colons (i.e. for Escherichia and Salmonella found, string would
     be 'Escherichia:Salmonella'
     """
     genera_present = list()
-    if type(reads) is str:
-        out, err, cmd = mash.screen('{database}/refseq.msh'.format(database=databases), reads,
-                                    threads=threads,
-                                    w='',
-                                    # i='0.95',
-                                    i='0.85',
-                                    output_file=os.path.join(tmpdir, 'screen.tab'),
-                                    returncmd=True)
-    else:
-        out, err, cmd = mash.screen('{database}/refseq.msh'.format(database=databases), reads[0],
-                                    reads[1],
-                                    threads=threads,
-                                    w='',
-                                    # i='0.95',
-                                    i='0.85',
-                                    output_file=os.path.join(tmpdir, 'screen.tab'),
-                                    returncmd=True)
-    write_to_logfile(log, out, err, cmd)
-    screen_output = mash.read_mash_screen(os.path.join(tmpdir, 'screen.tab'))
+    # Only run the MASH analyses if the screen.tab output file does not already exist
+    screen_file = os.path.join(tmpdir, '{sn}_screen.tab'.format(sn=sample_name))
+    if not os.path.isfile(screen_file):
+        if type(reads) is str:
+            out, err, cmd = mash.screen('{database}/refseq.msh'.format(database=databases), reads,
+                                        threads=threads,
+                                        w='',
+                                        i='0.85',
+                                        output_file=screen_file,
+                                        returncmd=True)
+        else:
+            out, err, cmd = mash.screen('{database}/refseq.msh'.format(database=databases), reads[0],
+                                        reads[1],
+                                        threads=threads,
+                                        w='',
+                                        i='0.85',
+                                        output_file=screen_file,
+                                        returncmd=True)
+        write_to_logfile(log, out, err, cmd)
+    screen_output = mash.read_mash_screen(os.path.join(tmpdir, '{sn}_screen.tab'.format(sn=sample_name)))
     for item in screen_output:
         mash_genus = item.query_id.split('/')[-3]
-        if mash_genus == 'Shigella':
+        if 'Shigella' in mash_genus:
             mash_genus = 'Escherichia'
         matching_hashes = int(item.shared_hashes.split('/')[0])
         # Only add the genus to the genera_present list of the number of matching hashes exceeds the cutoff
         if matching_hashes >= min_matching_hashes:
             if mash_genus not in genera_present:
                 genera_present.append(mash_genus)
     if len(genera_present) == 1:
@@ -215,172 +257,649 @@
             tmpstr += mash_genus + ':'
         genera_present = tmpstr[:-1]
     return genera_present
 
 
 def number_of_bases_above_threshold(high_quality_base_count, base_count_cutoff=2, base_fraction_cutoff=None):
     """
-    Finds if a site has at least two bases of  high quality, enough that it can be considered
+    Finds if a site has at least two bases of high quality, enough that it can be considered
     fairly safe to say that base is actually there.
     :param high_quality_base_count: Dictionary of count of HQ bases at a position where key is base and values is the
     count of that base.
     :param base_count_cutoff: Number of bases needed to support multiple allele presence.
     :param base_fraction_cutoff: Fraction of bases needed to support multiple allele presence.
     :return: True if site has at least base_count_cutoff/base_fraction_cutoff bases, False otherwise
     (changeable by user)
     """
 
     # make a dict by dictionary comprehension where values are True or False for each base depending on whether the
     # count meets the threshold.
     # Method differs depending on whether absolute or fraction cutoff is specified
     if base_fraction_cutoff:
         total_hq_base_count = sum(high_quality_base_count.values())
-        bases_above_threshold = {base: float(count)/total_hq_base_count >= base_fraction_cutoff and
-                                 count >= base_count_cutoff for (base, count) in high_quality_base_count.items()}
+        bases_above_threshold = {base: float(count) / total_hq_base_count >= base_fraction_cutoff and count
+                                 >= base_count_cutoff for (base, count) in high_quality_base_count.items()}
     else:
         bases_above_threshold = {base: count >= base_count_cutoff for (base, count) in high_quality_base_count.items()}
 
     # True is equal to 1 so sum of the number of Trues in the bases_above_threshold dict is the number of bases
     # passing threshold
     return sum(bases_above_threshold.values())
 
 
-def find_if_multibase(column, quality_cutoff, base_cutoff, base_fraction_cutoff):
+def parse_bam(bamfile_name, contig_name, pysam_fasta):
     """
-    Finds if a position in a pileup has more than one base present.
+    Use pysam to load the sorted BAM-formatted file, and subsequently the gene-specific read pileup
+    :param bamfile_name: Name and path of the sorted BAM file
+    :param contig_name: Name of the current gene
+    :param pysam_fasta: pysam.FastaFile object created from the reference gene sequence
+    :return: bamfile: pysam.AlignmentFile object of the BAM-formatted file
+    :return pileup: A pysam pileup object created from the BAM file
+    """
+    # Load the sorted BAM-formatted file using pysam
+    bamfile = pysam.AlignmentFile(bamfile_name, 'rb')
+    # These parameters seem to be fairly undocumented with pysam, but I think that they should make the output
+    # that I'm getting to match up with what I'm seeing in Tablet.
+    pileup = bamfile.pileup(contig_name,
+                            stepper='samtools',
+                            ignore_orphans=False,
+                            fastafile=pysam_fasta,
+                            min_base_quality=0)
+    return bamfile, pileup
+
+
+def characterise_read(column, reference_sequence, fastq_records, quality_cutoff,
+fasta=False, nanopore=False):
+    """
+    Parses a column to characterize all the bases present. Determines the number of bases that fit certain criteria
     :param column: A pileupColumn generated by pysam
+    :param reference_sequence: String of the FASTA reference gene sequence
+    :param fastq_records: Dictionary of SeqIO records parsed from filtered FASTQ reads
     :param quality_cutoff: Desired min phred quality for a base in order to be counted towards a multi-allelic column
-    :param base_cutoff: Minimum number of bases needed to support presence of a base.
-    :param base_fraction_cutoff: Minimum fraction of bases needed to support presence of a base.
-    If specified, noth the base_cutoff and base_fraction_cutoff will have to be met
-    :return: If position has more than one base, a dictionary with counts for the bases. Otherwise, returns
-    empty dictionary
-    """
-    # Sometimes the qualities come out to ridiculously high (>70) values. Looks to be because sometimes reads
-    # are overlapping and the qualities get summed for overlapping bases. Issue opened on pysam.
-    unfiltered_base_qualities = dict()
+    If specified, both the base_cutoff and base_fraction_cutoff will have to be met
+    :param fasta: Boolean of whether the samples are in FASTQ or FASTA format
+    :param nanopore: Boolean of whether Nanopore reads were provided. Default is False.
+    :return: filtered_read_dict: Dictionary with of base types: read direction: count
+    :return: qualities: List of all phred scores in the pileup
+    """
+    # Initialise a dictionary to store the base details
+    filtered_read_dict = {
+        'congruent_SNV': dict(),
+        'congruent_ref': dict(),
+        'forward_SNV_reverse_SNV1': dict(),
+        'reverse_SNV_forward_SNV1': dict(),
+        'forward_SNV_reverse_ref': dict(),
+        'reverse_SNV_forward_ref': dict(),
+        'forward_SNV_reverse_UM_QF': dict(),
+        'forward_ref_reverse_UM_QF': dict(),
+        'forward_quality_filtered': dict(),
+        'reverse_SNV_forward_UM_QF': dict(),
+        'reverse_ref_forward_UM_QF': dict(),
+        'reverse_quality_filtered': dict()
+    }
+    # Initialise a dictionary to store the details parsed from the pileup
+    unfiltered_read_details = dict()
+    # Initialise a list to store all the phred scores for the bases passing filter in the column
+    qualities = list()
+    # Iterate through every read present in the column of the pileup
     for read in column.pileups:
-        if read.query_position is not None:  # Not entirely sure why this is sometimes None, but it causes bad stuff
-            reference_sequence = read.alignment.get_reference_sequence()
-            previous_position = read.query_position - 1 if read.query_position > 1 else 0
-            next_position = read.query_position + 1  # This causes index errors. Fix at some point soon.
-            # Another stringency check - to make sure that we're actually looking at a point mutation, check that the
-            # base before and after the one we're looking at match the reference. With Nanopore data, lots of indels and
-            # the like cause false positives, so this filters those out.
-            try:  # Need to actually handle this at some point. For now, be lazy
-                previous_reference_base = reference_sequence[previous_position]
-                next_reference_base = reference_sequence[next_position]
-                previous_base = read.alignment.query_sequence[previous_position]
-                next_base = read.alignment.query_sequence[next_position]
-                base = read.alignment.query_sequence[read.query_position]
-                quality = read.alignment.query_qualities[read.query_position]
-                if previous_reference_base == previous_base and next_reference_base == next_base:
-                    if base not in unfiltered_base_qualities:
-                        unfiltered_base_qualities[base] = [quality]
+        # Not entirely sure why this is sometimes None, but it causes bad stuff
+        if read.query_position is not None:
+            #  Initialise the read name in the dictionary as required
+            if read.alignment.qname not in unfiltered_read_details:
+                unfiltered_read_details[read.alignment.qname] = dict()
+            # Extract the sequence of the base in the read
+            query_base = read.alignment.query_sequence[read.query_position]
+            # Extract the sequence of the base in the reference gene
+            ref_base = reference_sequence[column.pos]
+            # Create a boolean of whether the query base matches the reference base (is it a SNV?)
+            match = query_base == ref_base
+            # Read names in the pileup have the direction removed - add it back for future parsing. Not an issue for
+            # FASTA files
+            if not fasta and not nanopore:
+                read_name = read.alignment.qname.split(' ')[0] + '/1' if read.alignment.is_read1 else \
+                    read.alignment.qname.split(' ')[0] + '/2'
+            else:
+                read_name = read.alignment.qname
+            # Extract the phred quality score from the FASTQ records
+            quality = fastq_records[read_name].letter_annotations["phred_quality"][read.query_position]
+            # Initialise a dictionary to store the ran
+            range_dict = dict()
+            # Determine whether there are SNVs clustered together - they will be discarded from the analysis
+            # Iterate through a range of the five positions preceding, and five subsequent
+            # positions
+            for iterator, contig_pos in enumerate(
+                    chain(range(column.pos - 5, column.pos), range(column.pos + 1, column.pos + 6))):
+                # Ensure that the contig position being examined isn't beyond the length of the gene
+                if 0 <= contig_pos < len(reference_sequence) - 1:
+                    # Calculate the read position corresponding to the current column position
+                    read_pos = list(chain(range(read.query_position - 5, read.query_position),
+                                          range(read.query_position + 1, read.query_position + 6)))[iterator]
+                    # Ensure that read position being examined isn't beyond the length of the read
+                    if 0 <= read_pos < read.alignment.query_alignment_end - 1:
+                        # Populate the dictionary with the calculated positions
+                        range_dict[contig_pos] = read_pos
+            # Initialise a boolean of whether the current base passes filters, and should be added to the dictionary
+            add_base = True
+            # Iterate through the range_dict to extract the sequence of the bases in the range for both the read and
+            # the reference sequence
+            for contig_pos, read_pos in range_dict.items():
+                try:
+                    # Extract the sequence of the base
+                    reference_base = reference_sequence[contig_pos]
+                    base = read.alignment.query_sequence[read_pos]
+                    # If any of the downstream or upstream bases do not match, set the boolean to False
+                    if not match and reference_base != base:
+                        add_base = False
+                except KeyError:
+                    pass
+            # Populate the dictionary only if there are no other SNVs within five downstream and five upstream bases
+            if add_base:
+                unfiltered_read_details[read.alignment.qname][read.alignment.is_read1] = {
+                    'mate unmapped': read.alignment.mate_is_unmapped,
+                    'paired': read.alignment.is_paired,
+                    'forward': read.alignment.is_read1,
+                    'reverse': read.alignment.is_read2,
+                    'match': match,
+                    'qbase': query_base,
+                    'rbase': ref_base,
+                    'qual': quality,
+                    'pos': column.pos,
+                    'gene': column.reference_name
+                }
+                # Add the quality of the base
+                if quality >= quality_cutoff:
+                    qualities.append(quality)
+    # Parse the unfiltered reads to characterise the bases
+    for read_base, dir_dict in unfiltered_read_details.items():
+        # Check to see if paired reads are present at this position
+        if len(dir_dict) > 1:
+            # SNV in both forward and reverse reads
+            if not dir_dict[True]['match'] and not dir_dict[False]['match']:
+                # Same SNV sequence - don't quality filter as the reads agreeing acts as a quality check
+                if dir_dict[True]['qbase'] == dir_dict[False]['qbase']:
+                    # Forward and reverse SNV - add two matches (for forward and reverse reads)
+                    if dir_dict[True]['qbase'] not in filtered_read_dict['congruent_SNV']:
+                        filtered_read_dict['congruent_SNV'][dir_dict[True]['qbase']] = 2
+                    else:
+                        filtered_read_dict['congruent_SNV'][dir_dict[True]['qbase']] += 2
+                # Different SNV sequences
+                else:
+                    # Both SNV sequences pass quality
+                    if dir_dict[True]['qual'] >= quality_cutoff and dir_dict[False]['qual'] >= quality_cutoff:
+                        # Forward SNV1
+                        if dir_dict[True]['qbase'] not in filtered_read_dict['forward_SNV_reverse_SNV1']:
+                            filtered_read_dict['forward_SNV_reverse_SNV1'][dir_dict[True]['qbase']] = 1
+                        else:
+                            filtered_read_dict['forward_SNV_reverse_SNV1'][dir_dict[True]['qbase']] += 1
+                        # Reverse SNV2
+                        if dir_dict[False]['qbase'] not in filtered_read_dict['reverse_SNV_forward_SNV1']:
+                            filtered_read_dict['reverse_SNV_forward_SNV1'][dir_dict[False]['qbase']] = 1
+                        else:
+                            filtered_read_dict['reverse_SNV_forward_SNV1'][dir_dict[False]['qbase']] += 1
+                    # Only the forward reads pass quality
+                    elif dir_dict[True]['qual'] >= quality_cutoff:
+                        # Forward SNV reverse QF
+                        if dir_dict[True]['qbase'] not in filtered_read_dict['forward_SNV_reverse_UM_QF']:
+                            filtered_read_dict['forward_SNV_reverse_UM_QF'][dir_dict[True]['qbase']] = 1
+                        else:
+                            filtered_read_dict['forward_SNV_reverse_UM_QF'][dir_dict[True]['qbase']] += 1
+                        # Reverse QF
+                        if dir_dict[False]['qbase'] not in filtered_read_dict['reverse_quality_filtered']:
+                            filtered_read_dict['reverse_quality_filtered'][dir_dict[False]['qbase']] = 1
+                        else:
+                            filtered_read_dict['reverse_quality_filtered'][dir_dict[False]['qbase']] += 1
+                    # Only the reverse reads pass quality
+                    elif dir_dict[False]['qual'] >= quality_cutoff:
+                        # Reverse SNV forward QF
+                        if dir_dict[False]['qbase'] not in filtered_read_dict['reverse_SNV_forward_UM_QF']:
+                            filtered_read_dict['reverse_SNV_forward_UM_QF'][dir_dict[False]['qbase']] = 1
+                        else:
+                            filtered_read_dict['reverse_SNV_forward_UM_QF'][dir_dict[False]['qbase']] += 1
+                        # Forward QF
+                        if dir_dict[True]['qbase'] not in filtered_read_dict['forward_quality_filtered']:
+                            filtered_read_dict['forward_quality_filtered'][dir_dict[True]['qbase']] = 1
+                        else:
+                            filtered_read_dict['forward_quality_filtered'][dir_dict[True]['qbase']] += 1
+                    # Neither forward nor reverse reads pass quality
+                    else:
+                        # Forward QF
+                        if dir_dict[True]['qbase'] not in filtered_read_dict['forward_quality_filtered']:
+                            filtered_read_dict['forward_quality_filtered'][dir_dict[True]['qbase']] = 1
+                        else:
+                            filtered_read_dict['forward_quality_filtered'][dir_dict[True]['qbase']] += 1
+                        # Reverse QF
+                        if dir_dict[False]['qbase'] not in filtered_read_dict['reverse_quality_filtered']:
+                            filtered_read_dict['reverse_quality_filtered'][dir_dict[False]['qbase']] = 1
+                        else:
+                            filtered_read_dict['reverse_quality_filtered'][dir_dict[False]['qbase']] += 1
+            # SNV in forward read only
+            elif not dir_dict[True]['match'] and dir_dict[False]['match']:
+                # Since only the forward read supports the SNV, quality filter
+                if dir_dict[True]['qual'] >= quality_cutoff:
+                    if dir_dict[True]['qbase'] not in filtered_read_dict['forward_SNV_reverse_ref']:
+                        filtered_read_dict['forward_SNV_reverse_ref'][dir_dict[True]['qbase']] = 1
+                    else:
+                        filtered_read_dict['forward_SNV_reverse_ref'][dir_dict[True]['qbase']] += 1
+                    # Since the reverse base matches the reference, don't quality filter
+                    if dir_dict[False]['qbase'] not in filtered_read_dict['forward_SNV_reverse_ref']:
+                        filtered_read_dict['forward_SNV_reverse_ref'][dir_dict[False]['qbase']] = 1
+                    else:
+                        filtered_read_dict['forward_SNV_reverse_ref'][dir_dict[False]['qbase']] += 1
+                # Reverse ref forward QF
+                else:
+                    if dir_dict[False]['qbase'] not in filtered_read_dict['reverse_ref_forward_UM_QF']:
+                        filtered_read_dict['reverse_ref_forward_UM_QF'][dir_dict[False]['qbase']] = 1
+                    else:
+                        filtered_read_dict['reverse_ref_forward_UM_QF'][dir_dict[False]['qbase']] += 1
+            # SNV in reverse read only
+            elif dir_dict[True]['match'] and not dir_dict[False]['match']:
+                # Quality filter
+                if dir_dict[False]['qual'] >= quality_cutoff:
+                    if dir_dict[False]['qbase'] not in filtered_read_dict['reverse_SNV_forward_ref']:
+                        filtered_read_dict['reverse_SNV_forward_ref'][dir_dict[False]['qbase']] = 1
+                    else:
+                        filtered_read_dict['reverse_SNV_forward_ref'][dir_dict[False]['qbase']] += 1
+                    # Since the forward base matches the reference, don't quality filter
+                    if dir_dict[True]['qbase'] not in filtered_read_dict['reverse_SNV_forward_ref']:
+                        filtered_read_dict['reverse_SNV_forward_ref'][dir_dict[True]['qbase']] = 1
+                    else:
+                        filtered_read_dict['reverse_SNV_forward_ref'][dir_dict[True]['qbase']] += 1
+                # Forward ref reverse QF
+                else:
+                    if dir_dict[True]['qbase'] not in filtered_read_dict['forward_ref_reverse_UM_QF']:
+                        filtered_read_dict['forward_ref_reverse_UM_QF'][dir_dict[True]['qbase']] = 1
+                    else:
+                        filtered_read_dict['forward_ref_reverse_UM_QF'][dir_dict[True]['qbase']] += 1
+            # Both reads match the reference sequence - don't quality filter, and add two matches (for forward and
+            # reverse reads)
+            else:
+                if dir_dict[True]['qbase'] not in filtered_read_dict['congruent_ref']:
+                    filtered_read_dict['congruent_ref'][dir_dict[True]['qbase']] = 2
+                else:
+                    filtered_read_dict['congruent_ref'][dir_dict[True]['qbase']] += 2
+        # Either the reads are unpaired, or only a single read aligns to this position on the gene (no overlap)
+        else:
+            for direction in dir_dict:
+                # SNV supported by a single read
+                if not dir_dict[direction]['match']:
+                    if dir_dict[direction]['qual'] >= quality_cutoff:
+                        # Forward
+                        if direction:
+                            if dir_dict[direction]['qbase'] not in filtered_read_dict['forward_SNV_reverse_UM_QF']:
+                                filtered_read_dict['forward_SNV_reverse_UM_QF'][dir_dict[direction]['qbase']] = 1
+                            else:
+                                filtered_read_dict['forward_SNV_reverse_UM_QF'][dir_dict[direction]['qbase']] += 1
+                        # Reverse
+                        else:
+                            if dir_dict[direction]['qbase'] not in filtered_read_dict['reverse_SNV_forward_UM_QF']:
+                                filtered_read_dict['reverse_SNV_forward_UM_QF'][dir_dict[direction]['qbase']] = 1
+                            else:
+                                filtered_read_dict['reverse_SNV_forward_UM_QF'][dir_dict[direction]['qbase']] += 1
+                    else:
+                        # Forward QF
+                        if dir_dict[direction]['qbase'] not in filtered_read_dict['forward_quality_filtered']:
+                            filtered_read_dict['forward_quality_filtered'][dir_dict[direction]['qbase']] = 1
+                        else:
+                            filtered_read_dict['forward_quality_filtered'][dir_dict[direction]['qbase']] += 1
+
+                # Match to the reference sequence supported by a single read
+                else:
+                    if dir_dict[direction]['qual'] >= quality_cutoff:
+                        # Forward
+                        if direction:
+                            if dir_dict[direction]['qbase'] not in filtered_read_dict['forward_ref_reverse_UM_QF']:
+                                filtered_read_dict['forward_ref_reverse_UM_QF'][dir_dict[direction]['qbase']] = 1
+                            else:
+                                filtered_read_dict['forward_ref_reverse_UM_QF'][dir_dict[direction]['qbase']] += 1
+                        # Reverse
+                        else:
+                            if dir_dict[direction]['qbase'] not in filtered_read_dict['reverse_ref_forward_UM_QF']:
+                                filtered_read_dict['reverse_ref_forward_UM_QF'][dir_dict[direction]['qbase']] = 1
+                            else:
+                                filtered_read_dict['reverse_ref_forward_UM_QF'][dir_dict[direction]['qbase']] += 1
                     else:
-                        unfiltered_base_qualities[base].append(quality)
-            except IndexError:
-                pass
-    # Now check that at least two bases for each of the bases present high quality.
-    # first remove all low quality bases
-    # Use dictionary comprehension to make a new dictionary where only scores above threshold are kept.
-    # Internally list comprehension is used to filter the list
-    filtered_base_qualities = {base: [score for score in scores if score >= quality_cutoff] for (base, scores) in
-                               unfiltered_base_qualities.items()}
-
-    # Now remove bases that have no high quality scores
-    # Use dictionary comprehension to make a new dictionary where bases that have a non-empty scores list are kept
-    filtered_base_qualities = {base: scores for (base, scores) in filtered_base_qualities.items() if scores}
- 
-    # If we less than two bases with high quality scores, ignore things.
-    if len(filtered_base_qualities) < 2:
-        return dict()
-
-    # Now that filtered_base_qualities only contains bases with more than one HQ base, make just a dict with base
-    # counts with dict comprehension
-    high_quality_base_count = {base: len(scores) for (base, scores) in filtered_base_qualities.items()}
-    
-    if number_of_bases_above_threshold(high_quality_base_count,
-                                       base_count_cutoff=base_cutoff,
-                                       base_fraction_cutoff=base_fraction_cutoff) > 1:
-        logging.debug('base qualities before filtering: {0}'.format(unfiltered_base_qualities))
-        logging.debug('base qualities after filtering: {0}'.format(filtered_base_qualities))
-        logging.debug('SNVs found at position {0}: {1}\n'.format(column.pos, high_quality_base_count))
-        return high_quality_base_count
+                        # Reverse QF
+                        if dir_dict[direction]['qbase'] not in filtered_read_dict['reverse_quality_filtered']:
+                            filtered_read_dict['reverse_quality_filtered'][dir_dict[direction]['qbase']] = 1
+                        else:
+                            filtered_read_dict['reverse_quality_filtered'][dir_dict[direction]['qbase']] += 1
+    return filtered_read_dict, qualities
+
+
+def determine_cutoff(qualities, reference_sequence, base_cutoff, error_cutoff=1.0):
+    """
+    Determine the base cutoff value to use for SNV determination
+    :param qualities: List of phred scores for every base in the pileup
+    :param reference_sequence: String of the FASTA reference gene sequence
+    :param error_cutoff: Float of the error cutoff value to use. Default is 1.0%
+    :return: base_cutoff: Int of calculated gene-specific cutoff value to use
+    :return: The percentage error value corresponding to the base_cutoff value
+    """
+    depth_prob = 0
+    # Only find the cutoff if there are qualities (the gene is present in the sample)
+    if qualities:
+        # Convert the gene-specific phred score to its probability e.g phred score of 20 is 1x10^(-20/10) = 1x10^(-2)
+        # = 0.01
+        phred_prob = 1 * 10 ** (-(mean(qualities) / 10))
+        # Determine the probability that any base in the pileup will be incorrect. Multiply the phred probability by
+        # the average depth of the sample (number of bases / length of the gene)
+        depth_prob = phred_prob * len(qualities) / len(reference_sequence)
+        # Find the lowest value of the base cutoff that gives a false positive error value under the error cutoff value
+        # for the entire length of the gene. Take the depth_prob to the power of the current base_cutoff value.
+        # Multiply this by the length of the gene to find find that value for the entire gene, and by 100 to convert
+        # this to a percent value. e.g. 0.01^2 * 1674 * 100 = 16.74%. Note that this is above the default 1% threshold.
+        # The base_cutoff will be incremented by one, and the calculation will be run again: 0.01^3 * 1674 * 100 =
+        # 0.1674%, which is below the threshold, and would pass
+        while depth_prob ** base_cutoff * len(reference_sequence) > error_cutoff * 100:
+            base_cutoff += 1
+    return base_cutoff, depth_prob ** base_cutoff * 100 * len(reference_sequence)
+
+
+def find_multibase_positions(ref_base, filtered_read_dict, base_cutoff, base_fraction_cutoff):
+    """
+
+    :param ref_base: String of the sequence of the reference gene at the current position
+    :param filtered_read_dict: Dictionary with of base types: read direction: count
+    :param base_cutoff: Integer of the number of identical mismatches in a column required for a SNV call
+    :param base_fraction_cutoff: Float fraction of bases necessary to support a SNV call
+    :return: snv_dict: Dictionary of characterised bases of the current column e.g. total, number matching reference
+    sequence, number of SNVs in both forward and reverse reads, etc.
+    :return: passing_snv_dict: Dictionary summarising counts of categories of bases e.g. congruent, forward, reverse,
+    paired
+    :return: total_coverage: Integer of the total number of bases passing filter in the pileup
+    """
+    # Initialise a dictionary to store the counts of the characterised bases
+    snv_dict = {
+        'total': 0,
+        'total_congruent': 0,
+        'total_congruent_SNV': 0,
+        'total_forward': 0,
+        'total_forward_SNV': 0,
+        'total_reverse': 0,
+        'total_reverse_SNV': 0,
+        'total_SNV': 0
+    }
+    # Initialise the total depth of the column to zero
+    total_coverage = 0
+    # Initialise a dictionary to store the count for each individual nucleotide at this position e.g. A:24, G:2
+    base_count = dict()
+    # Iterate through the categories e.g. congruent_ref in the dictionary
+    for category, base_dict in filtered_read_dict.items():
+        # Iterate through the sequence of each query base, and the corresponding count
+        for base, count in base_dict.items():
+            # Do not process the base if it has been flagged as 'filtered'
+            if 'filtered' not in category:
+                # Populate the base counting dictionary with the base sequence and increment the count
+                if base not in base_count:
+                    base_count[base] = count
+                else:
+                    base_count[base] += count
+                # Update the total coverage
+                total_coverage += count
+                snv_dict['total'] += count
+            # Forward and reverse reads agree on base
+            if 'congruent' in category:
+                # Congruent reference sequence
+                snv_dict['total_congruent'] += count
+                snv_dict['total_forward'] += int(count / 2)
+                snv_dict['total_reverse'] += int(count / 2)
+                # Congruent SNVs
+                if 'SNV' in category and base != ref_base:
+                    snv_dict['total_congruent_SNV'] += count
+                    snv_dict['total_forward_SNV'] += int(count / 2)
+                    snv_dict['total_reverse_SNV'] += int(count / 2)
+                    snv_dict['total_SNV'] += count
+            # SNV in forward read
+            elif category.startswith('forward_SNV'):
+                snv_dict['total_forward'] += count
+                if base != ref_base:
+                    snv_dict['total_forward_SNV'] += count
+                    snv_dict['total_SNV'] += count
+            # Forward read matches reference
+            elif category.startswith('forward_ref'):
+                snv_dict['total_forward'] += count
+            # SNV in reverse read
+            elif category.startswith('reverse_SNV'):
+                snv_dict['total_reverse'] += count
+                if base != ref_base:
+                    snv_dict['total_reverse_SNV'] += count
+                    snv_dict['total_SNV'] += count
+            # Reverse read match reference
+            elif category.startswith('reverse_ref'):
+                snv_dict['total_reverse'] += count
+    # Initialise a dictionary to store the summary of characterised base types
+    passing_snv_dict = {
+        'congruent': dict(),
+        'forward': dict(),
+        'reverse': dict(),
+        'paired': dict()
+    }
+    # Boolean of whether there are bases passing filter, and the passing_snv_dict should be used
+    return_dict = False
+    # Iterate through the categories in the dictionary
+    for category, base_dict in filtered_read_dict.items():
+        # Iterate through each query base and its corresponding count
+        for base, count in base_dict.items():
+            # Congruent SNVs
+            if 'congruent' in category and base != ref_base:
+                # If the base_cutoff_fraction has been provided, use it in making SNV calls
+                if base_fraction_cutoff:
+                    # Ensure that the number of SNVs in the pileup is greater than the base_cutoff and the
+                    # fraction of SNVs in the pileup is greater than the base_cutoff_fraction
+                    if float(base_count[base] / snv_dict['total']) >= base_fraction_cutoff and base_count[base] \
+                            >= base_cutoff:
+                        # Update the summary dictionary with the base sequence and count
+                        if base not in passing_snv_dict['forward']:
+                            passing_snv_dict['congruent'][base] = count
+                        else:
+                            passing_snv_dict['congruent'][base] += count
+                        return_dict = True
+                # If base_cutoff_fraction is not supplied, only the number of SNVs in the pileup must be greater than
+                # the base_cutoff value in order for a SNV call
+                else:
+                    if base_count[base] >= base_cutoff:
+                        if base not in passing_snv_dict['congruent']:
+                            passing_snv_dict['congruent'][base] = count
+                        else:
+                            passing_snv_dict['congruent'][base] += count
+                    return_dict = True
+            # SNVs in the forward read
+            if category.startswith('forward_SNV') and base != ref_base:
+                if base_fraction_cutoff:
+                    if float(base_count[base] / snv_dict['total']) >= base_fraction_cutoff and base_count[base] \
+                            >= base_cutoff:
+                        if base not in passing_snv_dict['forward']:
+                            passing_snv_dict['forward'][base] = count
+                        else:
+                            passing_snv_dict['forward'][base] += count
+                        return_dict = True
+                else:
+                    if base_count[base] >= base_cutoff:
+                        if base not in passing_snv_dict['forward']:
+                            passing_snv_dict['forward'][base] = count
+                        else:
+                            passing_snv_dict['forward'][base] += count
+                        return_dict = True
+            # SNVs in the reverse read
+            if category.startswith('reverse_SNV') and base != ref_base:
+                if base_fraction_cutoff:
+                    if float(base_count[base] / snv_dict['total']) >= base_fraction_cutoff and base_count[base] \
+                            >= base_cutoff:
+                        if base not in passing_snv_dict['reverse']:
+                            passing_snv_dict['reverse'][base] = count
+                        else:
+                            passing_snv_dict['reverse'][base] += count
+                        return_dict = True
+                else:
+                    if base_count[base] >= base_cutoff:
+                        if base not in passing_snv_dict['reverse']:
+                            passing_snv_dict['reverse'][base] = count
+                        else:
+                            passing_snv_dict['reverse'][base] += count
+                        return_dict = True
+            # All unfiltered bases
+            if base != ref_base and 'filtered' not in category:
+                if base_fraction_cutoff:
+                    if float(base_count[base] / snv_dict['total']) >= base_fraction_cutoff and base_count[base] \
+                            >= base_cutoff:
+                        if base not in passing_snv_dict['paired']:
+                            passing_snv_dict['paired'][base] = count
+                        else:
+                            passing_snv_dict['paired'][base] += count
+                        return_dict = True
+                else:
+                    if base_count[base] >= base_cutoff:
+                        if base not in passing_snv_dict['paired']:
+                            passing_snv_dict['paired'][base] = count
+                        else:
+                            passing_snv_dict['paired'][base] += count
+                        return_dict = True
+    if return_dict:
+        return snv_dict, passing_snv_dict, total_coverage
     else:
-        # logging.debug('No SNVs\n')
-        return dict()
+        return snv_dict, dict(), total_coverage
 
 
-def get_contig_names(fasta_file):
+def position_details(actual_position, passing_snv_dict, contig_name, ref_base, total_coverage, base_cutoff, error_perc):
     """
-    Gets contig names from a fasta file using SeqIO.
-    :param fasta_file: Full path to uncompressed, fasta-formatted file
-    :return: List of contig names.
-    """
-    contig_names = list()
-    for contig in SeqIO.parse(fasta_file, 'fasta'):
-        contig_names.append(contig.id)
-    return contig_names
-
-
-def read_contig(contig_name, bamfile_name, reference_fasta, quality_cutoff=20, base_cutoff=2,
-                base_fraction_cutoff=None, fasta=False):
+    Create a string summarising the ConFindr results for current gene
+    :param actual_position: Integer of the adjusted position of the current base
+    :param passing_snv_dict: Dictionary summarising counts of categories of bases
+    :param contig_name: Name of current gene
+    :param ref_base: Sequence of the current reference base
+    :param total_coverage: Integer of the total depth at this position
+    :param base_cutoff: Integer of the SNV depth cutoff value
+    :param error_perc: Float of the calculated error value
+    :return: to_write: String containing formatted outputs to be entered into the final report
+    """
+    # List of the base categories present in passing_snv_dict
+    read_types = ['congruent', 'paired', 'forward', 'reverse']
+    # Update the to_write string with basic information
+    to_write = '{contig_name},{pos},{ref_base},'.format(contig_name=contig_name,
+                                                        pos=actual_position,
+                                                        ref_base=ref_base)
+    # Initialise the coverage value to zero
+    snv_coverage = 0
+    # Iterate through all the read types
+    for read_type in read_types:
+        # Boolean of whether a semi-colon needs to be added to the string to separate all the base sequences
+        semi_colon = False
+        for base, coverage in passing_snv_dict[read_type].items():
+            # Ensure that the base isn't empty
+            if base:
+                if semi_colon:
+                    to_write += ';'
+                to_write += '{base}:{depth}'.format(base=base,
+                                                    depth=coverage)
+                semi_colon = True
+                # Increment the coverage only if the read type isn't 'paired'
+                if read_type != 'paired':
+                    snv_coverage += coverage
+        to_write += ','
+    # Format the error_perc to be more readable
+    error_perc = '{:0.2f}'.format(error_perc) if error_perc else 'ND'
+    to_write += '{snv_cov},{total_cov},{base_cutoff},{error_perc}\n'\
+        .format(snv_cov=snv_coverage,
+                total_cov=total_coverage,
+                base_cutoff=base_cutoff,
+                error_perc=error_perc)
+    return to_write
+
+
+def read_contig(contig_name, bamfile_name, reference_fasta, allele_records, 
+                fastq_records, quality_cutoff=20, base_cutoff=None, 
+                base_fraction_cutoff=None, fasta=False, error_cutoff=1.0,
+                nanopore=False):
     """
     Examines a contig to find if there are positions where more than one base is present.
     :param contig_name: Name of contig as a string.
     :param bamfile_name: Full path to bamfile. Must be sorted/indexed
     :param reference_fasta: Full path to fasta file that was used to generate the bamfile.
+    :param allele_records:
+    :param fastq_records: Dictionary of SeqIO records parsed from filtered FASTQ reads
     :param quality_cutoff: Bases must have at least this phred score to be considered (INT)
     :param base_cutoff: At least this many bases must support a minor variant (INT)
     :param base_fraction_cutoff: At least this percentage of bases must support minor variant (FLOAT)
     :param fasta: Boolean on whether the samples are in FASTA format. Default is False
+    :param error_cutoff: Float of the error cutoff value to use. Default is 1.0%
+    :param nanopore: Boolean of whether Nanopore reads were provided. Default is False.
     :return: Dictionary of positions where more than one base is present. Keys are contig name, values are positions
     """
-    bamfile = pysam.AlignmentFile(bamfile_name, 'rb')
+    pysam_fasta = pysam.FastaFile(reference_fasta)
     multibase_position_dict = dict()
-    to_write = list()
+    to_write = str()
     # If analysing FASTA files, a single base difference is all that is expected
     if fasta:
         base_cutoff = 1
-    # These parameters seem to be fairly undocumented with pysam, but I think that they should make the output
-    # that I'm getting to match up with what I'm seeing in Tablet.
-    for column in bamfile.pileup(contig_name,
-                                 stepper='samtools',
-                                 ignore_orphans=False,
-                                 fastafile=pysam.FastaFile(reference_fasta),
-                                 min_base_quality=0):
-
-        base_dict = find_if_multibase(column,
-                                      quality_cutoff=quality_cutoff,
-                                      base_cutoff=base_cutoff,
-                                      base_fraction_cutoff=base_fraction_cutoff)
-
-        if base_dict:
+    reference_sequence = str(allele_records[contig_name].seq)
+    # Parse the BAM file with pysam to create AlignmentFile, and AlignmentFile.pileup objects
+    bamfile, pileup = parse_bam(bamfile_name=bamfile_name,
+                                contig_name=contig_name,
+                                pysam_fasta=pysam_fasta)
+    filtered_read_dict = dict()
+    quality_list = list()
+    for i, column in enumerate(pileup):
+        filtered_reads, qualities = characterise_read(column=column,
+                                                      reference_sequence=reference_sequence,
+                                                      fastq_records=fastq_records,
+                                                      quality_cutoff=quality_cutoff,
+                                                      fasta=fasta,
+                                                      nanopore=nanopore)
+        filtered_read_dict[i] = filtered_reads
+        quality_list += qualities
+    # Initialise the calculated error percentage to zero
+    error_perc = None
+    # If the base_cutoff is not manually specified on the command-line, adjust it based
+    # upon overall sequence quality
+    if base_cutoff != 3:
+        base_cutoff, error_perc = determine_cutoff(qualities=quality_list,
+                                                   reference_sequence=reference_sequence,
+                                                   base_cutoff = base_cutoff,
+                                                   error_cutoff=error_cutoff)
+    bamfile.close()
+    # It seems that the pileup (generator?) is used up above, so it must be recreated
+    bamfile, pileup = parse_bam(bamfile_name=bamfile_name,
+                                contig_name=contig_name,
+                                pysam_fasta=pysam_fasta)
+    for i, column in enumerate(pileup):
+        # Extract the sequence of the reference gene at the current position
+        ref_base = reference_sequence[column.pos]
+        # Summarise the pileup
+        snv_dict, passing_snv_dict, total_coverage = \
+            find_multibase_positions(ref_base=ref_base,
+                                     filtered_read_dict=filtered_read_dict[i],
+                                     base_cutoff=base_cutoff,
+                                     base_fraction_cutoff=base_fraction_cutoff)
+        # If there are any SNVs called for the gene, update the multibase_position_dict, and to_write string
+        if passing_snv_dict:
             # Pysam starts counting at 0, whereas we actually want to start counting at 1.
             actual_position = column.pos + 1
-            if column.reference_name in multibase_position_dict:
-                multibase_position_dict[column.reference_name].append(actual_position)
-            else:
-                multibase_position_dict[column.reference_name] = [actual_position]
-            to_write.append('{reference},{position},{bases},{coverage}\n'
-                            .format(reference=column.reference_name,
-                                    position=actual_position,
-                                    bases=base_dict_to_string(base_dict),
-                                    coverage=sum(base_dict.values())))
+            # Initialise the gene name in the dictionary as required
+            if column.reference_name not in multibase_position_dict:
+                multibase_position_dict[column.reference_name] = dict()
+            # Update the dictionary with the actual position:
+            multibase_position_dict[column.reference_name].update({actual_position: passing_snv_dict})
+            to_write += position_details(actual_position=actual_position,
+                                         passing_snv_dict=passing_snv_dict,
+                                         contig_name=contig_name,
+                                         ref_base=ref_base,
+                                         total_coverage=total_coverage,
+                                         base_cutoff=base_cutoff,
+                                         error_perc=error_perc)
     bamfile.close()
     return multibase_position_dict, to_write
 
 
 def find_rmlst_type(kma_report, rmlst_report):
     """
     Uses a report generated by KMA to determine what allele is present for each rMLST gene.
     :param kma_report: The .res report generated by KMA.
     :param rmlst_report: rMLST report file to write information to.
-    :return: a sorted list of loci present, in format gene_allele
+    :return: a sorted list of loci present, in format 'gene_allele'
     """
     genes_to_use = dict()
     score_dict = dict()
     gene_alleles = list()
     with open(kma_report) as tsvfile:
         reader = csv.DictReader(tsvfile, delimiter='\t')
         for row in reader:
@@ -429,39 +948,103 @@
     """
     total_length = 0
     for sequence in SeqIO.parse(fasta_file, 'fasta'):
         total_length += len(sequence.seq)
     return total_length
 
 
-def estimate_percent_contamination(contamination_report_file):
+# Removing percentage contamination estimation until it can be made more 
+# accurate
+#-------------------------------------------------------------------------------
+# def estimate_percent_contamination(contamination_report_file):
+#     """
+#     Estimates the percent contamination of a sample (and standard deviation).
+#     :param contamination_report_file: File created by read_contig,
+#     :return: Estimated percent contamination and standard deviation.
+#     """
+#     # Initialise a list to store the percentage of SNVs out of the total bases
+#     contam_levels = list()
+#     with open(contamination_report_file) as csvfile:
+#         reader = csv.DictReader(csvfile)
+#         for row in reader:
+#             base_counts = int(row['SNVCoverage'])
+#             total_coverage = int(row['TotalCoverage'])
+#             contam_levels.append(base_counts * 100 / total_coverage)
+#     return '%.2f' % (np.mean(contam_levels)), '%.2f' % np.std(contam_levels)
+
+
+def load_fastq_records(gz, paired, forward):
+    """
+    Use SeqIO to load FASTQ records from file
+    :param gz: Name and path of FASTQ file
+    :param paired: Boolean of whether the reads are paired
+    :param forward: Boolean of whether the current reads are in the forward direction
+    :return: records: Dictionary of SeqIO parsed FASTQ records with consistent ID naming
+    """
+    # Initialise a dictionary to store the FASTQ records
+    records = dict()
+    # Iterate through the reads
+    for record in SeqIO.parse(gz, 'fastq'):
+        # Only update the naming scheme for paired reads
+        if paired:
+            if forward:
+                # Change a :1: to /1 in the record.id
+                if ':1:' in record.id:
+                    record.id = record.id + '/1'
+                # Don't worry if the record.id already has a /1
+                elif '/1' in record.id:
+                    pass
+                # If the record.id doesn't have a read direction, add /1
+                else:
+                    record.id = record.id + '/1'
+            # Process reverse reads in a similar fashion to forward reads
+            else:
+                if ':2:' in record.id:
+                    record.id = record.id + '/2'
+                elif '/2' in record.id:
+                    pass
+                else:
+                    record.id = record.id + '/2'
+        else:
+            pass
+        records.update(SeqIO.to_dict([record]))
+    return records
+
+
+def index_databases(sample_database):
     """
-    Estimates the percent contamination of a sample (and standard deviation).
-    :param contamination_report_file: File created by read_contig,
-    :return: Estimated percent contamination and standard deviation.
-    """
-    contam_levels = list()
-    with open(contamination_report_file) as csvfile:
-        reader = csv.DictReader(csvfile)
-        for row in reader:
-            lowest_count = 99999
-            base_counts = row['Bases'].split(';')
-            for count in base_counts:
-                num_bases = int(count.split(':')[1])
-                if num_bases < lowest_count:
-                    lowest_count = num_bases
-            total_coverage = int(row['Coverage'])
-            contam_levels.append(lowest_count*100/total_coverage)
-    return '%.2f' % (np.mean(contam_levels)), '%.2f' % np.std(contam_levels)
+    Index the database file with pysam and kma
+    :param sample_database:
+    """
+    if not os.path.isfile(sample_database + '.fai'):  # Don't bother re-indexing, this only needs to happen once.
+        try:
+            pysam.faidx(sample_database)
+        except pysam.utils.SamtoolsError:
+            pass
+    kma_database = sample_database.replace('.fasta', '') + '_kma'
+
+    if not os.path.isfile(kma_database + '.name'):  # The .name is one of the files KMA creates when making a database.
+        logging.info('Since this is the first time you are using this database, it needs to be indexed by KMA. '
+                     'This might take a while')
+        cmd = 'kma index -i {} -o {}'.format(sample_database, kma_database)  # NOTE: Need KMA >=1.2.0 for this to work.
+        out = str()
+        try:
+            out, err = run_cmd(cmd)
+        except subprocess.CalledProcessError as e:
+            err = e
+        log = sample_database + '_log.txt'
+        write_to_logfile(log, out, err, cmd)
 
 
-def find_contamination(pair, output_folder, databases_folder, forward_id='_R1', threads=1, keep_files=False,
-                       quality_cutoff=20, base_cutoff=2, base_fraction_cutoff=0.05, cgmlst_db=None, xmx=None,
-                       tmpdir=None, data_type='Illumina', use_rmlst=False, cross_details=False, min_matching_hashes=40,
-                       fasta=False):
+# noinspection PyUnresolvedReferences
+def find_contamination(pair, output_folder, databases_folder, base_cutoff, forward_id='_R1', threads=1,
+                       keep_files=False,
+                       quality_cutoff=20, base_fraction_cutoff=0.05, cgmlst_db=None, xmx=None,
+                       tmpdir=None, data_type='Illumina', use_rmlst=False, min_matching_hashes=40,
+                       fasta=False, error_cutoff=1.0, debug=False):
     """
     This needs some documentation fairly badly, so here we go.
     :param pair: This has become a misnomer. If the input reads are actually paired, needs to be a list
     with the full filepath to forward reads at index 0 and full path to reverse reads at index 1.
     If reads are unpaired, should be a list of length 1 with the only entry being the full filepath to read set.
     :param output_folder: Folder where outputs (confindr log and report, and other stuff) will be stored.
     This will be created if it does not exist. (I think - should write a test that double checks this).
@@ -480,19 +1063,19 @@
     :param cgmlst_db: if None, we're using rMLST, if True, using some sort of custom cgMLST database. This requires some
     custom parameters.
     :param xmx: if None, BBTools will use auto memory detection. If string, BBTools will use what's specified as their
     memory request.
     :param tmpdir: if None, any genus-specifc databases that need to be created will be written to ConFindr DB location.
     :param data_type: Either Illumina or Nanopore, depending on what type your reads are. (STR)
     :param use_rmlst: If False, use cgderived data instead of rMLST where possible. If True, always use rMLST. (BOOL)
-    :param cross_details: If False, stop workflow when cross contamination is detected. If True, continue so estimates
-    of percent contamination can be found (BOOL)
     :param min_matching_hashes: Minimum number of matching hashes in a MASH screen in order for a genus to be
     considered present in a sample. Default is 40
     :param fasta: Boolean on whether the samples are in FASTA format. Default is False
+    :param error_cutoff: Float of the error cutoff value to use. Default is 1.0%
+    :param debug: Run the find_contamination with multi-processing to allow easier debugging
     """
     if os.path.isfile(os.path.join(databases_folder, 'download_date.txt')):
         with open(os.path.join(databases_folder, 'download_date.txt')) as f:
             database_download_date = f.readline().rstrip()
     else:
         database_download_date = 'ND'
     log = os.path.join(output_folder, 'confindr_log.txt')
@@ -508,39 +1091,38 @@
     if not os.path.isdir(sample_tmp_dir):
         os.makedirs(sample_tmp_dir)
 
     logging.info('Checking for cross-species contamination...')
     if paired:
         genus = find_cross_contamination(databases_folder,
                                          reads=pair,
+                                         sample_name=sample_name,
                                          tmpdir=sample_tmp_dir,
                                          log=log,
                                          threads=threads,
                                          min_matching_hashes=min_matching_hashes)
     else:
         genus = find_cross_contamination(databases_folder,
                                          reads=pair[0],
+                                         sample_name=sample_name,
                                          tmpdir=sample_tmp_dir,
                                          log=log,
                                          threads=threads,
                                          min_matching_hashes=min_matching_hashes)
-    if len(genus.split(':')) > 1:
-        if not cross_details:
-            write_output(output_report=os.path.join(output_folder, 'confindr_report.csv'),
-                         sample_name=sample_name,
-                         multi_positions=0,
-                         genus=genus,
-                         percent_contam='ND',
-                         contam_stddev='ND',
-                         total_gene_length=0,
-                         database_download_date=database_download_date)
-            logging.info('Found cross-contamination! Skipping rest of analysis...\n')
-            if keep_files is False:
-                shutil.rmtree(sample_tmp_dir)
-            return
+    # if len(genus.split(':')) > 1:
+    #     write_output(output_report=os.path.join(output_folder, 'confindr_report.csv'),
+    #                     sample_name=sample_name,
+    #                     multi_positions=0,
+    #                     genus=genus,
+    #                     total_gene_length=0,
+    #                     database_download_date=database_download_date)
+    #     logging.info('Found cross-contamination! Skipping rest of analysis...\n')
+    #     if keep_files is False:
+    #         shutil.rmtree(sample_tmp_dir)
+    #     return
     # Setup genus-specific databases, if necessary.
     if cgmlst_db is not None:
         # Sanity check that the DB specified is actually a file, otherwise, quit with appropriate error message.
         if not os.path.isfile(cgmlst_db):
             logging.error('ERROR: Specified cgMLST file ({}) does not exist. Please check the path and try again.'
                           .format(cgmlst_db))
             quit(code=1)
@@ -565,16 +1147,16 @@
                 sample_database = os.path.join(db_folder, '{}_db.fasta'.format(predominant_genus))
                 if not os.path.isfile(sample_database):
 
                     if os.path.isfile(os.path.join(db_folder, 'gene_allele.txt')) and \
                             os.path.isfile(os.path.join(db_folder, 'rMLST_combined.fasta')):
                         logging.info('Setting up rMLST genus-specific database for genus {}...'
                                      .format(predominant_genus))
-                        allele_list = find_genusspecific_allele_list(os.path.join(db_folder, 'gene_allele.txt'),
-                                                                     predominant_genus)
+                        allele_list = find_genus_specific_allele_list(os.path.join(db_folder, 'gene_allele.txt'),
+                                                                      predominant_genus)
                         # Create the allele-specific database
                         setup_allelespecific_database(fasta_file=sample_database,
                                                       database_folder=db_folder,
                                                       allele_list=allele_list)
             else:
                 # Check if a cgderived database is available. If not, try to use rMLST database.
                 sample_database = os.path.join(db_folder, '{}_db_cgderived.fasta'.format(predominant_genus))
@@ -582,16 +1164,16 @@
                     sample_database = os.path.join(db_folder, '{}_db.fasta'.format(predominant_genus))
                     # Create genus specific database if it doesn't already exist and we have the necessary rMLST files.
                     if os.path.isfile(os.path.join(db_folder, 'rMLST_combined.fasta')) and \
                             os.path.isfile(os.path.join(db_folder, 'gene_allele.txt')) and not \
                             os.path.isfile(sample_database):
                         logging.info('Setting up core genome genus-specific database for genus {}...'
                                      .format(predominant_genus))
-                        allele_list = find_genusspecific_allele_list(os.path.join(db_folder, 'gene_allele.txt'),
-                                                                     predominant_genus)
+                        allele_list = find_genus_specific_allele_list(os.path.join(db_folder, 'gene_allele.txt'),
+                                                                      predominant_genus)
                         setup_allelespecific_database(fasta_file=sample_database,
                                                       database_folder=db_folder,
                                                       allele_list=allele_list)
 
         else:
             sample_database = os.path.join(db_folder, 'rMLST_combined.fasta')
 
@@ -599,318 +1181,417 @@
     # they don't have rMLST downloaded and we don't have a cg-derived database available, boot them with a helpful
     # message.
     if not os.path.isfile(sample_database):
         write_output(output_report=os.path.join(output_folder, 'confindr_report.csv'),
                      sample_name=sample_name,
                      multi_positions=0,
                      genus=genus,
-                     percent_contam='ND',
-                     contam_stddev='ND',
                      total_gene_length=0,
                      database_download_date=database_download_date)
         logging.info('Did not find databases for genus {genus}. You can download the rMLST database to get access to '
                      'all genera (see https://olc-bioinformatics.github.io/ConFindr/install/). Alternatively, if you '
                      'have a high-quality core-genome derived database for your genome of interest, we would be happy '
                      'to add it - open an issue at https://github.com/OLC-Bioinformatics/ConFindr/issues with the '
                      'title "Add genus-specific database: {genus}"\n'.format(genus=genus))
         if keep_files is False:
             shutil.rmtree(sample_tmp_dir)
         return
 
     # Extract rMLST reads and quality trim.
     logging.info('Extracting conserved core genes...')
+    out, err, cmd = '', '', ''
+    forward_bait = str()
+    forward_trimmed = str()
+    reverse_bait = str()
+    reverse_trimmed = str()
+    unpaired_bait = str()
+    unpaired_trimmed = str()
     if paired:
-        if xmx is None:
-            out, err, cmd = bbtools.bbduk_bait(reference=sample_database,
-                                               forward_in=pair[0],
-                                               reverse_in=pair[1],
-                                               forward_out=os.path.join(sample_tmp_dir, 'rmlst_R1.fastq.gz'),
-                                               reverse_out=os.path.join(sample_tmp_dir, 'rmlst_R2.fastq.gz'),
-                                               threads=threads,
-                                               returncmd=True)
-        else:
-            out, err, cmd = bbtools.bbduk_bait(reference=sample_database,
-                                               forward_in=pair[0],
-                                               reverse_in=pair[1],
-                                               forward_out=os.path.join(sample_tmp_dir, 'rmlst_R1.fastq.gz'),
-                                               reverse_out=os.path.join(sample_tmp_dir, 'rmlst_R2.fastq.gz'),
-                                               threads=threads,
-                                               Xmx=xmx,
-                                               returncmd=True)
+        forward_bait = os.path.join(sample_tmp_dir, '{sn}_baited_R1.fastq.gz'.format(sn=sample_name))
+        reverse_bait = forward_bait.replace('_R1', '_R2')
+        if not os.path.isfile(forward_bait):
+            if xmx is None:
+                out, err, cmd = bbtools.bbduk_bait(reference=sample_database,
+                                                   forward_in=pair[0],
+                                                   reverse_in=pair[1],
+                                                   forward_out=forward_bait,
+                                                   reverse_out=reverse_bait,
+                                                   threads=threads,
+                                                   returncmd=True)
+            else:
+                out, err, cmd = bbtools.bbduk_bait(reference=sample_database,
+                                                   forward_in=pair[0],
+                                                   reverse_in=pair[1],
+                                                   forward_out=forward_bait,
+                                                   reverse_out=reverse_bait,
+                                                   threads=threads,
+                                                   Xmx=xmx,
+                                                   returncmd=True)
     else:
+        # Still name the file '_baited_trimmed' even if the file won't be trimmed
         if data_type == 'Nanopore' or fasta:
-            forward_out = os.path.join(sample_tmp_dir, 'trimmed.fastq.gz')
+            unpaired_bait = os.path.join(sample_tmp_dir, '{sn}_baited_trimmed.fastq.gz'.format(sn=sample_name))
         else:
-            forward_out = os.path.join(sample_tmp_dir, 'rmlst.fastq.gz')
-        if xmx is None:
-            out, err, cmd = bbtools.bbduk_bait(reference=sample_database, forward_in=pair[0],
-                                               forward_out=forward_out,
-                                               returncmd=True, threads=threads)
-        else:
-            out, err, cmd = bbtools.bbduk_bait(reference=sample_database, forward_in=pair[0],
-                                               forward_out=forward_out, Xmx=xmx,
-                                               returncmd=True, threads=threads)
-    write_to_logfile(log, out, err, cmd)
-    logging.info('Quality trimming...')
-    if data_type == 'Illumina':
-        if paired:
+            unpaired_bait = os.path.join(sample_tmp_dir, '{sn}_baited.fastq.gz'.format(sn=sample_name))
+        if not os.path.isfile(unpaired_bait):
             if xmx is None:
-                out, err, cmd = bbtools.bbduk_trim(forward_in=os.path.join(sample_tmp_dir, 'rmlst_R1.fastq.gz'),
-                                                   reverse_in=os.path.join(sample_tmp_dir, 'rmlst_R2.fastq.gz'),
-                                                   forward_out=os.path.join(sample_tmp_dir, 'trimmed_R1.fastq.gz'),
-                                                   reverse_out=os.path.join(sample_tmp_dir, 'trimmed_R2.fastq.gz'),
-                                                   threads=str(threads), returncmd=True)
+                out, err, cmd = bbtools.bbduk_bait(reference=sample_database,
+                                                   forward_in=pair[0],
+                                                   forward_out=unpaired_bait,
+                                                   returncmd=True, threads=threads)
             else:
-                out, err, cmd = bbtools.bbduk_trim(forward_in=os.path.join(sample_tmp_dir, 'rmlst_R1.fastq.gz'),
-                                                   reverse_in=os.path.join(sample_tmp_dir, 'rmlst_R2.fastq.gz'),
-                                                   forward_out=os.path.join(sample_tmp_dir, 'trimmed_R1.fastq.gz'),
-                                                   reverse_out=os.path.join(sample_tmp_dir, 'trimmed_R2.fastq.gz'),
+                out, err, cmd = bbtools.bbduk_bait(reference=sample_database,
+                                                   forward_in=pair[0],
+                                                   forward_out=unpaired_bait,
                                                    Xmx=xmx,
-                                                   threads=str(threads),
-                                                   returncmd=True)
+                                                   returncmd=True, threads=threads)
+    if out:
+        write_to_logfile(log, out, err, cmd)
+    logging.info('Quality trimming...')
+    out, err, cmd = '', '', ''
+    if data_type == 'Illumina':
+        if paired:
+            forward_trimmed = os.path.join(sample_tmp_dir, '{sn}_baited_trimmed_R1.fastq.gz'.format(sn=sample_name))
+            reverse_trimmed = forward_trimmed.replace('_R1', '_R2')
+            if not os.path.isfile(forward_trimmed):
+                if xmx is None:
+                    out, err, cmd = bbtools.bbduk_trim(forward_in=forward_bait,
+                                                       reverse_in=reverse_bait,
+                                                       forward_out=forward_trimmed,
+                                                       reverse_out=reverse_trimmed,
+                                                       threads=str(threads), returncmd=True)
+                else:
+                    out, err, cmd = bbtools.bbduk_trim(forward_in=forward_bait,
+                                                       reverse_in=reverse_bait,
+                                                       forward_out=forward_trimmed,
+                                                       reverse_out=reverse_trimmed,
+                                                       Xmx=xmx,
+                                                       threads=str(threads),
+                                                       returncmd=True)
+
+            with gzip.open(forward_trimmed, 'rt') as gz:
+                fastq_records = load_fastq_records(gz=gz,
+                                                   paired=True,
+                                                   forward=True)
+            with gzip.open(reverse_trimmed, 'rt') as gz:
+                # fastq_records.update(SeqIO.to_dict(SeqIO.parse(gz, 'fastq')))
+                fastq_records.update(load_fastq_records(gz=gz,
+                                                        paired=True,
+                                                        forward=False))
 
         else:
+            unpaired_trimmed = os.path.join(sample_tmp_dir, '{sn}_baited_trimmed.fastq.gz'.format(sn=sample_name))
+
             if not fasta:
-                if xmx is None:
-                    out, err, cmd = bbtools.bbduk_trim(forward_in=os.path.join(sample_tmp_dir, 'rmlst.fastq.gz'),
-                                                       forward_out=os.path.join(sample_tmp_dir, 'trimmed.fastq.gz'),
-                                                       returncmd=True,
-                                                       threads=threads)
-                else:
-                    out, err, cmd = bbtools.bbduk_trim(forward_in=os.path.join(sample_tmp_dir, 'rmlst.fastq.gz'),
-                                                       forward_out=os.path.join(sample_tmp_dir, 'trimmed.fastq.gz'),
-                                                       returncmd=True,
-                                                       threads=threads,
-                                                       Xmx=xmx)
+                if not os.path.isfile(unpaired_trimmed):
+                    if xmx is None:
+                        out, err, cmd = bbtools.bbduk_trim(forward_in=unpaired_bait,
+                                                           forward_out=unpaired_trimmed,
+                                                           returncmd=True,
+                                                           threads=threads)
+                    else:
+                        out, err, cmd = bbtools.bbduk_trim(forward_in=unpaired_bait,
+                                                           forward_out=unpaired_trimmed,
+                                                           returncmd=True,
+                                                           threads=threads,
+                                                           Xmx=xmx)
+                with gzip.open(unpaired_trimmed, 'rt') as gz:
+                    # fastq_records = SeqIO.to_dict(SeqIO.parse(gz, 'fastq'))
+                    fastq_records = load_fastq_records(gz=gz,
+                                                       paired=False,
+                                                       forward=True)
+            else:
+                # '''unpaired_bait'''
+                with gzip.open(unpaired_bait, 'rt') as gz:
+                    # fastq_records = SeqIO.to_dict(SeqIO.parse(gz, 'fastq'))
+                    fastq_records = load_fastq_records(gz=gz,
+                                                       paired=False,
+                                                       forward=True)
         write_to_logfile(log, out, err, cmd)
-
+    else:
+        if paired:
+            with gzip.open(forward_bait, 'rt') as gz:
+                # fastq_records = SeqIO.to_dict(SeqIO.parse(gz, 'fastq'))
+                fastq_records = load_fastq_records(gz=gz,
+                                                   paired=True,
+                                                   forward=True)
+            with gzip.open(reverse_bait, 'rt') as gz:
+                # fastq_records.update(SeqIO.to_dict(SeqIO.parse(gz, 'fastq')))
+                fastq_records.update(load_fastq_records(gz=gz,
+                                                        paired=True,
+                                                        forward=False))
+        else:
+            with gzip.open(unpaired_bait, 'rt') as gz:
+                # fastq_records = SeqIO.to_dict(SeqIO.parse(gz, 'fastq'))
+                fastq_records = load_fastq_records(gz=gz,
+                                                   paired=False,
+                                                   forward=True)
     logging.info('Detecting contamination...')
     # Now do mapping in two steps - first, map reads back to database with ambiguous reads matching all - this
     # will be used to get a count of number of reads aligned to each gene/allele so we can create a custom rmlst file
     # with only the most likely allele for each gene.
-    if not os.path.isfile(sample_database + '.fai'):  # Don't bother re-indexing, this only needs to happen once.
-        pysam.faidx(sample_database)
+    kma_report = os.path.join(sample_tmp_dir, '{sn}_kma'.format(sn=sample_name))
+    # if not os.path.isfile(sample_database + '.fai'):  # Don't bother re-indexing, this only needs to happen once.
+    #     pysam.faidx(sample_database)
     kma_database = sample_database.replace('.fasta', '') + '_kma'
-    kma_report = os.path.join(sample_tmp_dir, 'kma_rmlst')
-    if not os.path.isfile(kma_database + '.name'):  # The .name is one of the files KMA creates when making a database.
-        logging.info('Since this is the first time you are using this database, it needs to be indexed by KMA. '
-                     'This might take a while')
-        cmd = 'kma index -i {} -o {}'.format(sample_database, kma_database)  # NOTE: Need KMA >=1.2.0 for this to work.
-        out, err = run_cmd(cmd)
-        write_to_logfile(log, out, err, cmd)
-
+    #
+    # if not os.path.isfile(kma_database + '.name'):  # The .name is one of the files KMA creates when making a database
+    #     logging.info('Since this is the first time you are using this database, it needs to be indexed by KMA. '
+    #                  'This might take a while')
+    #     cmd = 'kma index -i {} -o {}'.format(sample_database, kma_database)  # NOTE: Need KMA >=1.2.0 for this to work
+    #     out, err = run_cmd(cmd)
+    #     write_to_logfile(log, out, err, cmd)
+    index_databases(sample_database=sample_database)
     # Run KMA.
     if paired:
-        cmd = 'kma -ipe {forward_in} {reverse_in} -t_db {kma_database} -o {kma_report} ' \
-              '-t {threads}'.format(forward_in=os.path.join(sample_tmp_dir, 'trimmed_R1.fastq.gz'),
-                                    reverse_in=os.path.join(sample_tmp_dir, 'trimmed_R2.fastq.gz'),
-                                    kma_database=kma_database,
-                                    kma_report=kma_report,
-                                    threads=threads)
-        out, err = run_cmd(cmd)
-        write_to_logfile(log, out, err, cmd)
+        if not os.path.isfile(kma_report + '.res'):
+            cmd = 'kma -ipe {forward_in} {reverse_in} -t_db {kma_database} -o {kma_report} ' \
+                  '-t {threads}'.format(forward_in=forward_trimmed,
+                                        reverse_in=reverse_trimmed,
+                                        kma_database=kma_database,
+                                        kma_report=kma_report,
+                                        threads=threads)
+            out, err = run_cmd(cmd)
+            write_to_logfile(log, out, err, cmd)
     else:
-        if data_type == 'Illumina':
-            # Use the FASTA file (rather than the readsd) as the input
-            if fasta:
-                cmd = 'kma -i {input_reads} -t_db {kma_database} -mem_mode -ID 100 -ConClave 2 -ex_mode ' \
-                      '-o {kma_report} -t {threads}'\
-                    .format(input_reads=pair[0],
-                            kma_database=kma_database,
-                            kma_report=kma_report,
-                            threads=threads)
+        if not os.path.isfile(kma_report + '.res'):
+            if data_type == 'Illumina':
+                # Use the FASTA file (rather than the reads) as the input
+                if fasta:
+                    cmd = 'kma -i {input_reads} -t_db {kma_database} -mem_mode -ID 100 -ConClave 2 -ex_mode ' \
+                          '-o {kma_report} -t {threads}' \
+                        .format(input_reads=pair[0],
+                                kma_database=kma_database,
+                                kma_report=kma_report,
+                                threads=threads)
+                else:
+                    cmd = 'kma -i {input_reads} -t_db {kma_database} -o {kma_report} ' \
+                          '-t {threads}'.format(input_reads=unpaired_trimmed,
+                                                kma_database=kma_database,
+                                                kma_report=kma_report,
+                                                threads=threads)
             else:
-                cmd = 'kma -i {input_reads} -t_db {kma_database} -o {kma_report} ' \
-                      '-t {threads}'.format(input_reads=os.path.join(sample_tmp_dir, 'trimmed.fastq.gz'),
+                # Recommended Nanopore settings from KMA repo: https://bitbucket.org/genomicepidemiology/kma
+                cmd = 'kma -i {input_reads} -t_db {kma_database} -o {kma_report} -mem_mode -mp 20 -mrs 0.0 -bcNano ' \
+                      '-t {threads}'.format(input_reads=unpaired_bait,
                                             kma_database=kma_database,
                                             kma_report=kma_report,
                                             threads=threads)
-        else:
-            # Recommended Nanopore settings from KMA repo: https://bitbucket.org/genomicepidemiology/kma
-            cmd = 'kma -i {input_reads} -t_db {kma_database} -o {kma_report} -mem_mode -mp 20 -mrs 0.0 -bcNano ' \
-                  '-t {threads}'.format(input_reads=os.path.join(sample_tmp_dir, 'trimmed.fastq.gz'),
-                                        kma_database=kma_database,
-                                        kma_report=kma_report,
-                                        threads=threads)
-        out, err = run_cmd(cmd)
-        write_to_logfile(log, out, err, cmd)
+            out, err = run_cmd(cmd)
+            write_to_logfile(log, out, err, cmd)
 
-    rmlst_report = os.path.join(output_folder, sample_name + '_rmlst.csv')
+    rmlst_report = os.path.join(output_folder, sample_name + '_alleles.csv')
     gene_alleles = find_rmlst_type(kma_report=kma_report + '.res',
                                    rmlst_report=rmlst_report)
 
-    with open(os.path.join(sample_tmp_dir, 'rmlst.fasta'), 'w') as f:
-        for contig in SeqIO.parse(sample_database, 'fasta'):
-            if contig.id in gene_alleles:
-                f.write('>{}\n'.format(contig.id))
-                f.write(str(contig.seq) + '\n')
-
-    rmlst_gene_length = find_total_sequence_length(os.path.join(sample_tmp_dir, 'rmlst.fasta'))
+    rmlst_fasta = os.path.join(sample_tmp_dir, '{sn}_alleles.fasta'.format(sn=sample_name))
+    if not os.path.isfile(rmlst_fasta):
+        with open(rmlst_fasta, 'w') as f:
+            for contig in SeqIO.parse(sample_database, 'fasta'):
+                if contig.id in gene_alleles:
+                    SeqIO.write(contig, f, 'fasta')
+                    # f.write('>{}\n'.format(contig.id))
+                    # f.write(str(contig.seq) + '\n')
+    rmlst_gene_length = find_total_sequence_length(rmlst_fasta)
     logging.debug('Total gene length is {}'.format(rmlst_gene_length))
     pysam_pass = True
     # Second step of mapping - Do a mapping of our baited reads against a fasta file that has only one allele per
     # rMLST gene.
     try:
-        pysam.faidx(os.path.join(sample_tmp_dir, 'rmlst.fasta'))
-        if paired:
-            cmd = 'bbmap.sh ref={ref} in={forward_in} in2={reverse_in} out={outbam} threads={threads} mdtag ' \
-                  'nodisk'.format(ref=os.path.join(sample_tmp_dir, 'rmlst.fasta'),
-                                  forward_in=os.path.join(sample_tmp_dir, 'trimmed_R1.fastq.gz'),
-                                  reverse_in=os.path.join(sample_tmp_dir, 'trimmed_R2.fastq.gz'),
-                                  outbam=os.path.join(sample_tmp_dir, 'out_2.bam'),
-                                  threads=threads)
-            if cgmlst_db is not None:
-                # Lots of core genes seem to have relatives within a genome that are at ~70 percent identity. This means
-                # that reads that shouldn't map do, and cause false positives. Adding in this sub-filter means that
-                # reads can only have one mismatch, so they actually have to be from the right gene for this to work.
-                cmd += ' subfilter=1'
-            if xmx:
-                cmd += ' -Xmx{}'.format(xmx)
-            out, err = run_cmd(cmd)
-            write_to_logfile(log, out, err, cmd)
-        else:
-            #
-            if data_type == 'Illumina' and not fasta:
-                cmd = 'bbmap.sh ref={ref} in={forward_in} out={outbam} threads={threads} mdtag ' \
-                      'nodisk'.format(ref=os.path.join(sample_tmp_dir, 'rmlst.fasta'),
-                                      forward_in=os.path.join(sample_tmp_dir, 'trimmed.fastq.gz'),
-                                      outbam=os.path.join(sample_tmp_dir, 'out_2.bam'),
+        if not os.path.isfile(rmlst_fasta + '.fai'):
+            pysam.faidx(rmlst_fasta)
+        outbam = os.path.join(sample_tmp_dir, '{sn}_contamination.bam'.format(sn=sample_name))
+        sorted_bam = os.path.join(sample_tmp_dir, '{sn}_contamination_sorted.bam'.format(sn=sample_name))
+        outsam = outbam.replace('.bam', '.sam')
+        if not os.path.isfile(sorted_bam):
+            if paired:
+                cmd = 'bbmap.sh ref={ref} in={forward_in} in2={reverse_in} out={outbam} threads={threads} mdtag ' \
+                      'nodisk'.format(ref=rmlst_fasta,
+                                      forward_in=forward_trimmed,
+                                      reverse_in=reverse_trimmed,
+                                      outbam=outbam,
                                       threads=threads)
                 if cgmlst_db is not None:
-                    # Core genes can have relatives within a genome that are at ~70 percent identity. This means
+                    # Lots of core genes seem to have relatives within a genome that are at ~70% identity. This means
                     # that reads that shouldn't map do, and cause false positives. Adding in this sub-filter means that
                     # reads can only have one mismatch, so they have to be from the right gene for this to work.
                     cmd += ' subfilter=1'
                 if xmx:
                     cmd += ' -Xmx{}'.format(xmx)
                 out, err = run_cmd(cmd)
                 write_to_logfile(log, out, err, cmd)
             else:
-                cmd = 'minimap2 --MD -t {threads} -ax map-ont {ref} {reads} ' \
-                      '> {outsam}'.format(ref=os.path.join(sample_tmp_dir, 'rmlst.fasta'),
-                                          reads=os.path.join(sample_tmp_dir, 'trimmed.fastq.gz'),
-                                          outsam=os.path.join(sample_tmp_dir, 'out_2.sam'),
+                #
+                if data_type == 'Illumina' and not fasta:
+                    cmd = 'bbmap.sh ref={ref} in={forward_in} out={outbam} threads={threads} mdtag ' \
+                          'nodisk'.format(ref=rmlst_fasta,
+                                          forward_in=unpaired_trimmed,
+                                          outbam=outbam,
                                           threads=threads)
-                out, err = run_cmd(cmd)
-                write_to_logfile(log, out, err, cmd)
-                outbam = os.path.join(sample_tmp_dir, 'out_2.bam')
-                # Apparently have to perform equivalent of a touch on this file for this to work.
-                fh = open(outbam, 'w')
-                fh.close()
-                pysam.view('-b', '-o', outbam, os.path.join(sample_tmp_dir, 'out_2.sam'), save_stdout=outbam)
-        pysam.sort('-o', os.path.join(sample_tmp_dir, 'contamination.bam'), os.path.join(sample_tmp_dir, 'out_2.bam'))
-        pysam.index(os.path.join(sample_tmp_dir, 'contamination.bam'))
+                    if cgmlst_db is not None:
+                        # Core genes can have relatives within a genome that are at ~70 percent identity. This means
+                        # that reads that shouldn't map do, and cause false positives. Adding in this sub-filter means
+                        # reads can only have one mismatch, so they have to be from the right gene for this to work.
+                        cmd += ' subfilter=1'
+                    if xmx:
+                        cmd += ' -Xmx{}'.format(xmx)
+                    out, err = run_cmd(cmd)
+                    write_to_logfile(log, out, err, cmd)
+                else:
+                    if fasta:
+                        ax = 'asm5'
+                        # ax = 'sr'
+                    # If Nanopore FASTQ:
+                    else:
+                        ax = 'map-ont'
+                    # '> {outsam}'
+                    cmd = 'minimap2 --MD -t {threads} -ax {ax} {ref} {reads}' \
+                        .format(ax=ax,
+                                ref=rmlst_fasta,
+                                reads=unpaired_bait,
+                                outsam=outsam,
+                                threads=threads)
+                    # ' | samtools rmdup - -S -' \
+                    cmd += ' | samtools view -@ {threads} -h -bT {abs_ref_link} -' \
+                           ' | samtools sort - -@ {threads} -o {sorted_bam}' \
+                        .format(threads=threads,
+                                abs_ref_link=rmlst_fasta,
+                                sorted_bam=sorted_bam)
+                    out, err = run_cmd(cmd)
+                    write_to_logfile(log, out, err, cmd)
+
+        if not os.path.isfile(sorted_bam):
+            # noinspection PyUnresolvedReferences
+            pysam.sort('-o', sorted_bam, outbam)
+        if not os.path.isfile(sorted_bam + '.bai'):
+            pysam.index(sorted_bam)
         # Now find number of multi-positions for each rMLST gene/allele combination
         multi_positions = 0
 
         # Run the BAM parsing in parallel! Some refactoring of the code would likely be a good idea so this
         # isn't quite so ugly, but it works.
         p = multiprocessing.Pool(processes=threads)
-        bamfile_list = [os.path.join(sample_tmp_dir, 'contamination.bam')] * len(gene_alleles)
-        # bamfile_list = [os.path.join(sample_tmp_dir, 'rmlst.bam')] * len(gene_alleles)
-        reference_fasta_list = [os.path.join(sample_tmp_dir, 'rmlst.fasta')] * len(gene_alleles)
+        nanopore = True if data_type == 'Nanopore' else False
+        nanopore_list = [nanopore] * len(gene_alleles)
+        allele_records = SeqIO.to_dict(SeqIO.parse(rmlst_fasta, 'fasta'))
+        bamfile_list = [sorted_bam] * len(gene_alleles)
+        reference_fasta_list = [rmlst_fasta] * len(gene_alleles)
         fasta_list = [fasta] * len(gene_alleles)
         quality_cutoff_list = [quality_cutoff] * len(gene_alleles)
         base_cutoff_list = [base_cutoff] * len(gene_alleles)
         base_fraction_list = [base_fraction_cutoff] * len(gene_alleles)
+        records_list = [allele_records] * len(gene_alleles)
+        fastq_records_list = [fastq_records] * len(gene_alleles)
+        error_cutoff_list = [error_cutoff] * len(gene_alleles)
         multibase_dict_list = list()
         report_write_list = list()
-        for multibase_dict, report_write in p.starmap(read_contig, zip(gene_alleles, bamfile_list, reference_fasta_list,
-                                                                       quality_cutoff_list, base_cutoff_list,
-                                                                       base_fraction_list, fasta_list), chunksize=1):
-            multibase_dict_list.append(multibase_dict)
-            report_write_list.append(report_write)
-        p.close()
-        p.join()
+        if debug == 'debug':
+            for i, gene in enumerate(gene_alleles):
+                multibase_dict, report_write = read_contig(
+                    contig_name=gene,
+                    bamfile_name=bamfile_list[i],
+                    reference_fasta=reference_fasta_list[i],
+                    allele_records=records_list[i],
+                    fastq_records=fastq_records_list[i],
+                    quality_cutoff=quality_cutoff_list[i],
+                    base_cutoff=base_cutoff_list[i],
+                    base_fraction_cutoff=base_fraction_list[i],
+                    fasta=fasta_list[i],
+                    nanopore = nanopore_list[i],
+                    error_cutoff=error_cutoff_list[i])
+                multibase_dict_list.append(multibase_dict)
+                report_write_list.append(report_write)
+        else:
+            for multibase_dict, report_write in p.starmap(read_contig,
+                                                          zip(gene_alleles,
+                                                              bamfile_list,
+                                                              reference_fasta_list,
+                                                              records_list,
+                                                              fastq_records_list,
+                                                              quality_cutoff_list,
+                                                              base_cutoff_list,
+                                                              base_fraction_list,
+                                                              fasta_list,
+                                                              error_cutoff_list,
+                                                              nanopore_list),
+                                                          chunksize=1):
+                multibase_dict_list.append(multibase_dict)
+                report_write_list.append(report_write)
+            p.close()
+            p.join()
     except SamtoolsError:
         pysam_pass = False
         multi_positions = 0
         multibase_dict_list = list()
         report_write_list = list()
     # Write out report info.
     report_file = os.path.join(output_folder, sample_name + '_contamination.csv')
     with open(report_file, 'w') as r:
-        r.write('{reference},{position},{bases},{coverage}\n'.format(reference='Gene',
-                                                                     position='Position',
-                                                                     bases='Bases',
-                                                                     coverage='Coverage'))
+        r.write('Gene,Position,RefBase,CongruentSNVs,TotalSNVs,ForwardSNVs,ReverseSNVs,SNVCoverage,TotalCoverage,'
+                'BaseCutoff,ErrorPercent\n')
         for item in report_write_list:
             for contamination_info in item:
                 r.write(contamination_info)
-
     # Total up the number of multibase positions.
     for multibase_position_dict in multibase_dict_list:
         multi_positions += sum([len(snp_positions) for snp_positions in multibase_position_dict.values()])
     if cgmlst_db is None:
-        snp_cutoff = int(rmlst_gene_length/10000) + 1
+        snp_cutoff = math.ceil(rmlst_gene_length / 10000) + 1
     elif fasta:
         snp_cutoff = 1
     else:
         snp_cutoff = 10
-    if multi_positions >= snp_cutoff:
-        percent_contam, contam_stddev = estimate_percent_contamination(contamination_report_file=report_file)
-    else:
-        percent_contam = 0
-        contam_stddev = 0
+
     logging.info('Done! Number of contaminating SNVs found: {}\n'.format(multi_positions))
     write_output(output_report=os.path.join(output_folder, 'confindr_report.csv'),
                  sample_name=sample_name,
                  multi_positions=multi_positions,
                  genus=genus,
-                 percent_contam=percent_contam,
-                 contam_stddev=contam_stddev,
                  total_gene_length=rmlst_gene_length,
                  snp_cutoff=snp_cutoff,
                  database_download_date=database_download_date,
                  pysam_pass=pysam_pass)
     if keep_files is False:
         shutil.rmtree(sample_tmp_dir)
 
 
-def write_output(output_report, sample_name, multi_positions, genus, percent_contam, contam_stddev, total_gene_length,
+def write_output(output_report, sample_name, multi_positions, genus, total_gene_length,
                  database_download_date, snp_cutoff=3, pysam_pass=True):
     """
     Function that writes the output generated by ConFindr to a report file. Appends to a file that already exists,
     or creates the file if it doesn't already exist.
-    :param output_report: Path to CSV output report file. Should have headers SampleName,Genus,NumContamSNVs,
-    ContamStatus,PercentContam, and PercentContamStandardDeviation, in that order.
+    :param output_report: Path to CSV output report file. Should have headers SampleName,Genus,NumContamSNVs, and
+    ContamStatus, in that order.
     :param sample_name: string - name of sample
     :param multi_positions: integer - number of positions that were found to have more than one base present.
     :param genus: string - The genus of your sample
-    :param percent_contam: float - Estimated percentage contamination
-    :param contam_stddev: float - Standard deviation of percentage contamination
     :param total_gene_length: integer - number of bases examined to make a contamination call.
     :param database_download_date:
     :param snp_cutoff: Number of cSNVs to use to call a sample contaminated. Default 3. (INT)
     :param pysam_pass: Boolean of whether pysam encountered an error
     """
     # If the report file hasn't been created, make it, with appropriate header.
     if not os.path.isfile(output_report):
         with open(os.path.join(output_report), 'w') as f:
-            f.write('Sample,Genus,NumContamSNVs,ContamStatus,PercentContam,PercentContamStandardDeviation,'
+            f.write('Sample,Genus,NumContamSNVs,ContamStatus,'
                     'BasesExamined,DatabaseDownloadDate\n')
     if pysam_pass:
         if multi_positions >= snp_cutoff or len(genus.split(':')) > 1:
             contaminated = True
         else:
             contaminated = False
     else:
         contaminated = 'Pysam SamtoolsError'
         multi_positions = 'ND'
-        percent_contam = 'ND'
-        contam_stddev = 'ND'
     with open(output_report, 'a+') as f:
-        f.write('{samplename},{genus},{numcontamsnvs},'
-                '{contamstatus},{percent_contam},{contam_stddev},'
+        f.write('{samplename},{genus},{numcontamsnvs},{contamstatus},'
                 '{gene_length},{database_download_date}\n'.format(samplename=sample_name,
                                                                   genus=genus,
                                                                   numcontamsnvs=multi_positions,
                                                                   contamstatus=contaminated,
-                                                                  percent_contam=percent_contam,
-                                                                  contam_stddev=contam_stddev,
                                                                   gene_length=total_gene_length,
                                                                   database_download_date=database_download_date))
 
 
 def check_for_databases_and_download(database_location):
     # Check for the files necessary - should have rMLST_combined.fasta, gene_allele.txt, profiles.txt, and refseq.msh
     necessary_files = ['Escherichia_db_cgderived.fasta', 'Listeria_db_cgderived.fasta',
@@ -970,249 +1651,13 @@
         logging.error('ERROR: Xmx strings must be integers, floating point numbers are not accepted.')
     if not str.isdigit(xmx_string[:-1]):
         acceptable_xmx = False
         logging.error('ERROR: The amount of memory requested was not an integer.')
     return acceptable_xmx
 
 
-def confindr(args):
-    # Check for dependencies.
-    all_dependencies_present = True
-    # Re-enable minimap2 as dependency once nanopore stuff actually works.
-    if args.data_type == 'Illumina':
-        dependencies = ['bbmap.sh', 'bbduk.sh', 'mash', 'kma']
-    else:
-        dependencies = ['bbduk.sh', 'mash', 'minimap2', 'kma']
-
-    for dependency in dependencies:
-        if dependency_check(dependency) is False:
-            logging.error('Dependency {} not found. Please make sure it is installed and present'
-                          ' on your $PATH.'.format(dependency))
-            all_dependencies_present = False
-    if not all_dependencies_present:
-        logging.error('Could not find all necessary dependencies, quitting...')
-        quit(code=1)
-
-    # Check that the base fraction specified actually makes sense.
-    if check_valid_base_fraction(args.base_fraction_cutoff) is False:
-        logging.error('Base fraction must be between 0 and 1 if specified. Input value was: {}'
-                      .format(args.base_fraction_cutoff))
-        quit(code=1)
-
-    # If user specified Xmx, make sure that they actually entered a value that will work. If not, the method will tell
-    # them what they did wrong. Then quit.
-    if args.Xmx:
-        valid_xmx = check_acceptable_xmx(args.Xmx)
-        if valid_xmx is False:
-            quit(code=1)
-
-    # Don't yet have cgmlst support with Nanopore reads - don't let user do this.
-    if args.cgmlst and args.data_type == 'Nanopore':
-        logging.error('ERROR: cgMLST schemes not yet supported for Nanopore reads. Quitting...')
-        quit(code=1)
-
-    if args.data_type == 'Nanopore':
-        logging.warning('WARNING: Nanopore contamination detection is highly experimental. Any results should be taken '
-                        'with several very large grains of salt. If you are going to try this, try setting -q to '
-                        'somewhere in the range of 12-15, and only count things as contaminated that have at least '
-                        '10 contaminating SNVs. Even then, results may be wonky. In particular, samples with lots of '
-                        'depth will probably always show up as contaminated.')
-
-    # Make the output directory.
-    if not os.path.isdir(args.output_name):
-        os.makedirs(args.output_name)
-    # Remove any reports created by previous iterations of ConFindr
-    try:
-        os.remove(os.path.join(args.output_name, 'confindr_report.csv'))
-    except FileNotFoundError:
-        pass
-    # Set the minimum number of matching hashes
-    min_matching_hashes = args.min_matching_hashes
-    # Check if databases necessary to run are present, and download them if they aren't
-    check_for_databases_and_download(database_location=args.databases)
-
-    # Figure out what pairs of reads, as well as unpaired reads, are present.
-    paired_reads = find_paired_reads(args.input_directory,
-                                     forward_id=args.forward_id,
-                                     reverse_id=args.reverse_id)
-    unpaired_reads = find_unpaired_reads(args.input_directory,
-                                         forward_id=args.forward_id,
-                                         reverse_id=args.reverse_id,
-                                         find_fasta=args.fasta)
-    # Consolidate read lists
-    reads = sorted(paired_reads + unpaired_reads)
-    # Process paired reads, one sample at a time.
-    for fastq in reads:
-        if len(fastq) == 1:
-            sample_name = os.path.split(fastq[0])[-1].split('.')[0]
-        else:
-            sample_name = os.path.split(fastq[0])[-1].split(args.forward_id)[0]
-        logging.info('Beginning analysis of sample {}...'.format(sample_name))
-        try:
-            find_contamination(pair=fastq,
-                               forward_id=args.forward_id,
-                               threads=args.threads,
-                               output_folder=args.output_name,
-                               databases_folder=args.databases,
-                               keep_files=args.keep_files,
-                               quality_cutoff=args.quality_cutoff,
-                               base_cutoff=args.base_cutoff,
-                               base_fraction_cutoff=args.base_fraction_cutoff,
-                               cgmlst_db=args.cgmlst,
-                               xmx=args.Xmx,
-                               tmpdir=args.tmp,
-                               data_type=args.data_type,
-                               use_rmlst=args.rmlst,
-                               cross_details=args.cross_details,
-                               min_matching_hashes=min_matching_hashes,
-                               fasta=args.fasta)
-        except subprocess.CalledProcessError:
-            # If something unforeseen goes wrong, traceback will be printed to screen.
-            # We then add the sample to the report with a note that it failed.
-            multi_positions = 0
-            genus = 'Error processing sample'
-            write_output(output_report=os.path.join(args.output_name, 'confindr_report.csv'),
-                         sample_name=sample_name,
-                         multi_positions=multi_positions,
-                         genus=genus,
-                         percent_contam='ND',
-                         contam_stddev='ND',
-                         total_gene_length=0,
-                         database_download_date='ND')
-            logging.warning('Encountered error when attempting to run ConFindr on sample '
-                            '{sample}. Skipping...'.format(sample=sample_name))
-            logging.warning('Error encounted was:\n{}'.format(traceback.format_exc()))
-            if args.keep_files is False:
-                shutil.rmtree(os.path.join(args.output_name, sample_name))
-    if args.keep_files is False and args.tmp is not None:
-        shutil.rmtree(args.tmp)
-    logging.info('Contamination detection complete!')
-
-
 def get_version():
     try:
         version = 'ConFindr {}'.format(pkg_resources.get_distribution('confindr').version)
     except pkg_resources.DistributionNotFound:
         version = 'ConFindr (Unknown version)'
     return version
-        
-
-def main():
-    version = get_version()
-    cpu_count = multiprocessing.cpu_count()
-    parser = argparse.ArgumentParser()
-    parser.add_argument('-i', '--input_directory',
-                        type=str,
-                        required=True,
-                        help='Folder that contains fastq files you want to check for contamination. '
-                             'Will find any file that contains .fq or .fastq in the filename.')
-    parser.add_argument('-o', '--output_name',
-                        type=str,
-                        required=True,
-                        help='Base name for output/temporary directories.')
-    parser.add_argument('-d', '--databases',
-                        type=str,
-                        default=os.environ.get('CONFINDR_DB', os.path.expanduser('~/.confindr_db')),
-                        help='Databases folder. To download these, you will need to get access to the rMLST databases. '
-                             'For complete instructions on how to do this, please see '
-                             'https://olc-bioinformatics.github.io/ConFindr/install/#downloading-confindr-databases')
-    parser.add_argument('--rmlst',
-                        default=False,
-                        action='store_true',
-                        help='Activate to prefer using rMLST databases over core-gene derived databases. By default,'
-                             'ConFindr will use core-gene derived databases where available.')
-    parser.add_argument('-t', '--threads',
-                        type=int,
-                        default=cpu_count,
-                        help='Number of threads to run analysis with.')
-    parser.add_argument('-tmp', '--tmp',
-                        type=str,
-                        help='If your ConFindr databases are in a location you don\'t have write access to, '
-                             'you can enter this option to specify a temporary directory to put genus-specific '
-                             'databases to.')
-    parser.add_argument('-k', '--keep_files',
-                        default=False,
-                        action='store_true',
-                        help='By default, intermediate files are deleted. Activate this flag to keep intermediate '
-                             'files.')
-    parser.add_argument('-q', '--quality_cutoff',
-                        type=int,
-                        default=20,
-                        help='Base quality needed to support a multiple allele call. Defaults to 20.')
-    parser.add_argument('-b', '--base_cutoff',
-                        type=int,
-                        default=2,
-                        help='Number of bases necessary to support a multiple allele call. Defaults to 2.')
-    parser.add_argument('-bf', '--base_fraction_cutoff',
-                        type=float,
-                        default=0.05,
-                        help='Fraction of bases necessary to support a multiple allele call. Particularly useful when '
-                             'dealing with very high coverage samples. Default is 0.05.')
-    parser.add_argument('-fid', '--forward_id',
-                        type=str,
-                        default='_R1',
-                        help='Identifier for forward reads.')
-    parser.add_argument('-rid', '--reverse_id',
-                        type=str,
-                        default='_R2',
-                        help='Identifier for reverse reads.')
-    parser.add_argument('-v', '--version',
-                        action='version',
-                        version=version)
-    parser.add_argument('-dt', '--data_type',
-                        choices=['Illumina', 'Nanopore'],
-                        default='Illumina',
-                        help='Type of input data. Default is Illumina, but can be used for Nanopore too. No PacBio '
-                             'support (yet).')
-    parser.add_argument('-Xmx', '--Xmx',
-                        type=str,
-                        help='Very occasionally, parts of the pipeline that use the BBMap suite will have their memory '
-                             'reservation fail and request not enough, or sometimes negative, memory. If this happens '
-                             'to you, you can use this flag to override automatic memory reservation and use an amount '
-                             'of memory requested by you. -Xmx 20g will specify 20 gigs of RAM, and -Xmx 800m '
-                             'will specify 800 megs.')
-    parser.add_argument('-cgmlst', '--cgmlst',
-                        type=str,
-                        help='Path to a cgMLST database to use for contamination detection instead of using the default'
-                             ' rMLST database. Sequences in this file should have headers in format '
-                             '>genename_allelenumber. To speed up ConFindr runs, clustering the cgMLST database with '
-                             'CD-HIT before running ConFindr is recommended. This is highly experimental, results '
-                             'should be interpreted with great care.')
-    parser.add_argument('--fasta',
-                        default=False,
-                        action='store_true',
-                        help='If activated, will look for FASTA files instead of FASTQ for unpaired reads.')
-    parser.add_argument('-verbosity', '--verbosity',
-                        choices=['debug', 'info', 'warning'],
-                        default='info',
-                        help='Amount of output you want printed to the screen. Defaults to info, which should be good '
-                             'for most users.')
-    parser.add_argument('-cross_details', '--cross_details',
-                        action='store_true',
-                        help='Continue ConFindr analyses on samples with two or more genera identified. Default is '
-                             'False')
-    parser.add_argument('-m', '--min_matching_hashes',
-                        default=150,
-                        type=int,
-                        help='Minimum number of matching hashes in a MASH screen in order for a genus to be considered '
-                             'present in a sample. Default is 150')
-    args = parser.parse_args()
-    # Setup the logger. TODO: Different colors for different levels.
-    if args.verbosity == 'info':
-        logging.basicConfig(format='\033[92m \033[1m %(asctime)s \033[0m %(message)s ',
-                            level=logging.INFO,
-                            datefmt='%Y-%m-%d %H:%M:%S')
-    elif args.verbosity == 'debug':
-        logging.basicConfig(format='\033[92m \033[1m %(asctime)s \033[0m %(message)s ',
-                            level=logging.DEBUG,
-                            datefmt='%Y-%m-%d %H:%M:%S')
-    elif args.verbosity == 'warning':
-        logging.basicConfig(format='\033[92m \033[1m %(asctime)s \033[0m %(message)s ',
-                            level=logging.WARNING,
-                            datefmt='%Y-%m-%d %H:%M:%S')
-
-    logging.info('Welcome to {version}! Beginning analysis of your samples...'.format(version=version))
-    confindr(args)
-    
-
-if __name__ == '__main__':
-    main()
```

### Comparing `confindr-0.7.4/confindr_src/wrappers/bbtools.py` & `confindr-0.8.1/confindr_src/wrappers/bbtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,31 +79,31 @@
         reverse_in = forward_in.replace('_R1', '_R2')
         if reverse_out == 'NA':
             if '_R1' in forward_out:
                 reverse_out = forward_out.replace('_R1', '_R2')
             else:
                 raise ValueError('If you do not specify reverse_out, forward_out must contain R1.\n\n')
         cmd = 'bbduk.sh in1={f_in} in2={r_in} out1={f_out} out2={r_out} qtrim=w trimq=20 k=25 minlength=50 ' \
-              'forcetrimleft=15 ref=adapters overwrite hdist=1 tpe tbo{optn}'\
+              'forcetrimleft=15 ref=adapters overwrite hdist=1 qin=33 tpe tbo{optn}'\
             .format(f_in=forward_in,
                     r_in=reverse_in,
                     f_out=forward_out,
                     r_out=reverse_out,
                     optn=options)
     elif reverse_in == 'NA':
         cmd = 'bbduk.sh in={f_in} out={f_out} qtrim=w trimq=20 k=25 minlength=50 forcetrimleft=15' \
-              ' ref=adapters overwrite hdist=1 tpe tbo{optn}'\
+              ' ref=adapters overwrite hdist=1 qin=33 tpe tbo{optn}'\
             .format(f_in=forward_in,
                     f_out=forward_out,
                     optn=options)
     else:
         if reverse_out == 'NA':
             raise ValueError('Reverse output reads must be specified.')
         cmd = 'bbduk.sh in1={f_in} in2={r_in} out1={f_out} out2={r_out} qtrim=w trimq=20 k=25 minlength=50 ' \
-              'forcetrimleft=15 ref=adapters overwrite hdist=1 tpe tbo{optn}'\
+              'forcetrimleft=15 ref=adapters overwrite hdist=1 qin=33 tpe tbo{optn}'\
             .format(f_in=forward_in,
                     r_in=reverse_in,
                     f_out=forward_out,
                     r_out=reverse_out,
                     optn=options)
     out, err = run_subprocess(cmd)
     if returncmd:
@@ -240,23 +240,23 @@
     if os.path.isfile(forward_in.replace('_R1', '_R2')) and reverse_in == 'NA' and '_R1' in forward_in:
         reverse_in = forward_in.replace('_R1', '_R2')
         if reverse_out == 'NA':
             if '_R1' in forward_out:
                 reverse_out = forward_out.replace('_R1', '_R2')
             else:
                 raise ValueError('If you do not specify reverse_out, forward_out must contain _R1.\n\n')
-        cmd = 'bbduk.sh in={} in2={} outm={} outm2={} ref={}{}'.format(forward_in, reverse_in,
+        cmd = 'bbduk.sh qin=33 in={} in2={} outm={} outm2={} ref={}{}'.format(forward_in, reverse_in,
                                                                        forward_out, reverse_out,
                                                                        reference, options)
     elif reverse_in == 'NA':
-        cmd = 'bbduk.sh in={} outm={} ref={}{}'.format(forward_in, forward_out, reference, options)
+        cmd = 'bbduk.sh qin=33 in={} outm={} ref={}{}'.format(forward_in, forward_out, reference, options)
     else:
         if reverse_out == 'NA':
             raise ValueError('Reverse output reads must be specified.')
-        cmd = 'bbduk.sh in={} in2={} outm={} outm2={} ref={}{}'.format(forward_in, reverse_in,
+        cmd = 'bbduk.sh qin=33 in={} in2={} outm={} outm2={} ref={}{}'.format(forward_in, reverse_in,
                                                                        forward_out, reverse_out,
                                                                        reference, options)
     out, err = run_subprocess(cmd)
     if returncmd:
         return out, err, cmd
     else:
         return out, err
@@ -278,23 +278,23 @@
     if os.path.isfile(forward_in.replace('_R1', '_R2')) and reverse_in == 'NA' and '_R1' in forward_in:
         reverse_in = forward_in.replace('_R1', '_R2')
         if reverse_out == 'NA':
             if '_R1' in forward_out:
                 reverse_out = forward_out.replace('_R1', '_R2')
             else:
                 raise ValueError('If you do not specify reverse_out, forward_out must contain _R1.\n\n')
-        cmd = 'bbduk.sh in={} in2={} out={} out2={} ref={}{}'.format(forward_in, reverse_in,
+        cmd = 'bbduk.sh qin=33 in={} in2={} out={} out2={} ref={}{}'.format(forward_in, reverse_in,
                                                                      forward_out, reverse_out,
                                                                      reference, options)
     elif reverse_in == 'NA':
-        cmd = 'bbduk.sh in={} out={} ref={}{}'.format(forward_in, forward_out, reference, options)
+        cmd = 'bbduk.sh qin=33 in={} out={} ref={}{}'.format(forward_in, forward_out, reference, options)
     else:
         if reverse_out == 'NA':
             raise ValueError('Reverse output reads must be specified.')
-        cmd = 'bbduk.sh in={} in2={} out={} out2={} ref={}{}'.format(forward_in, reverse_in,
+        cmd = 'bbduk.sh qin=33 in={} in2={} out={} out2={} ref={}{}'.format(forward_in, reverse_in,
                                                                      forward_out, reverse_out,
                                                                      reference, options)
     out, err = run_subprocess(cmd)
     if returncmd:
         return out, err, cmd
     else:
         return out, err
```

### Comparing `confindr-0.7.4/confindr_src/wrappers/mash.py` & `confindr-0.8.1/confindr_src/wrappers/mash.py`

 * *Files identical despite different names*

### Comparing `confindr-0.7.4/confindr_src/database_setup.py` & `confindr-0.8.1/confindr_src/database_setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 #!/usr/bin/env python
-
+from confindr_src.methods import download_cgmlst_derived_data, download_mash_sketch, index
 from rauth import OAuth1Session
 from Bio import SeqIO
 import argparse
 import datetime
 import logging
-import urllib.request
-import tarfile
 import shutil
 import glob
+import ssl
 import csv
 import re
 import os
 
-
 class RmlstRest(object):
 
     def get_session_token(self):
         session_request = OAuth1Session(self.consumer_key,
                                         self.consumer_secret,
                                         access_token=self.access_token,
                                         access_token_secret=self.access_secret)
         url = self.test_rest_url + '/oauth/get_session_token'
-        r = session_request.get(url)
+        if self.unverified:
+            r = session_request.get(url, verify=False)
+        else:
+            r = session_request.get(url)
         if r.status_code == 200:
             self.session_token = r.json()['oauth_token']
             self.session_secret = r.json()['oauth_token_secret']
         else:
             logging.error('ERROR: Couldn\'t get a session token for rMLST database download. Check that your consumer '
                           'secret and access token files have valid credentials and try again.')
             quit(code=1)
 
     def get_loci_and_scheme_url(self):
         session = OAuth1Session(self.consumer_key,
                                 self.consumer_secret,
                                 access_token=self.session_token,
                                 access_token_secret=self.session_secret)
-        r = session.get(self.test_rest_url)
+        if self.unverified:
+            r = session.get(self.test_rest_url, verify=False)
+        else:
+            r = session.get(self.test_rest_url)
         if r.status_code == 200 or r.status_code == 201:
             if re.search('json', r.headers['content-type'], flags=0):
                 decoded = r.json()
             else:
                 decoded = r.text
             # Extract the URLs from the returned data
             self.loci = decoded['loci']
@@ -51,26 +55,32 @@
             quit(code=1)
 
     def download_loci(self):
         session = OAuth1Session(self.consumer_key,
                                 self.consumer_secret,
                                 access_token=self.session_token,
                                 access_token_secret=self.session_secret)
-        r = session.get(self.loci)
+        if self.unverified:
+            r = session.get(self.loci, verify=False)
+        else:
+            r = session.get(self.loci)
         if r.status_code == 200 or r.status_code == 201:
             if re.search('json', r.headers['content-type'], flags=0):
                 decoded = r.json()
             else:
                 decoded = r.text
             # Extract all the URLs in the decoded dictionary under the key 'loci'
             for locus_url in decoded['loci']:
                 output_file = os.path.join(self.output_folder, '{}.tfa'.format(os.path.split(locus_url)[1]))
                 logging.info('Downloading {}...'.format(os.path.split(locus_url)[1]))
                 with open(output_file, 'w') as f:
-                    download = session.get(locus_url + '/alleles_fasta')
+                    if self.unverified:
+                        download = session.get(locus_url + '/alleles_fasta', verify=False)
+                    else:
+                        download = session.get(locus_url + '/alleles_fasta')
                     if download.status_code == 200 or download.status_code == 201:
                         if re.search('json', download.headers['content-type'], flags=0):
                             decoded = download.json()
                         else:
                             decoded = download.text
                         with open(output_file, 'w') as locus_fasta:
                             locus_fasta.write(decoded)
@@ -82,15 +92,18 @@
 
     def download_profile(self):
         profile_file = os.path.join(self.output_folder, 'profiles.txt')
         session = OAuth1Session(self.consumer_key,
                                 self.consumer_secret,
                                 access_token=self.session_token,
                                 access_token_secret=self.session_secret)
-        r = session.get(self.profile + '/1/profiles_csv')
+        if self.unverified:
+            r = session.get(self.profile + '/1/profiles_csv', verify=False)
+        else:
+            r = session.get(self.profile + '/1/profiles_csv')
         logging.info('Downloading rMLST profiles...')
         if r.status_code == 200 or r.status_code == 201:
             if re.search('json', r.headers['content-type'], flags=0):
                 decoded = r.json()
             else:
                 decoded = r.text
             # Write the profile file to disk
@@ -113,36 +126,43 @@
         print('Visit this URL in your browser: ' + authorize_url)
         verifier = input('Enter oauth_verifier from browser: ')
         session_request = OAuth1Session(consumer_key=self.consumer_key,
                                         consumer_secret=self.consumer_secret,
                                         access_token=self.request_token,
                                         access_token_secret=self.request_secret)
         # Perform a GET request with the appropriate keys and tokens
-        r = session_request.get(self.access_token_url,
-                                params={
-                                    'oauth_verifier': verifier
-                                })
+        if self.unverified:
+            r = session_request.get(self.access_token_url, verify=False,
+                                    params={
+                                        'oauth_verifier': verifier
+                                    })
+        else:
+            r = session_request.get(self.access_token_url,
+                                    params={
+                                        'oauth_verifier': verifier
+                                    })
         # If the status code is '200' (OK), proceed
         if r.status_code == 200:
             # Save the JSON-decoded token secret and token
             self.access_token = r.json()['oauth_token']
             self.access_secret = r.json()['oauth_token_secret']
 
-    def __init__(self, consumer_secret_file, output_folder):
+    def __init__(self, consumer_secret_file, output_folder, unverified=False):
         self.test_rest_url = 'http://rest.pubmlst.org/db/pubmlst_rmlst_seqdef'
         self.test_web_url = 'http://pubmlst.org/cgi-bin/bigsdb/bigsdb.pl?db=pubmlst_rmlst_seqdef'
         self.request_token_url = self.test_rest_url + '/oauth/get_request_token'
         self.access_token_url = self.test_rest_url + '/oauth/get_access_token'
         self.authorize_url = self.test_web_url + '&page=authorizeClient'
         self.output_folder = output_folder
+        self.unverified = unverified
          
         # Get the consumer secret set up.
         if not os.path.isfile(consumer_secret_file):
-            logging.error('ERROR: Could not find consumer secret file. Please make sure the file you specified ({}) exists '
-                          'and try again.'.format(consumer_secret_file))
+            logging.error('ERROR: Could not find consumer secret file. Please make sure the file you specified '
+                          '({}) exists and try again.'.format(consumer_secret_file))
             quit(code=1)
         with open(consumer_secret_file) as f:
             lines = f.readlines()
         try:
             self.consumer_key = lines[0].rstrip()
             self.consumer_secret = lines[1].rstrip()
         except IndexError:
@@ -158,18 +178,23 @@
         self.request_secret = str()
         self.access_token = str()
         self.access_secret = str()
 
 
 def create_gene_allele_file(profiles_file, gene_allele_file):
     genus_allele_info = dict()
+    genera = set()
     with open(profiles_file) as tsvfile:
         reader = csv.DictReader(tsvfile, delimiter='\t')
         for row in reader:
             genus = row['genus']
+            # If the genus is uncertain e.g. Escherichia/Shigella, split on the /, and use Escherichia as the genus
+            if '/' in genus:
+                genus = genus.split('/')[0]
+            genera.add(genus)
             if genus not in genus_allele_info:
                 genus_allele_info[genus] = list()
             for i in range(1, 66):
                 if i < 10:
                     gene = 'BACT00000' + str(i)
                 else:
                     gene = 'BACT0000' + str(i)
@@ -180,98 +205,107 @@
                         genus_allele_info[genus].append(gene_allele)
     with open(gene_allele_file, 'w') as f:
         for genus in genus_allele_info:
             f.write(str(genus) + ':')
             for allele in genus_allele_info[genus]:
                 f.write(str(allele) + ',')
             f.write('\n')
+    return genera
 
 
-def setup_confindr_database(output_folder, consumer_secret):
-    # Remove previous output folder if it existed.
-
+def setup_confindr_database(output_folder, consumer_secret, index_databases=False, unverified=False):
     # Go through the REST API in order to get profiles downloaded.
     rmlst_rest = RmlstRest(consumer_secret_file=consumer_secret,
-                           output_folder=output_folder)
+                           output_folder=output_folder, unverified=unverified)
     rmlst_rest.get_request_token()
     rmlst_rest.get_access_token()
     rmlst_rest.get_session_token()
     rmlst_rest.get_loci_and_scheme_url()
     rmlst_rest.download_loci()
     rmlst_rest.download_profile()
 
     # With the sequences downloaded, make a file of all rMLST sequences combined.
     logging.info('Combining rMLST files...')
     with open(os.path.join(output_folder, 'rMLST_combined.fasta'), 'w') as f:
         locus_files = sorted(glob.glob(os.path.join(output_folder, 'BACT*.tfa')))
         for locus_file in locus_files:
             for record in SeqIO.parse(locus_file, 'fasta'):
                 record.id = record.id.replace('-', '_')
-                record.seq._data = record.seq._data.replace('-', '').replace('N', '')
+                try:
+                    record.seq._data = record.seq._data.replace('-', '').replace('N', '')
+                except TypeError:
+                    record.seq._data = record.seq._data.replace(b'-', b'').replace(b'N', b'')
+
+                # If the entire FASTA sequence is encoded in byte-like
+                # formatting (b' at the beginning and ' at the end of the 
+                # sequence), fix:
+                if record.seq._data[0:2] == "b'" and record.seq._data[-1] == "'":
+                    record.seq._data = record.seq._data.replace("b'", "").replace("'", "")
+                
                 record.name = ''
                 record.description = ''
                 SeqIO.write(record, f, 'fasta')
             # Clean up individual file.
             try:
                 os.remove(locus_file)
             except OSError:
                 logging.warning('WARNING: Could not delete {}. This won\'t affect ConFindr performance, but '
                                 ' you may want to delete it to save on disk space.'.format(locus_file))
 
     logging.info('Assigning alleles to genera...')
     # Parse profiles so that we know what alleles are found with each genus.
-    create_gene_allele_file(profiles_file=os.path.join(output_folder, 'profiles.txt'),
-                            gene_allele_file=os.path.join(output_folder, 'gene_allele.txt'))
-    
-    
-def download_mash_sketch(output_folder):
-    logging.info('Downloading mash refseq sketch...')
-    urllib.request.urlretrieve('https://github.com/OLC-Bioinformatics/ConFindr/raw/master/refseq_sketch/refseq.msh',
-                               os.path.join(output_folder, 'refseq.msh'))
-
-
-def download_cgmlst_derived_data(output_folder):
-    logging.info('Downloading cgMLST-derived data for Escherichia, Salmonella, and Listeria...')
-    urllib.request.urlretrieve('https://ndownloader.figshare.com/files/14771267',
-                               os.path.join(output_folder, 'confindr_db.tar.gz'))
-    confindr_tar = os.path.join(output_folder, 'confindr_db.tar.gz')
-    tar = tarfile.open(confindr_tar)
-    tar.extractall(path=output_folder)
-    tar.close()
-    os.remove(confindr_tar)
+    genera = create_gene_allele_file(profiles_file=os.path.join(output_folder, 'profiles.txt'),
+                                     gene_allele_file=os.path.join(output_folder, 'gene_allele.txt'))
+    if index_databases:
+        index(output_folder=output_folder,
+              genera=sorted(list(genera)),
+              cgderived=False)
 
 
 def main():
     logging.basicConfig(format='\033[92m \033[1m %(asctime)s \033[0m %(message)s ',
                         level=logging.INFO,
                         datefmt='%Y-%m-%d %H:%M:%S')
     parser = argparse.ArgumentParser()
     parser.add_argument('-o', '--output_folder',
                         default=os.environ.get('CONFINDR_DB', os.path.expanduser('~/.confindr_db')),
-                        help='Path to download databases to - if folder does not exist, will be created. If folder does '
-                             'exist, will be deleted and updated sequences downloaded. Defaults to ~/.confindr_db, or '
+                        help='Path to download databases to - if folder does not exist, will be created. If folder does'
+                             ' exist, will be deleted and updated sequences downloaded. Defaults to ~/.confindr_db, or '
                              'the CONFINDR_DB environmental variable.')
     parser.add_argument('-s', '--secret_file',
                         type=str,
                         help='Path to consumer secret file for rMLST database.')
+    parser.add_argument('-i', '--index_databases',
+                        action='store_true',
+                        help='Enable this option if you are installing the databases to a drive that will be read-only '
+                             'after the installation. The script will create and index all the necessary genus-specific'
+                             ' database files. Note that this is very slow for the rMLST database.')
+    parser.add_argument('-u', '--unverified',
+                        action='store_true',
+                        help="Enable this option if you plan on running ConFindr behind a firewall and/or have a self- "
+                        "signed certificate. Adds 'verify=False' during session requests.")
     args = parser.parse_args()
     if os.path.isdir(args.output_folder):
         logging.info('Removing old databases...')
         shutil.rmtree(args.output_folder)
     os.makedirs(args.output_folder)
+    if args.unverified:
+        ssl._create_default_https_context = ssl._create_unverified_context
     download_cgmlst_derived_data(args.output_folder)
     if args.secret_file is None:
         logging.warning('WARNING: Without an rMLST secret file, data will only be downloaded for Escherichia, '
                         'Salmonella, and Listeria. See '
                         'https://olc-bioinformatics.github.io/ConFindr/install/#downloading-confindr-databases for '
                         'instructions on how to get access to rMLST databases so ConFindr can be used for other species'
                         ' as well')
     else:
-        setup_confindr_database(args.output_folder,
-                                args.secret_file)
+        setup_confindr_database(output_folder=args.output_folder,
+                                consumer_secret=args.secret_file,
+                                index_databases=args.index_databases,
+                                unverified=args.unverified)
     download_mash_sketch(args.output_folder)
     current_year = datetime.datetime.utcnow().year
     current_month = datetime.datetime.utcnow().month
     current_day = datetime.datetime.utcnow().day
     with open(os.path.join(args.output_folder, 'download_date.txt'), 'w') as f:
         f.write('{}-{}-{}'.format(current_year, current_month, current_day))
     logging.info('Done downloading ConFindr databases!')
```

