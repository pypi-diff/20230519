# Comparing `tmp/servicex_databinder-0.4.0b6.tar.gz` & `tmp/servicex_databinder-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicex_databinder-0.4.0b6.tar", last modified: Tue Dec 20 03:08:36 2022, max compression
+gzip compressed data, was "servicex_databinder-0.4.1.tar", last modified: Fri May 19 20:10:53 2023, max compression
```

## Comparing `servicex_databinder-0.4.0b6.tar` & `servicex_databinder-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2022-12-20 03:08:36.504110 servicex_databinder-0.4.0b6/
--rw-r--r--   0 kchoi      (501) staff       (20)     1521 2021-09-10 04:56:21.000000 servicex_databinder-0.4.0b6/LICENSE
--rw-r--r--   0 kchoi      (501) staff       (20)     9151 2022-12-20 03:08:36.503654 servicex_databinder-0.4.0b6/PKG-INFO
--rw-r--r--   0 kchoi      (501) staff       (20)     8403 2022-12-08 01:38:00.000000 servicex_databinder-0.4.0b6/README.md
-drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2022-12-20 03:08:36.501079 servicex_databinder-0.4.0b6/servicex_databinder/
--rw-r--r--   0 kchoi      (501) staff       (20)      194 2022-12-20 03:00:41.000000 servicex_databinder-0.4.0b6/servicex_databinder/__init__.py
--rw-r--r--   0 kchoi      (501) staff       (20)     4265 2022-12-09 02:05:25.000000 servicex_databinder-0.4.0b6/servicex_databinder/configuration.py
--rw-r--r--   0 kchoi      (501) staff       (20)     4980 2022-12-15 06:43:06.000000 servicex_databinder-0.4.0b6/servicex_databinder/get_servicex_data.py
--rw-r--r--   0 kchoi      (501) staff       (20)     3135 2022-11-11 14:54:29.000000 servicex_databinder-0.4.0b6/servicex_databinder/old_frontend.py
--rw-r--r--   0 kchoi      (501) staff       (20)    14312 2022-11-10 06:04:16.000000 servicex_databinder-0.4.0b6/servicex_databinder/old_output.py
--rw-r--r--   0 kchoi      (501) staff       (20)     9487 2022-12-20 02:53:17.000000 servicex_databinder-0.4.0b6/servicex_databinder/output_handler.py
--rw-r--r--   0 kchoi      (501) staff       (20)     4604 2022-12-09 02:38:51.000000 servicex_databinder-0.4.0b6/servicex_databinder/request.py
--rw-r--r--   0 kchoi      (501) staff       (20)     1401 2022-12-15 06:52:50.000000 servicex_databinder-0.4.0b6/servicex_databinder/servicex_databinder.py
-drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2022-12-20 03:08:36.503176 servicex_databinder-0.4.0b6/servicex_databinder.egg-info/
--rw-r--r--   0 kchoi      (501) staff       (20)     9151 2022-12-20 03:08:36.000000 servicex_databinder-0.4.0b6/servicex_databinder.egg-info/PKG-INFO
--rw-r--r--   0 kchoi      (501) staff       (20)      532 2022-12-20 03:08:36.000000 servicex_databinder-0.4.0b6/servicex_databinder.egg-info/SOURCES.txt
--rw-r--r--   0 kchoi      (501) staff       (20)        1 2022-12-20 03:08:36.000000 servicex_databinder-0.4.0b6/servicex_databinder.egg-info/dependency_links.txt
--rw-r--r--   0 kchoi      (501) staff       (20)      136 2022-12-20 03:08:36.000000 servicex_databinder-0.4.0b6/servicex_databinder.egg-info/requires.txt
--rw-r--r--   0 kchoi      (501) staff       (20)       20 2022-12-20 03:08:36.000000 servicex_databinder-0.4.0b6/servicex_databinder.egg-info/top_level.txt
--rw-r--r--   0 kchoi      (501) staff       (20)       38 2022-12-20 03:08:36.504217 servicex_databinder-0.4.0b6/setup.cfg
--rw-r--r--   0 kchoi      (501) staff       (20)     2148 2022-12-09 05:22:58.000000 servicex_databinder-0.4.0b6/setup.py
+drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2023-05-19 20:10:53.396991 servicex_databinder-0.4.1/
+-rw-r--r--   0 kchoi      (501) staff       (20)     1521 2021-09-10 04:56:21.000000 servicex_databinder-0.4.1/LICENSE
+-rw-r--r--   0 kchoi      (501) staff       (20)     9996 2023-05-19 20:10:53.396359 servicex_databinder-0.4.1/PKG-INFO
+-rw-r--r--   0 kchoi      (501) staff       (20)     9230 2023-05-19 20:08:18.000000 servicex_databinder-0.4.1/README.md
+drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2023-05-19 20:10:53.392432 servicex_databinder-0.4.1/servicex_databinder/
+-rw-r--r--   0 kchoi      (501) staff       (20)      200 2023-05-19 20:06:27.000000 servicex_databinder-0.4.1/servicex_databinder/__init__.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     7030 2023-05-09 00:07:57.000000 servicex_databinder-0.4.1/servicex_databinder/configuration.py
+-rw-r--r--   0 kchoi      (501) staff       (20)    10174 2023-05-09 00:07:45.000000 servicex_databinder-0.4.1/servicex_databinder/get_servicex_data.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     3135 2022-11-11 14:54:29.000000 servicex_databinder-0.4.1/servicex_databinder/old_frontend.py
+-rw-r--r--   0 kchoi      (501) staff       (20)    14312 2022-11-10 06:04:16.000000 servicex_databinder-0.4.1/servicex_databinder/old_output.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     7138 2023-05-19 19:57:15.000000 servicex_databinder-0.4.1/servicex_databinder/output_handler.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     5313 2023-05-19 20:00:13.000000 servicex_databinder-0.4.1/servicex_databinder/request.py
+-rw-r--r--   0 kchoi      (501) staff       (20)     1493 2023-05-05 22:26:25.000000 servicex_databinder-0.4.1/servicex_databinder/servicex_databinder.py
+drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2023-05-19 20:10:53.394850 servicex_databinder-0.4.1/servicex_databinder.egg-info/
+-rw-r--r--   0 kchoi      (501) staff       (20)     9996 2023-05-19 20:10:53.000000 servicex_databinder-0.4.1/servicex_databinder.egg-info/PKG-INFO
+-rw-r--r--   0 kchoi      (501) staff       (20)      553 2023-05-19 20:10:53.000000 servicex_databinder-0.4.1/servicex_databinder.egg-info/SOURCES.txt
+-rw-r--r--   0 kchoi      (501) staff       (20)        1 2023-05-19 20:10:53.000000 servicex_databinder-0.4.1/servicex_databinder.egg-info/dependency_links.txt
+-rw-r--r--   0 kchoi      (501) staff       (20)      123 2023-05-19 20:10:53.000000 servicex_databinder-0.4.1/servicex_databinder.egg-info/requires.txt
+-rw-r--r--   0 kchoi      (501) staff       (20)       20 2023-05-19 20:10:53.000000 servicex_databinder-0.4.1/servicex_databinder.egg-info/top_level.txt
+-rw-r--r--   0 kchoi      (501) staff       (20)       38 2023-05-19 20:10:53.397081 servicex_databinder-0.4.1/setup.cfg
+-rw-r--r--   0 kchoi      (501) staff       (20)     2117 2023-05-10 03:52:22.000000 servicex_databinder-0.4.1/setup.py
+drwxr-xr-x   0 kchoi      (501) staff       (20)        0 2023-05-19 20:10:53.395358 servicex_databinder-0.4.1/tests/
+-rw-r--r--   0 kchoi      (501) staff       (20)     5461 2021-10-28 07:08:46.000000 servicex_databinder-0.4.1/tests/test_config.py
```

### Comparing `servicex_databinder-0.4.0b6/LICENSE` & `servicex_databinder-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.0b6/PKG-INFO` & `servicex_databinder-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,163 +1,180 @@
 Metadata-Version: 2.1
 Name: servicex_databinder
-Version: 0.4.0b6
-Summary: ServiceX data management using a configuration file
+Version: 0.4.1
+Summary: ServiceX data management                     using a configuration file
 Home-page: https://github.com/kyungeonchoi/ServiceXDataBinder
 Author: KyungEon Choi (UT Austin)
 Author-email: kyungeonchoi@utexas.edu
 License: BSD 3-clause
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ServiceX DataBinder
 
-<p align="right"> Release v0.4.0b2 </p>
+<p align="right"> Release v0.4.1 </p>
 
 [![PyPI version](https://badge.fury.io/py/servicex-databinder.svg)](https://badge.fury.io/py/servicex-databinder)
 
-<!-- `servicex-databinder` is a Python package for making multiple ServiceX requests and managing ServiceX delivered data from a configuration file.  -->
-
-`servicex-databinder` is a Python package to interact with ServiceX instance to make ServiceX request(s) and manage ServiceX delivered data efficiently from a single configuration file.
-
-The package is particularly useful when accessing multiple remote data via ServiceX, e.g. full-scale analysis or extracting input data for machine learning.
-
-Brief introduction of ServiceX and walk-though of various DataBinder features can be found 
-in this [Jupyter notebook](https://nbviewer.org/github/kyungeonchoi/irishep_topical_ServiceXDataBinder/blob/main/16Nov2022_choi.ipynb).
+`servicex-databinder` is a user-analysis data management package using a single configuration file. 
+Samples with external data sources (e.g. `RucioDID` or `XRootDFiles`) utilize ServiceX to deliver user-selected columns with optional row filtering.
+<!-- to interact with ServiceX instance to make ServiceX request(s) and manage ServiceX delivered data from a single configuration file. -->
+
+The following table shows supported ServiceX transformers by DataBinder
+
+| Input format | Code generator | Transformer | Output format
+| :--- | :---: | :---: | :---: |
+| ROOT Ntuple | func-adl | `uproot` | `root` or `parquet` |
+| ATLAS Release 21 xAOD | func-adl | `atlasr21`| `root` |
+<!-- | ROOT Ntuple | python function | `python`| -->
 
 <!-- [`ServiceX`](https://github.com/ssl-hep/ServiceX) is a scalable HEP event data extraction, transformation and delivery system. 
 
 ['ServiceX Client library'](https://github.com/ssl-hep/ServiceX_frontend) provides  --> 
 
 ## Prerequisite
 - [Access to a ServiceX instance](https://servicex.readthedocs.io/en/latest/user/getting-started/)
-- Python 3.6+
+- Python 3.7+
 
 ## Installation
 ```shell
 pip install servicex-databinder
 ```
 
 ## Configuration file
 
 The configuration file is a yaml file containing all the information.
-An example configuration file is shown below:
+
+The [following example configuration file](config_minimum.yaml) contains minimal fields. You can also download [`servicex-opendata.yaml`](servicex-opendata.yaml) file (rename to `servicex.yaml`) at your working directory, and run DataBinder for OpenData without an access token.
 
 ```yaml
 General:
-  ServiceXBackendName: uproot
-  OutputDirectory: /path/to/output
+  ServiceXName: servicex-opendata
   OutputFormat: parquet
   
 Sample:
-  - Name: ttH
-    RucioDID: user.kchoi:user.kchoi.sampleA, 
-             user.kchoi:user.kchoi.sampleB
-    Tree: nominal
-    FuncADL: "Select(lambda event: {'jet_e': event.jet_e})"
-  - Name: ttW
-    XRootDFiles: root://ttW.root
-    Tree: nominal
-    Filter: n_jet > 5 
-    Columns: jet_e, jet_pt
-  - Name: ttZ
-    LocalPath: /home/kchoi/ttZ
-    Tree: nominal
+  - Name: ggH125_ZZ4lep
+    XRootDFiles: "root://eospublic.cern.ch//eos/opendata/atlas/OutreachDatasets\
+                  /2020-01-22/4lep/MC/mc_345060.ggH125_ZZ4lep.4lep.root"
+    Tree: mini
+    Columns: lep_pt, lep_eta
 ```
 
-`General` block requires three mandatory options as in the example above.
+`General` block requires two mandatory options (`ServiceXName` and `OutputFormat`) as in the example above.
 
-Input dataset for each Sample can be defined either by `RucioDID` or `XRootDFiles` or `LocalPath`. You need to make sure whether the ServiceX backend you specified in `ServiceXBackendName` supports Rucio and/or XRootD. 
+Input dataset for each Sample can be defined either by `RucioDID` or `XRootDFiles` or `LocalPath`.
 
 ServiceX query can be constructed with either TCut syntax or func-adl.
 - Options for TCut syntax: `Filter`<sup>1</sup> and `Columns`
 - Option for Func-adl expression: `FuncADL`
 
 &nbsp; &nbsp; &nbsp; <sup>1</sup> `Filter` works only for scalar-type of TBranch.
 
 Output format can be either `Apache parquet` or `ROOT ntuple` for `uproot` backend. Only `ROOT ntuple` format is supported for `xAOD` backend.
 
-Please find other example configurations for ATLAS opendata, xAOD, and Uproot ServiceX endpoints.
-
 
 The followings are available options:
 
 <!-- `General` block: -->
 | Option for `General` block | Description       | DataType |
 |:--------:|:------:|:------|
-| `ServiceXBackendName`* | ServiceX backend name in your `servicex.yaml` file <br> (name MUST contain either `uproot` or `xaod` to distinguish the type of transformer) | `String` |
-| `OutputDirectory`* | Path to the directory for ServiceX delivered files | `String` |
+| `ServiceXName`* | ServiceX backend name in your `servicex.yaml` file <br>  | `String` |
+| `OutputDirectory` | Path to the directory for ServiceX delivered files | `String` |
 | `OutputFormat`* | Output file format of ServiceX delivered data (`parquet` or `root` for `uproot` / `root` for `xaod`) | `String` |
-| `ZipROOTColumns` | Zip columns that share prefix to generate one counter branch (see detail at [uproot readthedoc](https://uproot.readthedocs.io/en/latest/basic.html#writing-ttrees-to-a-file)) | `Boolean` |
 | `WriteOutputDict` | Name of an ouput yaml file containing Python nested dictionary of output file paths (located in the `OutputDirectory`) | `String` |
 | `IgnoreServiceXCache` | Ignore the existing ServiceX cache and force to make ServiceX requests | `Boolean` |
 <p align="right"> *Mandatory options</p>
 
 | Option for `Sample` block | Description       |DataType |
 |:--------:|:------:|:------|
 | `Name`   | sample name defined by a user |`String` |
 | `RucioDID` | Rucio Dataset Id (DID) for a given sample; <br> Can be multiple DIDs separated by comma |`String` |
 | `XRootDFiles` | XRootD files (e.g. `root://`) for a given sample; <br> Can be multiple files separated by comma |`String` |
 | `Tree` | Name of the input ROOT `TTree`; <br> Can be multiple `TTree`s separated by comma (`uproot` ONLY) |`String` |
 | `Filter` | Selection in the TCut syntax, e.g. `jet_pt > 10e3 && jet_eta < 2.0` (TCut ONLY) |`String` |
 | `Columns` | List of columns (or branches) to be delivered; multiple columns separately by comma (TCut ONLY) |`String` |
-| `FuncADL` | func-adl expression for a given sample (see [example](config_example_xaod.yml)) |`String` |
+| `FuncADL` | func-adl expression for a given sample |`String` |
 | `LocalPath` | File path directly from local path (NO ServiceX tranformation) | `String` |
 
  <!-- Options exclusively for TCut syntax (CANNOT combine with the option `FuncADL`) -->
 
  <!-- Option for func-adl expression (CANNOT combine with the option `Fitler` and `Columns`) -->
 
-A config file can be simplified by utilizing `Definition` block. You can define placeholders under `Definition` block, which will replace all matched placeholders in the values of `Sample` block. Note that placeholders must start with `DEF_`. The example configuration file can be also written as below with `Definition` block:
+A config file can be simplified by utilizing `Definition` block. You can define placeholders under `Definition` block, which will replace all matched placeholders in the values of `Sample` block. Note that placeholders must start with `DEF_`.
+
+You can source each Sample using different ServiceX transformers. 
+The default transformer is set by `type` of `servicex.yaml`, but `Transformer` in the `General` block overwrites if present, and `Transformer` in each `Sample` overwrites any previous transformer selection.
+
+The [following example configuration](config_maximum.yaml) shows how to use each Options.
 
 ```yaml
 General:
-  ServiceXBackendName: uproot
-  OutputDirectory: /path/to/output
-  OutputFormat: parquet
+  ServiceXName: servicex-uc-af
+  Transformer: uproot
+  OutputFormat: root
+  OutputDirectory: /Users/kchoi/data_for_MLstudy
+  WriteOutputDict: fileset_ml_study
+  IgnoreServiceXCache: False
   
-Sample:
-  - Name: ttH
-    RucioDID: DEF_ttH_dids
-    Tree: nominal
-    FuncADL: DEF_nominal_selection
-  - Name: ttW
-    RucioDID: user.kchoi:user.kchoi.sampleC
+Sample:  
+  - Name: Signal
+    RucioDID: user.kchoi:user.kchoi.signalA,
+              user.kchoi:user.kchoi.signalB,
+              user.kchoi:user.kchoi.signalC
     Tree: nominal
-    Filter: n_jet > 5 
-    Columns: jet_e, jet_pt
+    FuncADL: DEF_ttH_nominal_query
+  - Name: Background1
+    XRootDFiles: DEF_ggH_input
+    Tree: mini
+    Filter: lep_n>2
+    Columns: lep_pt, lep_eta
+  - Name: Background2
+    Transformer: atlasr21
+    RucioDID: DEF_Zee_input
+    FuncADL: DEF_Zee_query
+  - Name: Background3
+    LocalPath: /Users/kchoi/Work/data/background3
 
 Definition:
-  DEF_ttH_dids: user.kchoi:user.kchoi.sampleA, 
-             user.kchoi:user.kchoi.sampleB
-  DEF_nominal_selection: "Select(lambda event: {'jet_e': event.jet_e})"
+  DEF_ttH_nominal_query: "Where(lambda e: e.met_met>150e3). \
+              Select(lambda event: {'el_pt': event.el_pt, 'jet_e': event.jet_e, \
+              'jet_pt': event.jet_pt, 'met_met': event.met_met})"
+  DEF_ggH_input: "root://eospublic.cern.ch//eos/opendata/atlas/OutreachDatasets\
+                  /2020-01-22/4lep/MC/mc_345060.ggH125_ZZ4lep.4lep.root"
+  DEF_Zee_input: "mc15_13TeV:mc15_13TeV.361106.PowhegPythia8EvtGen_AZNLOCTEQ6L1_Zee.\
+                merge.DAOD_STDM3.e3601_s2576_s2132_r6630_r6264_p2363_tid05630052_00"
+  DEF_Zee_query: "SelectMany('lambda e: e.Jets(\"AntiKt4EMTopoJets\")'). \
+              Where('lambda j: (j.pt() / 1000) > 30'). \
+              Select('lambda j: j.pt() / 1000.0'). \
+              AsROOTTTree('junk.root', 'my_tree', [\"JetPt\"])"
 ```
 
+
 ## Deliver data
 
 ```python
 from servicex_databinder import DataBinder
 sx_db = DataBinder('<CONFIG>.yml')
 out = sx_db.deliver()
 ```
 
-The function `deliver()` returns a Python nested dictionary that contains delivered files: 
-- for `uproot` backend and `parquet` output format: `out['<SAMPLE>']['<TREE>'] = [ List of output parquet files ]`
+The function `deliver()` returns a Python nested dictionary that contains delivered files.
+<!-- - for `uproot` backend and `parquet` output format: `out['<SAMPLE>']['<TREE>'] = [ List of output parquet files ]`
 - for `uproot` backend and `root` output format: `out['<SAMPLE>'] = [ List of output root files ]`
-- for `xAOD` backend: `out['<SAMPLE>'] = [ List of output root files ]`
+- for `xAOD` backend: `out['<SAMPLE>'] = [ List of output root files ]` -->
 
 Input configuration can be also passed in a form of a Python dictionary.
 
 Delivered Samples and files in the `OutputDirectory` are always synced with the DataBinder config file.
 
 <!-- ## Currently available 
 - Dataset as Rucio DID + Input file format is ROOT TTree + ServiceX delivers output in parquet format
```

### Comparing `servicex_databinder-0.4.0b6/README.md` & `servicex_databinder-0.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,142 +1,159 @@
 # ServiceX DataBinder
 
-<p align="right"> Release v0.4.0b2 </p>
+<p align="right"> Release v0.4.1 </p>
 
 [![PyPI version](https://badge.fury.io/py/servicex-databinder.svg)](https://badge.fury.io/py/servicex-databinder)
 
-<!-- `servicex-databinder` is a Python package for making multiple ServiceX requests and managing ServiceX delivered data from a configuration file.  -->
-
-`servicex-databinder` is a Python package to interact with ServiceX instance to make ServiceX request(s) and manage ServiceX delivered data efficiently from a single configuration file.
-
-The package is particularly useful when accessing multiple remote data via ServiceX, e.g. full-scale analysis or extracting input data for machine learning.
-
-Brief introduction of ServiceX and walk-though of various DataBinder features can be found 
-in this [Jupyter notebook](https://nbviewer.org/github/kyungeonchoi/irishep_topical_ServiceXDataBinder/blob/main/16Nov2022_choi.ipynb).
+`servicex-databinder` is a user-analysis data management package using a single configuration file. 
+Samples with external data sources (e.g. `RucioDID` or `XRootDFiles`) utilize ServiceX to deliver user-selected columns with optional row filtering.
+<!-- to interact with ServiceX instance to make ServiceX request(s) and manage ServiceX delivered data from a single configuration file. -->
+
+The following table shows supported ServiceX transformers by DataBinder
+
+| Input format | Code generator | Transformer | Output format
+| :--- | :---: | :---: | :---: |
+| ROOT Ntuple | func-adl | `uproot` | `root` or `parquet` |
+| ATLAS Release 21 xAOD | func-adl | `atlasr21`| `root` |
+<!-- | ROOT Ntuple | python function | `python`| -->
 
 <!-- [`ServiceX`](https://github.com/ssl-hep/ServiceX) is a scalable HEP event data extraction, transformation and delivery system. 
 
 ['ServiceX Client library'](https://github.com/ssl-hep/ServiceX_frontend) provides  --> 
 
 ## Prerequisite
 - [Access to a ServiceX instance](https://servicex.readthedocs.io/en/latest/user/getting-started/)
-- Python 3.6+
+- Python 3.7+
 
 ## Installation
 ```shell
 pip install servicex-databinder
 ```
 
 ## Configuration file
 
 The configuration file is a yaml file containing all the information.
-An example configuration file is shown below:
+
+The [following example configuration file](config_minimum.yaml) contains minimal fields. You can also download [`servicex-opendata.yaml`](servicex-opendata.yaml) file (rename to `servicex.yaml`) at your working directory, and run DataBinder for OpenData without an access token.
 
 ```yaml
 General:
-  ServiceXBackendName: uproot
-  OutputDirectory: /path/to/output
+  ServiceXName: servicex-opendata
   OutputFormat: parquet
   
 Sample:
-  - Name: ttH
-    RucioDID: user.kchoi:user.kchoi.sampleA, 
-             user.kchoi:user.kchoi.sampleB
-    Tree: nominal
-    FuncADL: "Select(lambda event: {'jet_e': event.jet_e})"
-  - Name: ttW
-    XRootDFiles: root://ttW.root
-    Tree: nominal
-    Filter: n_jet > 5 
-    Columns: jet_e, jet_pt
-  - Name: ttZ
-    LocalPath: /home/kchoi/ttZ
-    Tree: nominal
+  - Name: ggH125_ZZ4lep
+    XRootDFiles: "root://eospublic.cern.ch//eos/opendata/atlas/OutreachDatasets\
+                  /2020-01-22/4lep/MC/mc_345060.ggH125_ZZ4lep.4lep.root"
+    Tree: mini
+    Columns: lep_pt, lep_eta
 ```
 
-`General` block requires three mandatory options as in the example above.
+`General` block requires two mandatory options (`ServiceXName` and `OutputFormat`) as in the example above.
 
-Input dataset for each Sample can be defined either by `RucioDID` or `XRootDFiles` or `LocalPath`. You need to make sure whether the ServiceX backend you specified in `ServiceXBackendName` supports Rucio and/or XRootD. 
+Input dataset for each Sample can be defined either by `RucioDID` or `XRootDFiles` or `LocalPath`.
 
 ServiceX query can be constructed with either TCut syntax or func-adl.
 - Options for TCut syntax: `Filter`<sup>1</sup> and `Columns`
 - Option for Func-adl expression: `FuncADL`
 
 &nbsp; &nbsp; &nbsp; <sup>1</sup> `Filter` works only for scalar-type of TBranch.
 
 Output format can be either `Apache parquet` or `ROOT ntuple` for `uproot` backend. Only `ROOT ntuple` format is supported for `xAOD` backend.
 
-Please find other example configurations for ATLAS opendata, xAOD, and Uproot ServiceX endpoints.
-
 
 The followings are available options:
 
 <!-- `General` block: -->
 | Option for `General` block | Description       | DataType |
 |:--------:|:------:|:------|
-| `ServiceXBackendName`* | ServiceX backend name in your `servicex.yaml` file <br> (name MUST contain either `uproot` or `xaod` to distinguish the type of transformer) | `String` |
-| `OutputDirectory`* | Path to the directory for ServiceX delivered files | `String` |
+| `ServiceXName`* | ServiceX backend name in your `servicex.yaml` file <br>  | `String` |
+| `OutputDirectory` | Path to the directory for ServiceX delivered files | `String` |
 | `OutputFormat`* | Output file format of ServiceX delivered data (`parquet` or `root` for `uproot` / `root` for `xaod`) | `String` |
-| `ZipROOTColumns` | Zip columns that share prefix to generate one counter branch (see detail at [uproot readthedoc](https://uproot.readthedocs.io/en/latest/basic.html#writing-ttrees-to-a-file)) | `Boolean` |
 | `WriteOutputDict` | Name of an ouput yaml file containing Python nested dictionary of output file paths (located in the `OutputDirectory`) | `String` |
 | `IgnoreServiceXCache` | Ignore the existing ServiceX cache and force to make ServiceX requests | `Boolean` |
 <p align="right"> *Mandatory options</p>
 
 | Option for `Sample` block | Description       |DataType |
 |:--------:|:------:|:------|
 | `Name`   | sample name defined by a user |`String` |
 | `RucioDID` | Rucio Dataset Id (DID) for a given sample; <br> Can be multiple DIDs separated by comma |`String` |
 | `XRootDFiles` | XRootD files (e.g. `root://`) for a given sample; <br> Can be multiple files separated by comma |`String` |
 | `Tree` | Name of the input ROOT `TTree`; <br> Can be multiple `TTree`s separated by comma (`uproot` ONLY) |`String` |
 | `Filter` | Selection in the TCut syntax, e.g. `jet_pt > 10e3 && jet_eta < 2.0` (TCut ONLY) |`String` |
 | `Columns` | List of columns (or branches) to be delivered; multiple columns separately by comma (TCut ONLY) |`String` |
-| `FuncADL` | func-adl expression for a given sample (see [example](config_example_xaod.yml)) |`String` |
+| `FuncADL` | func-adl expression for a given sample |`String` |
 | `LocalPath` | File path directly from local path (NO ServiceX tranformation) | `String` |
 
  <!-- Options exclusively for TCut syntax (CANNOT combine with the option `FuncADL`) -->
 
  <!-- Option for func-adl expression (CANNOT combine with the option `Fitler` and `Columns`) -->
 
-A config file can be simplified by utilizing `Definition` block. You can define placeholders under `Definition` block, which will replace all matched placeholders in the values of `Sample` block. Note that placeholders must start with `DEF_`. The example configuration file can be also written as below with `Definition` block:
+A config file can be simplified by utilizing `Definition` block. You can define placeholders under `Definition` block, which will replace all matched placeholders in the values of `Sample` block. Note that placeholders must start with `DEF_`.
+
+You can source each Sample using different ServiceX transformers. 
+The default transformer is set by `type` of `servicex.yaml`, but `Transformer` in the `General` block overwrites if present, and `Transformer` in each `Sample` overwrites any previous transformer selection.
+
+The [following example configuration](config_maximum.yaml) shows how to use each Options.
 
 ```yaml
 General:
-  ServiceXBackendName: uproot
-  OutputDirectory: /path/to/output
-  OutputFormat: parquet
+  ServiceXName: servicex-uc-af
+  Transformer: uproot
+  OutputFormat: root
+  OutputDirectory: /Users/kchoi/data_for_MLstudy
+  WriteOutputDict: fileset_ml_study
+  IgnoreServiceXCache: False
   
-Sample:
-  - Name: ttH
-    RucioDID: DEF_ttH_dids
-    Tree: nominal
-    FuncADL: DEF_nominal_selection
-  - Name: ttW
-    RucioDID: user.kchoi:user.kchoi.sampleC
+Sample:  
+  - Name: Signal
+    RucioDID: user.kchoi:user.kchoi.signalA,
+              user.kchoi:user.kchoi.signalB,
+              user.kchoi:user.kchoi.signalC
     Tree: nominal
-    Filter: n_jet > 5 
-    Columns: jet_e, jet_pt
+    FuncADL: DEF_ttH_nominal_query
+  - Name: Background1
+    XRootDFiles: DEF_ggH_input
+    Tree: mini
+    Filter: lep_n>2
+    Columns: lep_pt, lep_eta
+  - Name: Background2
+    Transformer: atlasr21
+    RucioDID: DEF_Zee_input
+    FuncADL: DEF_Zee_query
+  - Name: Background3
+    LocalPath: /Users/kchoi/Work/data/background3
 
 Definition:
-  DEF_ttH_dids: user.kchoi:user.kchoi.sampleA, 
-             user.kchoi:user.kchoi.sampleB
-  DEF_nominal_selection: "Select(lambda event: {'jet_e': event.jet_e})"
+  DEF_ttH_nominal_query: "Where(lambda e: e.met_met>150e3). \
+              Select(lambda event: {'el_pt': event.el_pt, 'jet_e': event.jet_e, \
+              'jet_pt': event.jet_pt, 'met_met': event.met_met})"
+  DEF_ggH_input: "root://eospublic.cern.ch//eos/opendata/atlas/OutreachDatasets\
+                  /2020-01-22/4lep/MC/mc_345060.ggH125_ZZ4lep.4lep.root"
+  DEF_Zee_input: "mc15_13TeV:mc15_13TeV.361106.PowhegPythia8EvtGen_AZNLOCTEQ6L1_Zee.\
+                merge.DAOD_STDM3.e3601_s2576_s2132_r6630_r6264_p2363_tid05630052_00"
+  DEF_Zee_query: "SelectMany('lambda e: e.Jets(\"AntiKt4EMTopoJets\")'). \
+              Where('lambda j: (j.pt() / 1000) > 30'). \
+              Select('lambda j: j.pt() / 1000.0'). \
+              AsROOTTTree('junk.root', 'my_tree', [\"JetPt\"])"
 ```
 
+
 ## Deliver data
 
 ```python
 from servicex_databinder import DataBinder
 sx_db = DataBinder('<CONFIG>.yml')
 out = sx_db.deliver()
 ```
 
-The function `deliver()` returns a Python nested dictionary that contains delivered files: 
-- for `uproot` backend and `parquet` output format: `out['<SAMPLE>']['<TREE>'] = [ List of output parquet files ]`
+The function `deliver()` returns a Python nested dictionary that contains delivered files.
+<!-- - for `uproot` backend and `parquet` output format: `out['<SAMPLE>']['<TREE>'] = [ List of output parquet files ]`
 - for `uproot` backend and `root` output format: `out['<SAMPLE>'] = [ List of output root files ]`
-- for `xAOD` backend: `out['<SAMPLE>'] = [ List of output root files ]`
+- for `xAOD` backend: `out['<SAMPLE>'] = [ List of output root files ]` -->
 
 Input configuration can be also passed in a form of a Python dictionary.
 
 Delivered Samples and files in the `OutputDirectory` are always synced with the DataBinder config file.
 
 <!-- ## Currently available 
 - Dataset as Rucio DID + Input file format is ROOT TTree + ServiceX delivers output in parquet format
```

### Comparing `servicex_databinder-0.4.0b6/servicex_databinder/old_frontend.py` & `servicex_databinder-0.4.1/servicex_databinder/old_frontend.py`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.0b6/servicex_databinder/old_output.py` & `servicex_databinder-0.4.1/servicex_databinder/old_output.py`

 * *Files identical despite different names*

### Comparing `servicex_databinder-0.4.0b6/servicex_databinder/output_handler.py` & `servicex_databinder-0.4.1/servicex_databinder/output_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,194 +1,174 @@
 import yaml
 from pathlib import Path
-from typing import Any, Dict, List
-import time
-from filecmp import cmp
+from typing import Any, Dict
 from shutil import rmtree
-from aioshutil import copy
 
 import pyarrow.parquet as pq
 import awkward as ak
 import uproot
 
 import logging
 log = logging.getLogger(__name__)
 
+
 class OutputHandler:
 
     def __init__(self, config: Dict[str, Any]) -> None:
         self._config = config
-        if "uproot" in config['General']['ServiceXBackendName'].lower():
-            self._backend = "uproot"
-        elif "xaod" in config['General']['ServiceXBackendName'].lower():
-            self._backend = "xaod"
-        self._outputformat = self._config.get('General')['OutputFormat'].lower()
 
-        """Prepare output path dictionary"""        
-        out_paths = {}    
+        """
+        Prepare output path dictionary
+        """
+        out_paths = {}
         samples = []
-        [samples.append(sample['Name']) for sample in config['Sample'] if sample['Name'] not in samples]
+        [samples.append(sample['Name'])
+            for sample in config['Sample'] if sample['Name'] not in samples]
         for sample in samples:
             out_paths[sample] = {}
-        # if self._outputformat == "parquet":
-        # if "uproot" == self._backend:
         for sample in config['Sample']:
+            # if sample['Transformer'] == "uproot":
             if 'Tree' in sample.keys():
                 for tree in sample['Tree'].split(','):
                     out_paths[sample['Name']][tree.strip()] = []
+
         self.out_paths_dict = out_paths
 
-        """Create output directory"""
+        """
+        Create output directory
+        """
         if 'OutputDirectory' in self._config['General'].keys():
-            self.output_path = Path(self._config['General']['OutputDirectory']).absolute()
+            self.output_path = Path(
+                self._config['General']['OutputDirectory']
+                ).absolute()
             self.output_path.mkdir(parents=True, exist_ok=True)
         else:
             self.output_path = Path('ServiceXData').absolute()
             self.output_path.mkdir(parents=True, exist_ok=True)
 
-
-    ##################################
-    ### parquet to ROOT conversion ###
-    ##################################
     def parquet_to_root(self, tree_name, pq_file, root_file):
-        """Write ROOT ntuple from parquet file"""
+        """
+        Write ROOT ntuple from parquet file
+        """
         if pq.read_metadata(pq_file).num_rows == 0:
             pass
         else:
             outfile = uproot.recreate(root_file)
             tree_dict = {}
             ak_arr = ak.from_parquet(pq_file)
             for field in ak_arr.fields:
                 tree_dict[field] = ak_arr[field]
             outfile[tree_name] = tree_dict
             outfile.close()
 
-
-    #################################
-    ### Copy, update and clean up ###
-    #################################
-    
-    async def copy_files(self, req, files: List[Path]):
-        if (self._backend, self._outputformat) == ('uproot', 'root'):
+    def update_output_paths_dict(self, req, files, format: str = "parquet"):
+        """
+        Outfile paths dictionary
+        Add files based on the returned file list from ServiceX
+        """
+        if req['codegen'] == "uproot":
             target_path = Path(self.output_path, req['Sample'], req['tree'])
-            if not target_path.exists():
-                target_path.mkdir(parents=True, exist_ok=True)
-                for file in files:
-                    outfile = Path(target_path, Path(file).name)
-                    await copy(file, outfile)
-                return f"  {req['Sample']} | {req['tree']} | {str(req['dataset'])[:100]} is delivered"
-            else: # target directory exists
-                servicex_files = {Path(file).name for file in files}
-                local_files = {Path(file).name for file in list(target_path.glob("*"))}
-                servicex_file_path = Path(files[0]).parent
-                
-                # copy files in servicex but not in local
-                files_not_in_local = servicex_files.difference(local_files)
-                if files_not_in_local:
-                    for file in files_not_in_local:
-                        await copy(Path(servicex_file_path, file), Path(target_path, file))
-
-                # copy updated files                
-                files_intersect = servicex_files.intersection(local_files)
-                if files_intersect:
-                    for file in files_intersect:
-                        if not cmp(Path(servicex_file_path, file), Path(target_path, file)):
-                            await copy(Path(servicex_file_path, file), Path(target_path, file))
-                        
-                return f"  {req['Sample']} | {req['tree']} | {str(req['dataset'])[:100]} is delivered"                
-
-
-    def clean_up_files_not_in_requests(self, out_paths_dict):
-
-        samples_in_requests = out_paths_dict.keys()
-        samples_local = [sa.name for sa in self.output_path.iterdir() if sa.is_dir()]
-
-        if self._backend == "uproot":
-            for sample in samples_local:
-                if not sample in samples_in_requests:
-                    rmtree(Path(self.output_path, sample))
-                else:
-                    # if self._outputformat == "parquet":
-                    for tree in [tr.name for tr in Path(self.output_path, sample).iterdir() if tr.is_dir()]:
-                        if tree in out_paths_dict[sample].keys():
-                            files_local = set(Path(self.output_path, sample, tree).glob("*"))
-                            files_request = set([Path(item) for item in out_paths_dict[sample][tree]])
-                            for tbd in files_local.difference(files_request):
-                                Path.unlink(tbd)
-                        else:
-                            rmtree(Path(self.output_path, sample, tree))
-                    # delete files if output format was root before
-                    for fi in [fi.name for fi in Path(self.output_path, sample).iterdir() if fi.is_file()]:
-                        Path.unlink(Path(self.output_path, sample, fi))
-                    # elif self._outputformat == "root":
-                    #     for tree in [tr.name for tr in Path(self.output_path, sample).iterdir() if tr.is_dir()]:
-                    #         rmtree(Path(self.output_path, sample, tree))                            
-                    #     files_local = set(Path(self.output_path, sample).glob("*"))
-                    #     files_request = set([Path(item) for item in out_paths_dict[sample]])
-                    #     for tbd in files_local.difference(files_request):
-                    #         Path.unlink(tbd)
-                        
-        elif self._backend == "xaod":
-            for sample in samples_local:
-                if not sample in samples_in_requests:
-                    rmtree(Path(self.output_path, sample))
-                else:
-                    files_local = set(Path(self.output_path, sample).glob("*"))
-                    files_request = set([Path(item) for item in out_paths_dict[sample]])
-                    for tbd in files_local.difference(files_request):
-                        Path.unlink(tbd)
-
-        return
-
-    
-    ########################################
-    ### Dictionary for output file paths ###
-    ########################################
-    def update_output_paths_dict(self, req, files, format:str = "parquet"):
-        # if self._outputformat == "parquet":
-            # Outfile paths dictionary - add files based on the returned file list from ServiceX
-        target_path = Path(self.output_path, req['Sample'], req['tree'])
-        paths_in_output_dict = self.out_paths_dict[req['Sample']][req['tree']]
-        new_files = [str(Path(target_path, Path(file).name)) for file in files]
-        if paths_in_output_dict:
-            output_dict = list(set(paths_in_output_dict + new_files))
-        else:
-            output_dict = new_files
-        self.out_paths_dict[req['Sample']][req['tree']] = output_dict
-        # elif self._outputformat == "root":
-        #     target_path = Path(self.output_path, req['Sample'])
-        #     paths_in_output_dict = self.out_paths_dict[req['Sample']]
-        #     new_files = [str(Path(target_path, Path(file).name)) for file in files]
-        #     if paths_in_output_dict:
-        #         output_dict = list(set(paths_in_output_dict + new_files))
-        #     else:
-        #         output_dict = new_files
-        #     self.out_paths_dict[req['Sample']] = output_dict
-
+            paths_in_output_dict = \
+                self.out_paths_dict[req['Sample']][req['tree']]
+            if format == "parquet":
+                new_files = [str(Path(target_path,
+                                      Path(file).name)) for file in files]
+            elif format == "root":
+                new_files = [
+                    str(Path(target_path, Path(file).name)
+                        .with_suffix('.root'))
+                    for file in files
+                            ]
+
+            if paths_in_output_dict:
+                output_dict = list(set(paths_in_output_dict + new_files))
+            else:
+                output_dict = new_files
+
+            self.out_paths_dict[req['Sample']][req['tree']] = output_dict
+        elif req['codegen'] == "atlasr21":
+            target_path = Path(self.output_path, req['Sample'])
+            paths_in_output_dict = self.out_paths_dict[req['Sample']]
+            new_files = [
+                str(Path(target_path, Path(file).name))
+                for file in files
+                ]
+            if paths_in_output_dict:
+                output_dict = list(set(paths_in_output_dict + new_files))
+            else:
+                output_dict = new_files
+            self.out_paths_dict[req['Sample']] = output_dict
 
     def add_local_output_paths_dict(self):
-        local_samples = [sample for sample in self._config.get('Sample') if 'LocalPath' in sample.keys()]
+        local_samples = [sample for sample in self._config.get('Sample')
+                         if 'LocalPath' in sample.keys()]
         for sample in local_samples:
-            if self._outputformat == "parquet":
-                for tree, fpath in zip(sample['Tree'].split(','), sample['LocalPath'].split(',')):
+            if 'Tree' in sample.keys():
+                for tree, fpath in zip(sample['Tree'].split(','),
+                                       sample['LocalPath'].split(',')):
                     tree = tree.strip()
                     fpath = fpath.strip()
-                    self.out_paths_dict[sample['Name']][tree] = [str(Path(f)) for f in Path(fpath).glob("*")]
-                    log.info(f"  {sample['Name']} | {tree} | {fpath} is from local path")
-            elif self._outputformat == "root":
+                    self.out_paths_dict[sample['Name']][tree] \
+                        = [str(Path(f)) for f in Path(fpath).glob("*")]
+                    log.info(f"  {sample['Name']} "
+                             f"| {tree} | {fpath} is from local path")
+            else:
                 for fpath in sample['LocalPath'].split(','):
                     fpath = fpath.strip()
-                    self.out_paths_dict[sample['Name']] = [str(Path(f)) for f in Path(fpath).glob("*")]
-                    log.info(f"  {sample['Name']} | {fpath} is from local path")
-
+                    self.out_paths_dict[sample['Name']] = \
+                        [str(Path(f)) for f in Path(fpath).glob("*")]
+                    log.info(f"  {sample['Name']} "
+                             f"| {fpath} is from local path")
 
     def write_output_paths_dict(self, out_paths_dict):
-        """ Write yaml of output dict """
+        """
+        Write yaml of output dict
+        """
         if 'WriteOutputDict' in self._config['General'].keys():
-            file_out_paths = f"{self.output_path}/{self._config['General']['WriteOutputDict']}.yml"
+            file_out_paths = \
+                (f"{self.output_path}/"
+                 f"{self._config['General']['WriteOutputDict']}.yml")
             with open(file_out_paths, 'w') as f:
-                log.debug(f"write a yaml file containg delivered file paths: {f.name}")
+                log.debug("YAML file containing delivered file paths: "
+                          f"{f.name}")
                 yaml.dump(out_paths_dict, f, default_flow_style=False)
-            log.info(f"Wrote a yaml file containing delivered file paths: {file_out_paths}")
+            log.info("YAML file containing delivered file paths: "
+                     f"{file_out_paths}")
         else:
             for yl in list(Path(self.output_path).glob("*yml")):
                 Path.unlink(yl)
+
+    def clean_up_files_not_in_requests(self, out_paths_dict):
+
+        samples_in_requests = list(out_paths_dict.keys())
+        samples_local = [sa.name for sa in self.output_path.iterdir()
+                         if sa.is_dir()]
+        for sample in samples_local:
+            if not (sample in samples_in_requests):
+                rmtree(Path(self.output_path, sample))
+            else:
+                if list(Path(self.output_path, sample).iterdir())[0].is_dir():
+                    for tree in out_paths_dict[sample].keys():
+                        for tree in [tr.name for tr in
+                                     Path(self.output_path, sample).iterdir()
+                                     if tr.is_dir()]:
+                            if tree in out_paths_dict[sample].keys():
+                                files_local = set(Path(self.output_path,
+                                                       sample, tree).glob("*"))
+                                files_request = set(
+                                    [Path(item)
+                                     for item in out_paths_dict[sample][tree]]
+                                    )
+                                for tbd in \
+                                        files_local.difference(files_request):
+                                    Path.unlink(tbd)
+                            else:
+                                rmtree(Path(self.output_path, sample, tree))
+                else:
+                    files_local = set(Path(self.output_path, sample).glob("*"))
+                    files_request = set(
+                        [Path(item) for item in out_paths_dict[sample]]
+                        )
+                    for tbd in files_local.difference(files_request):
+                        Path.unlink(tbd)
+
+        return
```

### Comparing `servicex_databinder-0.4.0b6/servicex_databinder/request.py` & `servicex_databinder-0.4.1/servicex_databinder/request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,132 @@
 from typing import Any, Dict, List
 import tcut_to_qastle as tq
 import qastle
 import ast
 import logging
-from func_adl_servicex import ServiceXSourceXAOD
+from func_adl_servicex import ServiceXSourceXAOD # NOQA
+from servicex import ServiceXDataset # NOQA
 
 log = logging.getLogger(__name__)
 
+
 class ServiceXRequest():
-    """Prepare ServiceX requests"""
+    """
+    Prepare ServiceX requests
+    """
     def __init__(self, config: Dict[str, Any]) -> None:
         self._config = config
-        self._backend = self._config.get('General')['ServiceXBackendName'].lower()
 
     def get_requests(self) -> List:
-        log.debug(f"ServiceX backend: {self._config.get('General')['ServiceXBackendName']}")
+        log.debug(f"ServiceX backend: "
+                  f"{self._config.get('General')['ServiceXName']}")
         list_requests = []
         for sample in self._config.get('Sample'):
             list_requests.append(self._build_request(sample))
-        flist_requests = [request for x in list_requests for request in x] # flatten nested lists
-        log.debug(f"number of total ServiceX requests in the config: {len(flist_requests)}")
+        # flatten nested lists
+        flist_requests = [request for x in list_requests for request in x]
+        log.debug("number of total ServiceX requests in the config: "
+                  f"{len(flist_requests)}")
         log.debug(f"ServiceX requests in the config: {flist_requests}")
         return flist_requests
 
-
     def _build_request(self, sample: Dict) -> Dict:
-        """Return a list containing ServiceX request(s) of the given sample"""
+        """
+        Return a list containing ServiceX request(s) of the given sample
+        """
         requests_sample = []
+
         if 'RucioDID' in sample.keys():
             dids = sample['RucioDID'].split(',')
-            if 'uproot' in self._backend:
+            if sample['Type'] == "uproot":
                 trees = sample['Tree'].split(',')
-                log.debug(f"  Sample {sample['Name']} has {len(dids)} DID(s) and {len(trees)} Tree(s)")
-            else:
+                log.debug(f"  Sample {sample['Name']} has "
+                          f"{len(dids)} DID(s) and {len(trees)} Tree(s)")
+            elif sample['Type'] == "xaod":
                 trees = ['dummy']
-                log.debug(f"  Sample {sample['Name']} has {len(dids)} DID(s)")            
-
-            if 'TransformerImage' in sample.keys():
-                transformer_image = sample['TransformerImage']
-            else:
-                transformer_image = None
+                log.debug(f"  Sample {sample['Name']} has {len(dids)} DID(s)")
 
             for tree in trees:
                 for did in dids:
                     requests_sample.append(
                         {
-                        'Sample': sample['Name'],
-                        'transformerImage': transformer_image,
-                        'dataset': did.strip(),
-                        'tree': tree.strip(),
-                        'query': self._build_query(sample, tree.strip())
+                            'Sample': sample['Name'],
+                            'dataset': did.strip(),
+                            'type': sample['Type'],
+                            'codegen': sample['Transformer'],
+                            'tree': tree.strip(),
+                            'query': self._build_query(sample, tree.strip())
                         }
                     )
         elif 'XRootDFiles' in sample.keys():
-            xrootd_filelist = [file.strip() for file in sample['XRootDFiles'].split(",")]
-            if 'uproot' in self._backend:
+            xrootd_filelist = [file.strip()
+                               for file in sample['XRootDFiles'].split(",")]
+            if sample['Type'] == "uproot":
                 trees = sample['Tree'].split(',')
-                log.debug(f"  Sample {sample['Name']} has {len(xrootd_filelist)} file(s) and {len(trees)} Tree(s)")
-            else:
+                log.debug(f"  Sample {sample['Name']} has "
+                          f"{len(xrootd_filelist)} file(s) and "
+                          f"{len(trees)} Tree(s)")
+            elif sample['Type'] == "xaod":
                 trees = ['dummy']
-                log.debug(f"  Sample {sample['Name']} has {len(xrootd_filelist)} file(s)")
+                log.debug(f"  Sample {sample['Name']} has "
+                          f"{len(xrootd_filelist)} file(s)")
             for tree in trees:
                 requests_sample.append(
                     {
-                    'Sample': sample['Name'],
-                    'dataset': xrootd_filelist,
-                    'tree': tree.strip(),
-                    'query': self._build_query(sample, tree)
-                    } 
+                        'Sample': sample['Name'],
+                        'dataset': xrootd_filelist,
+                        'type': sample['Type'],
+                        'codegen': sample['Transformer'],
+                        'tree': tree.strip(),
+                        'query': self._build_query(sample, tree)
+                    }
                 )
         return requests_sample
-        
 
-    def _build_query(self, sample: Dict, tree:str) -> str:
-        """ 
+    def _build_query(self, sample: Dict, tree: str) -> str:
+        """
         Get query for each sample
         Option Columns for TCut syntax
         Option FuncADL for func-adl syntax
         """
-        if 'uproot' in self._backend:
+        if sample['Transformer'] == "uproot":
             if 'Columns' in sample:
-                if 'Filter' not in sample or sample['Filter'] == None: sample['Filter'] = ''
-                try:                    
+                if ('Filter' not in sample) or (sample['Filter'] is None):
+                    sample['Filter'] = ''
+                # else:
+                try:
                     query = tq.translate(
                         tree,
                         sample['Columns'],
                         sample['Filter']
                     )
                     return query
-                except:
-                    log.exception(f"Exception occured for the query of Sample {sample['Name']}")
+                except Exception:
+                    log.exception(
+                        "Exception occured for the query "
+                        f"of Sample {sample['Name']}"
+                        )
             elif 'FuncADL' in sample:
-                query = f"EventDataset('ServiceXDatasetSource', '{tree}')." + sample['FuncADL']
+                query = ("EventDataset('ServiceXDatasetSource', "
+                         f"'{tree}')." + sample['FuncADL'])
                 try:
-                    qastle_query = qastle.python_ast_to_text_ast(qastle.insert_linq_nodes(ast.parse(query)))
+                    qastle_query = qastle.python_ast_to_text_ast(
+                        qastle.insert_linq_nodes(ast.parse(query)))
                     return qastle_query
-                except:
-                    log.exception(f"Exception occured for the query of Sample {sample['Name']}")
-        elif 'xaod' in self._backend:
-            query = f"ServiceXSourceXAOD('')." + sample['FuncADL']
+                except Exception:
+                    log.exception(
+                        "Exception occured for the query "
+                        f"of Sample {sample['Name']}"
+                        )
+        elif sample['Transformer'] == "atlasr21":
+            query = "ServiceXSourceXAOD(ServiceXDataset('', backend_name='" \
+                + self._config.get('General')['ServiceXName'] + "'))." \
+                + sample['FuncADL']
             try:
                 o = eval(query)
                 qastle_query = qastle.python_ast_to_text_ast(o._q_ast)
                 return qastle_query
-            except:
-                log.exception(f"Exception occured for the query of Sample {sample['Name']}")
+            except Exception:
+                log.exception(
+                    "Exception occured for the query "
+                    f"of Sample {sample['Name']}"
+                    )
```

### Comparing `servicex_databinder-0.4.0b6/servicex_databinder/servicex_databinder.py` & `servicex_databinder-0.4.1/servicex_databinder/servicex_databinder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 from typing import Union, Dict, Any
 from pathlib import Path
-import time
 import asyncio
 from threading import Thread
 
-from .configuration import _load_config
+from .configuration import LoadConfig
 from .request import ServiceXRequest
 from .get_servicex_data import DataBinderDataset
 from .output_handler import OutputHandler
 
 import logging
 log = logging.getLogger(__name__)
 
+
 class DataBinder:
-    """ Manage and categorize numerous ServiceX data from a configuration file"""
+    """
+    Manage and categorize numerous ServiceX data from a configuration file
+    """
 
     def __init__(self, config: Union[str, Path, Dict[str, Any]]):
-        self._config = _load_config(config)
+        self._config = LoadConfig(config)
         self._requests = ServiceXRequest(self._config).get_requests()
         self._sx_db = DataBinderDataset(self._config, self._requests)
 
-        log.info(f"  {len(self._config.get('Sample'))} Samples and {len(self._requests)} ServiceX requests")
+        log.info(f"  {len(self._config.get('Sample'))} Samples"
+                 f" and {len(self._requests)} ServiceX requests")
 
     def deliver(self, overall_progress_only: bool = False) -> Dict:
 
-        out_paths_dict = asyncio.run(self._sx_db.get_data(overall_progress_only))
+        out_paths_dict = asyncio.run(
+                self._sx_db.get_data(overall_progress_only)
+            )
 
-        x = Thread(target=OutputHandler(self._config).clean_up_files_not_in_requests, args=(out_paths_dict,))
+        x = Thread(target=OutputHandler(self._config)
+                   .clean_up_files_not_in_requests, args=(out_paths_dict,))
         x.start()
 
         if len(self._sx_db.failed_request):
-            log.warning(f"{len(self._sx_db.failed_request)} failed delivery request(s)")
-            log.warning(f"get_failed_requests() for detail of failed requests")
+            log.warning(f"{len(self._sx_db.failed_request)} "
+                        "failed delivery request(s)")
+            log.warning("get_failed_requests() for detail of failed requests")
 
         return out_paths_dict
 
     def get_failed_requests(self):
-        return self._sx_db.failed_request
+        return self._sx_db.failed_request
```

### Comparing `servicex_databinder-0.4.0b6/servicex_databinder.egg-info/PKG-INFO` & `servicex_databinder-0.4.1/servicex_databinder.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,163 +1,180 @@
 Metadata-Version: 2.1
 Name: servicex-databinder
-Version: 0.4.0b6
-Summary: ServiceX data management using a configuration file
+Version: 0.4.1
+Summary: ServiceX data management                     using a configuration file
 Home-page: https://github.com/kyungeonchoi/ServiceXDataBinder
 Author: KyungEon Choi (UT Austin)
 Author-email: kyungeonchoi@utexas.edu
 License: BSD 3-clause
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ServiceX DataBinder
 
-<p align="right"> Release v0.4.0b2 </p>
+<p align="right"> Release v0.4.1 </p>
 
 [![PyPI version](https://badge.fury.io/py/servicex-databinder.svg)](https://badge.fury.io/py/servicex-databinder)
 
-<!-- `servicex-databinder` is a Python package for making multiple ServiceX requests and managing ServiceX delivered data from a configuration file.  -->
-
-`servicex-databinder` is a Python package to interact with ServiceX instance to make ServiceX request(s) and manage ServiceX delivered data efficiently from a single configuration file.
-
-The package is particularly useful when accessing multiple remote data via ServiceX, e.g. full-scale analysis or extracting input data for machine learning.
-
-Brief introduction of ServiceX and walk-though of various DataBinder features can be found 
-in this [Jupyter notebook](https://nbviewer.org/github/kyungeonchoi/irishep_topical_ServiceXDataBinder/blob/main/16Nov2022_choi.ipynb).
+`servicex-databinder` is a user-analysis data management package using a single configuration file. 
+Samples with external data sources (e.g. `RucioDID` or `XRootDFiles`) utilize ServiceX to deliver user-selected columns with optional row filtering.
+<!-- to interact with ServiceX instance to make ServiceX request(s) and manage ServiceX delivered data from a single configuration file. -->
+
+The following table shows supported ServiceX transformers by DataBinder
+
+| Input format | Code generator | Transformer | Output format
+| :--- | :---: | :---: | :---: |
+| ROOT Ntuple | func-adl | `uproot` | `root` or `parquet` |
+| ATLAS Release 21 xAOD | func-adl | `atlasr21`| `root` |
+<!-- | ROOT Ntuple | python function | `python`| -->
 
 <!-- [`ServiceX`](https://github.com/ssl-hep/ServiceX) is a scalable HEP event data extraction, transformation and delivery system. 
 
 ['ServiceX Client library'](https://github.com/ssl-hep/ServiceX_frontend) provides  --> 
 
 ## Prerequisite
 - [Access to a ServiceX instance](https://servicex.readthedocs.io/en/latest/user/getting-started/)
-- Python 3.6+
+- Python 3.7+
 
 ## Installation
 ```shell
 pip install servicex-databinder
 ```
 
 ## Configuration file
 
 The configuration file is a yaml file containing all the information.
-An example configuration file is shown below:
+
+The [following example configuration file](config_minimum.yaml) contains minimal fields. You can also download [`servicex-opendata.yaml`](servicex-opendata.yaml) file (rename to `servicex.yaml`) at your working directory, and run DataBinder for OpenData without an access token.
 
 ```yaml
 General:
-  ServiceXBackendName: uproot
-  OutputDirectory: /path/to/output
+  ServiceXName: servicex-opendata
   OutputFormat: parquet
   
 Sample:
-  - Name: ttH
-    RucioDID: user.kchoi:user.kchoi.sampleA, 
-             user.kchoi:user.kchoi.sampleB
-    Tree: nominal
-    FuncADL: "Select(lambda event: {'jet_e': event.jet_e})"
-  - Name: ttW
-    XRootDFiles: root://ttW.root
-    Tree: nominal
-    Filter: n_jet > 5 
-    Columns: jet_e, jet_pt
-  - Name: ttZ
-    LocalPath: /home/kchoi/ttZ
-    Tree: nominal
+  - Name: ggH125_ZZ4lep
+    XRootDFiles: "root://eospublic.cern.ch//eos/opendata/atlas/OutreachDatasets\
+                  /2020-01-22/4lep/MC/mc_345060.ggH125_ZZ4lep.4lep.root"
+    Tree: mini
+    Columns: lep_pt, lep_eta
 ```
 
-`General` block requires three mandatory options as in the example above.
+`General` block requires two mandatory options (`ServiceXName` and `OutputFormat`) as in the example above.
 
-Input dataset for each Sample can be defined either by `RucioDID` or `XRootDFiles` or `LocalPath`. You need to make sure whether the ServiceX backend you specified in `ServiceXBackendName` supports Rucio and/or XRootD. 
+Input dataset for each Sample can be defined either by `RucioDID` or `XRootDFiles` or `LocalPath`.
 
 ServiceX query can be constructed with either TCut syntax or func-adl.
 - Options for TCut syntax: `Filter`<sup>1</sup> and `Columns`
 - Option for Func-adl expression: `FuncADL`
 
 &nbsp; &nbsp; &nbsp; <sup>1</sup> `Filter` works only for scalar-type of TBranch.
 
 Output format can be either `Apache parquet` or `ROOT ntuple` for `uproot` backend. Only `ROOT ntuple` format is supported for `xAOD` backend.
 
-Please find other example configurations for ATLAS opendata, xAOD, and Uproot ServiceX endpoints.
-
 
 The followings are available options:
 
 <!-- `General` block: -->
 | Option for `General` block | Description       | DataType |
 |:--------:|:------:|:------|
-| `ServiceXBackendName`* | ServiceX backend name in your `servicex.yaml` file <br> (name MUST contain either `uproot` or `xaod` to distinguish the type of transformer) | `String` |
-| `OutputDirectory`* | Path to the directory for ServiceX delivered files | `String` |
+| `ServiceXName`* | ServiceX backend name in your `servicex.yaml` file <br>  | `String` |
+| `OutputDirectory` | Path to the directory for ServiceX delivered files | `String` |
 | `OutputFormat`* | Output file format of ServiceX delivered data (`parquet` or `root` for `uproot` / `root` for `xaod`) | `String` |
-| `ZipROOTColumns` | Zip columns that share prefix to generate one counter branch (see detail at [uproot readthedoc](https://uproot.readthedocs.io/en/latest/basic.html#writing-ttrees-to-a-file)) | `Boolean` |
 | `WriteOutputDict` | Name of an ouput yaml file containing Python nested dictionary of output file paths (located in the `OutputDirectory`) | `String` |
 | `IgnoreServiceXCache` | Ignore the existing ServiceX cache and force to make ServiceX requests | `Boolean` |
 <p align="right"> *Mandatory options</p>
 
 | Option for `Sample` block | Description       |DataType |
 |:--------:|:------:|:------|
 | `Name`   | sample name defined by a user |`String` |
 | `RucioDID` | Rucio Dataset Id (DID) for a given sample; <br> Can be multiple DIDs separated by comma |`String` |
 | `XRootDFiles` | XRootD files (e.g. `root://`) for a given sample; <br> Can be multiple files separated by comma |`String` |
 | `Tree` | Name of the input ROOT `TTree`; <br> Can be multiple `TTree`s separated by comma (`uproot` ONLY) |`String` |
 | `Filter` | Selection in the TCut syntax, e.g. `jet_pt > 10e3 && jet_eta < 2.0` (TCut ONLY) |`String` |
 | `Columns` | List of columns (or branches) to be delivered; multiple columns separately by comma (TCut ONLY) |`String` |
-| `FuncADL` | func-adl expression for a given sample (see [example](config_example_xaod.yml)) |`String` |
+| `FuncADL` | func-adl expression for a given sample |`String` |
 | `LocalPath` | File path directly from local path (NO ServiceX tranformation) | `String` |
 
  <!-- Options exclusively for TCut syntax (CANNOT combine with the option `FuncADL`) -->
 
  <!-- Option for func-adl expression (CANNOT combine with the option `Fitler` and `Columns`) -->
 
-A config file can be simplified by utilizing `Definition` block. You can define placeholders under `Definition` block, which will replace all matched placeholders in the values of `Sample` block. Note that placeholders must start with `DEF_`. The example configuration file can be also written as below with `Definition` block:
+A config file can be simplified by utilizing `Definition` block. You can define placeholders under `Definition` block, which will replace all matched placeholders in the values of `Sample` block. Note that placeholders must start with `DEF_`.
+
+You can source each Sample using different ServiceX transformers. 
+The default transformer is set by `type` of `servicex.yaml`, but `Transformer` in the `General` block overwrites if present, and `Transformer` in each `Sample` overwrites any previous transformer selection.
+
+The [following example configuration](config_maximum.yaml) shows how to use each Options.
 
 ```yaml
 General:
-  ServiceXBackendName: uproot
-  OutputDirectory: /path/to/output
-  OutputFormat: parquet
+  ServiceXName: servicex-uc-af
+  Transformer: uproot
+  OutputFormat: root
+  OutputDirectory: /Users/kchoi/data_for_MLstudy
+  WriteOutputDict: fileset_ml_study
+  IgnoreServiceXCache: False
   
-Sample:
-  - Name: ttH
-    RucioDID: DEF_ttH_dids
-    Tree: nominal
-    FuncADL: DEF_nominal_selection
-  - Name: ttW
-    RucioDID: user.kchoi:user.kchoi.sampleC
+Sample:  
+  - Name: Signal
+    RucioDID: user.kchoi:user.kchoi.signalA,
+              user.kchoi:user.kchoi.signalB,
+              user.kchoi:user.kchoi.signalC
     Tree: nominal
-    Filter: n_jet > 5 
-    Columns: jet_e, jet_pt
+    FuncADL: DEF_ttH_nominal_query
+  - Name: Background1
+    XRootDFiles: DEF_ggH_input
+    Tree: mini
+    Filter: lep_n>2
+    Columns: lep_pt, lep_eta
+  - Name: Background2
+    Transformer: atlasr21
+    RucioDID: DEF_Zee_input
+    FuncADL: DEF_Zee_query
+  - Name: Background3
+    LocalPath: /Users/kchoi/Work/data/background3
 
 Definition:
-  DEF_ttH_dids: user.kchoi:user.kchoi.sampleA, 
-             user.kchoi:user.kchoi.sampleB
-  DEF_nominal_selection: "Select(lambda event: {'jet_e': event.jet_e})"
+  DEF_ttH_nominal_query: "Where(lambda e: e.met_met>150e3). \
+              Select(lambda event: {'el_pt': event.el_pt, 'jet_e': event.jet_e, \
+              'jet_pt': event.jet_pt, 'met_met': event.met_met})"
+  DEF_ggH_input: "root://eospublic.cern.ch//eos/opendata/atlas/OutreachDatasets\
+                  /2020-01-22/4lep/MC/mc_345060.ggH125_ZZ4lep.4lep.root"
+  DEF_Zee_input: "mc15_13TeV:mc15_13TeV.361106.PowhegPythia8EvtGen_AZNLOCTEQ6L1_Zee.\
+                merge.DAOD_STDM3.e3601_s2576_s2132_r6630_r6264_p2363_tid05630052_00"
+  DEF_Zee_query: "SelectMany('lambda e: e.Jets(\"AntiKt4EMTopoJets\")'). \
+              Where('lambda j: (j.pt() / 1000) > 30'). \
+              Select('lambda j: j.pt() / 1000.0'). \
+              AsROOTTTree('junk.root', 'my_tree', [\"JetPt\"])"
 ```
 
+
 ## Deliver data
 
 ```python
 from servicex_databinder import DataBinder
 sx_db = DataBinder('<CONFIG>.yml')
 out = sx_db.deliver()
 ```
 
-The function `deliver()` returns a Python nested dictionary that contains delivered files: 
-- for `uproot` backend and `parquet` output format: `out['<SAMPLE>']['<TREE>'] = [ List of output parquet files ]`
+The function `deliver()` returns a Python nested dictionary that contains delivered files.
+<!-- - for `uproot` backend and `parquet` output format: `out['<SAMPLE>']['<TREE>'] = [ List of output parquet files ]`
 - for `uproot` backend and `root` output format: `out['<SAMPLE>'] = [ List of output root files ]`
-- for `xAOD` backend: `out['<SAMPLE>'] = [ List of output root files ]`
+- for `xAOD` backend: `out['<SAMPLE>'] = [ List of output root files ]` -->
 
 Input configuration can be also passed in a form of a Python dictionary.
 
 Delivered Samples and files in the `OutputDirectory` are always synced with the DataBinder config file.
 
 <!-- ## Currently available 
 - Dataset as Rucio DID + Input file format is ROOT TTree + ServiceX delivers output in parquet format
```

### Comparing `servicex_databinder-0.4.0b6/servicex_databinder.egg-info/SOURCES.txt` & `servicex_databinder-0.4.1/servicex_databinder.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 servicex_databinder/output_handler.py
 servicex_databinder/request.py
 servicex_databinder/servicex_databinder.py
 servicex_databinder.egg-info/PKG-INFO
 servicex_databinder.egg-info/SOURCES.txt
 servicex_databinder.egg-info/dependency_links.txt
 servicex_databinder.egg-info/requires.txt
-servicex_databinder.egg-info/top_level.txt
+servicex_databinder.egg-info/top_level.txt
+tests/test_config.py
```

### Comparing `servicex_databinder-0.4.0b6/setup.py` & `servicex_databinder-0.4.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,47 +2,50 @@
 import codecs
 import os.path
 
 
 with open("README.md") as fh:
     long_description = fh.read()
 
+
 def read(rel_path):
     here = os.path.abspath(os.path.dirname(__file__))
     with codecs.open(os.path.join(here, rel_path), 'r') as fp:
         return fp.read()
 
+
 def get_version(rel_path):
     for line in read(rel_path).splitlines():
         if line.startswith('__version__'):
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
+
 setuptools.setup(name="servicex_databinder",
                  version=get_version("servicex_databinder/__init__.py"),
                  packages=setuptools.find_packages(exclude=['tests']),
-                 description="ServiceX data management using a configuration file",
+                 description="ServiceX data management \
+                    using a configuration file",
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  author="KyungEon Choi (UT Austin)",
                  author_email="kyungeonchoi@utexas.edu",
                  url="https://github.com/kyungeonchoi/ServiceXDataBinder",
                  license="BSD 3-clause",
-                 python_requires='>=3.8',
+                 python_requires='>=3.7',
                  install_requires=[
-                    "servicex>=2.5",
-                    "tcut-to-qastle>=0.7",                    
+                    "servicex>=2.6.2",
+                    "tcut-to-qastle>=0.7",
                     "nest-asyncio>=1.5.1",
                     "tqdm>=4.60.0",
                     "pyarrow>=3.0.0",
                     "backoff>=1.11.1",
-                    "func_adl_servicex>=1.1",
-                    "aioshutil>=1.2"
+                    "func_adl_servicex>=2.2"
                     ],
                  classifiers=[
                     "Development Status :: 3 - Alpha",
                     "Intended Audience :: Developers",
                     "Intended Audience :: Information Technology",
                     "Intended Audience :: Science/Research",
                     "Programming Language :: Python",
```

