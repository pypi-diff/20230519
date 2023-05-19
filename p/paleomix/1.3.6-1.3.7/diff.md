# Comparing `tmp/paleomix-1.3.6.tar.gz` & `tmp/paleomix-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paleomix-1.3.6.tar", last modified: Sun Nov 28 18:38:52 2021, max compression
+gzip compressed data, was "paleomix-1.3.7.tar", last modified: Mon Aug 22 20:42:22 2022, max compression
```

## Comparing `paleomix-1.3.6.tar` & `paleomix-1.3.7.tar`

### file list

```diff
@@ -1,299 +1,299 @@
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.014485 paleomix-1.3.6/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       50 2021-11-28 18:35:31.000000 paleomix-1.3.6/.coveragerc
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    40948 2021-11-28 18:35:32.000000 paleomix-1.3.6/CHANGES.md
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1023 2021-11-28 18:35:08.000000 paleomix-1.3.6/LICENSE
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      418 2021-11-28 18:35:08.000000 paleomix-1.3.6/MANIFEST.in
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3502 2021-11-28 18:38:52.014485 paleomix-1.3.6/PKG-INFO
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2660 2021-11-28 18:35:31.000000 paleomix-1.3.6/README.rst
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.006486 paleomix-1.3.6/docs/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      580 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/Makefile
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.002486 paleomix-1.3.6/docs/_static/
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.006486 paleomix-1.3.6/docs/_static/zonkey/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    18823 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/_static/zonkey/incl_ts_0_tree_rooted.png
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    17608 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/_static/zonkey/incl_ts_0_tree_unrooted.png
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    12751 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/_static/zonkey/mito_phylo.png
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      578 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/acknowledgements.rst
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.006486 paleomix-1.3.6/docs/bam_pipeline/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1156 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/bam_pipeline/configuration.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8561 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/bam_pipeline/filestructure.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1105 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/bam_pipeline/index.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    39892 2021-11-28 18:35:31.000000 paleomix-1.3.6/docs/bam_pipeline/makefile.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6331 2021-11-28 18:35:31.000000 paleomix-1.3.6/docs/bam_pipeline/makefile.yaml
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2990 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/bam_pipeline/overview.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2927 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/bam_pipeline/requirements.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    29659 2021-11-28 18:35:31.000000 paleomix-1.3.6/docs/bam_pipeline/usage.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5384 2021-11-28 18:35:32.000000 paleomix-1.3.6/docs/conf.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4870 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/examples.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2671 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/index.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5107 2021-11-28 18:35:32.000000 paleomix-1.3.6/docs/installation.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2663 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/introduction.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1325 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/other_tools.rst
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.006486 paleomix-1.3.6/docs/phylo_pipeline/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1078 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/phylo_pipeline/configuration.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       81 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/phylo_pipeline/filestructure.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1244 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/phylo_pipeline/index.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      169 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/phylo_pipeline/makefile.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      959 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/phylo_pipeline/overview.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2626 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/phylo_pipeline/requirements.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11286 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/phylo_pipeline/usage.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3974 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/references.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      728 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/related.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      467 2021-11-28 18:35:31.000000 paleomix-1.3.6/docs/release.rst
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.006486 paleomix-1.3.6/docs/troubleshooting/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    12642 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/troubleshooting/bam_pipeline.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6889 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/troubleshooting/common.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      394 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/troubleshooting/index.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1229 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/troubleshooting/install.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      203 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/troubleshooting/phylo_pipeline.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      106 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/troubleshooting/zonkey_pipeline.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6361 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/yaml.rst
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.006486 paleomix-1.3.6/docs/zonkey_pipeline/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2424 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/zonkey_pipeline/configuration.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3561 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/zonkey_pipeline/filestructure.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1588 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/zonkey_pipeline/index.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4401 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/zonkey_pipeline/overview.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    15441 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/zonkey_pipeline/panel.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2330 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/zonkey_pipeline/requirements.rst
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11026 2021-11-28 18:35:08.000000 paleomix-1.3.6/docs/zonkey_pipeline/usage.rst
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.006486 paleomix-1.3.6/misc/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      438 2021-11-28 18:35:31.000000 paleomix-1.3.6/misc/setup_bam_pipeline_example.makefile.yaml
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2347 2021-11-28 18:35:31.000000 paleomix-1.3.6/misc/setup_bam_pipeline_example.sh
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     2093 2021-11-28 18:35:31.000000 paleomix-1.3.6/misc/setup_phylo_pipeline_example.sh
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1379 2021-11-28 18:35:31.000000 paleomix-1.3.6/misc/skeleton.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    14808 2021-11-28 18:35:31.000000 paleomix-1.3.6/misc/synthesize_reads.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.006486 paleomix-1.3.6/paleomix/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1213 2021-11-28 18:38:39.000000 paleomix-1.3.6/paleomix/__init__.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.006486 paleomix-1.3.6/paleomix/atomiccmd/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/atomiccmd/__init__.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16171 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/atomiccmd/builder.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    19800 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/atomiccmd/command.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     7252 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/atomiccmd/pprint.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     7256 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/atomiccmd/sets.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.006486 paleomix-1.3.6/paleomix/common/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/common/__init__.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2126 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/common/argparse.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4838 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/bamfiles.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     9702 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/bedtools.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11322 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/fileutils.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.006486 paleomix-1.3.6/paleomix/common/formats/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1209 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/formats/__init__.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1183 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/common/formats/_common.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11181 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/formats/_graph.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4450 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/formats/fasta.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     7064 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/formats/fastq.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8404 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/formats/msa.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    12784 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/formats/newick.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2538 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/formats/phylip.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4759 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/common/logging.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    33460 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/makefile.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3836 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/procs.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1701 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/rtools.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2563 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/sampling.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4016 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/sequences.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1837 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/system.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1743 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/testing.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4298 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/text.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4462 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/timer.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     9423 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/utilities.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11900 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/vcffilter.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4391 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/vcfwrap.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16075 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/common/versions.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     4764 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/main.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    12011 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/node.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    19636 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/nodegraph.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/nodes/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/nodes/__init__.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5359 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/nodes/adapterremoval.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2884 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/nodes/bedtools.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4666 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/nodes/bowtie2.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    10359 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/nodes/bwa.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8068 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/nodes/commands.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8268 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/nodes/examl.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     5135 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/nodes/formats.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3073 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/nodes/mafft.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    10011 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/nodes/mapdamage.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4138 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/nodes/newick.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     7305 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/nodes/phylip.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8012 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/nodes/picard.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8819 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/nodes/raxml.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5591 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/nodes/samtools.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5612 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/nodes/sequences.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    13730 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/nodes/validation.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    13751 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/pipeline.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/pipelines/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/pipelines/__init__.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/pipelines/bam/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1180 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/bam/__init__.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6120 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/pipelines/bam/config.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    26482 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/pipelines/bam/makefile.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    12841 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/bam/mkfile.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2822 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/pipelines/bam/nodes.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/pipelines/bam/parts/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      329 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/bam/parts/__init__.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    10391 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/pipelines/bam/parts/lane.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8861 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/bam/parts/library.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3323 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/pipelines/bam/parts/prefix.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4818 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/bam/parts/reads.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1675 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/bam/parts/sample.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6903 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/bam/parts/statistics.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    21103 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/bam/parts/summary.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1521 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/bam/parts/target.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3375 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/bam/paths.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     9281 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/bam/pipeline.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1330 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/bam/trim_pipeline.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/pipelines/phylo/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/pipelines/phylo/__init__.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4503 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/phylo/config.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2248 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/pipelines/phylo/example.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    29089 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/phylo/makefile.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     7491 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/phylo/mkfile.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/pipelines/phylo/parts/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/pipelines/phylo/parts/__init__.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    10290 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/phylo/parts/genotype.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     3788 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/phylo/parts/msa.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11820 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/phylo/parts/phylo.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4097 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/pipelines/phylo/pipeline.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/pipelines/zonkey/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1159 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/__init__.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    11288 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/build_db.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     6150 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/build_mito.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    12317 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/build_tped.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2760 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/common.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5734 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/config.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    23272 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/database.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/pipelines/zonkey/parts/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1159 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/parts/__init__.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5447 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/parts/admixture.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2632 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/parts/common.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4012 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/parts/mitochondria.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    25619 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/parts/nuclear.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    29304 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/parts/report.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    18432 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/parts/summary.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    23012 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/pipelines/zonkey/pipeline.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/resources/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2844 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/resources/__init__.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.002486 paleomix-1.3.6/paleomix/resources/examples/
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37455 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_01.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37120 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_02.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37566 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_03.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    13322 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_04.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37461 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_01.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37220 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_02.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37533 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_03.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    13408 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_04.fastq.gz
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L2/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)   109199 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L2/reads.collapsed.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       20 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L2/reads.collapsed.truncated.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       20 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L2/reads.singleton.truncated.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37021 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/GCTCTG_L1_R1_01.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    31401 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/GCTCTG_L1_R1_02.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11443 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/GCTCTG_L1_R1_03.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37160 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L1_R1_01.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37211 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L1_R1_02.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    34271 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L1_R1_03.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    36990 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R1_01.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    36916 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R1_02.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3594 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R1_03.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37054 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R2_01.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    36999 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R2_02.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3580 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R2_03.fastq.gz
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6929 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/makefile.yaml
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/prefixes/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16820 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/prefixes/rCRS.fasta
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6498 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/makefile.yaml
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16874 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/bonobo.fasta
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16868 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/chimpanzee.fasta
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16734 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/gorilla.fasta
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16820 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/rCRS.fasta
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       27 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/rCRS.fasta.fai
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16809 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/sumatran_orangutan.fasta
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16818 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/white_handed_gibbon.fasta
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     1350 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/setup.sh
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/phylogeny/
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.002486 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/phylogeny/data/
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.010486 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/phylogeny/data/regions/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      452 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/phylogeny/data/regions/rCRS.non_coding.bed
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      558 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/phylogeny/data/regions/rCRS.protein_coding.CDS.bed
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6150 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/phylogeny/makefile.yaml
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     2093 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/setup.sh
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    14808 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/synthesize_reads.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.002486 paleomix-1.3.6/paleomix/resources/reports/
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.014485 paleomix-1.3.6/paleomix/resources/reports/zonkey/
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     4289 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/reports/zonkey/report.css
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.002486 paleomix-1.3.6/paleomix/resources/rscripts/
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.014485 paleomix-1.3.6/paleomix/resources/rscripts/common/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      594 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/rscripts/common/requires.r
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.014485 paleomix-1.3.6/paleomix/resources/rscripts/zonkey/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3606 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/rscripts/zonkey/admixture.r
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4129 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/rscripts/zonkey/coverage.r
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2046 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/rscripts/zonkey/pca.r
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    18491 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/rscripts/zonkey/tinytree.r
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    19506 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/resources/rscripts/zonkey/treemix.r
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.014485 paleomix-1.3.6/paleomix/tools/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/tools/__init__.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.014485 paleomix-1.3.6/paleomix/tools/bam_stats/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/tools/bam_stats/__init__.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6576 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/tools/bam_stats/common.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     7887 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/tools/bam_stats/coverage.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    12008 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/tools/cleanup.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     6337 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/tools/coverage.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    14125 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/tools/depths.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3224 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/tools/dupcheck.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2026 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/tools/factory.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    11627 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/tools/gtf_to_bed.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     8663 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/tools/rmdup_collapsed.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3456 2021-11-28 18:35:08.000000 paleomix-1.3.6/paleomix/tools/validate_fastq.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     3391 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/tools/vcf_filter.py
--rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    12886 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/tools/vcf_to_fasta.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1484 2021-11-28 18:35:31.000000 paleomix-1.3.6/paleomix/yaml.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.006486 paleomix-1.3.6/paleomix.egg-info/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3502 2021-11-28 18:38:51.000000 paleomix-1.3.6/paleomix.egg-info/PKG-INFO
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     9506 2021-11-28 18:38:51.000000 paleomix-1.3.6/paleomix.egg-info/SOURCES.txt
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)        1 2021-11-28 18:38:51.000000 paleomix-1.3.6/paleomix.egg-info/dependency_links.txt
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       56 2021-11-28 18:38:51.000000 paleomix-1.3.6/paleomix.egg-info/entry_points.txt
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)        1 2021-11-28 18:38:51.000000 paleomix-1.3.6/paleomix.egg-info/not-zip-safe
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       95 2021-11-28 18:38:51.000000 paleomix-1.3.6/paleomix.egg-info/requires.txt
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)        9 2021-11-28 18:38:51.000000 paleomix-1.3.6/paleomix.egg-info/top_level.txt
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      324 2021-11-28 18:35:32.000000 paleomix-1.3.6/paleomix_environment.yaml
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      120 2021-11-28 18:38:52.014485 paleomix-1.3.6/setup.cfg
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2925 2021-11-28 18:35:31.000000 paleomix-1.3.6/setup.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.014485 paleomix-1.3.6/tests/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       86 2021-11-28 18:35:08.000000 paleomix-1.3.6/tests/README.rst
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.014485 paleomix-1.3.6/tests/atomiccmd_test/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/atomiccmd_test/__init__.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    24491 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/atomiccmd_test/builder_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    27027 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/atomiccmd_test/command_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16163 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/atomiccmd_test/pprint_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    12133 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/atomiccmd_test/sets_test.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.014485 paleomix-1.3.6/tests/common_tests/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2021-11-28 18:35:08.000000 paleomix-1.3.6/tests/common_tests/__init__.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11942 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/common_tests/bedtools_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    25501 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/common_tests/fileutils_test.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.014485 paleomix-1.3.6/tests/common_tests/formats_tests/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2021-11-28 18:35:08.000000 paleomix-1.3.6/tests/common_tests/formats_tests/__init__.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11220 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/common_tests/formats_tests/fasta_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11238 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/common_tests/formats_tests/fastq_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    14636 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/common_tests/formats_tests/msa_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    23882 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/common_tests/formats_tests/newick_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5355 2021-11-28 18:35:08.000000 paleomix-1.3.6/tests/common_tests/formats_tests/phylip_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    40627 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/common_tests/makefile_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4715 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/common_tests/sampling_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4182 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/common_tests/sequences_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8746 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/common_tests/text_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    20383 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/common_tests/utilities_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    22916 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/common_tests/versions_test.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.014485 paleomix-1.3.6/tests/data/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:35:08.000000 paleomix-1.3.6/tests/data/empty_file_1
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:35:08.000000 paleomix-1.3.6/tests/data/empty_file_2
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16882 2021-11-28 18:35:08.000000 paleomix-1.3.6/tests/data/rCRS.fasta
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       45 2021-11-28 18:35:08.000000 paleomix-1.3.6/tests/data/rCRS.fasta.fai
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    21255 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/node_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4411 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/nodegraph_test.py
-drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2021-11-28 18:38:52.014485 paleomix-1.3.6/tests/tools_test/
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3240 2021-11-28 18:35:31.000000 paleomix-1.3.6/tests/tools_test/factory_test.py
--rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      610 2021-11-28 18:35:31.000000 paleomix-1.3.6/tox.ini
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.853564 paleomix-1.3.7/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       50 2022-08-22 20:41:17.000000 paleomix-1.3.7/.coveragerc
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    41790 2022-08-22 20:41:17.000000 paleomix-1.3.7/CHANGES.md
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1023 2022-08-22 20:41:05.000000 paleomix-1.3.7/LICENSE
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      418 2022-08-22 20:41:05.000000 paleomix-1.3.7/MANIFEST.in
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3502 2022-08-22 20:42:22.853564 paleomix-1.3.7/PKG-INFO
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2660 2022-08-22 20:41:17.000000 paleomix-1.3.7/README.rst
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.841564 paleomix-1.3.7/docs/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      580 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/Makefile
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.841564 paleomix-1.3.7/docs/_static/
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.841564 paleomix-1.3.7/docs/_static/zonkey/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    18823 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/_static/zonkey/incl_ts_0_tree_rooted.png
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    17608 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/_static/zonkey/incl_ts_0_tree_unrooted.png
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    12751 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/_static/zonkey/mito_phylo.png
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      578 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/acknowledgements.rst
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.841564 paleomix-1.3.7/docs/bam_pipeline/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1156 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/bam_pipeline/configuration.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8561 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/bam_pipeline/filestructure.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1105 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/bam_pipeline/index.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    39892 2022-08-22 20:41:17.000000 paleomix-1.3.7/docs/bam_pipeline/makefile.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6331 2022-08-22 20:41:17.000000 paleomix-1.3.7/docs/bam_pipeline/makefile.yaml
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2990 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/bam_pipeline/overview.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2927 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/bam_pipeline/requirements.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    29659 2022-08-22 20:41:17.000000 paleomix-1.3.7/docs/bam_pipeline/usage.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5384 2022-08-22 20:41:17.000000 paleomix-1.3.7/docs/conf.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4870 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/examples.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2671 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/index.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5107 2022-08-22 20:41:17.000000 paleomix-1.3.7/docs/installation.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2663 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/introduction.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1325 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/other_tools.rst
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.841564 paleomix-1.3.7/docs/phylo_pipeline/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1078 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/phylo_pipeline/configuration.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       81 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/phylo_pipeline/filestructure.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1244 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/phylo_pipeline/index.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      169 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/phylo_pipeline/makefile.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      959 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/phylo_pipeline/overview.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2626 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/phylo_pipeline/requirements.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11286 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/phylo_pipeline/usage.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3974 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/references.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      728 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/related.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      467 2022-08-22 20:41:17.000000 paleomix-1.3.7/docs/release.rst
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.841564 paleomix-1.3.7/docs/troubleshooting/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    12642 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/troubleshooting/bam_pipeline.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6889 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/troubleshooting/common.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      394 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/troubleshooting/index.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1229 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/troubleshooting/install.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      203 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/troubleshooting/phylo_pipeline.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      106 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/troubleshooting/zonkey_pipeline.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6361 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/yaml.rst
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.841564 paleomix-1.3.7/docs/zonkey_pipeline/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2424 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/zonkey_pipeline/configuration.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3561 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/zonkey_pipeline/filestructure.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1588 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/zonkey_pipeline/index.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4401 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/zonkey_pipeline/overview.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    15441 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/zonkey_pipeline/panel.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2330 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/zonkey_pipeline/requirements.rst
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11026 2022-08-22 20:41:05.000000 paleomix-1.3.7/docs/zonkey_pipeline/usage.rst
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.841564 paleomix-1.3.7/misc/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      438 2022-08-22 20:41:17.000000 paleomix-1.3.7/misc/setup_bam_pipeline_example.makefile.yaml
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2347 2022-08-22 20:41:17.000000 paleomix-1.3.7/misc/setup_bam_pipeline_example.sh
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     2093 2022-08-22 20:41:17.000000 paleomix-1.3.7/misc/setup_phylo_pipeline_example.sh
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1379 2022-08-22 20:41:17.000000 paleomix-1.3.7/misc/skeleton.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    14808 2022-08-22 20:41:17.000000 paleomix-1.3.7/misc/synthesize_reads.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.841564 paleomix-1.3.7/paleomix/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1213 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/__init__.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.845564 paleomix-1.3.7/paleomix/atomiccmd/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/atomiccmd/__init__.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16171 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/atomiccmd/builder.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    19800 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/atomiccmd/command.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     7252 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/atomiccmd/pprint.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     7256 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/atomiccmd/sets.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.845564 paleomix-1.3.7/paleomix/common/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/common/__init__.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2132 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/argparse.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4838 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/bamfiles.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     9702 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/bedtools.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11322 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/fileutils.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.845564 paleomix-1.3.7/paleomix/common/formats/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1209 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/formats/__init__.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1183 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/common/formats/_common.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11181 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/formats/_graph.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4450 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/formats/fasta.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     7064 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/formats/fastq.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8404 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/formats/msa.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    12784 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/formats/newick.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2538 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/formats/phylip.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4759 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/logging.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    33460 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/makefile.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3836 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/procs.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1701 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/rtools.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2563 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/sampling.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4016 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/sequences.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1837 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/system.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1743 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/testing.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4298 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/text.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4462 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/timer.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     9423 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/utilities.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11900 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/vcffilter.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4391 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/vcfwrap.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16075 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/common/versions.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     4764 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/main.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    12011 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/node.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    19814 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodegraph.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.845564 paleomix-1.3.7/paleomix/nodes/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/nodes/__init__.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5359 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/adapterremoval.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2884 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/bedtools.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4666 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/bowtie2.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    10359 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/bwa.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8080 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/commands.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8268 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/examl.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     5135 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/formats.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3073 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/mafft.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    10011 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/mapdamage.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4138 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/newick.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     7305 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/phylip.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8012 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/picard.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8819 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/raxml.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5591 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/samtools.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5612 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/sequences.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    13730 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/nodes/validation.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    13838 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipeline.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.845564 paleomix-1.3.7/paleomix/pipelines/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/pipelines/__init__.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.845564 paleomix-1.3.7/paleomix/pipelines/bam/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1180 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/__init__.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6120 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/config.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    26482 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/makefile.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    13036 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/mkfile.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2822 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/nodes.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.845564 paleomix-1.3.7/paleomix/pipelines/bam/parts/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      329 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/parts/__init__.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    10420 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/parts/lane.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8861 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/parts/library.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3323 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/parts/prefix.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4818 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/parts/reads.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1675 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/parts/sample.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6903 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/parts/statistics.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    21108 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/parts/summary.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1521 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/parts/target.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3375 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/paths.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     9316 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/pipeline.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1330 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/bam/trim_pipeline.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.845564 paleomix-1.3.7/paleomix/pipelines/phylo/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/pipelines/phylo/__init__.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4503 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/phylo/config.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2248 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/phylo/example.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    29089 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/phylo/makefile.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     7491 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/phylo/mkfile.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.845564 paleomix-1.3.7/paleomix/pipelines/phylo/parts/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/pipelines/phylo/parts/__init__.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    10290 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/phylo/parts/genotype.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     3788 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/phylo/parts/msa.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11820 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/phylo/parts/phylo.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4097 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/phylo/pipeline.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.845564 paleomix-1.3.7/paleomix/pipelines/zonkey/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1159 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/__init__.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    11288 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/build_db.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     6150 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/build_mito.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    12317 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/build_tped.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2760 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/common.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5734 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/config.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    23272 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/database.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/pipelines/zonkey/parts/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1159 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/parts/__init__.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5447 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/parts/admixture.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2632 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/parts/common.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4012 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/parts/mitochondria.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    25619 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/parts/nuclear.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    29304 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/parts/report.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    18432 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/parts/summary.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    23012 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/pipelines/zonkey/pipeline.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/resources/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2844 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/resources/__init__.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.841564 paleomix-1.3.7/paleomix/resources/examples/
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37455 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_01.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37120 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_02.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37566 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_03.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    13322 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_04.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37461 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_01.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37220 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_02.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37533 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_03.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    13408 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_04.fastq.gz
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L2/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)   109199 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L2/reads.collapsed.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       20 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L2/reads.collapsed.truncated.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       20 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L2/reads.singleton.truncated.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37021 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/GCTCTG_L1_R1_01.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    31401 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/GCTCTG_L1_R1_02.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11443 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/GCTCTG_L1_R1_03.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37160 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L1_R1_01.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37211 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L1_R1_02.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    34271 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L1_R1_03.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    36990 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R1_01.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    36916 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R1_02.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3594 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R1_03.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    37054 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R2_01.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    36999 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R2_02.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3580 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R2_03.fastq.gz
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6929 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/makefile.yaml
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/prefixes/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16820 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/prefixes/rCRS.fasta
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6498 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/makefile.yaml
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16874 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/bonobo.fasta
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16868 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/chimpanzee.fasta
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16734 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/gorilla.fasta
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16820 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/rCRS.fasta
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       27 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/rCRS.fasta.fai
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16809 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/sumatran_orangutan.fasta
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16818 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/white_handed_gibbon.fasta
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     1350 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/setup.sh
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/phylogeny/
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.841564 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/phylogeny/data/
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/phylogeny/data/regions/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      452 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/phylogeny/data/regions/rCRS.non_coding.bed
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      558 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/phylogeny/data/regions/rCRS.protein_coding.CDS.bed
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6150 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/phylogeny/makefile.yaml
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     2093 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/setup.sh
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    14808 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/synthesize_reads.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.841564 paleomix-1.3.7/paleomix/resources/reports/
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/resources/reports/zonkey/
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     4289 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/resources/reports/zonkey/report.css
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.841564 paleomix-1.3.7/paleomix/resources/rscripts/
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/resources/rscripts/common/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      594 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/rscripts/common/requires.r
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/resources/rscripts/zonkey/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3606 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/rscripts/zonkey/admixture.r
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4129 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/rscripts/zonkey/coverage.r
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2046 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/rscripts/zonkey/pca.r
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    18491 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/rscripts/zonkey/tinytree.r
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    19506 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/resources/rscripts/zonkey/treemix.r
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/tools/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/tools/__init__.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/paleomix/tools/bam_stats/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/tools/bam_stats/__init__.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     6576 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/tools/bam_stats/common.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     7887 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/tools/bam_stats/coverage.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    12008 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/tools/cleanup.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     6337 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/tools/coverage.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    14125 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/tools/depths.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3224 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/tools/dupcheck.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2026 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/tools/factory.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    11627 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/tools/gtf_to_bed.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     8663 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/tools/rmdup_collapsed.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3456 2022-08-22 20:41:05.000000 paleomix-1.3.7/paleomix/tools/validate_fastq.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)     3391 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/tools/vcf_filter.py
+-rwxrwxr-x   0 jdoe      (1000) jdoe      (1000)    12886 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/tools/vcf_to_fasta.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1484 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix/yaml.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.845564 paleomix-1.3.7/paleomix.egg-info/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3502 2022-08-22 20:42:22.000000 paleomix-1.3.7/paleomix.egg-info/PKG-INFO
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     9506 2022-08-22 20:42:22.000000 paleomix-1.3.7/paleomix.egg-info/SOURCES.txt
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)        1 2022-08-22 20:42:22.000000 paleomix-1.3.7/paleomix.egg-info/dependency_links.txt
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       56 2022-08-22 20:42:22.000000 paleomix-1.3.7/paleomix.egg-info/entry_points.txt
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)        1 2022-08-22 20:42:08.000000 paleomix-1.3.7/paleomix.egg-info/not-zip-safe
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       95 2022-08-22 20:42:22.000000 paleomix-1.3.7/paleomix.egg-info/requires.txt
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)        9 2022-08-22 20:42:22.000000 paleomix-1.3.7/paleomix.egg-info/top_level.txt
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      326 2022-08-22 20:41:17.000000 paleomix-1.3.7/paleomix_environment.yaml
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      120 2022-08-22 20:42:22.853564 paleomix-1.3.7/setup.cfg
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     2925 2022-08-22 20:41:17.000000 paleomix-1.3.7/setup.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/tests/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       86 2022-08-22 20:41:05.000000 paleomix-1.3.7/tests/README.rst
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.849564 paleomix-1.3.7/tests/atomiccmd_test/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/atomiccmd_test/__init__.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    24491 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/atomiccmd_test/builder_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    27027 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/atomiccmd_test/command_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16163 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/atomiccmd_test/pprint_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    12133 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/atomiccmd_test/sets_test.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.853564 paleomix-1.3.7/tests/common_tests/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2022-08-22 20:41:05.000000 paleomix-1.3.7/tests/common_tests/__init__.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11942 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/common_tests/bedtools_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    25501 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/common_tests/fileutils_test.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.853564 paleomix-1.3.7/tests/common_tests/formats_tests/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     1139 2022-08-22 20:41:05.000000 paleomix-1.3.7/tests/common_tests/formats_tests/__init__.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11220 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/common_tests/formats_tests/fasta_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    11238 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/common_tests/formats_tests/fastq_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    14636 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/common_tests/formats_tests/msa_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    23882 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/common_tests/formats_tests/newick_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     5355 2022-08-22 20:41:05.000000 paleomix-1.3.7/tests/common_tests/formats_tests/phylip_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    40627 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/common_tests/makefile_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4715 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/common_tests/sampling_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4182 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/common_tests/sequences_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     8746 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/common_tests/text_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    20383 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/common_tests/utilities_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    22916 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/common_tests/versions_test.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.853564 paleomix-1.3.7/tests/data/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:41:05.000000 paleomix-1.3.7/tests/data/empty_file_1
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:41:05.000000 paleomix-1.3.7/tests/data/empty_file_2
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    16882 2022-08-22 20:41:05.000000 paleomix-1.3.7/tests/data/rCRS.fasta
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)       45 2022-08-22 20:41:05.000000 paleomix-1.3.7/tests/data/rCRS.fasta.fai
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)    21255 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/node_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     4411 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/nodegraph_test.py
+drwxrwxr-x   0 jdoe      (1000) jdoe      (1000)        0 2022-08-22 20:42:22.853564 paleomix-1.3.7/tests/tools_test/
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)     3240 2022-08-22 20:41:17.000000 paleomix-1.3.7/tests/tools_test/factory_test.py
+-rw-rw-r--   0 jdoe      (1000) jdoe      (1000)      610 2022-08-22 20:41:17.000000 paleomix-1.3.7/tox.ini
```

### Comparing `paleomix-1.3.6/CHANGES.md` & `paleomix-1.3.7/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,27 @@
 # Changelog
 
+## [1.3.7] - 2022-08-22
+
+#### Added
+  - Added example to BAM pipeline YAML template, showing how to increase the maximum
+    allowed Phred score for AdapterRemoval. This is needed due to the value being
+    capped at 41 by default, lower than the maximum observed in some modern data.
+
+#### Fixed
+  - Fixed regression in config file parsing, that would cause failure if no value
+    was specified for an option.
+  - Fixed error message not being printed correctly when attempting to use Phred+64
+    data with BWA mem/bwasw.
+  - Fixed regressions that prevented the use of "regions of interest" in the BAM
+    pipeline.
+  - Fixed failure when using `--list-output-files` and auxilary files were missing
+    or dependecies were unmet. Output files are now printed.
+
+
 ## [1.3.6] - 2021-11-28
 
 ### Added
   - Added explicit support for the AdapterRemoval `--trim5p` and `--trim3p` options,
     which may take one or two values (as a list).
 
 ### Changed
@@ -764,14 +782,15 @@
 
 
 ## [1.0.0] - 2014-04-16
 ### Changed
   - Switching to more traditional version-number tracking.
 
 
+[1.3.7]: https://github.com/MikkelSchubert/paleomix/compare/v1.3.6...v1.3.7
 [1.3.6]: https://github.com/MikkelSchubert/paleomix/compare/v1.3.5...v1.3.6
 [1.3.5]: https://github.com/MikkelSchubert/paleomix/compare/v1.3.4...v1.3.5
 [1.3.4]: https://github.com/MikkelSchubert/paleomix/compare/v1.3.3...v1.3.4
 [1.3.3]: https://github.com/MikkelSchubert/paleomix/compare/v1.3.2...v1.3.3
 [1.3.2]: https://github.com/MikkelSchubert/paleomix/compare/v1.3.1...v1.3.2
 [1.3.1]: https://github.com/MikkelSchubert/paleomix/compare/v1.3.0...v1.3.1
 [1.3.0]: https://github.com/MikkelSchubert/paleomix/compare/v1.2.14...v1.3.0
```

### Comparing `paleomix-1.3.6/LICENSE` & `paleomix-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/PKG-INFO` & `paleomix-1.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: paleomix
-Version: 1.3.6
+Version: 1.3.7
 Summary: Bioinformatics pipelines for HTS data
 Home-page: https://github.com/MikkelSchubert/paleomix
 Author: Mikkel Schubert
 Author-email: MikkelSch@gmail.com
 License: MIT
 Description: **********************
         The PALEOMIX pipelines
```

### Comparing `paleomix-1.3.6/README.rst` & `paleomix-1.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/Makefile` & `paleomix-1.3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/_static/zonkey/incl_ts_0_tree_rooted.png` & `paleomix-1.3.7/docs/_static/zonkey/incl_ts_0_tree_rooted.png`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/_static/zonkey/incl_ts_0_tree_unrooted.png` & `paleomix-1.3.7/docs/_static/zonkey/incl_ts_0_tree_unrooted.png`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/_static/zonkey/mito_phylo.png` & `paleomix-1.3.7/docs/_static/zonkey/mito_phylo.png`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/acknowledgements.rst` & `paleomix-1.3.7/docs/acknowledgements.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/bam_pipeline/configuration.rst` & `paleomix-1.3.7/docs/bam_pipeline/configuration.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/bam_pipeline/filestructure.rst` & `paleomix-1.3.7/docs/bam_pipeline/filestructure.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/bam_pipeline/index.rst` & `paleomix-1.3.7/docs/bam_pipeline/index.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/bam_pipeline/makefile.rst` & `paleomix-1.3.7/docs/bam_pipeline/makefile.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/bam_pipeline/makefile.yaml` & `paleomix-1.3.7/docs/bam_pipeline/makefile.yaml`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/bam_pipeline/overview.rst` & `paleomix-1.3.7/docs/bam_pipeline/overview.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/bam_pipeline/requirements.rst` & `paleomix-1.3.7/docs/bam_pipeline/requirements.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/bam_pipeline/usage.rst` & `paleomix-1.3.7/docs/bam_pipeline/usage.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/conf.py` & `paleomix-1.3.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/examples.rst` & `paleomix-1.3.7/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/index.rst` & `paleomix-1.3.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/installation.rst` & `paleomix-1.3.7/docs/installation.rst`

 * *Files 0% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 
 In addition, some libraries used by PALEOMIX may require additional development files, namely those for `zlib`, `libbz2`, `liblzma`, and for Python 3::
 
     $ sudo apt-get install libz-dev libbz2-dev liblzma-dev python3-dev
 
 Once all requirements have been installed, PALEOMIX may be installed using `pip`::
 
-    $ python3 -m pip install paleomix==1.3.6
+    $ python3 -m pip install paleomix==1.3.7
 
 To verify that the installation was carried out correctly, run the command `paleomix`::
 
     $ paleomix
     PALEOMIX - pipelines and tools for NGS data analyses
-    Version: v1.3.6
+    Version: v1.3.7
 
     ...
 
 If you have not previously used pip, then you may need to add the pip `bin` folder to your `PATH` and restart your terminal before running the `paleomix` command::
 
     $ echo 'export PATH=~/.local/bin:$PATH' >> ~/.bashrc
 
@@ -41,15 +41,15 @@
 This installation method requires the `venv` module. On Debian based systems, this module must be installed separately::
 
     $ sudo apt-get install python3-venv
 
 Once `venv` is installed, creation of a virtual environment and installation of PALEOMIX may be carried out as shown here::
 
     $ python3 -m venv venv
-    $ ./venv/bin/pip install paleomix==v1.3.6
+    $ ./venv/bin/pip install paleomix==v1.3.7
 
 Following successful completion of these commands, the `paleomix` executable will be accessible in the `./venv/bin/` folder. However, as this folder also contains a copy of Python itself, it is not recommended to add it to your `PATH`. Instead, simply link the `paleomix` executable to a folder in your `PATH`. This can be accomplished as follows::
 
     $ mkdir -p ~/.local/bin/
     $ ln -s ${PWD}/venv/bin/paleomix ~/.local/bin/
 
 If ~/.local/bin is not already in your PATH, then it can be added as follows::
@@ -74,15 +74,15 @@
 
 `Conda`_ can be used to automatically setup a self-contained environment that includes the software required by PALEOMIX.
 
 To install `conda` and also set it up so it can use the `bioconda`_ bioinformatics repository, follow the instructions on the bioconda website `here`_.
 
 Next, run the following commands to download the conda environment template for this release of PALEOMIX and to create a new conda environment named `paleomix` using that template::
 
-    $ curl -fL https://github.com/MikkelSchubert/paleomix/releases/download/v1.3.6/paleomix_environment.yaml > paleomix_environment.yaml
+    $ curl -fL https://github.com/MikkelSchubert/paleomix/releases/download/v1.3.7/paleomix_environment.yaml > paleomix_environment.yaml
     $ conda env create -n paleomix -f paleomix_environment.yaml
 
 You can now activate the paleomix environment with::
 
     $ conda activate paleomix
 
 PALEOMIX requires that the Picard JAR file can be found in a specific location, so we can symlink the versions in your conda environment into the correct place::
```

### Comparing `paleomix-1.3.6/docs/introduction.rst` & `paleomix-1.3.7/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/other_tools.rst` & `paleomix-1.3.7/docs/other_tools.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/phylo_pipeline/configuration.rst` & `paleomix-1.3.7/docs/phylo_pipeline/configuration.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/phylo_pipeline/index.rst` & `paleomix-1.3.7/docs/phylo_pipeline/index.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/phylo_pipeline/overview.rst` & `paleomix-1.3.7/docs/phylo_pipeline/overview.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/phylo_pipeline/requirements.rst` & `paleomix-1.3.7/docs/phylo_pipeline/requirements.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/phylo_pipeline/usage.rst` & `paleomix-1.3.7/docs/phylo_pipeline/usage.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/references.rst` & `paleomix-1.3.7/docs/references.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/related.rst` & `paleomix-1.3.7/docs/related.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/troubleshooting/bam_pipeline.rst` & `paleomix-1.3.7/docs/troubleshooting/bam_pipeline.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/troubleshooting/common.rst` & `paleomix-1.3.7/docs/troubleshooting/common.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/troubleshooting/install.rst` & `paleomix-1.3.7/docs/troubleshooting/install.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/yaml.rst` & `paleomix-1.3.7/docs/yaml.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/zonkey_pipeline/configuration.rst` & `paleomix-1.3.7/docs/zonkey_pipeline/configuration.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/zonkey_pipeline/filestructure.rst` & `paleomix-1.3.7/docs/zonkey_pipeline/filestructure.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/zonkey_pipeline/index.rst` & `paleomix-1.3.7/docs/zonkey_pipeline/index.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/zonkey_pipeline/overview.rst` & `paleomix-1.3.7/docs/zonkey_pipeline/overview.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/zonkey_pipeline/panel.rst` & `paleomix-1.3.7/docs/zonkey_pipeline/panel.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/zonkey_pipeline/requirements.rst` & `paleomix-1.3.7/docs/zonkey_pipeline/requirements.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/docs/zonkey_pipeline/usage.rst` & `paleomix-1.3.7/docs/zonkey_pipeline/usage.rst`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/misc/setup_bam_pipeline_example.sh` & `paleomix-1.3.7/misc/setup_bam_pipeline_example.sh`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/misc/setup_phylo_pipeline_example.sh` & `paleomix-1.3.7/misc/setup_phylo_pipeline_example.sh`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/misc/skeleton.py` & `paleomix-1.3.7/misc/skeleton.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/misc/synthesize_reads.py` & `paleomix-1.3.7/misc/synthesize_reads.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/__init__.py` & `paleomix-1.3.7/paleomix/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
-__version_info__ = (1, 3, 6)
+__version_info__ = (1, 3, 7)
 __version__ = "%i.%i.%i" % __version_info__
```

### Comparing `paleomix-1.3.6/paleomix/atomiccmd/__init__.py` & `paleomix-1.3.7/paleomix/atomiccmd/__init__.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/atomiccmd/builder.py` & `paleomix-1.3.7/paleomix/atomiccmd/builder.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/atomiccmd/command.py` & `paleomix-1.3.7/paleomix/atomiccmd/command.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/atomiccmd/pprint.py` & `paleomix-1.3.7/paleomix/atomiccmd/pprint.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/atomiccmd/sets.py` & `paleomix-1.3.7/paleomix/atomiccmd/sets.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/__init__.py` & `paleomix-1.3.7/paleomix/common/__init__.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/argparse.py` & `paleomix-1.3.7/paleomix/common/argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,11 +54,11 @@
             if key not in keys:
                 keys.append(key)
 
         return keys
 
     def convert_item_to_command_line_arg(self, action, key, value):
         # Ignore empty options from old config files
-        if action and value == "=":
+        if action and value in ("", "="):
             return []
 
         return super().convert_item_to_command_line_arg(action, key, value)
```

### Comparing `paleomix-1.3.6/paleomix/common/bamfiles.py` & `paleomix-1.3.7/paleomix/common/bamfiles.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/bedtools.py` & `paleomix-1.3.7/paleomix/common/bedtools.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/fileutils.py` & `paleomix-1.3.7/paleomix/common/fileutils.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/formats/__init__.py` & `paleomix-1.3.7/paleomix/common/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/formats/_common.py` & `paleomix-1.3.7/paleomix/common/formats/_common.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/formats/_graph.py` & `paleomix-1.3.7/paleomix/common/formats/_graph.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/formats/fasta.py` & `paleomix-1.3.7/paleomix/common/formats/fasta.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/formats/fastq.py` & `paleomix-1.3.7/paleomix/common/formats/fastq.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/formats/msa.py` & `paleomix-1.3.7/paleomix/common/formats/msa.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/formats/newick.py` & `paleomix-1.3.7/paleomix/common/formats/newick.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/formats/phylip.py` & `paleomix-1.3.7/paleomix/common/formats/phylip.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/logging.py` & `paleomix-1.3.7/paleomix/common/logging.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/makefile.py` & `paleomix-1.3.7/paleomix/common/makefile.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/procs.py` & `paleomix-1.3.7/paleomix/common/procs.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/rtools.py` & `paleomix-1.3.7/paleomix/common/rtools.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/sampling.py` & `paleomix-1.3.7/paleomix/common/sampling.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/sequences.py` & `paleomix-1.3.7/paleomix/common/sequences.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/system.py` & `paleomix-1.3.7/paleomix/common/system.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/testing.py` & `paleomix-1.3.7/paleomix/common/testing.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/text.py` & `paleomix-1.3.7/paleomix/common/text.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/timer.py` & `paleomix-1.3.7/paleomix/common/timer.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/utilities.py` & `paleomix-1.3.7/paleomix/common/utilities.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/vcffilter.py` & `paleomix-1.3.7/paleomix/common/vcffilter.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/vcfwrap.py` & `paleomix-1.3.7/paleomix/common/vcfwrap.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/common/versions.py` & `paleomix-1.3.7/paleomix/common/versions.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/main.py` & `paleomix-1.3.7/paleomix/main.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/node.py` & `paleomix-1.3.7/paleomix/node.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodegraph.py` & `paleomix-1.3.7/paleomix/nodegraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,20 @@
     pass
 
 
 class NodeGraph:
     NUMBER_OF_STATES = 6
     DONE, RUNNING, RUNABLE, QUEUED, OUTDATED, ERROR = range(NUMBER_OF_STATES)
 
-    def __init__(self, nodes, cache_factory=FileStatusCache):
+    def __init__(
+        self,
+        nodes,
+        allow_missing_files=False,
+        cache_factory=FileStatusCache,
+    ):
         self._cache_factory = cache_factory
         self._states = {}
         self._state_counts = [0] * self.NUMBER_OF_STATES
 
         nodes = safe_coerce_to_frozenset(nodes)
 
         self._logger = logging.getLogger(__name__)
@@ -122,25 +127,27 @@
 
         self._logger.info("Checking file dependencies")
         if not self._check_file_dependencies(self._reverse_dependencies):
             raise NodeGraphError("Aborting due to input/output file error")
 
         self._logger.info("Checking for auxiliary files")
         if not self._check_auxiliary_files(self._reverse_dependencies):
-            raise NodeGraphError(
-                "Please refer to the PALEOMIX installation instructions at "
-                "https://paleomix.readthedocs.io/en/stable/"
-            )
+            if not allow_missing_files:
+                raise NodeGraphError(
+                    "Please refer to the PALEOMIX installation instructions at "
+                    "https://paleomix.readthedocs.io/en/stable/"
+                )
 
         self._logger.info("Checking required software")
         if not self._check_version_requirements(self._reverse_dependencies):
-            raise NodeGraphError(
-                "Please refer to the PALEOMIX installation instructions at "
-                "https://paleomix.readthedocs.io/en/stable/"
-            )
+            if not allow_missing_files:
+                raise NodeGraphError(
+                    "Please refer to the PALEOMIX installation instructions at "
+                    "https://paleomix.readthedocs.io/en/stable/"
+                )
 
         self._logger.info("Determining states")
         self._refresh_states()
         self._logger.info("Ready")
 
     def get_node_state(self, node):
         return self._states[node]
```

### Comparing `paleomix-1.3.6/paleomix/nodes/__init__.py` & `paleomix-1.3.7/paleomix/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/adapterremoval.py` & `paleomix-1.3.7/paleomix/nodes/adapterremoval.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/bedtools.py` & `paleomix-1.3.7/paleomix/nodes/bedtools.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/bowtie2.py` & `paleomix-1.3.7/paleomix/nodes/bowtie2.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/bwa.py` & `paleomix-1.3.7/paleomix/nodes/bwa.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/commands.py` & `paleomix-1.3.7/paleomix/nodes/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,16 @@
         builder.add_value("%(OUT_FILE)s")
         builder.set_option("--target-name", target_name)
         builder.set_kwargs(OUT_FILE=output_file, IN_BAM=input_file)
 
         if regions_file:
             builder.set_option("--regions-file", "%(IN_REGIONS)s")
             builder.set_kwargs(
-                IN_REGIONS=regions_file, TEMP_IN_INDEX=input_file + index_format
+                IN_REGIONS=regions_file,
+                IN_INDEX=input_file + index_format,
             )
 
         CommandNode.__init__(
             self,
             command=builder.finalize(),
             description="calculating depth histogram for %s" % (input_file,),
             dependencies=dependencies,
```

### Comparing `paleomix-1.3.6/paleomix/nodes/examl.py` & `paleomix-1.3.7/paleomix/nodes/examl.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/formats.py` & `paleomix-1.3.7/paleomix/nodes/formats.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/mafft.py` & `paleomix-1.3.7/paleomix/nodes/mafft.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/mapdamage.py` & `paleomix-1.3.7/paleomix/nodes/mapdamage.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/newick.py` & `paleomix-1.3.7/paleomix/nodes/newick.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/phylip.py` & `paleomix-1.3.7/paleomix/nodes/phylip.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/picard.py` & `paleomix-1.3.7/paleomix/nodes/picard.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/raxml.py` & `paleomix-1.3.7/paleomix/nodes/raxml.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/samtools.py` & `paleomix-1.3.7/paleomix/nodes/samtools.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/sequences.py` & `paleomix-1.3.7/paleomix/nodes/sequences.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/nodes/validation.py` & `paleomix-1.3.7/paleomix/nodes/validation.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipeline.py` & `paleomix-1.3.7/paleomix/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,19 @@
 
         self.walk_nodes(collect_output_files)
 
         return input_files - output_files
 
     def list_output_files(self):
         cache = FileStatusCache()
-        nodegraph = NodeGraph(self._nodes, lambda: cache)
+        nodegraph = NodeGraph(
+            self._nodes,
+            allow_missing_files=True,
+            cache_factory=lambda: cache,
+        )
         output_files = {}
 
         def collect_output_files(node):
             state = None
             if nodegraph.is_done(node, cache):
                 state = nodegraph.DONE
                 if nodegraph.is_outdated(node, cache):
```

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/__init__.py` & `paleomix-1.3.7/paleomix/pipelines/bam/__init__.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/config.py` & `paleomix-1.3.7/paleomix/pipelines/bam/config.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/makefile.py` & `paleomix-1.3.7/paleomix/pipelines/bam/makefile.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/mkfile.py` & `paleomix-1.3.7/paleomix/pipelines/bam/mkfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,17 @@
      # To override, change these value(s):
      --mm: 3
      --minlength: 25
      # Extra features enabled by default; change 'yes' to 'no' to disable
      --collapse: yes
      --trimns: yes
      --trimqualities: yes
+     # Increase the maximum Phred allowed for input FASTQs, as well as for merged bases
+     # when using --collapse (default = 41). This is needed for some modern FASTQs.
+#     --qualitymax: 42
 """
 
 _TEMPLATE_BAM_OPTIONS = """  # Settings for aligners supported by the pipeline
   Aligners:
     # Choice of aligner software to use, either "BWA" or "Bowtie2"
     Program: BWA
```

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/nodes.py` & `paleomix-1.3.7/paleomix/pipelines/bam/nodes.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/parts/lane.py` & `paleomix-1.3.7/paleomix/pipelines/bam/parts/lane.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         )
 
     def _build_bwa_algorithm(self, config, prefix, record, parameters):
         if self.options["QualityOffset"] != 33:
             raise MakefileError(
                 "Mapping with BWA using the %r algorithm currently does not support "
                 "QualityOffsets other than 33; please convert your FASTQ if you wish "
-                "to proceed."
+                "to proceed." % (parameters["algorithm"],)
             )
 
         parameters = self._set_pe_input_files(parameters)
         parameters["mapping_options"] = self.options["Aligners"]["BWA"]
         parameters["cleanup_options"] = self._cleanup_options("BWA")
 
         return BWAAlgorithmNode(**parameters)
```

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/parts/library.py` & `paleomix-1.3.7/paleomix/pipelines/bam/parts/library.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/parts/prefix.py` & `paleomix-1.3.7/paleomix/pipelines/bam/parts/prefix.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/parts/reads.py` & `paleomix-1.3.7/paleomix/pipelines/bam/parts/reads.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/parts/sample.py` & `paleomix-1.3.7/paleomix/pipelines/bam/parts/sample.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/parts/statistics.py` & `paleomix-1.3.7/paleomix/pipelines/bam/parts/statistics.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/parts/summary.py` & `paleomix-1.3.7/paleomix/pipelines/bam/parts/summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,16 @@
             table.write("#     %s\n" % (os.getcwd()))
             table.write("#\n")
             self._write_genomes(table, genomes)
             table.write("#\n")
             self._write_areas_of_interest(table, rois)
             table.write("#\n#\n")
 
-            for roi in rois.values():
-                genomes[roi["Label"]] = {"Size": roi["Size"]}
+            for key, roi in rois.items():
+                genomes[":".join(key)] = {"Size": roi["Size"]}
             self._write_tables(table, genomes)
 
     def _teardown(self, _config, temp):
         move_file(reroot_path(temp, self._output_file), self._output_file)
 
     def _write_genomes(self, table, genomes):
         table.write("# Genomes:\n")
```

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/parts/target.py` & `paleomix-1.3.7/paleomix/pipelines/bam/parts/target.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/paths.py` & `paleomix-1.3.7/paleomix/pipelines/bam/paths.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/pipeline.py` & `paleomix-1.3.7/paleomix/pipelines/bam/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 import paleomix
 import paleomix.common.logging
 import paleomix.resources
 import paleomix.yaml
 
 from paleomix.pipeline import Pypeline
+from paleomix.node import NodeError
 from paleomix.nodes.samtools import FastaIndexNode
 from paleomix.nodes.bwa import BWAIndexNode
 from paleomix.nodes.bowtie2 import Bowtie2IndexNode
 from paleomix.nodes.validation import ValidateFASTAFilesNode
 
 from paleomix.pipelines.bam.makefile import MakefileError, read_makefiles
 
@@ -202,18 +203,17 @@
 
         pipeline_func = build_pipeline_full
 
     for makefile in makefiles:
         logger.info("Building BAM pipeline for %r", makefile["Filename"])
         try:
             nodes = pipeline_func(config, makefile)
-        except paleomix.node.NodeError as error:
-            logger.error(
-                "Error while building pipeline for %r:\n%s", makefile["Filename"], error
-            )
+        except (NodeError, MakefileError) as error:
+            logger.error("Error while building pipeline for %r", makefile["Filename"])
+            logger.error("%s", error)
             return 1
 
         pipeline.add_nodes(*nodes)
 
     if config.list_input_files:
         logger.info("Printing output files")
         pipeline.print_input_files()
```

### Comparing `paleomix-1.3.6/paleomix/pipelines/bam/trim_pipeline.py` & `paleomix-1.3.7/paleomix/pipelines/bam/trim_pipeline.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/phylo/__init__.py` & `paleomix-1.3.7/paleomix/pipelines/phylo/__init__.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/phylo/config.py` & `paleomix-1.3.7/paleomix/pipelines/phylo/config.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/phylo/example.py` & `paleomix-1.3.7/paleomix/pipelines/phylo/example.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/phylo/makefile.py` & `paleomix-1.3.7/paleomix/pipelines/phylo/makefile.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/phylo/mkfile.py` & `paleomix-1.3.7/paleomix/pipelines/phylo/mkfile.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/phylo/parts/__init__.py` & `paleomix-1.3.7/paleomix/pipelines/phylo/parts/__init__.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/phylo/parts/genotype.py` & `paleomix-1.3.7/paleomix/pipelines/phylo/parts/genotype.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/phylo/parts/msa.py` & `paleomix-1.3.7/paleomix/pipelines/phylo/parts/msa.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/phylo/parts/phylo.py` & `paleomix-1.3.7/paleomix/pipelines/phylo/parts/phylo.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/phylo/pipeline.py` & `paleomix-1.3.7/paleomix/pipelines/phylo/pipeline.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/__init__.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/__init__.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/build_db.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/build_db.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/build_mito.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/build_mito.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/build_tped.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/build_tped.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/common.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/common.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/config.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/config.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/database.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/database.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/parts/__init__.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/parts/__init__.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/parts/admixture.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/parts/admixture.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/parts/common.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/parts/common.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/parts/mitochondria.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/parts/mitochondria.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/parts/nuclear.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/parts/nuclear.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/parts/report.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/parts/report.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/parts/summary.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/parts/summary.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/pipelines/zonkey/pipeline.py` & `paleomix-1.3.7/paleomix/pipelines/zonkey/pipeline.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/__init__.py` & `paleomix-1.3.7/paleomix/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_01.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_01.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_02.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_02.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_03.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_03.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_04.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R1_04.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_01.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_01.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_02.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_02.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_03.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_03.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_04.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L1_R2_04.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/ACGATA_L2/reads.collapsed.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/ACGATA_L2/reads.collapsed.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/GCTCTG_L1_R1_01.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/GCTCTG_L1_R1_01.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/GCTCTG_L1_R1_02.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/GCTCTG_L1_R1_02.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/GCTCTG_L1_R1_03.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/GCTCTG_L1_R1_03.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L1_R1_01.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L1_R1_01.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L1_R1_02.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L1_R1_02.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L1_R1_03.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L1_R1_03.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R1_01.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R1_01.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R1_02.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R1_02.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R1_03.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R1_03.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R2_01.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R2_01.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R2_02.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R2_02.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R2_03.fastq.gz` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/data/TGCTCA_L2_R2_03.fastq.gz`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/makefile.yaml` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/makefile.yaml`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/bam_pipeline/prefixes/rCRS.fasta` & `paleomix-1.3.7/paleomix/resources/examples/bam_pipeline/prefixes/rCRS.fasta`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/makefile.yaml` & `paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/makefile.yaml`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/bonobo.fasta` & `paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/bonobo.fasta`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/chimpanzee.fasta` & `paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/chimpanzee.fasta`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/gorilla.fasta` & `paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/gorilla.fasta`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/rCRS.fasta` & `paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/rCRS.fasta`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/sumatran_orangutan.fasta` & `paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/sumatran_orangutan.fasta`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/white_handed_gibbon.fasta` & `paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/prefixes/white_handed_gibbon.fasta`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/alignment/setup.sh` & `paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/alignment/setup.sh`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/phylogeny/data/regions/rCRS.protein_coding.CDS.bed` & `paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/phylogeny/data/regions/rCRS.protein_coding.CDS.bed`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/phylogeny/makefile.yaml` & `paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/phylogeny/makefile.yaml`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/setup.sh` & `paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/setup.sh`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/examples/phylo_pipeline/synthesize_reads.py` & `paleomix-1.3.7/paleomix/resources/examples/phylo_pipeline/synthesize_reads.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/reports/zonkey/report.css` & `paleomix-1.3.7/paleomix/resources/reports/zonkey/report.css`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/rscripts/common/requires.r` & `paleomix-1.3.7/paleomix/resources/rscripts/common/requires.r`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/rscripts/zonkey/admixture.r` & `paleomix-1.3.7/paleomix/resources/rscripts/zonkey/admixture.r`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/rscripts/zonkey/coverage.r` & `paleomix-1.3.7/paleomix/resources/rscripts/zonkey/coverage.r`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/rscripts/zonkey/pca.r` & `paleomix-1.3.7/paleomix/resources/rscripts/zonkey/pca.r`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/rscripts/zonkey/tinytree.r` & `paleomix-1.3.7/paleomix/resources/rscripts/zonkey/tinytree.r`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/resources/rscripts/zonkey/treemix.r` & `paleomix-1.3.7/paleomix/resources/rscripts/zonkey/treemix.r`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/tools/__init__.py` & `paleomix-1.3.7/paleomix/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/tools/bam_stats/common.py` & `paleomix-1.3.7/paleomix/tools/bam_stats/common.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/tools/bam_stats/coverage.py` & `paleomix-1.3.7/paleomix/tools/bam_stats/coverage.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/tools/cleanup.py` & `paleomix-1.3.7/paleomix/tools/cleanup.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/tools/coverage.py` & `paleomix-1.3.7/paleomix/tools/coverage.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/tools/depths.py` & `paleomix-1.3.7/paleomix/tools/depths.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/tools/dupcheck.py` & `paleomix-1.3.7/paleomix/tools/dupcheck.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/tools/factory.py` & `paleomix-1.3.7/paleomix/tools/factory.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/tools/gtf_to_bed.py` & `paleomix-1.3.7/paleomix/tools/gtf_to_bed.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/tools/rmdup_collapsed.py` & `paleomix-1.3.7/paleomix/tools/rmdup_collapsed.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/tools/validate_fastq.py` & `paleomix-1.3.7/paleomix/tools/validate_fastq.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/tools/vcf_filter.py` & `paleomix-1.3.7/paleomix/tools/vcf_filter.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/tools/vcf_to_fasta.py` & `paleomix-1.3.7/paleomix/tools/vcf_to_fasta.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix/yaml.py` & `paleomix-1.3.7/paleomix/yaml.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/paleomix.egg-info/PKG-INFO` & `paleomix-1.3.7/paleomix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: paleomix
-Version: 1.3.6
+Version: 1.3.7
 Summary: Bioinformatics pipelines for HTS data
 Home-page: https://github.com/MikkelSchubert/paleomix
 Author: Mikkel Schubert
 Author-email: MikkelSch@gmail.com
 License: MIT
 Description: **********************
         The PALEOMIX pipelines
```

### Comparing `paleomix-1.3.6/paleomix.egg-info/SOURCES.txt` & `paleomix-1.3.7/paleomix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/setup.py` & `paleomix-1.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/atomiccmd_test/__init__.py` & `paleomix-1.3.7/tests/atomiccmd_test/__init__.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/atomiccmd_test/builder_test.py` & `paleomix-1.3.7/tests/atomiccmd_test/builder_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/atomiccmd_test/command_test.py` & `paleomix-1.3.7/tests/atomiccmd_test/command_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/atomiccmd_test/pprint_test.py` & `paleomix-1.3.7/tests/atomiccmd_test/pprint_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/atomiccmd_test/sets_test.py` & `paleomix-1.3.7/tests/atomiccmd_test/sets_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/__init__.py` & `paleomix-1.3.7/tests/common_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/bedtools_test.py` & `paleomix-1.3.7/tests/common_tests/bedtools_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/fileutils_test.py` & `paleomix-1.3.7/tests/common_tests/fileutils_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/formats_tests/__init__.py` & `paleomix-1.3.7/tests/common_tests/formats_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/formats_tests/fasta_test.py` & `paleomix-1.3.7/tests/common_tests/formats_tests/fasta_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/formats_tests/fastq_test.py` & `paleomix-1.3.7/tests/common_tests/formats_tests/fastq_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/formats_tests/msa_test.py` & `paleomix-1.3.7/tests/common_tests/formats_tests/msa_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/formats_tests/newick_test.py` & `paleomix-1.3.7/tests/common_tests/formats_tests/newick_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/formats_tests/phylip_test.py` & `paleomix-1.3.7/tests/common_tests/formats_tests/phylip_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/makefile_test.py` & `paleomix-1.3.7/tests/common_tests/makefile_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/sampling_test.py` & `paleomix-1.3.7/tests/common_tests/sampling_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/sequences_test.py` & `paleomix-1.3.7/tests/common_tests/sequences_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/text_test.py` & `paleomix-1.3.7/tests/common_tests/text_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/utilities_test.py` & `paleomix-1.3.7/tests/common_tests/utilities_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/common_tests/versions_test.py` & `paleomix-1.3.7/tests/common_tests/versions_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/data/rCRS.fasta` & `paleomix-1.3.7/tests/data/rCRS.fasta`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/node_test.py` & `paleomix-1.3.7/tests/node_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/nodegraph_test.py` & `paleomix-1.3.7/tests/nodegraph_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tests/tools_test/factory_test.py` & `paleomix-1.3.7/tests/tools_test/factory_test.py`

 * *Files identical despite different names*

### Comparing `paleomix-1.3.6/tox.ini` & `paleomix-1.3.7/tox.ini`

 * *Files identical despite different names*

