# Comparing `tmp/wgd-2.0.13.tar.gz` & `tmp/wgd-2.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wgd-2.0.13.tar", last modified: Wed May 17 12:42:30 2023, max compression
+gzip compressed data, was "dist/wgd-2.0.14.tar", last modified: Fri May 19 19:43:05 2023, max compression
```

## Comparing `wgd-2.0.13.tar` & `wgd-2.0.14.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-17 12:42:30.193328 wgd-2.0.13/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.13/LICENSE
--rwxrwxrwx   0 heche     (1000) heche     (1000)    34148 2023-05-17 12:42:30.195320 wgd-2.0.13/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)    30341 2023-05-10 06:37:55.000000 wgd-2.0.13/README.md
--rwxrwxrwx   0 heche     (1000) heche     (1000)    48990 2023-05-11 09:03:45.000000 wgd-2.0.13/cli.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-17 12:42:30.196325 wgd-2.0.13/setup.cfg
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1895 2023-05-17 12:39:50.000000 wgd-2.0.13/setup.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-17 12:42:30.163813 wgd-2.0.13/test/
--rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-05-08 19:45:47.000000 wgd-2.0.13/test/test_core.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-17 12:42:30.184322 wgd-2.0.13/wgd/
--rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.13/wgd/__init__.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.13/wgd/beast.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.13/wgd/cluster.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.13/wgd/codeml.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   134351 2023-05-10 07:50:19.000000 wgd-2.0.13/wgd/core.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.13/wgd/mcmctree.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.13/wgd/mix.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   103647 2023-05-10 05:58:49.000000 wgd-2.0.13/wgd/peak.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     8513 2023-05-08 19:45:47.000000 wgd-2.0.13/wgd/syn.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    28648 2022-09-30 07:30:21.000000 wgd-2.0.13/wgd/utils.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    95109 2023-05-09 11:58:52.000000 wgd-2.0.13/wgd/viz.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-17 12:42:30.192319 wgd-2.0.13/wgd.egg-info/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    34148 2023-05-17 12:42:30.000000 wgd-2.0.13/wgd.egg-info/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)      369 2023-05-17 12:42:30.000000 wgd-2.0.13/wgd.egg-info/SOURCES.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-17 12:42:30.000000 wgd-2.0.13/wgd.egg-info/dependency_links.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       51 2023-05-17 12:42:30.000000 wgd-2.0.13/wgd.egg-info/entry_points.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)      740 2023-05-17 12:42:30.000000 wgd-2.0.13/wgd.egg-info/requires.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-05-17 12:42:30.000000 wgd-2.0.13/wgd.egg-info/top_level.txt
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-19 19:43:05.427006 wgd-2.0.14/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.14/LICENSE
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    36301 2023-05-19 19:43:05.427006 wgd-2.0.14/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    36063 2023-05-19 19:40:15.000000 wgd-2.0.14/README.md
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    49510 2023-05-19 17:07:00.000000 wgd-2.0.14/cli.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-19 19:43:05.428024 wgd-2.0.14/setup.cfg
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1904 2023-05-19 19:42:30.000000 wgd-2.0.14/setup.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-19 19:43:05.402999 wgd-2.0.14/test/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-05-08 19:45:47.000000 wgd-2.0.14/test/test_core.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-19 19:43:05.419001 wgd-2.0.14/wgd/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.14/wgd/__init__.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.14/wgd/beast.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.14/wgd/cluster.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.14/wgd/codeml.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   134238 2023-05-19 10:45:47.000000 wgd-2.0.14/wgd/core.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.14/wgd/mcmctree.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.14/wgd/mix.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   103647 2023-05-10 05:58:49.000000 wgd-2.0.14/wgd/peak.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     8513 2023-05-08 19:45:47.000000 wgd-2.0.14/wgd/syn.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    28648 2022-09-30 07:30:21.000000 wgd-2.0.14/wgd/utils.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    95587 2023-05-19 19:32:45.000000 wgd-2.0.14/wgd/viz.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-19 19:43:05.425025 wgd-2.0.14/wgd.egg-info/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    36301 2023-05-19 19:43:05.000000 wgd-2.0.14/wgd.egg-info/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      369 2023-05-19 19:43:05.000000 wgd-2.0.14/wgd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-19 19:43:05.000000 wgd-2.0.14/wgd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       32 2023-05-19 19:43:05.000000 wgd-2.0.14/wgd.egg-info/entry_points.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      749 2023-05-19 19:43:05.000000 wgd-2.0.14/wgd.egg-info/requires.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-05-19 19:43:05.000000 wgd-2.0.14/wgd.egg-info/top_level.txt
```

### Comparing `wgd-2.0.13/LICENSE` & `wgd-2.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `wgd-2.0.13/PKG-INFO` & `wgd-2.0.14/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,456 +1,505 @@
-Metadata-Version: 2.1
-Name: wgd
-Version: 2.0.13
-Summary: wgd
-Home-page: http://github.com/heche-psb/wgd
-Author: Hengchi Chen
-Author-email: heche@psb.vib-ugent.be
-License: GPL
-Description: <div align="center">
-        
-        # `wgd v2` : a suite tool of WGD inference and timing
-        
-        [![Build Status](https://app.travis-ci.com/heche-psb/wgd.svg?branch=phylodating)](https://travis-ci.com/heche-psb/wgd)
-        
-        **Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
-        
-        [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
-        
-        [**Introduction**](#Introduction) | 
-        [**Installation**](#Installation) | 
-        [**Parameters**](#Parameters) | 
-        [**Usage**](#Usage) | 
-        [**Illustration**](#Illustration) |
-        [**Citation**](#Citation)
-        
-        </div>
-        
-        `wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
-        
-        ## Introduction
-        
-        Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
-        
-        The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
-        
-        ## Installation
-        
-        The easiest way to install `wgd v2` is using PYPI
-        
-        ```
-        pip install wgd
-        ```
-        
-        To install `wgd v2` in a virtual environment, the following command lines could be used.
-        
-        ```
-        git clone <wgd repo>
-        cd wgd
-        virtualenv -p=python3 ENV (or python3 -m venv ENV)
-        source ENV/bin/activate
-        pip install -r requirements.txt
-        pip install .
-        ```
-        
-        When met with permission problem in installation, please try the following command line.
-        
-        ```
-        pip install -e .
-        ```
-        
-        If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
-        
-        ```
-        export PATH="$PATH:~/.local/bin/wgd"
-        ```
-        
-        ## Parameters
-        
-        There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
-        
-        The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
-        ```
-        wgd dmd sequences (option)
-        --------------------------------------------------------------------------------
-        -o, --outdir, the output directory, default wgd_dmd
-        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
-        -c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
-        -I, --inflation, the inflation factor for MCL program, default 2.0
-        -e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
-        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
-        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
-        -f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
-        -ap, --anchorpoints, the anchor points data file, default None
-        -coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
-        -sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
-        -le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
-        -gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
-        -kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
-        -kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
-        -gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
-        -n, --nthreads, the number of threads to use, default 4
-        -oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
-        -oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
-        -gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
-        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
-        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
-        -mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
-        -ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
-        -am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
-        -sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
-        -fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
-        -cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
-        -te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
-        -bs, --bins, the number of bins divided in gene length normalization, default 100
-        -np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
-        -nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
-        -bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
-        -bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
-        -bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
-        ```
-        
-        The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
-        ```
-        wgd focus families sequences (option)
-        --------------------------------------------------------------------------------
-        -o, --outdir, the output directory, default wgd_focus
-        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
-        -n, --nthreads, the number of threads to use, default 4
-        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
-        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
-        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
-        -a, --aligner, which alignment program to use, default mafft
-        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
-        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
-        --concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
-        --coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
-        -sp, --speciestree, species tree darafile for dating, default None
-        -d, --dating, which molecular dating program to use, default none
-        -ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
-        -ns, --nsites, the nsites information for r8s dating, default None
-        -ot, --outgroup, the outgroup information for r8s dating, default None
-        -pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
-        -am, --aamodel, which protein model to be used in mcmctree, default poisson
-        -ks, flag option, whether to initiate Ks analysis
-        --annotation, which annotation program to use, default none
-        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
-        -ed, --eggnogdata, the eggnog annotation datafile, default None
-        --pfam, which option to use for pfam annotation, default none
-        --dmnb, the diamond database for annotation, default None
-        --hmm, the HMM profile for annotation, default None
-        --evalue, the e-value cut-off for annotation, default 1e-10
-        --exepath, the path to the interproscan executable, default None
-        -f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
-         -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
-        -cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
-        --beastlgjar, the path to beastLG.jar, default None
-        --beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
-        --protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
-        ```
-        
-        The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
-        ```
-        wgd ksd families sequences (option)
-        --------------------------------------------------------------------------------
-        -o, --outdir, the output directory, default wgd_ksd
-        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
-        -n, --nthreads, the number of threads to use, default 4
-        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
-        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
-        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
-        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
-        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
-        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
-        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
-        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
-        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
-        ```
-        
-        The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
-        ```
-        wgd mix ks_datafile (option)
-        --------------------------------------------------------------------------------
-        -f, --filters, the cutoff alignment length, default 300
-        -r, --ks_range, the Ks range to be considered, default (0.005, 3)
-        -b, --bins, the number of bins in Ks distribution, default 50
-        -o, --outdir, the output directory, default wgd_mix
-        --method, which mixture model to use, default gmm
-        -n, --components, the range of the number of components to fit, default (1, 4)
-        -g, --gamma, the gamma parameter for bgmm models, default 0.001
-        -ni, --n_init, the number of k-means initializations, default 200
-        -mi, --max_iter, the maximum number of iterations, default 1000
-        ```
-        
-        The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
-        ```
-        wgd peak ks_datafile (option)
-        --------------------------------------------------------------------------------
-        -ap, --anchorpoints, the anchor points datafile, default None
-        -sm, --segments, the segments datafile, default None
-        -le, --listelements, the listsegments datafile, default None 
-        -mp, --multipliconpairs, the multipliconpairs datafile, default None
-        -o, --outdir, the output directory, default wgd_peak
-        -af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
-        -r, --ksrange, range of Ks to be analyzed, default (0, 5)
-        -bw, --bin_width, bandwidth of Ks distribution, default 0.1
-        -ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
-        -m, --method, which mixture model to use, default gmm
-        --seed, random seed given to initialization, default 2352890
-        -ei, --em_iter, the number of EM iterations to perform, default 200
-        -ni, --n_init, the number of k-means initializations, default 200
-        -n, --components, the range of the number of components to fit, default (1, 4)
-        --boots, the number of bootstrap replicates of kde, default 200
-        --weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
-        -p, --plot, the plotting method to be used, default identical
-        -bm, --bw_method, the bandwidth method to be used, default silverman
-        --n_medoids, the number of medoids to fit, default 2
-        -km, --kdemethod, the kde method to be used, default scipy
-        --n_clusters, the number of clusters to plot Elbow loss function, default 5
-        --kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
-        -gd, --guide, the regime residing anchors, default: segment
-        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
-        -kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
-        -f, --family, the family to filter Ks upon, default None
-        --manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
-        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
-        --ci, the confidence level of log-normal distribution to date, default 95
-        --hdr, the highest densidy region (HDR) in a given distribution to date, default 95
-        --heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
-        -kc, --kscutoff, the Ks saturation cutoff in dating, default 5
-        ```
-        
-        The program `wgd syn` can realize the intra- and inter-specific synteny inference.
-        ```
-        wgd syn families gffs (option)
-        --------------------------------------------------------------------------------
-        -ks, --ks_distribution, ks distribution datafile, default None
-        -o, --outdir, the output directory, default wgd_syn
-        -f, --feature, the feature for parsing gene IDs from GFF files, default gene
-        -a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
-        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
-        -ms, --maxsize, the maximum family size to include, default 200
-        -r, --ks_range, the Ks range in colored dotplot, default (0, 5)
-        --iadhore_options, the parameter setting in iadhore, default 
-        -ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
-        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
-        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-        ```
-        
-        The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
-        ```
-        wgd viz (option)
-        --------------------------------------------------------------------------------
-        -d, --datafile, the Ks datafile, default None
-        -o, --outdir, the output directory, default wgd_viz
-        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
-        -gs, --gsmap, the gene name-species name map, default None
-        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
-        -pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
-        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
-        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
-        -iter, --em_iterations, the maximum EM iterations, default 200
-        -init, --em_initializations, the maximum EM initializations, default 200
-        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
-        -sm, --segments, the segments data file, default None
-        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
-        -ms, --maxsize, the maximum family size to include, default 200
-        -ap, --anchorpoints, the anchor points datafile, default None
-        -mt, --multiplicon, the multiplicons datafile, default None
-        -gt, --genetable, the gene table datafile, default None
-        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
-        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
-        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-        ```
-        
-        ## Usage
-        
-        Here we provided the basic usage for each program.
-        
-        ### wgd dmd
-        
-        **The delineation of whole paranome**
-        ```
-        wgd dmd sequence
-        ``` 
-        
-        **The delineation of RBHs**
-        ```
-        wgd dmd sequence1 sequence2
-        ```
-        
-        **The delineation of local MRBHs**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -f sequence1
-        ```
-        
-        **The delineation of global MRBHs**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -gm
-        ```
-        
-        **The delineation of orthogroups**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -oi (option)
-        ```
-        Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
-        
-        **The collinear coalescence inference of phylogeny**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
-        ```
-        
-        ### wgd focus
-        
-        **The concatenation-based/coalescence-based phylogenetic inference**
-        ```
-        wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
-        ```
-        
-        **The functional annotation of gene families**
-        ```
-        wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
-        ```
-        
-        **The phylogenetic dating of WGDs**
-        ```
-        wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
-        ```
-        
-        ### wgd ksd
-        
-        **The construction of whole paranome *K*<sub>S</sub> age distribution**
-        ```
-        wgd ksd families sequence
-        ```
-        
-        **The construction of orthologous *K*<sub>S</sub> age distribution**
-        ```
-        wgd ksd families sequence1 sequence2
-        ```
-        
-        **The construction of *K*<sub>S</sub> age distribution with rate correction**
-        ```
-        wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
-        ```
-        
-        ### wgd mix
-        
-        **The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
-        ```
-        wgd mix ksdata
-        ```
-        
-        ### wgd peak
-        
-        **The search of crediable *K*<sub>S</sub> range used in WGD dating**
-        ```
-        wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
-        ```
-        Note that users can add the flag --heuristic to implement the heuristic search analysis
-        
-        ### wgd syn
-        
-        **The intra-specific synteny inference**
-        ```
-        wgd syn families gff
-        ```
-        
-        **The inter-specific synteny inference**
-        ```
-        wgd syn families gff1 gff2
-        ```
-        
-        ### wgd viz
-        
-        **The visualization of *K*<sub>S</sub> age distribution**
-        ```
-        wgd viz -d ksdata
-        ```
-        
-        **The visualization of *K*<sub>S</sub> age distribution with rate correction**
-        ```
-        wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
-        ```
-        
-        **The visualization of synteny**
-        ```
-        wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
-        ```
-        
-        ## Illustration
-        
-        We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
-        
-        The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
-        
-        First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
-        
-        ```
-        wgd dmd Aquilegia_coerulea
-        wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
-        ```
-        
-        The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
-        
-        ![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
-        
-        We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
-        
-        ```
-        wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
-        ```
-        
-        As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
-        
-        ![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
-        
-        The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes, except for the chr_07, which seems to experience more severe fragmentization than the other chromosomes.
-        
-        ![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
-        
-        The associated dotplot in oxford grid also presents numerous densely aggregated anchor points throughout most of the chromosomes.
-        
-        ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
-        
-        A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
-        
-        ![](data/Syndepth.svg)
-        
-        We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
-        
-        ```
-        wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
-        ```
-        
-        The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
-        
-        ![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
-        
-        Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
-        
-        ```
-        wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
-        ```
-        
-        The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
-        
-        ![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
-        
-        Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis.
-        
-        ## Citation
-         
-        Please cite us at https://doi.org/10.1093/bioinformatics/bty915
-        
-        ```
-        Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
-        
-        Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
-        ```
-        
-        For citation of the tools used in wgd, please consult the documentation at
-        https://wgd.readthedocs.io/en/latest/index.html#citation.
-        
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+<div align="center">
+
+# `wgd v2` : a suite tool of WGD inference and timing
+
+**Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
+
+[**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
+
+[**Introduction**](#Introduction) | 
+[**Installation**](#Installation) | 
+[**Parameters**](#Parameters) | 
+[**Usage**](#Usage) | 
+[**Illustration**](#Illustration) |
+[**Citation**](#Citation)
+
+</div>
+
+`wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
+
+## Introduction
+
+Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
+
+The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
+
+## Installation
+
+The easiest way to install `wgd v2` is using PYPI
+
+```
+pip install wgd
+```
+
+To install `wgd v2` in a virtual environment, the following command lines could be used.
+
+```
+git clone <wgd repo>
+cd wgd
+virtualenv -p=python3 ENV (or python3 -m venv ENV)
+source ENV/bin/activate
+pip install -r requirements.txt
+pip install .
+```
+
+When met with permission problem in installation, please try the following command line.
+
+```
+pip install -e .
+```
+
+If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
+
+```
+export PATH="$PATH:~/.local/bin/wgd"
+```
+
+Note that the version of `numpy` is important (for many other packages are the same of course), especially for `fastcluster` package. In our test, the `numpy` 1.19.0 works fine on `python3.6/8`. If you met some errors or warnings about numpy, maybe considering pre-install `numpy` as 1.19.0 or other close-by versions before you install `wgd`.
+
+## Parameters
+
+There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
+
+The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
+```
+wgd dmd sequences (option)
+--------------------------------------------------------------------------------
+-o, --outdir, the output directory, default wgd_dmd
+-t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+-c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
+-I, --inflation, the inflation factor for MCL program, default 2.0
+-e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
+--to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+--cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+-f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
+-ap, --anchorpoints, the anchor points data file, default None
+-coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
+-sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
+-le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
+-gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
+-kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
+-kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
+-gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
+-n, --nthreads, the number of threads to use, default 4
+-oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
+-oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
+-gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
+-tree, --tree_method, which gene tree inference program to invoke, default fasttree
+-ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+-mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
+-ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
+-am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
+-sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
+-fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
+-cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
+-te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
+-bs, --bins, the number of bins divided in gene length normalization, default 100
+-np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
+-nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
+-bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
+-bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
+-bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
+```
+
+The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
+```
+wgd focus families sequences (option)
+--------------------------------------------------------------------------------
+-o, --outdir, the output directory, default wgd_focus
+-t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+-n, --nthreads, the number of threads to use, default 4
+--to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+--cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+--strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+-a, --aligner, which alignment program to use, default mafft
+-tree, --tree_method, which gene tree inference program to invoke, default fasttree
+-ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+--concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
+--coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
+-sp, --speciestree, species tree darafile for dating, default None
+-d, --dating, which molecular dating program to use, default none
+-ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
+-ns, --nsites, the nsites information for r8s dating, default None
+-ot, --outgroup, the outgroup information for r8s dating, default None
+-pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
+-am, --aamodel, which protein model to be used in mcmctree, default poisson
+-ks, flag option, whether to initiate Ks analysis
+--annotation, which annotation program to use, default none
+--pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+-ed, --eggnogdata, the eggnog annotation datafile, default None
+--pfam, which option to use for pfam annotation, default none
+--dmnb, the diamond database for annotation, default None
+--hmm, the HMM profile for annotation, default None
+--evalue, the e-value cut-off for annotation, default 1e-10
+--exepath, the path to the interproscan executable, default None
+-f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
+ -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
+-cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
+--beastlgjar, the path to beastLG.jar, default None
+--beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
+--protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
+```
+
+The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
+```
+wgd ksd families sequences (option)
+--------------------------------------------------------------------------------
+-o, --outdir, the output directory, default wgd_ksd
+-t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+-n, --nthreads, the number of threads to use, default 4
+--to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+--cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+--pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+--strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+-tree, --tree_method, which gene tree inference program to invoke, default fasttree
+-sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+-sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+-rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+-or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+```
+
+The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
+```
+wgd mix ks_datafile (option)
+--------------------------------------------------------------------------------
+-f, --filters, the cutoff alignment length, default 300
+-r, --ks_range, the Ks range to be considered, default (0.005, 3)
+-b, --bins, the number of bins in Ks distribution, default 50
+-o, --outdir, the output directory, default wgd_mix
+--method, which mixture model to use, default gmm
+-n, --components, the range of the number of components to fit, default (1, 4)
+-g, --gamma, the gamma parameter for bgmm models, default 0.001
+-ni, --n_init, the number of k-means initializations, default 200
+-mi, --max_iter, the maximum number of iterations, default 1000
+```
+
+The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
+```
+wgd peak ks_datafile (option)
+--------------------------------------------------------------------------------
+-ap, --anchorpoints, the anchor points datafile, default None
+-sm, --segments, the segments datafile, default None
+-le, --listelements, the listsegments datafile, default None 
+-mp, --multipliconpairs, the multipliconpairs datafile, default None
+-o, --outdir, the output directory, default wgd_peak
+-af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
+-r, --ksrange, range of Ks to be analyzed, default (0, 5)
+-bw, --bin_width, bandwidth of Ks distribution, default 0.1
+-ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
+-m, --method, which mixture model to use, default gmm
+--seed, random seed given to initialization, default 2352890
+-ei, --em_iter, the number of EM iterations to perform, default 200
+-ni, --n_init, the number of k-means initializations, default 200
+-n, --components, the range of the number of components to fit, default (1, 4)
+--boots, the number of bootstrap replicates of kde, default 200
+--weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
+-p, --plot, the plotting method to be used, default identical
+-bm, --bw_method, the bandwidth method to be used, default silverman
+--n_medoids, the number of medoids to fit, default 2
+-km, --kdemethod, the kde method to be used, default scipy
+--n_clusters, the number of clusters to plot Elbow loss function, default 5
+--kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
+-gd, --guide, the regime residing anchors, default: segment
+-prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+-kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
+-f, --family, the family to filter Ks upon, default None
+--manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
+-rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+--ci, the confidence level of log-normal distribution to date, default 95
+--hdr, the highest densidy region (HDR) in a given distribution to date, default 95
+--heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
+-kc, --kscutoff, the Ks saturation cutoff in dating, default 5
+```
+
+The program `wgd syn` can realize the intra- and inter-specific synteny inference.
+```
+wgd syn families gffs (option)
+--------------------------------------------------------------------------------
+-ks, --ks_distribution, ks distribution datafile, default None
+-o, --outdir, the output directory, default wgd_syn
+-f, --feature, the feature for parsing gene IDs from GFF files, default gene
+-a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
+-ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+-ms, --maxsize, the maximum family size to include, default 200
+-r, --ks_range, the Ks range in colored dotplot, default (0, 5)
+--iadhore_options, the parameter setting in iadhore, default 
+-ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
+-mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+-kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+```
+
+The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
+```
+wgd viz (option)
+--------------------------------------------------------------------------------
+-d, --datafile, the Ks datafile, default None
+-o, --outdir, the output directory, default wgd_viz
+-sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+-gs, --gsmap, the gene name-species name map, default None
+-sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+-pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
+-rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+-or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+-iter, --em_iterations, the maximum EM iterations, default 200
+-init, --em_initializations, the maximum EM initializations, default 200
+-prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+-sm, --segments, the segments data file, default None
+-ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+-ms, --maxsize, the maximum family size to include, default 200
+-ap, --anchorpoints, the anchor points datafile, default None
+-mt, --multiplicon, the multiplicons datafile, default None
+-gt, --genetable, the gene table datafile, default None
+-rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+-mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+-kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+```
+
+## Usage
+
+Here we provided the basic usage for each program.
+
+### wgd dmd
+
+**The delineation of whole paranome**
+```
+wgd dmd sequence
+``` 
+
+**The delineation of RBHs**
+```
+wgd dmd sequence1 sequence2
+```
+
+**The delineation of local MRBHs**
+```
+wgd dmd sequence1 sequence2 sequence3 -f sequence1
+```
+
+**The delineation of global MRBHs**
+```
+wgd dmd sequence1 sequence2 sequence3 -gm
+```
+
+**The delineation of orthogroups**
+```
+wgd dmd sequence1 sequence2 sequence3 -oi (option)
+```
+Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
+
+**The collinear coalescence inference of phylogeny**
+```
+wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
+```
+
+### wgd focus
+
+**The concatenation-based/coalescence-based phylogenetic inference**
+```
+wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
+```
+
+**The functional annotation of gene families**
+```
+wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
+```
+
+**The phylogenetic dating of WGDs**
+```
+wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
+```
+
+### wgd ksd
+
+**The construction of whole paranome *K*<sub>S</sub> age distribution**
+```
+wgd ksd families sequence
+```
+
+**The construction of orthologous *K*<sub>S</sub> age distribution**
+```
+wgd ksd families sequence1 sequence2
+```
+
+**The construction of *K*<sub>S</sub> age distribution with rate correction**
+```
+wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
+```
+
+### wgd mix
+
+**The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
+```
+wgd mix ksdata
+```
+
+### wgd peak
+
+**The search of crediable *K*<sub>S</sub> range used in WGD dating**
+```
+wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
+```
+Note that users can add the flag --heuristic to implement the heuristic search analysis
+
+### wgd syn
+
+**The intra-specific synteny inference**
+```
+wgd syn families gff
+```
+
+**The inter-specific synteny inference**
+```
+wgd syn families gff1 gff2
+```
+
+### wgd viz
+
+**The visualization of *K*<sub>S</sub> age distribution**
+```
+wgd viz -d ksdata
+```
+
+**The visualization of *K*<sub>S</sub> age distribution with rate correction**
+```
+wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
+```
+
+**The visualization of synteny**
+```
+wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
+```
+
+## Illustration
+
+We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
+
+The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
+
+First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
+
+```
+wgd dmd Aquilegia_coerulea
+wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
+```
+
+The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
+
+![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
+
+We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
+
+```
+wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+```
+
+As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
+
+![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
+
+The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes, except for the chr_07, which seems to experience more severe fragmentization than the other chromosomes.
+
+![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
+
+The associated dotplot in oxford grid also presents numerous densely aggregated anchor points throughout most of the chromosomes.
+
+![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
+
+A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
+
+![](data/Syndepth.svg)
+
+We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
+
+```
+wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+```
+
+The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
+
+![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
+
+Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
+
+```
+wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
+```
+
+The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
+
+![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
+
+Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis. First, we built a global MRBH family using the command below.
+
+```
+wgd dmd --globalmrbh Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera -o wgd_globalmrbh
+```
+
+In the global MRBH family, every pair of orthologous genes is the reciprocal best hit, suggesting true orthologous relationships. We would use the *K*<sub>S</sub> values associated with these orthologous pairs to delimit the divergence *K*<sub>S</sub> peak. Together with the whole paranome *K*<sub>S</sub> distribution, we conduct the rate correction using the command below.
+
+```
+wgd ksd wgd_globalmrbh/global_MRBH.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
+```
+
+The file `speciestree.nw` is the text file of species tree in newick that rate correction would be conducted on. Its content is as below. Users need to provide the species pairs to be plotted. We suggest adding the option `--reweight` to recalculate the weight per species pair such that the weight of orthologous gene pairs will become 1 as the paralogous gene pairs. The flag `--plotkde` can be added when the kde curve of orthologous *K*<sub>S</sub> is desired. Extra collinear data can be added by the option `-ap`.
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
+
+As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
+
+```
+(((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
+```
+
+If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
+```
+
+Note that a necessary gene-species map file is needed for its implementation in `wgd viz`, which should be automately produced by the last `wgd ksd` step. The `gene_species.map` has contents as below in which each line is the joined string of gene name and species name by space.
+
+```
+Aqcoe6G057800.1 Aquilegia_coerulea
+Vvi_VIT_201s0011g01530.1 Vitis_vinifera
+Pcy_Procy01g08510 Protea_cynaroides
+Aam_Acora.04G142900.1 Acorus_americanus
+```
+
+An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
+
+```
+wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
+```
+
+Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
+
+```
+wgd ksd wgd_ortho/Orthogroups.sp.tsv -sp speciestree.nw --reweight -o wgd_ortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
+```
+
+![](data/Aquilegia_coerulea_OrthoKs_Corrected.ksd.svg)
+
+As shown above, the number of both paralogous gene pairs and orthologous gene pairs is different than the one from global MRBH family in that here we plotted all orthologous gene pairs instead of only global MRBH and potentially new paralogous gene pairs might be produced in the orthogroup inference step, together with different recalculated weights.
+
+If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
+
+```
+wgd ksd wgd_globalmrbh/global_MRBH.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus"
+```
+
+We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
+![](data/Raw_Orthologues.ksd.svg)
+
+## Citation
+ 
+Please cite us at https://doi.org/10.1093/bioinformatics/bty915
+
+```
+Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
+
+Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
+```
+
+For citation of the tools used in wgd, please consult the documentation at
+https://wgd.readthedocs.io/en/latest/index.html#citation.
+
```

### Comparing `wgd-2.0.13/README.md` & `wgd-2.0.14/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,22 @@
+Metadata-Version: 2.1
+Name: wgd
+Version: 2.0.14
+Summary: wgd
+Home-page: http://github.com/heche-psb/wgd
+Author: Hengchi Chen
+Author-email: heche@psb.vib-ugent.be
+License: GPL
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 
 # `wgd v2` : a suite tool of WGD inference and timing
 
-[![Build Status](https://app.travis-ci.com/heche-psb/wgd.svg?branch=phylodating)](https://travis-ci.com/heche-psb/wgd)
-
 **Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
 
 [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
 
 [**Introduction**](#Introduction) | 
 [**Installation**](#Installation) | 
 [**Parameters**](#Parameters) | 
@@ -52,14 +61,16 @@
 
 If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
 
 ```
 export PATH="$PATH:~/.local/bin/wgd"
 ```
 
+Note that the version of `numpy` is important (for many other packages are the same of course), especially for `fastcluster` package. In our test, the `numpy` 1.19.0 works fine on `python3.6/8`. If you met some errors or warnings about numpy, maybe considering pre-install `numpy` as 1.19.0 or other close-by versions before you install `wgd`.
+
 ## Parameters
 
 There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
 
 The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
 ```
 wgd dmd sequences (option)
@@ -424,15 +435,75 @@
 wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
 ```
 
 The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
 
 ![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
 
-Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis.
+Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis. First, we built a global MRBH family using the command below.
+
+```
+wgd dmd --globalmrbh Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera -o wgd_globalmrbh
+```
+
+In the global MRBH family, every pair of orthologous genes is the reciprocal best hit, suggesting true orthologous relationships. We would use the *K*<sub>S</sub> values associated with these orthologous pairs to delimit the divergence *K*<sub>S</sub> peak. Together with the whole paranome *K*<sub>S</sub> distribution, we conduct the rate correction using the command below.
+
+```
+wgd ksd wgd_globalmrbh/global_MRBH.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
+```
+
+The file `speciestree.nw` is the text file of species tree in newick that rate correction would be conducted on. Its content is as below. Users need to provide the species pairs to be plotted. We suggest adding the option `--reweight` to recalculate the weight per species pair such that the weight of orthologous gene pairs will become 1 as the paralogous gene pairs. The flag `--plotkde` can be added when the kde curve of orthologous *K*<sub>S</sub> is desired. Extra collinear data can be added by the option `-ap`.
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
+
+As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
+
+```
+(((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
+```
+
+If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
+```
+
+Note that a necessary gene-species map file is needed for its implementation in `wgd viz`, which should be automately produced by the last `wgd ksd` step. The `gene_species.map` has contents as below in which each line is the joined string of gene name and species name by space.
+
+```
+Aqcoe6G057800.1 Aquilegia_coerulea
+Vvi_VIT_201s0011g01530.1 Vitis_vinifera
+Pcy_Procy01g08510 Protea_cynaroides
+Aam_Acora.04G142900.1 Acorus_americanus
+```
+
+An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
+
+```
+wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
+```
+
+Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
+
+```
+wgd ksd wgd_ortho/Orthogroups.sp.tsv -sp speciestree.nw --reweight -o wgd_ortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
+```
+
+![](data/Aquilegia_coerulea_OrthoKs_Corrected.ksd.svg)
+
+As shown above, the number of both paralogous gene pairs and orthologous gene pairs is different than the one from global MRBH family in that here we plotted all orthologous gene pairs instead of only global MRBH and potentially new paralogous gene pairs might be produced in the orthogroup inference step, together with different recalculated weights.
+
+If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
+
+```
+wgd ksd wgd_globalmrbh/global_MRBH.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus"
+```
+
+We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
+![](data/Raw_Orthologues.ksd.svg)
 
 ## Citation
  
 Please cite us at https://doi.org/10.1093/bioinformatics/bty915
 
 ```
 Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
```

### Comparing `wgd-2.0.13/cli.py` & `wgd-2.0.14/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,14 +420,17 @@
     type=click.Choice(['cluster', 'fasttree', 'iqtree']), 
     default='fasttree', show_default=True,
     help="Tree inference method for node weighting")
 @click.option('--spair', '-sr', multiple=True, default=None, show_default=True,help='species pair to be plotted')
 @click.option('--speciestree', '-sp', default=None, show_default=True,help='species tree to perform rate correction')
 @click.option('--reweight', '-rw', is_flag=True, help='recalculate the weight per species pair')
 @click.option('--onlyrootout', '-or', is_flag=True, help='only consider the outgroup at root')
+@click.option('--extraparanomeks', '-epk', default=None, help='extra paranome ks data')
+@click.option('--anchorpoints', '-ap', default=None, show_default=True, help='anchorpoints.txt file')
+@click.option('--plotkde', '-pk', is_flag=True, help='plot kde curve over histogram')
 def ksd(**kwargs):
     """
     Paranome and one-to-one ortholog Ks distribution inference pipeline.
 
     Example 1 - whole-paranome:
 
         wgd ksd families.mcl cds.fasta
@@ -438,15 +441,15 @@
 
     If you want to keep intermediate (temporary) files, please provide a directory
     name for the `--tmpdir` option.
     """
     _ksd(**kwargs)
 
 def _ksd(families, sequences, outdir, tmpdir, nthreads, to_stop, cds, pairwise,
-        strip_gaps, tree_method,spair, speciestree, reweight, onlyrootout):
+        strip_gaps, tree_method,spair, speciestree, reweight, onlyrootout, extraparanomeks, anchorpoints, plotkde):
     from wgd.core import get_gene_families, SequenceData, KsDistributionBuilder
     from wgd.core import read_gene_families, merge_seqs
     from wgd.viz import default_plot, apply_filters,multi_sp_plot
     start = timer()
     if tmpdir != None and not os.path.isdir(tmpdir): os.mkdir(tmpdir)
     if len(sequences) == 0: 
         logging.error("Please provide at least one sequence file")
@@ -473,15 +476,15 @@
     logging.info("Making plots")
     df = apply_filters(ksdb.df, [("dS", 0., 5.)])
     ylabel = "Duplications"
     if len(sequences) == 2:
         ylabel = "RBH orthologs"
     elif len(sequences) > 2:
         ylabel = "Homologous pairs"
-    if len(spair)!= 0:  multi_sp_plot(df,spair,spgenemap,outdir,onlyrootout,title=prefix,ylabel=ylabel,ksd=True,reweight=reweight,sptree=speciestree)
+    if len(spair)!= 0:  multi_sp_plot(df,spair,spgenemap,outdir,onlyrootout,title=prefix,ylabel=ylabel,ksd=True,reweight=reweight,sptree=speciestree,extraparanomeks=extraparanomeks, ap = anchorpoints,plotkde=plotkde)
     fig = default_plot(df, title=prefix, bins=50, ylabel=ylabel)
     fig.savefig(os.path.join(outdir, "{}.ksd.svg".format(prefix)))
     fig.savefig(os.path.join(outdir, "{}.ksd.pdf".format(prefix)))
     plt.close()
     if tmpdir is None:
         [x.remove_tmp(prompt=False) for x in seqs]
     end = timer()
@@ -506,21 +509,22 @@
 @click.option('--maxsize', '-ms', default=200, show_default=True, help="maximum family size to include in analysis")
 @click.option('--anchorpoints', '-ap', default=None, show_default=True, help='anchorpoints.txt file')
 @click.option('--multiplicon', '-mt', default=None, show_default=True, help='multiplicons.txt file')
 @click.option('--genetable', '-gt', default=None, show_default=True, help='gene-table.csv file')
 @click.option('--rel_height', '-rh', type=float, default=0.4, show_default=True, help='relative height at which the peak width is measured')
 @click.option('--minseglen', '-mg', default=10000, show_default=True, help="minimum length (ratio if <=1) of segments to show in marco-synteny")
 @click.option('--keepredun', '-kr', is_flag=True, help='keep redundant multiplicons')
+@click.option('--extraparanomeks', '-epk', default=None, help='extra paranome ks data')
 def viz(**kwargs):
     """
     Visualization of Ks distribution or synteny
     """
     _viz(**kwargs)
 
-def _viz(datafile,spair,outdir,gsmap,plotkde,reweight,em_iterations,em_initializations,prominence_cutoff,segments,minlen,maxsize,anchorpoints,multiplicon,genetable,rel_height,speciestree,onlyrootout,minseglen,keepredun):
+def _viz(datafile,spair,outdir,gsmap,plotkde,reweight,em_iterations,em_initializations,prominence_cutoff,segments,minlen,maxsize,anchorpoints,multiplicon,genetable,rel_height,speciestree,onlyrootout,minseglen,keepredun,extraparanomeks):
     from wgd.viz import elmm_plot, apply_filters, multi_sp_plot, default_plot,all_dotplots,filter_by_minlength
     from wgd.core import _mkdir
     from wgd.syn import get_anchors,get_multi,get_segments_profile
     if datafile!=None: prefix = os.path.basename(datafile)
     _mkdir(outdir)
     if datafile ==None:
         table = pd.read_csv(genetable,header=0,index_col=0,sep=',')
@@ -533,15 +537,15 @@
             v.savefig(os.path.join(outdir, "{}.dot.pdf".format(k)))
             v.savefig(os.path.join(outdir, "{}.dot.png".format(k)))
         logging.info('Done')
         exit()
     ksdb_df = pd.read_csv(datafile,header=0,index_col=0,sep='\t')
     df = apply_filters(ksdb_df, [("dS", 0., 5.)])
     ylabel = "Duplications" if spair == () else "Homologous pairs"
-    if len(spair)!= 0: multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title=prefix,ylabel=ylabel,viz=True,plotkde=plotkde,reweight=reweight,sptree=speciestree,ap = anchorpoints)
+    if len(spair)!= 0: multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title=prefix,ylabel=ylabel,viz=True,plotkde=plotkde,reweight=reweight,sptree=speciestree,ap = anchorpoints, extraparanomeks=extraparanomeks)
     fig = default_plot(df, title=prefix, bins=50, ylabel=ylabel)
     fig.savefig(os.path.join(outdir, "{}.ksd.svg".format(prefix)))
     fig.savefig(os.path.join(outdir, "{}.ksd.pdf".format(prefix)))
     plt.close()
     if spair == ():
         logging.info('Exponential-Lognormal mixture modeling on node-weighted Ks distribution')
         elmm_plot(df,prefix,outdir,max_EM_iterations=em_iterations,num_EM_initializations=em_initializations,peak_threshold=prominence_cutoff,rel_height=rel_height)
```

### Comparing `wgd-2.0.13/setup.py` & `wgd-2.0.14/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='wgd',
-    version='2.0.13',
+    version='2.0.14',
     packages=['wgd'],
     url='http://github.com/heche-psb/wgd',
     license='GPL',
     author='Hengchi Chen',
     author_email='heche@psb.vib-ugent.be',
     description='wgd',
     long_description=long_description,
@@ -33,15 +33,15 @@
        'iniconfig==1.1.1',
        'Jinja2==2.11.2',
        'joblib==0.11',
        'KDEpy==1.1.0',
        'kiwisolver==1.2.0',
        'MarkupSafe==1.1.1',
        'matplotlib==3.2.2',
-       'numpy>=1.19.0',
+       'numpy>=1.19.0,!=1.24.3',
        'numexpr>=2.7.3',
        'packaging==20.4',
        'pandas<=1.4.4',
        'Pillow<=8.4.0',
        'pluggy==0.13.1',
        'plumbum==1.6.9',
        'progressbar2==3.51.4',
```

### Comparing `wgd-2.0.13/test/test_core.py` & `wgd-2.0.14/test/test_core.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.13/wgd/__init__.py` & `wgd-2.0.14/wgd/__init__.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.13/wgd/beast.py` & `wgd-2.0.14/wgd/beast.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.13/wgd/cluster.py` & `wgd-2.0.14/wgd/cluster.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.13/wgd/codeml.py` & `wgd-2.0.14/wgd/codeml.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.13/wgd/core.py` & `wgd-2.0.14/wgd/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -804,33 +804,33 @@
         logging.info("Multiple CDS files: will compute RBH orthologs or cscore-defined homologs between focus species and remaining species")
         x = 0
         table = pd.DataFrame()
         focusname = os.path.join(outdir, 'merge_focus.tsv')
         for i in range(len(s)):
             if s[i].prefix == focus: x = x+i
         if x == 0:
-            Parallel(n_jobs=nthreads,backend='multiprocessing',batch_size=20)(delayed(get_mrbh)(s[0],s[j],cscore,eval) for j in range(1,len(s)))
+            Parallel(n_jobs=nthreads,backend='multiprocessing')(delayed(get_mrbh)(s[0],s[j],cscore,eval) for j in range(1,len(s)))
             for j in range(1, len(s)):
                 df = getrbhf(s[0],s[j],outdir)
                 if table.empty: table = df
                 else:
                     table = table.merge(df)
                     if not keepduplicates: table.drop_duplicates([focus])
             #if not keepduplicates: table = table.drop_duplicates([focus])
             table.insert(0, focus, table.pop(focus))
         else:
-            Parallel(n_jobs=nthreads,backend='multiprocessing',batch_size=20)(delayed(get_mrbh)(s[x],s[k],cscore,eval) for k in range(0,x))
+            Parallel(n_jobs=nthreads,backend='multiprocessing')(delayed(get_mrbh)(s[x],s[k],cscore,eval) for k in range(0,x))
             for k in range(0,x):
                 df = getrbhf(s[x],s[k],outdir)
                 if table.empty: table = df
                 else:
                     table = table.merge(df)
                     if not keepduplicates: table.drop_duplicates([focus])
             if not len(s) == 2 and not x+1 == len(s):
-                Parallel(n_jobs=nthreads,backend='multiprocessing',batch_size=20)(delayed(get_mrbh)(s[x],s[l],cscore,eval) for l in range(x+1,len(s)))
+                Parallel(n_jobs=nthreads,backend='multiprocessing')(delayed(get_mrbh)(s[x],s[l],cscore,eval) for l in range(x+1,len(s)))
                 for l in range(x+1,len(s)):
                     df = getrbhf(s[x],s[l],outdir)
                     table = table.merge(df)
                     if not keepduplicates: table = table.drop_duplicates([focus])
             #if not keepduplicates: table = table.drop_duplicates([focus])
             table.insert(0, focus, table.pop(focus))
         #gfid = ['GF{:0>8}'.format(str(i+1)) for i in range(table.shape[0])]
@@ -866,30 +866,30 @@
             seq_cds = {}
             seq_pro = {}
             for i in range(len(s)):
                 seq_cds.update(s[i].cds_sequence)
                 seq_pro.update(s[i].pro_sequence)
             rbhgfdirname = outdir + '/' + 'MRBH_GF_FASTA' + '/'
             os.mkdir(rbhgfdirname)
-            Parallel(n_jobs=nthreads,backend='multiprocessing',batch_size=20)(delayed(getfastaf)(i,fam,rbhgfdirname,seq_pro,idmap,seq_cds) for i, fam in enumerate(seqid_table))
+            Parallel(n_jobs=nthreads,backend='multiprocessing')(delayed(getfastaf)(i,fam,rbhgfdirname,seq_pro,idmap,seq_cds) for i, fam in enumerate(seqid_table))
            # for i, fam in enumerate(seqid_table):
            #     for seqs in fam:
            #         fname = os.path.join(rbhgfdirname, 'GF{:0>5}'.format(i+1) + ".pep")
            #         with open(fname,'a') as f:
            #             Record = seq_pro.get(idmap.get(seqs))
            #             f.write(">{}\n{}\n".format(seqs, Record))
            #         fname2 = os.path.join(rbhgfdirname, 'GF{:0>5}'.format(i+1) + ".cds")
            #         with open(fname2,'a') as f:
            #             Record = seq_cds.get(idmap.get(seqs))
            #             f.write(">{}\n{}\n".format(seqs, Record))
             if not anchorpoints is None:
                 seqid_table = read_MultiRBH_gene_families(focusapname)
                 rbhgfapdirname = outdir + '/' + 'MRBH_AP_GF_FASTA' + '/'
                 os.mkdir(rbhgfapdirname)
-                Parallel(n_jobs=nthreads,backend='multiprocessing',batch_size=20)(delayed(getfastaf)(i,fam,rbhgfapdirname,seq_pro,idmap,seq_cds) for i, fam in enumerate(seqid_table))
+                Parallel(n_jobs=nthreads,backend='multiprocessing')(delayed(getfastaf)(i,fam,rbhgfapdirname,seq_pro,idmap,seq_cds) for i, fam in enumerate(seqid_table))
                 #for i, fam in enumerate(seqid_table):
                 #    for seqs in fam:
                 #        fname = os.path.join(rbhgfapdirname, 'GF{:0>5}'.format(i+1) + ".pep")
                 #        with open(fname,'a') as f:
                 #            Record = seq_pro.get(idmap.get(seqs))
                 #            f.write(">{}\n{}\n".format(seqs, Record))
                 #        fname2 = os.path.join(rbhgfapdirname, 'GF{:0>5}'.format(i+1) + ".cds")
@@ -1256,15 +1256,15 @@
         famid = "GF{:0>8}".format(fam+1)
         cds_aln_rn = cds_alns_rn[famid]
         pro_aln_rn = pro_alns_rn[famid]
         calnf = calnfs[fam]
         beast_i = beast(calnf, cds_aln_rn, pro_aln_rn, tmpdir, outdir, speciestree, datingset, slist, fossil, chainset, rootheight)
         beasts.append(beast_i)
     beast_i.run_beast(beastlgjar,beagle)
-    Parallel(n_jobs=nthreads,backend='multiprocessing',batch_size=20)(delayed(i.run_beast)(beastlgjar,beagle) for i in beasts)
+    Parallel(n_jobs=nthreads,backend='multiprocessing')(delayed(i.run_beast)(beastlgjar,beagle) for i in beasts)
 
 # Run MCMCtree
 def Run_MCMCTREE(Concat_caln, Concat_paln, Concat_calnf, Concat_palnf, cds_alns_rn, pro_alns_rn, calnfs, palnfs, tmpdir, outdir, speciestree, datingset, aamodel, partition, slist, nthreads):
     CI_table = {}
     PM_table = {}
     wgd_mrca = [sp for sp in slist if sp[-4:] == '_ap1' or sp[-4:] == '_ap2']
     Concat_calnf_paml = fasta2paml(Concat_caln,Concat_calnf)
@@ -1299,15 +1299,15 @@
             McMctree = mcmctree(calnfpartitioned_paml, palnf_rn, tmpdir, outdir, speciestree, datingset, aamodel, partition)
             McMctrees.append(McMctree)
             #McMctree.run_mcmctree(CI_table,PM_table,wgd_mrca)
         #logging.info("Running mcmctree on GF{:0>5} codon and peptide alignment without partition".format(fam+1))
         McMctree = mcmctree(calnf_rn, palnf_rn, tmpdir, outdir, speciestree, datingset, aamodel, partition=False)
         McMctrees.append(McMctree)
         #McMctree.run_mcmctree(CI_table,PM_table,wgd_mrca)
-    Parallel(n_jobs=nthreads,backend='multiprocessing',batch_size=20)(delayed(McMctree.run_mcmctree)(CI_table,PM_table,wgd_mrca) for McMctree in McMctrees)
+    Parallel(n_jobs=nthreads,backend='multiprocessing')(delayed(McMctree.run_mcmctree)(CI_table,PM_table,wgd_mrca) for McMctree in McMctrees)
     Getback_CIPM(outdir,CI_table,PM_table,wgd_mrca,calnfs_rn,Concat_calnf_paml,partition)
     df_CI = pd.DataFrame.from_dict(CI_table,orient='index',columns=['CI_lower','CI_upper'])
     df_PM = pd.DataFrame.from_dict(PM_table,orient='index',columns=['PM'])
     fname_CI = os.path.join(outdir,'mcmctree','CI.tsv')
     fname_PM = os.path.join(outdir,'mcmctree','PM.tsv')
     df_CI.to_csv(fname_CI,header = True,index=True,sep='\t')
     df_PM.to_csv(fname_PM,header = True,index=True,sep='\t')
@@ -2752,15 +2752,15 @@
     def __init__(self, gene_families, seqs, n_threads=4):
         self.families = gene_families
         self.df = None
         self.seqs = seqs
         self.n_threads = n_threads
 
     def get_distribution(self):
-        Parallel(n_jobs=self.n_threads,backend='multiprocessing',batch_size=200)(
+        Parallel(n_jobs=self.n_threads,backend='multiprocessing')(
             delayed(_get_ks)(family) for family in self.families)
         df = pd.concat([pd.read_csv(x.out, index_col=0) 
             for x in self.families], sort=True)
         self.df = add_original_ids(df, self.seqs)
 
 def reverse_map(seqs):
     return {v: k for k, v in seqs.items()}
```

### Comparing `wgd-2.0.13/wgd/mcmctree.py` & `wgd-2.0.14/wgd/mcmctree.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.13/wgd/mix.py` & `wgd-2.0.14/wgd/mix.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.13/wgd/peak.py` & `wgd-2.0.14/wgd/peak.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.13/wgd/syn.py` & `wgd-2.0.14/wgd/syn.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.13/wgd/utils.py` & `wgd-2.0.14/wgd/utils.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.13/wgd/viz.py` & `wgd-2.0.14/wgd/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,22 @@
     maxy_iloc = np.argmax(kde_y)
     mode = kde_x[maxy_iloc]
     return mode, max(kde_y)
 
 def reweighted(df_per):
     return 1 / df_per.groupby(["family", "node"])["dS"].transform('count')
 
-def multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title='',ylabel='',viz=False,plotkde=False,reweight=True,sptree=None,ksd=False,ap=None):
+def multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title='',ylabel='',viz=False,plotkde=False,reweight=True,sptree=None,ksd=False,ap=None,extraparanomeks=None):
+    if extraparanomeks != None:
+        df_para = pd.read_csv(extraparanomeks,header=0,index_col=0,sep='\t')
+        df_para = apply_filters(df_para, [("dS", 0., 5.)])
+        df_para["family"] = df_para["family"].apply(lambda x:"ExtraParalog_"+x)
+        df = pd.concat([df,df_para])
+    # I add this dropduplicates to prevent the same paralogous pair from occuring twice and also use preferentially paranome
+    df = df[~df.index.duplicated(keep='last')]
     if not ksd: spgenemap = getgsmap(gsmap)
     else: spgenemap = gsmap
     if not viz: writespgenemap(spgenemap,outdir)
     df_perspair,allspair,paralog_pair,corrected_ks_spair,Outgroup_spnames = getspair_ks(spair,df,spgenemap,reweight,onlyrootout,sptree=sptree)
     if len(paralog_pair) != 0:
         fnames = os.path.join(outdir,'{}_Corrected.ksd.svg'.format(paralog_pair[0].split('__')[0]))
         fnamep = os.path.join(outdir,'{}_Corrected.ksd.pdf'.format(paralog_pair[0].split('__')[0]))
```

### Comparing `wgd-2.0.13/wgd.egg-info/PKG-INFO` & `wgd-2.0.14/wgd.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,456 +1,516 @@
 Metadata-Version: 2.1
 Name: wgd
-Version: 2.0.13
+Version: 2.0.14
 Summary: wgd
 Home-page: http://github.com/heche-psb/wgd
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
-Description: <div align="center">
-        
-        # `wgd v2` : a suite tool of WGD inference and timing
-        
-        [![Build Status](https://app.travis-ci.com/heche-psb/wgd.svg?branch=phylodating)](https://travis-ci.com/heche-psb/wgd)
-        
-        **Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
-        
-        [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
-        
-        [**Introduction**](#Introduction) | 
-        [**Installation**](#Installation) | 
-        [**Parameters**](#Parameters) | 
-        [**Usage**](#Usage) | 
-        [**Illustration**](#Illustration) |
-        [**Citation**](#Citation)
-        
-        </div>
-        
-        `wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
-        
-        ## Introduction
-        
-        Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
-        
-        The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
-        
-        ## Installation
-        
-        The easiest way to install `wgd v2` is using PYPI
-        
-        ```
-        pip install wgd
-        ```
-        
-        To install `wgd v2` in a virtual environment, the following command lines could be used.
-        
-        ```
-        git clone <wgd repo>
-        cd wgd
-        virtualenv -p=python3 ENV (or python3 -m venv ENV)
-        source ENV/bin/activate
-        pip install -r requirements.txt
-        pip install .
-        ```
-        
-        When met with permission problem in installation, please try the following command line.
-        
-        ```
-        pip install -e .
-        ```
-        
-        If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
-        
-        ```
-        export PATH="$PATH:~/.local/bin/wgd"
-        ```
-        
-        ## Parameters
-        
-        There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
-        
-        The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
-        ```
-        wgd dmd sequences (option)
-        --------------------------------------------------------------------------------
-        -o, --outdir, the output directory, default wgd_dmd
-        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
-        -c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
-        -I, --inflation, the inflation factor for MCL program, default 2.0
-        -e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
-        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
-        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
-        -f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
-        -ap, --anchorpoints, the anchor points data file, default None
-        -coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
-        -sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
-        -le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
-        -gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
-        -kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
-        -kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
-        -gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
-        -n, --nthreads, the number of threads to use, default 4
-        -oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
-        -oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
-        -gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
-        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
-        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
-        -mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
-        -ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
-        -am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
-        -sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
-        -fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
-        -cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
-        -te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
-        -bs, --bins, the number of bins divided in gene length normalization, default 100
-        -np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
-        -nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
-        -bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
-        -bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
-        -bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
-        ```
-        
-        The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
-        ```
-        wgd focus families sequences (option)
-        --------------------------------------------------------------------------------
-        -o, --outdir, the output directory, default wgd_focus
-        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
-        -n, --nthreads, the number of threads to use, default 4
-        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
-        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
-        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
-        -a, --aligner, which alignment program to use, default mafft
-        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
-        -ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
-        --concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
-        --coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
-        -sp, --speciestree, species tree darafile for dating, default None
-        -d, --dating, which molecular dating program to use, default none
-        -ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
-        -ns, --nsites, the nsites information for r8s dating, default None
-        -ot, --outgroup, the outgroup information for r8s dating, default None
-        -pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
-        -am, --aamodel, which protein model to be used in mcmctree, default poisson
-        -ks, flag option, whether to initiate Ks analysis
-        --annotation, which annotation program to use, default none
-        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
-        -ed, --eggnogdata, the eggnog annotation datafile, default None
-        --pfam, which option to use for pfam annotation, default none
-        --dmnb, the diamond database for annotation, default None
-        --hmm, the HMM profile for annotation, default None
-        --evalue, the e-value cut-off for annotation, default 1e-10
-        --exepath, the path to the interproscan executable, default None
-        -f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
-         -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
-        -cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
-        --beastlgjar, the path to beastLG.jar, default None
-        --beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
-        --protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
-        ```
-        
-        The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
-        ```
-        wgd ksd families sequences (option)
-        --------------------------------------------------------------------------------
-        -o, --outdir, the output directory, default wgd_ksd
-        -t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
-        -n, --nthreads, the number of threads to use, default 4
-        --to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
-        --cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
-        --pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
-        --strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
-        -tree, --tree_method, which gene tree inference program to invoke, default fasttree
-        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
-        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
-        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
-        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
-        ```
-        
-        The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
-        ```
-        wgd mix ks_datafile (option)
-        --------------------------------------------------------------------------------
-        -f, --filters, the cutoff alignment length, default 300
-        -r, --ks_range, the Ks range to be considered, default (0.005, 3)
-        -b, --bins, the number of bins in Ks distribution, default 50
-        -o, --outdir, the output directory, default wgd_mix
-        --method, which mixture model to use, default gmm
-        -n, --components, the range of the number of components to fit, default (1, 4)
-        -g, --gamma, the gamma parameter for bgmm models, default 0.001
-        -ni, --n_init, the number of k-means initializations, default 200
-        -mi, --max_iter, the maximum number of iterations, default 1000
-        ```
-        
-        The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
-        ```
-        wgd peak ks_datafile (option)
-        --------------------------------------------------------------------------------
-        -ap, --anchorpoints, the anchor points datafile, default None
-        -sm, --segments, the segments datafile, default None
-        -le, --listelements, the listsegments datafile, default None 
-        -mp, --multipliconpairs, the multipliconpairs datafile, default None
-        -o, --outdir, the output directory, default wgd_peak
-        -af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
-        -r, --ksrange, range of Ks to be analyzed, default (0, 5)
-        -bw, --bin_width, bandwidth of Ks distribution, default 0.1
-        -ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
-        -m, --method, which mixture model to use, default gmm
-        --seed, random seed given to initialization, default 2352890
-        -ei, --em_iter, the number of EM iterations to perform, default 200
-        -ni, --n_init, the number of k-means initializations, default 200
-        -n, --components, the range of the number of components to fit, default (1, 4)
-        --boots, the number of bootstrap replicates of kde, default 200
-        --weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
-        -p, --plot, the plotting method to be used, default identical
-        -bm, --bw_method, the bandwidth method to be used, default silverman
-        --n_medoids, the number of medoids to fit, default 2
-        -km, --kdemethod, the kde method to be used, default scipy
-        --n_clusters, the number of clusters to plot Elbow loss function, default 5
-        --kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
-        -gd, --guide, the regime residing anchors, default: segment
-        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
-        -kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
-        -f, --family, the family to filter Ks upon, default None
-        --manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
-        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
-        --ci, the confidence level of log-normal distribution to date, default 95
-        --hdr, the highest densidy region (HDR) in a given distribution to date, default 95
-        --heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
-        -kc, --kscutoff, the Ks saturation cutoff in dating, default 5
-        ```
-        
-        The program `wgd syn` can realize the intra- and inter-specific synteny inference.
-        ```
-        wgd syn families gffs (option)
-        --------------------------------------------------------------------------------
-        -ks, --ks_distribution, ks distribution datafile, default None
-        -o, --outdir, the output directory, default wgd_syn
-        -f, --feature, the feature for parsing gene IDs from GFF files, default gene
-        -a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
-        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
-        -ms, --maxsize, the maximum family size to include, default 200
-        -r, --ks_range, the Ks range in colored dotplot, default (0, 5)
-        --iadhore_options, the parameter setting in iadhore, default 
-        -ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
-        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
-        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-        ```
-        
-        The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
-        ```
-        wgd viz (option)
-        --------------------------------------------------------------------------------
-        -d, --datafile, the Ks datafile, default None
-        -o, --outdir, the output directory, default wgd_viz
-        -sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
-        -gs, --gsmap, the gene name-species name map, default None
-        -sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
-        -pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
-        -rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
-        -or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
-        -iter, --em_iterations, the maximum EM iterations, default 200
-        -init, --em_initializations, the maximum EM initializations, default 200
-        -prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
-        -sm, --segments, the segments data file, default None
-        -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
-        -ms, --maxsize, the maximum family size to include, default 200
-        -ap, --anchorpoints, the anchor points datafile, default None
-        -mt, --multiplicon, the multiplicons datafile, default None
-        -gt, --genetable, the gene table datafile, default None
-        -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
-        -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
-        -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
-        ```
-        
-        ## Usage
-        
-        Here we provided the basic usage for each program.
-        
-        ### wgd dmd
-        
-        **The delineation of whole paranome**
-        ```
-        wgd dmd sequence
-        ``` 
-        
-        **The delineation of RBHs**
-        ```
-        wgd dmd sequence1 sequence2
-        ```
-        
-        **The delineation of local MRBHs**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -f sequence1
-        ```
-        
-        **The delineation of global MRBHs**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -gm
-        ```
-        
-        **The delineation of orthogroups**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -oi (option)
-        ```
-        Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
-        
-        **The collinear coalescence inference of phylogeny**
-        ```
-        wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
-        ```
-        
-        ### wgd focus
-        
-        **The concatenation-based/coalescence-based phylogenetic inference**
-        ```
-        wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
-        ```
-        
-        **The functional annotation of gene families**
-        ```
-        wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
-        ```
-        
-        **The phylogenetic dating of WGDs**
-        ```
-        wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
-        ```
-        
-        ### wgd ksd
-        
-        **The construction of whole paranome *K*<sub>S</sub> age distribution**
-        ```
-        wgd ksd families sequence
-        ```
-        
-        **The construction of orthologous *K*<sub>S</sub> age distribution**
-        ```
-        wgd ksd families sequence1 sequence2
-        ```
-        
-        **The construction of *K*<sub>S</sub> age distribution with rate correction**
-        ```
-        wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
-        ```
-        
-        ### wgd mix
-        
-        **The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
-        ```
-        wgd mix ksdata
-        ```
-        
-        ### wgd peak
-        
-        **The search of crediable *K*<sub>S</sub> range used in WGD dating**
-        ```
-        wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
-        ```
-        Note that users can add the flag --heuristic to implement the heuristic search analysis
-        
-        ### wgd syn
-        
-        **The intra-specific synteny inference**
-        ```
-        wgd syn families gff
-        ```
-        
-        **The inter-specific synteny inference**
-        ```
-        wgd syn families gff1 gff2
-        ```
-        
-        ### wgd viz
-        
-        **The visualization of *K*<sub>S</sub> age distribution**
-        ```
-        wgd viz -d ksdata
-        ```
-        
-        **The visualization of *K*<sub>S</sub> age distribution with rate correction**
-        ```
-        wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
-        ```
-        
-        **The visualization of synteny**
-        ```
-        wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
-        ```
-        
-        ## Illustration
-        
-        We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
-        
-        The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
-        
-        First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
-        
-        ```
-        wgd dmd Aquilegia_coerulea
-        wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
-        ```
-        
-        The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
-        
-        ![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
-        
-        We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
-        
-        ```
-        wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
-        ```
-        
-        As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
-        
-        ![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
-        
-        The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes, except for the chr_07, which seems to experience more severe fragmentization than the other chromosomes.
-        
-        ![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
-        
-        The associated dotplot in oxford grid also presents numerous densely aggregated anchor points throughout most of the chromosomes.
-        
-        ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
-        
-        A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
-        
-        ![](data/Syndepth.svg)
-        
-        We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
-        
-        ```
-        wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
-        ```
-        
-        The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
-        
-        ![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
-        
-        Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
-        
-        ```
-        wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
-        ```
-        
-        The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
-        
-        ![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
-        
-        Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis.
-        
-        ## Citation
-         
-        Please cite us at https://doi.org/10.1093/bioinformatics/bty915
-        
-        ```
-        Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
-        
-        Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
-        ```
-        
-        For citation of the tools used in wgd, please consult the documentation at
-        https://wgd.readthedocs.io/en/latest/index.html#citation.
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+
+# `wgd v2` : a suite tool of WGD inference and timing
+
+**Hengchi Chen, Arthur Zwaenepoel, Yves Van de Peer**
+
+[**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/)**, VIB-UGent Center for Plant Systems Biology**
+
+[**Introduction**](#Introduction) | 
+[**Installation**](#Installation) | 
+[**Parameters**](#Parameters) | 
+[**Usage**](#Usage) | 
+[**Illustration**](#Illustration) |
+[**Citation**](#Citation)
+
+</div>
+
+`wgd v2` is a python package upgraded from the original `wgd` package aiming for the inference and timing of ancient whole-genome duplication (WGD) events. For the propose of illustrating the principle and usage of `wgd v2`, we compiled this documentation. Below we first give an introduction over the scope and mechanism of `wgd v2` and then the practical information of installation and usage. An examplar workflow is provided in the tutorial section on how to seek evidence for a putative WGD event and perform proper timing with a freshly obtained genome assembly in hand. For those who are interested, we recommend turning to our paper and book chapter for more detailed description and insightful discussions. If you use `wgd v2` in your research, please cite us. 
+
+## Introduction
+
+Polyploidizations, the evolutionary process that the entire genome of an organism is duplicated, also named as whole-genome duplications (WGDs), occur recurrently across the tree of life. There are two modes of polyploidizations, autopolyploidizations and allopolyploidizations. Autopolyploidizations are the duplication of the same genome, resulting in two identical subgenomes at the time it emerged. While the allopolyploidizations are normally achieved in two steps, first the hybridization between two different species, resulting in the arising of transient homoploidy,second the duplication of the homoploidy, resulting in the emergence of allopolyploidy. Due to the unstability and unbalanced tetrasomic inheritance, for instance the nuclear-cytoplasmic incompatibility, the polyploidy genome will then experience a process called diploidization, also named as fractionation, during which a large portion of gene duplicates will get lost and only a fraction can be retained. The traces of polyploidizations can be thus unearthed from these retained gene duplicates. Three approaches based on gene duplicates, namely, *K*<sub>S</sub> method, gene tree - species tree reconciliation method and synteny method, are commonly used in detecting evidence for WGDs. The gene tree - species tree reconciliation method is not within the scope of `wgd v2`, but we kindly refer readers who are interested to the phylogenomic program developed by Arthur Zwaenepoel named [WHALE](https://github.com/arzwa/Whale.jl) and the associated [paper](https://doi.org/10.1093/molbev/msz088) for more technical and theoretical details.
+
+The *K*<sub>S</sub> method is established on a model of gene family evolution that each gene family is allowed to evolve via gene duplication and loss. Note that the gene family here is assumed to be the cluster of all genes descended from an ancestral gene in a single genome. Recovering the gene tree of such gene family informs the timing, scilicet the age, of gene duplication events. The age refered here, is not in real geological time, but in the unit of evolutionary distance, i.e., the number of substitutions per site. When the evolutionary rate remains approximately constant, the evolutionary distance is then supposed to be proportional to the real evolutionary time. The synonymous distance *K*<sub>S</sub>, the number of synonymous substitutions per synonymous site, is such candidate that synonymous substitutions would not incur the change of amino acid and are thus regarded as neutral, which according to the neutral theory should occur in constant rate. Given a model of gene family that allows the gene to duplicate and get lost in a fixed rate, one can derive that the probability density function of the *K*<sub>S</sub> age distribution of retained gene duplicates is a quasi-exponential function that most retained gene duplicates are recently borned with ~0 age while as the age going older the associated number of retained gene duplicates decay quasi-exponentially. Therefore, the occurance of large-scale gene duplication events, for instane WGDs, with varied retention rate, will leave an age peak from the burst of gene duplicates in a short time-frame upon the initial age distribution, and can be unveiled from mixture modeling analysis. However, WGDs identified from the paralogous *K*<sub>S</sub> age distributions can only inform the WGD timing in the time-scale of that specific species, which is not comparable in the phylogenetic context. Only with the orthologous *K*<sub>S</sub> age distributions, which convert the estimated body from paralogues to orthologues and inform the relative timing of speciation events, can we decipher the phylogenetic placement of WGDs after proper rate correction. `wgd v2` is such program that helps users construct paralogous and orthologous *K*<sub>S</sub> age distributions and realize both the identification and placement of WGDs.
+
+## Installation
+
+The easiest way to install `wgd v2` is using PYPI
+
+```
+pip install wgd
+```
+
+To install `wgd v2` in a virtual environment, the following command lines could be used.
+
+```
+git clone <wgd repo>
+cd wgd
+virtualenv -p=python3 ENV (or python3 -m venv ENV)
+source ENV/bin/activate
+pip install -r requirements.txt
+pip install .
+```
+
+When met with permission problem in installation, please try the following command line.
+
+```
+pip install -e .
+```
+
+If multiply versions of `wgd` were installed in the system, please add the right path of interested version into the environment variables, for example
+
+```
+export PATH="$PATH:~/.local/bin/wgd"
+```
+
+Note that the version of `numpy` is important (for many other packages are the same of course), especially for `fastcluster` package. In our test, the `numpy` 1.19.0 works fine on `python3.6/8`. If you met some errors or warnings about numpy, maybe considering pre-install `numpy` as 1.19.0 or other close-by versions before you install `wgd`.
+
+## Parameters
+
+There are 7 main programs in `wgd v2`: `dmd`,`focus`,`ksd`,`mix`,`peak`,`syn`,`viz`. Hereafter we will provide a detailed elucidation on each of the program and its associated parameters.
+
+The program `wgd dmd` can realize the delineation of whole paranome, RBHs, MRBHs, orthogroups and some other orthogroup-related functions, including circumscription of nested single-copy orthogroups (NSOGs), unbiased uest of single-copy orthogroups (SOGs) over missing inparalogs, construction of BUSCO-guided single-copy orthogroups (SOGs),and the collinear coalescence inference of phylogeny.
+```
+wgd dmd sequences (option)
+--------------------------------------------------------------------------------
+-o, --outdir, the output directory, default wgd_dmd
+-t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+-c, --cscore, the c-score to restrict the homologs of MRBHs, default None, if None was given, the c-score funcion won't be activated
+-I, --inflation, the inflation factor for MCL program, default 2.0
+-e, --eval, the e-value cut-off for similarity in diamond and/or hmmer, default 1e-10
+--to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+--cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+-f, --focus, the species to be merged on local MRBHs, default None, if None was given, the local MRBHs won't be inferred
+-ap, --anchorpoints, the anchor points data file, default None
+-coc, --collinearcoalescence, flag option, whether to initiate the collinear coalescence analysis, if the flag was set, the analysis will be initiated
+-sm, --segments, the segments data file used in collinear coalescence analysis if initiated, default None
+-le, --listelements, the listsegments data file used in collinear coalescence analysis if initiated, default None
+-gt, --genetable, the gene table datafile used in collinear coalescence analysis if initiated, default None
+-kf, --keepfasta, flag option, whether to output the sequence information of MRBHs, if the flag was set, the sequences of MRBHs will be in output
+-kd, --keepduplicates, flag option, whether to allow the same gene to occur in different MRBHs, if the flag was set, the same gene can be assigned to different MRBHs
+-gm, --globalmrbh, flag option, whether to initiate global MRBHs construction, if the flag was set, the --focus option will be ignored and only global MRBHs will be built
+-n, --nthreads, the number of threads to use, default 4
+-oi, --orthoinfer, flag option, whether to initiate orthogroup infernece, if the flag was set, the orthogroup infernece program will be initiated
+-oo, --onlyortho, flag option, whether to only conduct orthogroup infernece, if the flag was set, only the orthogroup infernece program will be conducted while the other analysis won't be initiated
+-gn, --getnsog, flag option, whether to initiate the searching for nested single-copy gene families (NSOGs), if the flag was set, additional NSOGs analysis will be performed besides the basic orthogroup infernece
+-tree, --tree_method, which gene tree inference program to invoke, default fasttree
+-ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+-mc, --msogcut, the ratio cutoff for mostly single-copy family and species representation in collinear coalescence inference, default 0.8.
+-ga, --geneassign, flag option, whether to initiate the gene-to-family assignment analysis, if the flag was set, the analysis will be initiated
+-am, --assign_method, which method to conduct the gene-to-family assignment analysis, default hmmer
+-sa, --seq2assign, the queried sequences data file in gene-to-family assignment analysis, default None, this option can be provided multiple times
+-fa, --fam2assign, the queried familiy data file in gene-to-family assignment analysis, default None
+-cc, --concat, flag option, whether to initiate the concatenation pipeline for orthogroup infernece, if the flag was set, the analysis will be initiated
+-te, --testsog, flag option, whether to initiate the unbiased test of single-copy gene families, if the flag was set, the analysis will be initiated
+-bs, --bins, the number of bins divided in gene length normalization, default 100
+-np, --normalizedpercent, the percentage of upper hits used for gene length normalization, default 5
+-nn, --nonormalization, flag option, whether to call off the normalization, if the flag was set, no normalization will be conducted
+-bsog, --buscosog, flag option, whether to initiate the busco-guided single-copy gene family analysis, if the flag was set, the analysis will be initiated
+-bhmm, --buscohmm, the HMM profile datafile in the busco-guided single-copy gene family analysis, default None
+-bctf, --buscocutoff, the HMM score cutoff datafile in the busco-guided single-copy gene family analysis, default None
+```
+
+The program `wgd focus` can realize the concatenation-based and coalescence-based phylogenetic inference, functional annotation of gene families and phylogenetic dating of WGDs.
+```
+wgd focus families sequences (option)
+--------------------------------------------------------------------------------
+-o, --outdir, the output directory, default wgd_focus
+-t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+-n, --nthreads, the number of threads to use, default 4
+--to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+--cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+--strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+-a, --aligner, which alignment program to use, default mafft
+-tree, --tree_method, which gene tree inference program to invoke, default fasttree
+-ts, --treeset, the parameters setting for gene tree inference, default None, this option can be provided multiple times
+--concatenation, flag option, whether to initiate the concatenation-based species tree inference, if the flag was set, concatenation-based species tree will be infered
+--coalescence, flag option, whether to initiate the coalescence-based species tree inference, if the flag was set, coalescence-based species tree will be infered
+-sp, --speciestree, species tree darafile for dating, default None
+-d, --dating, which molecular dating program to use, default none
+-ds, --datingset, the parameters setting for dating program, default None, this option can be provided multiple times
+-ns, --nsites, the nsites information for r8s dating, default None
+-ot, --outgroup, the outgroup information for r8s dating, default None
+-pt, --partition, flag option, whether to initiate partition dating analysis for codon, if the flag was set, an additional partition dating analysis will be initiated
+-am, --aamodel, which protein model to be used in mcmctree, default poisson
+-ks, flag option, whether to initiate Ks analysis
+--annotation, which annotation program to use, default none
+--pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+-ed, --eggnogdata, the eggnog annotation datafile, default None
+--pfam, which option to use for pfam annotation, default none
+--dmnb, the diamond database for annotation, default None
+--hmm, the HMM profile for annotation, default None
+--evalue, the e-value cut-off for annotation, default 1e-10
+--exepath, the path to the interproscan executable, default None
+-f, --fossil, the fossil calibration information in Beast, default ('clade1;clade2', 'taxa1,taxa2;taxa3,taxa4', '4;5', '0.5;0.6', '400;500')
+ -rh, --rootheight, the root height calibration info in Beast, default (4,0.5,400)
+-cs, --chainset, the parameters of MCMC chain in Beast, default (10000,100)
+--beastlgjar, the path to beastLG.jar, default None
+--beagle, flag option, whether to use beagle in Beast, if the flag was set, beagle will be used
+--protdating, flag option, whether to only initiate the protein-concatenation based dating analysis, if the flag was set, the analysis will be initiated
+```
+
+The program `wgd ksd` can realize the construction of *K*<sub>S</sub> age distribution and rate correction.
+```
+wgd ksd families sequences (option)
+--------------------------------------------------------------------------------
+-o, --outdir, the output directory, default wgd_ksd
+-t, --tmpdir, the temporary working directory, default None, if None was given, the tmpdir will be assigned random names in current directory and automately removed at the completion of program, else the tmpdir will be kept
+-n, --nthreads, the number of threads to use, default 4
+--to_stop, flag option, whether to translate through STOP codons, if the flag was set, translation will be terminated at the first in frame stop codon, else a full translation continuing on past any stop codons will be initiated
+--cds, flag option, whether to only translate the complete CDS that starts with a valid start codon and only contains a single in frame stop codon at the end and must be dividable by three, if the flag was set, only the complete CDS will be translated
+--pairwise, flag option, whether to initiate pairwise Ks estimation, if the flag was set, pairwise Ks values will be estimated
+--strip_gaps, flag option, whether to drop all gaps in multiple sequence alignment, if the flag was set, all gaps will be dropped
+-tree, --tree_method, which gene tree inference program to invoke, default fasttree
+-sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+-sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+-rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+-or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+```
+
+The program `wgd mix` can realize the mixture model clustering analysis of *K*<sub>S</sub> age distribution.
+```
+wgd mix ks_datafile (option)
+--------------------------------------------------------------------------------
+-f, --filters, the cutoff alignment length, default 300
+-r, --ks_range, the Ks range to be considered, default (0.005, 3)
+-b, --bins, the number of bins in Ks distribution, default 50
+-o, --outdir, the output directory, default wgd_mix
+--method, which mixture model to use, default gmm
+-n, --components, the range of the number of components to fit, default (1, 4)
+-g, --gamma, the gamma parameter for bgmm models, default 0.001
+-ni, --n_init, the number of k-means initializations, default 200
+-mi, --max_iter, the maximum number of iterations, default 1000
+```
+
+The program `wgd peak` can realize the search of crediable *K*<sub>S</sub> range used in WGD dating.
+```
+wgd peak ks_datafile (option)
+--------------------------------------------------------------------------------
+-ap, --anchorpoints, the anchor points datafile, default None
+-sm, --segments, the segments datafile, default None
+-le, --listelements, the listsegments datafile, default None 
+-mp, --multipliconpairs, the multipliconpairs datafile, default None
+-o, --outdir, the output directory, default wgd_peak
+-af, --alignfilter, cutoff for alignment identity, length and coverage, default 0.0, 0, 0.0
+-r, --ksrange, range of Ks to be analyzed, default (0, 5)
+-bw, --bin_width, bandwidth of Ks distribution, default 0.1
+-ic, --weights_outliers_included, flag option, whether to include Ks outliers, if the flag was set, Ks outliers will be included in the analysis
+-m, --method, which mixture model to use, default gmm
+--seed, random seed given to initialization, default 2352890
+-ei, --em_iter, the number of EM iterations to perform, default 200
+-ni, --n_init, the number of k-means initializations, default 200
+-n, --components, the range of the number of components to fit, default (1, 4)
+--boots, the number of bootstrap replicates of kde, default 200
+--weighted, flag option, whether to use node-weighted method of de-redundancy, if the flag was set, the node-weighted method will be used
+-p, --plot, the plotting method to be used, default identical
+-bm, --bw_method, the bandwidth method to be used, default silverman
+--n_medoids, the number of medoids to fit, default 2
+-km, --kdemethod, the kde method to be used, default scipy
+--n_clusters, the number of clusters to plot Elbow loss function, default 5
+--kmedoids, flag option, whether to initiate K-Medoids clustering analysis, if the flag was set, the analysis will be initiated
+-gd, --guide, the regime residing anchors, default: segment
+-prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+-kd, --kstodate, the range of Ks to be dated, default (0.5, 1.5)
+-f, --family, the family to filter Ks upon, default None
+--manualset, flag option, whether to output anchor pairs with manually set Ks range, if the flag was set, manually set Ks range will be used
+-rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+--ci, the confidence level of log-normal distribution to date, default 95
+--hdr, the highest densidy region (HDR) in a given distribution to date, default 95
+--heuristic, flag option, whether to initiate heuristic method of defining CI for dating, if the flag was set, the heuristic method will be initiated
+-kc, --kscutoff, the Ks saturation cutoff in dating, default 5
+```
+
+The program `wgd syn` can realize the intra- and inter-specific synteny inference.
+```
+wgd syn families gffs (option)
+--------------------------------------------------------------------------------
+-ks, --ks_distribution, ks distribution datafile, default None
+-o, --outdir, the output directory, default wgd_syn
+-f, --feature, the feature for parsing gene IDs from GFF files, default gene
+-a, --attribute, the attribute for parsing the gene IDs from the GFF files, default ID
+-ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+-ms, --maxsize, the maximum family size to include, default 200
+-r, --ks_range, the Ks range in colored dotplot, default (0, 5)
+--iadhore_options, the parameter setting in iadhore, default 
+-ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
+-mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+-kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+```
+
+The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
+```
+wgd viz (option)
+--------------------------------------------------------------------------------
+-d, --datafile, the Ks datafile, default None
+-o, --outdir, the output directory, default wgd_viz
+-sr, --spair, the species pair to be plotted, default None, this option can be provided multiple times
+-gs, --gsmap, the gene name-species name map, default None
+-sp, --speciestree, the species tree to perform rate correction, default None, if None was given, the rate correction analysis will be called off
+-pk, --plotkde, flag option, whether to plot kde curve upon histogram, if the flag was set, kde curve will be added
+-rw, --reweight, flag option, whether to recalculate the weight per species pair, if the flag was set, the weight will be recalculated
+-or, --onlyrootout, flag option, whether to only conduct rate correction using the outgroup at root as outgroup, if the flag was set, only the outgroup at root will be used as outgroup
+-iter, --em_iterations, the maximum EM iterations, default 200
+-init, --em_initializations, the maximum EM initializations, default 200
+-prct, --prominence_cutoff, the prominence cutoff of acceptable peaks, default 0.1
+-sm, --segments, the segments data file, default None
+-ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
+-ms, --maxsize, the maximum family size to include, default 200
+-ap, --anchorpoints, the anchor points datafile, default None
+-mt, --multiplicon, the multiplicons datafile, default None
+-gt, --genetable, the gene table datafile, default None
+-rh, --rel_height, the relative height at which the peak width is measured, default 0.4
+-mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
+-kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+```
+
+## Usage
+
+Here we provided the basic usage for each program.
+
+### wgd dmd
+
+**The delineation of whole paranome**
+```
+wgd dmd sequence
+``` 
+
+**The delineation of RBHs**
+```
+wgd dmd sequence1 sequence2
+```
+
+**The delineation of local MRBHs**
+```
+wgd dmd sequence1 sequence2 sequence3 -f sequence1
+```
+
+**The delineation of global MRBHs**
+```
+wgd dmd sequence1 sequence2 sequence3 -gm
+```
+
+**The delineation of orthogroups**
+```
+wgd dmd sequence1 sequence2 sequence3 -oi (option)
+```
+Note that users can add the analysis including NSOGs and BUSCO-guided SOGs etc, by adding the corresponding flags, for instance --getnsog and --buscosog.
+
+**The collinear coalescence inference of phylogeny**
+```
+wgd dmd sequence1 sequence2 sequence3 -ap apdata -sm smdata -le ledata -gt gtdata --collinearcoalescence
+```
+
+### wgd focus
+
+**The concatenation-based/coalescence-based phylogenetic inference**
+```
+wgd focus families sequence1 sequence2 sequence3 --concatenation/--coalescence
+```
+
+**The functional annotation of gene families**
+```
+wgd focus families sequence1 sequence2 sequence3 --annotation eggnog -ed eddata --dmnb dbdata
+```
+
+**The phylogenetic dating of WGDs**
+```
+wgd focus families sequence1 sequence2 sequence3 -d mcmctree -sp spdata
+```
+
+### wgd ksd
+
+**The construction of whole paranome *K*<sub>S</sub> age distribution**
+```
+wgd ksd families sequence
+```
+
+**The construction of orthologous *K*<sub>S</sub> age distribution**
+```
+wgd ksd families sequence1 sequence2
+```
+
+**The construction of *K*<sub>S</sub> age distribution with rate correction**
+```
+wgd ksd families sequence1 sequence2 sequence3 -sr srdata -sp spdata
+```
+
+### wgd mix
+
+**The mixture model clustering analysis of *K*<sub>S</sub> age distribution**
+```
+wgd mix ksdata
+```
+
+### wgd peak
+
+**The search of crediable *K*<sub>S</sub> range used in WGD dating**
+```
+wgd peak ksdata -ap apdata -sm smdata -le ledata -mp mpdata
+```
+Note that users can add the flag --heuristic to implement the heuristic search analysis
+
+### wgd syn
+
+**The intra-specific synteny inference**
+```
+wgd syn families gff
+```
+
+**The inter-specific synteny inference**
+```
+wgd syn families gff1 gff2
+```
+
+### wgd viz
+
+**The visualization of *K*<sub>S</sub> age distribution**
+```
+wgd viz -d ksdata
+```
+
+**The visualization of *K*<sub>S</sub> age distribution with rate correction**
+```
+wgd viz -d ksdata -sr srdata -sp spdata -gs gsdata
+```
+
+**The visualization of synteny**
+```
+wgd viz -ap apdata -sm smdata -mt mtdata -gt gtdata
+```
+
+## Illustration
+
+We illustrate our program on an exemplary WGD inference and dating upon species *Aquilegia coerulea*.
+
+The *Aquilegia coerulea* was reported to experience an paleo-polyploidization event after the divergence of core eudicots, which is likely shared by all Ranunculales.
+
+First above all, let's delineate the whole paranome *K*<sub>S</sub> age distribution and have a basic observation for potentially conceivable WGDs, using the command line below.
+
+```
+wgd dmd Aquilegia_coerulea
+wgd ksd wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea
+```
+
+The constructed whole paranome *K*<sub>S</sub> age distribution of *Aquilegia coerulea* is as below, we can see that there seems to be a hump at *K*<sub>S</sub> 1 but not clear.
+
+![](data/Aquilegia_coerulea.tsv.ksd_wp.svg)
+
+We then construct the anchor *K*<sub>S</sub> age distribution using the command line below.
+
+```
+wgd syn -f mRNA -a Name wgd_dmd/Aquilegia_coerulea.tsv Aquilegia_coerulea.gff3 -ks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+```
+
+As shown below, there are some retained anchor pairs with *K*<sub>S</sub> between 1 and 2, which seems to suggest a WGD event.
+
+![](data/Aquilegia_coerulea.tsv.ksd_wp_ap.svg)
+
+The associated `dupStack` plot shows that there are numerous duplicated segments across most of the chromosomes, except for the chr_07, which seems to experience more severe fragmentization than the other chromosomes.
+
+![](data/Aquilegia_coerulea_Aquilegia_coerulea_multiplicons_level.svg)
+
+The associated dotplot in oxford grid also presents numerous densely aggregated anchor points throughout most of the chromosomes.
+
+![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
+
+A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
+
+![](data/Syndepth.svg)
+
+We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
+
+```
+wgd viz -d wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv
+```
+
+The result of ELMM mixture model clustering shows that there is a likely WGD component at *K*<sub>S</sub> 1.19.
+
+![](data/elmm_Aquilegia_coerulea.tsv.ks.tsv_best_models_weighted.svg)
+
+Let's do a mixture model clustering for anchor *K*<sub>S</sub> too, using the command line below.
+
+```
+wgd peak wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv --anchorpoints wgd_syn/iadhore-out/anchorpoints.txt --segments wgd_syn/iadhore-out/segments.txt --listelements wgd_syn/iadhore-out/list_elements.txt --multipliconpairs wgd_syn/iadhore-out/multiplicon_pairs.txt --weighted
+```
+
+The anchor *K*<sub>S</sub> age distribution also has a likely WGD component with mode 1.28.
+
+![](data/Original_AnchorKs_GMM_Component3_node_weighted_Lognormal.svg)
+
+Now that we have seen the evidence of numerous duplicated segments and the aggregation of duplicates age in *K*<sub>S</sub> around 1.2 for anchor pairs and non-anchor pairs throughout the whole genome. We can claim with some confidence that *Aquilegia coerulea* might have experienced a paleo-polyploidization event. Next, Let's have a further look about its phylogenetic location. We know that there are uncertainties about whether this putative paleo-polyploidization event is shared with all eudicots or not. We can choose some other eudicot genomes to see the ordering of speciation and polyploidization events. Here we choose *Vitis vinifera*, *Protea cynaroides* and *Acorus americanus* in the following *K*<sub>S</sub> analysis. First, we built a global MRBH family using the command below.
+
+```
+wgd dmd --globalmrbh Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera -o wgd_globalmrbh
+```
+
+In the global MRBH family, every pair of orthologous genes is the reciprocal best hit, suggesting true orthologous relationships. We would use the *K*<sub>S</sub> values associated with these orthologous pairs to delimit the divergence *K*<sub>S</sub> peak. Together with the whole paranome *K*<sub>S</sub> distribution, we conduct the rate correction using the command below.
+
+```
+wgd ksd wgd_globalmrbh/global_MRBH.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
+```
+
+The file `speciestree.nw` is the text file of species tree in newick that rate correction would be conducted on. Its content is as below. Users need to provide the species pairs to be plotted. We suggest adding the option `--reweight` to recalculate the weight per species pair such that the weight of orthologous gene pairs will become 1 as the paralogous gene pairs. The flag `--plotkde` can be added when the kde curve of orthologous *K*<sub>S</sub> is desired. Extra collinear data can be added by the option `-ap`.
+
+![](data/Aquilegia_coerulea_GlobalmrbhKs_Corrected.ksd.svg)
+
+As shown above, because of the higher substitution rate of *Aquilegia coerulea*, the original orthologous *K*<sub>S</sub> values were actually underestimated in the time-frame of *Aquilegia coerulea*. When we recovered the divergence substitution distance in terms of two times of the branch-specific contribution of *Aquilegia coerulea* since its divergence with the sister species plus the shared substitution distance before divergence (in relative to the outgroup), the corrected *K*<sub>S</sub> mode became larger.
+
+```
+(((Vitis_vinifera,Protea_cynaroides),Aquilegia_coerulea),Acorus_americanus);
+```
+
+If one had the orthologous *K*<sub>S</sub> data already, one could also apply the program `wgd viz` to conduct the rate correction analysis using the command below.
+
+```
+wgd viz -d wgd_globalmrbh_ks/global_MRBH.tsv.ks.tsv --extraparanomeks wgd_ksd/Aquilegia_coerulea.tsv.ks.tsv -sp speciestree.nw --reweight -ap wgd_syn/iadhore-out/anchorpoints.txt -o wgd_viz_mixed_Ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --gsmap gene_species.map --plotkde
+```
+
+Note that a necessary gene-species map file is needed for its implementation in `wgd viz`, which should be automately produced by the last `wgd ksd` step. The `gene_species.map` has contents as below in which each line is the joined string of gene name and species name by space.
+
+```
+Aqcoe6G057800.1 Aquilegia_coerulea
+Vvi_VIT_201s0011g01530.1 Vitis_vinifera
+Pcy_Procy01g08510 Protea_cynaroides
+Aam_Acora.04G142900.1 Acorus_americanus
+```
+
+An alternative way to calculate the orthologous *K*<sub>S</sub> is to directly use the orthogroups instead of global MRBH family. That way we don't use the pre-inferred paranome *K*<sub>S</sub> but the paralogous gene pairs inside each orthogroup instead. To achieve that, we first need to infer orthogroups using the command below.
+
+```
+wgd dmd Aquilegia_coerulea Protea_cynaroides Acorus_americanus Vitis_vinifera --orthoinfer -o wgd_ortho (--onlyortho) 
+```
+
+Users can decide to only conduct the orthogroup analysis while skipping other analysis by adding the flag `--onlyortho`. Next step is the same with global MRBH family except that we don't use the extra pre-inferred paranome *K*<sub>S</sub> anymore. We infer the *K*<sub>S</sub> using the command below. Note that the program `wgd viz` can plot the same just as shown above.
+
+```
+wgd ksd wgd_ortho/Orthogroups.sp.tsv -sp speciestree.nw --reweight -o wgd_ortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus" --spair "Aquilegia_coerulea;Aquilegia_coerulea" --plotkde (-ap wgd_syn/iadhore-out/anchorpoints.txt)
+```
+
+![](data/Aquilegia_coerulea_OrthoKs_Corrected.ksd.svg)
+
+As shown above, the number of both paralogous gene pairs and orthologous gene pairs is different than the one from global MRBH family in that here we plotted all orthologous gene pairs instead of only global MRBH and potentially new paralogous gene pairs might be produced in the orthogroup inference step, together with different recalculated weights.
+
+If one only wanted to plot the orthologous *K*<sub>S</sub> distribution, it can be easily achieved by removing the paralogous species pair `Aquilegia_coerulea;Aquilegia_coerulea`, using the command below.
+
+```
+wgd ksd wgd_globalmrbh/global_MRBH.tsv -sp speciestree.nw --reweight -o wgd_globalmrbh_onlyortho_ks --spair "Aquilegia_coerulea;Protea_cynaroides" --spair "Aquilegia_coerulea;Vitis_vinifera" --spair "Aquilegia_coerulea;Acorus_americanus"
+```
+
+We can clearly see that *Vitis vinifera* has higher substitution rate than *Protea cynaroides* in that their orthologous *K*<sub>S</sub> peaks with *Aquilegia coerulea*, although representing the same divergence event, differed in substitution distance.
+![](data/Raw_Orthologues.ksd.svg)
+
+## Citation
+ 
+Please cite us at https://doi.org/10.1093/bioinformatics/bty915
+
+```
+Arthur Zwaenepoel, Yves Van de Peer, wgd—simple command line tools for the analysis of ancient whole-genome duplications, Bioinformatics, Volume 35, Issue 12, June 2019, Pages 2153–2155, https://doi.org/10.1093/bioinformatics/bty915
+
+Hengchi Chen, Arthur Zwaenepoel (2023). Inference of Ancient Polyploidy from Genomic Data. In: Van de Peer, Y. (eds) Polyploidy. Methods in Molecular Biology, vol 2545. Humana, New York, NY. https://doi.org/10.1007/978-1-0716-2561-3_1
+```
+
+For citation of the tools used in wgd, please consult the documentation at
+https://wgd.readthedocs.io/en/latest/index.html#citation.
+
```

### Comparing `wgd-2.0.13/wgd.egg-info/requires.txt` & `wgd-2.0.14/wgd.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 iniconfig==1.1.1
 Jinja2==2.11.2
 joblib==0.11
 KDEpy==1.1.0
 kiwisolver==1.2.0
 MarkupSafe==1.1.1
 matplotlib==3.2.2
-numpy>=1.19.0
+numpy!=1.24.3,>=1.19.0
 numexpr>=2.7.3
 packaging==20.4
 pandas<=1.4.4
 Pillow<=8.4.0
 pluggy==0.13.1
 plumbum==1.6.9
 progressbar2==3.51.4
```

