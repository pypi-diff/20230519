# Comparing `tmp/geodata-harvester-1.0.0.tar.gz` & `tmp/geodata-harvester-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodata-harvester-1.0.0.tar", last modified: Tue May  9 03:44:35 2023, max compression
+gzip compressed data, was "geodata-harvester-1.0.1.tar", last modified: Fri May 19 06:20:41 2023, max compression
```

## Comparing `geodata-harvester-1.0.0.tar` & `geodata-harvester-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-09 03:44:35.031032 geodata-harvester-1.0.0/
--rw-r--r--   0 seb        (504) staff       (20)     7652 2023-01-10 23:44:41.000000 geodata-harvester-1.0.0/LICENSE.txt
--rw-r--r--   0 seb        (504) staff       (20)    12715 2023-05-09 03:44:35.030834 geodata-harvester-1.0.0/PKG-INFO
--rw-r--r--   0 seb        (504) staff       (20)    12301 2023-05-09 03:40:12.000000 geodata-harvester-1.0.0/README.md
--rw-r--r--   0 seb        (504) staff       (20)       38 2023-05-09 03:44:35.031084 geodata-harvester-1.0.0/setup.cfg
--rw-r--r--   0 seb        (504) staff       (20)     1981 2023-05-09 03:28:52.000000 geodata-harvester-1.0.0/setup.py
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-09 03:44:35.026524 geodata-harvester-1.0.0/src/
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-09 03:44:35.029114 geodata-harvester-1.0.0/src/geodata_harvester/
--rw-r--r--   0 seb        (504) staff       (20)     1030 2023-05-09 03:28:44.000000 geodata-harvester-1.0.0/src/geodata_harvester/__init__.py
--rw-r--r--   0 seb        (504) staff       (20)     1040 2022-03-23 04:23:00.000000 geodata-harvester-1.0.0/src/geodata_harvester/arc2meter.py
--rw-r--r--   0 seb        (504) staff       (20)    35525 2023-01-23 03:29:23.000000 geodata-harvester-1.0.0/src/geodata_harvester/getdata_dea.py
--rw-r--r--   0 seb        (504) staff       (20)    10787 2023-01-18 01:59:45.000000 geodata-harvester-1.0.0/src/geodata_harvester/getdata_dem.py
--rw-r--r--   0 seb        (504) staff       (20)     8655 2023-01-18 01:54:54.000000 geodata-harvester-1.0.0/src/geodata_harvester/getdata_landscape.py
--rw-r--r--   0 seb        (504) staff       (20)    11275 2023-01-18 01:55:09.000000 geodata-harvester-1.0.0/src/geodata_harvester/getdata_radiometric.py
--rw-r--r--   0 seb        (504) staff       (20)    18323 2023-05-08 08:11:38.000000 geodata-harvester-1.0.0/src/geodata_harvester/getdata_silo.py
--rw-r--r--   0 seb        (504) staff       (20)    15851 2023-02-06 06:20:02.000000 geodata-harvester-1.0.0/src/geodata_harvester/getdata_slga.py
--rw-r--r--   0 seb        (504) staff       (20)    23169 2023-05-09 01:43:38.000000 geodata-harvester-1.0.0/src/geodata_harvester/harvest.py
--rw-r--r--   0 seb        (504) staff       (20)      738 2023-01-15 23:19:22.000000 geodata-harvester-1.0.0/src/geodata_harvester/settingshandler.py
--rw-r--r--   0 seb        (504) staff       (20)     6228 2023-01-27 00:29:41.000000 geodata-harvester-1.0.0/src/geodata_harvester/spatial.py
--rw-r--r--   0 seb        (504) staff       (20)    12970 2023-05-08 08:12:08.000000 geodata-harvester-1.0.0/src/geodata_harvester/temporal.py
--rw-r--r--   0 seb        (504) staff       (20)    30584 2023-05-09 01:49:21.000000 geodata-harvester-1.0.0/src/geodata_harvester/utils.py
--rw-r--r--   0 seb        (504) staff       (20)    11604 2023-01-18 02:18:57.000000 geodata-harvester-1.0.0/src/geodata_harvester/validate_settings.py
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-09 03:44:35.030120 geodata-harvester-1.0.0/src/geodata_harvester/widgets/
--rw-rw-r--   0 seb        (504) staff       (20)       40 2016-10-31 16:56:29.000000 geodata-harvester-1.0.0/src/geodata_harvester/widgets/__init__.py
--rw-r--r--   0 seb        (504) staff       (20)    25214 2023-02-16 02:40:52.000000 geodata-harvester-1.0.0/src/geodata_harvester/widgets/harvesterwidgets.py
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-09 03:44:35.030642 geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/
--rwxr-xr-x   0 seb        (504) staff       (20)       60 2021-09-15 22:24:00.000000 geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/__init__.py
--rw-rw-r--   0 seb        (504) staff       (20)     1056 2021-09-15 22:24:00.000000 geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/errors.py
--rw-rw-r--   0 seb        (504) staff       (20)    22928 2022-06-09 00:48:28.000000 geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/filechooser.py
--rw-rw-r--   0 seb        (504) staff       (20)     3976 2021-09-15 22:24:00.000000 geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/utils.py
--rw-rw-r--   0 seb        (504) staff       (20)     1996 2016-10-31 16:56:29.000000 geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipywidgets_file_selector.py
--rw-r--r--   0 seb        (504) staff       (20)     3703 2022-07-14 05:17:29.000000 geodata-harvester-1.0.0/src/geodata_harvester/write_logs.py
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-09 03:44:35.029724 geodata-harvester-1.0.0/src/geodata_harvester.egg-info/
--rw-r--r--   0 seb        (504) staff       (20)    12715 2023-05-09 03:44:34.000000 geodata-harvester-1.0.0/src/geodata_harvester.egg-info/PKG-INFO
--rw-r--r--   0 seb        (504) staff       (20)     1188 2023-05-09 03:44:34.000000 geodata-harvester-1.0.0/src/geodata_harvester.egg-info/SOURCES.txt
--rw-r--r--   0 seb        (504) staff       (20)        1 2023-05-09 03:44:34.000000 geodata-harvester-1.0.0/src/geodata_harvester.egg-info/dependency_links.txt
--rw-r--r--   0 seb        (504) staff       (20)      217 2023-05-09 03:44:34.000000 geodata-harvester-1.0.0/src/geodata_harvester.egg-info/requires.txt
--rw-r--r--   0 seb        (504) staff       (20)       18 2023-05-09 03:44:34.000000 geodata-harvester-1.0.0/src/geodata_harvester.egg-info/top_level.txt
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-19 06:20:41.110603 geodata-harvester-1.0.1/
+-rw-r--r--   0 seb        (504) staff       (20)     7652 2023-01-10 23:44:41.000000 geodata-harvester-1.0.1/LICENSE.txt
+-rw-r--r--   0 seb        (504) staff       (20)    12790 2023-05-19 06:20:41.110365 geodata-harvester-1.0.1/PKG-INFO
+-rw-r--r--   0 seb        (504) staff       (20)    12376 2023-05-09 05:44:57.000000 geodata-harvester-1.0.1/README.md
+-rw-r--r--   0 seb        (504) staff       (20)       38 2023-05-19 06:20:41.110643 geodata-harvester-1.0.1/setup.cfg
+-rw-r--r--   0 seb        (504) staff       (20)     1981 2023-05-19 06:10:22.000000 geodata-harvester-1.0.1/setup.py
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-19 06:20:41.105059 geodata-harvester-1.0.1/src/
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-19 06:20:41.108245 geodata-harvester-1.0.1/src/geodata_harvester/
+-rw-r--r--   0 seb        (504) staff       (20)     1030 2023-05-19 06:10:00.000000 geodata-harvester-1.0.1/src/geodata_harvester/__init__.py
+-rw-r--r--   0 seb        (504) staff       (20)     1040 2022-03-23 04:23:00.000000 geodata-harvester-1.0.1/src/geodata_harvester/arc2meter.py
+-rw-r--r--   0 seb        (504) staff       (20)    35525 2023-01-23 03:29:23.000000 geodata-harvester-1.0.1/src/geodata_harvester/getdata_dea.py
+-rw-r--r--   0 seb        (504) staff       (20)    10787 2023-01-18 01:59:45.000000 geodata-harvester-1.0.1/src/geodata_harvester/getdata_dem.py
+-rw-r--r--   0 seb        (504) staff       (20)     8655 2023-01-18 01:54:54.000000 geodata-harvester-1.0.1/src/geodata_harvester/getdata_landscape.py
+-rw-r--r--   0 seb        (504) staff       (20)    11275 2023-01-18 01:55:09.000000 geodata-harvester-1.0.1/src/geodata_harvester/getdata_radiometric.py
+-rw-r--r--   0 seb        (504) staff       (20)    18323 2023-05-08 08:11:38.000000 geodata-harvester-1.0.1/src/geodata_harvester/getdata_silo.py
+-rw-r--r--   0 seb        (504) staff       (20)    15851 2023-02-06 06:20:02.000000 geodata-harvester-1.0.1/src/geodata_harvester/getdata_slga.py
+-rw-r--r--   0 seb        (504) staff       (20)    23169 2023-05-09 01:43:38.000000 geodata-harvester-1.0.1/src/geodata_harvester/harvest.py
+-rw-r--r--   0 seb        (504) staff       (20)      738 2023-01-15 23:19:22.000000 geodata-harvester-1.0.1/src/geodata_harvester/settingshandler.py
+-rw-r--r--   0 seb        (504) staff       (20)     6228 2023-01-27 00:29:41.000000 geodata-harvester-1.0.1/src/geodata_harvester/spatial.py
+-rw-r--r--   0 seb        (504) staff       (20)    13346 2023-05-19 06:07:38.000000 geodata-harvester-1.0.1/src/geodata_harvester/temporal.py
+-rw-r--r--   0 seb        (504) staff       (20)    30584 2023-05-09 01:49:21.000000 geodata-harvester-1.0.1/src/geodata_harvester/utils.py
+-rw-r--r--   0 seb        (504) staff       (20)    11604 2023-01-18 02:18:57.000000 geodata-harvester-1.0.1/src/geodata_harvester/validate_settings.py
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-19 06:20:41.109500 geodata-harvester-1.0.1/src/geodata_harvester/widgets/
+-rw-rw-r--   0 seb        (504) staff       (20)       40 2016-10-31 16:56:29.000000 geodata-harvester-1.0.1/src/geodata_harvester/widgets/__init__.py
+-rw-r--r--   0 seb        (504) staff       (20)    25214 2023-02-16 02:40:52.000000 geodata-harvester-1.0.1/src/geodata_harvester/widgets/harvesterwidgets.py
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-19 06:20:41.110082 geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/
+-rwxr-xr-x   0 seb        (504) staff       (20)       60 2021-09-15 22:24:00.000000 geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/__init__.py
+-rw-rw-r--   0 seb        (504) staff       (20)     1056 2021-09-15 22:24:00.000000 geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/errors.py
+-rw-rw-r--   0 seb        (504) staff       (20)    22928 2022-06-09 00:48:28.000000 geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/filechooser.py
+-rw-rw-r--   0 seb        (504) staff       (20)     3976 2021-09-15 22:24:00.000000 geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/utils.py
+-rw-rw-r--   0 seb        (504) staff       (20)     1996 2016-10-31 16:56:29.000000 geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipywidgets_file_selector.py
+-rw-r--r--   0 seb        (504) staff       (20)     3703 2022-07-14 05:17:29.000000 geodata-harvester-1.0.1/src/geodata_harvester/write_logs.py
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-19 06:20:41.109005 geodata-harvester-1.0.1/src/geodata_harvester.egg-info/
+-rw-r--r--   0 seb        (504) staff       (20)    12790 2023-05-19 06:20:41.000000 geodata-harvester-1.0.1/src/geodata_harvester.egg-info/PKG-INFO
+-rw-r--r--   0 seb        (504) staff       (20)     1188 2023-05-19 06:20:41.000000 geodata-harvester-1.0.1/src/geodata_harvester.egg-info/SOURCES.txt
+-rw-r--r--   0 seb        (504) staff       (20)        1 2023-05-19 06:20:41.000000 geodata-harvester-1.0.1/src/geodata_harvester.egg-info/dependency_links.txt
+-rw-r--r--   0 seb        (504) staff       (20)      217 2023-05-19 06:20:41.000000 geodata-harvester-1.0.1/src/geodata_harvester.egg-info/requires.txt
+-rw-r--r--   0 seb        (504) staff       (20)       18 2023-05-19 06:20:41.000000 geodata-harvester-1.0.1/src/geodata_harvester.egg-info/top_level.txt
```

### Comparing `geodata-harvester-1.0.0/LICENSE.txt` & `geodata-harvester-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/PKG-INFO` & `geodata-harvester-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodata-harvester
-Version: 1.0.0
+Version: 1.0.1
 Summary: An automation tool for harvesting and processing geodata from the web
 Home-page: https://github.com/Sydney-Informatics-Hub/geodata-harvester
 License: LGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -27,41 +27,41 @@
 
 <!-- Badges end -->
 
 The Geodata-Harvester Python package offers reusable and automated workflows for data extraction from a wide range of geospatial and environmental data sources. User provided data is auto-completed with a suitable set of spatial- and temporal-aligned covariates as a ready-made dataset for machine learning and environmental models. In addition, all requested data layer maps are automatically extracted and aligned for a specific region and time period.
 
 For the R-package wrapper of the Geodata-Harvester, please visit the [Github dataharvesteR project](https://github.com/Sydney-Informatics-Hub/dataharvester).
 
-## Content
+## 📚 Table of Contents
 
-- [Introduction](#introduction)
-- [Data Sources](#data-sources)
-- [Functionality](#functionality)
-- [Key Features](#key-features)
-- [Installation](#installation)
+- [Introduction](#-introduction)
+- [Data Sources](#-data-sources)
+- [Functionality](#-functionality)
+- [Key Features](#-key-features)
+- [Installation](#-installation)
     - [Conda or Mamba](#conda-or-mamba)
     - [PyPI](#pypi)
     - [Google Earth Engine extension](#google-earth-engine-extension)
     - [Local development](#local-development)
     - [Workshop Cloud Sandbox](#workshop-cloud-sandbox)
-- [How to get started](#how-to-get-started)
-- [How to add new data source modules](#how-to-add-new-data-source-modules)
-- [Code reference API](#code-reference-api)
-- [Contributions](#contributions)
-- [Attribution and Acknowledgments](#attribution-and-acknowledgments)
-- [License](#license)
+- [How to get started](#-how-to-get-started)
+- [How to add new data source modules](#-how-to-add-new-data-source-modules)
+- [Code reference API](#-code-reference-api)
+- [Contributions](#-contributions)
+- [Attribution and Acknowledgments](#-attribution-and-acknowledgments)
+- [License](#-license)
 
 
-## Introduction
+## 💡 Introduction
 
 There is an enormous amount of national/global space-time data that is free and accessible. Examples are the numerous satellite platforms, weather, soil landscape grid of Australia. Many have a temporal dimension so for any point in Australia you can extract a time series of remote sensing and weather data and soil and terrain site variables. In the case of time series covariates there are a number of post-processing steps that a user can undertake to extract meaning, e.g. temporal means, aggregating in time. All of the above is a non-trivial task and a workflow where a user could enter a point (s) and get a tidy data frame of data cube variables would be a step towards people understanding its value and being able to jumpstart their analysis. This project will contribute processing tools for finding, extracting and converting these key data layers.
 
 Developed as part of the Agricultural Research Federation (AgReFed), Geodata-Harvester is an open-source software that allows users to jumpstart their analysis with a suitable set of spatial-temporal aligned raster maps and dataframes.
 
-## Data Sources
+## 🌍 Data Sources
 
 A detailed list of all available layers and their description can be found in [Data Overview](quarto/docs/Data_Overview.md).
 
 The following main data sources are currently implemented:
 
 - Soil and Landscape Grid of Australia (SLGA)
 - SILO Climate Database
@@ -77,15 +77,15 @@
 
 1. Retrieve: given set of locations, automatically access and download multiple data sources (APIs) from a diverse range of geospatial and soil data sources
 2. Process: Spatial and temporal processing, conversion to dataframes and custom raster-files
 3. Output: Ready-made dataset for machine learning (training set and prediction mapping)
 
 Geodata-Harvester is designed as a modular and maintainable project in the form of a multi-stage pipeline by providing explicit boundaries among tasks. To encourage interaction and experimentation with the pipeline, multiple frontend notebooks and use case scenarios are provided.
 
-## Key Features
+## 🌟 Key Features
 
 Below is a list of features available for the geodata-harvester package. Please check the project Github webpage and notebooks for examples, data selection, and other settings.
 
 - enabling reproducible workflows via YAML settings files.
 - automatic data retrieval from geodata APIs for given locations and dates.
 - automatic download and spatiotemporal processing of geo-spatial maps for user-specified bounding box, resolution, and time-scale.
 - support for time-series data extraction for multiple time slices. 
@@ -94,15 +94,15 @@
 - preview of downloaded and aligned maps.
 - support for saving and loading settings via interactive widgets.
 - with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices.
 - example notebooks and use-cases are provided for the user to get started.
 
 For more features, please see the [API reference documentation](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
 
-## Installation
+## 🔧 Installation
 
 Geodata-Harvester can be run on cloud-servers (e.g., in JupyterHub environment) or on your local machine. 
 Example notebooks for importing and using the package can be found in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks). The package can be installed via PyPI or Conda:
 
 ### Conda or Mamba
 
 The package geodata-harvester is available via the conda-forge channel:
@@ -151,15 +151,15 @@
 As play-ground for workshop training sessions and testing of the Geodata-Harvester we provide a pre-installed cloud Python Jupyterlab environment, which does not require any local installation. For login instructions and how to access the sandbox, please visit our [Python workshop page](https://sydney-informatics-hub.github.io/AgReFed-Workshop/pydocs/py00-workshop.html).
 
 The Jupyter environment is hosted on the ARDC Nectar Research Cloud in partnership with AgReFed and Australian Research Data Commons (ARDC). Note that this sandbox is currently hosted for test purposes only and generated data is not permanently stored.
 
 The Geodata-Harvester can be easily installed also on other cloud services (e.g., Google Colab, Azure Notebooks).
 
 
-## How to get started
+## 🚀 How to get started
 
 You may now invoke the geodata-harvester directly from a python terminal with:
 
 ```python
 import geodata_harvester as gdh
 gdh.harvest.run(PATH_TO_SETTINGS_YAMLFILE)
 ```
@@ -170,44 +170,44 @@
 
 1. Options and user settings are defined by the user in the settings; see for settings documentation [Settings_Overview](quarto/docs/Settings_Overview.md)
 
 2. Run the jupyter notebook in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks).
 
 If you would like to learn more about the Geodata-Harvester, please visit our [Workshop webpage](https://sydney-informatics-hub.github.io/AgReFed-Workshop/).
 
-## How to add new data source modules
+## ➕ How to add new data source modules
 
 The Geodata-Harvester is designed to be extendable and new data source modules can be added as Python modules (for examples, see `getdata_*.py` modules). If you would like to add a new data source, please follow the [adding new data source guidelines](quarto/docs/How_to_add_DataSources.md)  
 
 We recommend to fork the geodata-harvester repo and develop new modules in a local environment. If you would like to contribute your data source module to the geodata-harvester package, please visit the [geodata-harvester contribution guidelines](quarto/docs/Contributing.md).
 
 
-## Code reference API
+## 📚 Code reference API
 
 An auto-generated API reference documentation is available [here](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
 
-## Contributions
+## 🤝 Contributions
 We are happy for any contribution to the geodata-harvester, whether feedbacks and bug reports via github Issues, adding use-case examples via notebook contributions, to improving source-code and adding new or updating existing data source modules. 
 
 For more details about about how to contribute to the development, please visit the [Geodata-Harvester contribution guidelines](quarto/docs/Contributing.md).
 
 
-## Attribution and Acknowledgments
+## 👏 Attribution and Acknowledgments
 
 This software was developed by the Sydney Informatics Hub, a core research facility of the University of Sydney, as part of the Data Harvesting project for the Agricultural Research Federation (AgReFed).
 
 Acknowledgments are an important way for us to demonstrate the value we bring to your research. Your research outcomes are vital for ongoing funding of the Sydney Informatics Hub.
 
 If you make use of this software for your research project, please include the following acknowledgment:
 
 “This research was supported by the Sydney Informatics Hub, a Core Research Facility of the University of Sydney, and the Agricultural Research Federation (AgReFed)."
 
 AgReFed is supported by the Australian Research Data Commons (ARDC) and the Australian Government through the National Collaborative Research Infrastructure Strategy (NCRIS).
 
-## License
+## 📄 License
 
 Copyright 2023 The University of Sydney
 
 This is free software: you can redistribute it and/or modify it under
 the terms of the GNU Lesser General Public License (LGPL version 3) as
 published by the Free Software Foundation.
```

### Comparing `geodata-harvester-1.0.0/README.md` & `geodata-harvester-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,41 +15,41 @@
 
 <!-- Badges end -->
 
 The Geodata-Harvester Python package offers reusable and automated workflows for data extraction from a wide range of geospatial and environmental data sources. User provided data is auto-completed with a suitable set of spatial- and temporal-aligned covariates as a ready-made dataset for machine learning and environmental models. In addition, all requested data layer maps are automatically extracted and aligned for a specific region and time period.
 
 For the R-package wrapper of the Geodata-Harvester, please visit the [Github dataharvesteR project](https://github.com/Sydney-Informatics-Hub/dataharvester).
 
-## Content
+## 📚 Table of Contents
 
-- [Introduction](#introduction)
-- [Data Sources](#data-sources)
-- [Functionality](#functionality)
-- [Key Features](#key-features)
-- [Installation](#installation)
+- [Introduction](#-introduction)
+- [Data Sources](#-data-sources)
+- [Functionality](#-functionality)
+- [Key Features](#-key-features)
+- [Installation](#-installation)
     - [Conda or Mamba](#conda-or-mamba)
     - [PyPI](#pypi)
     - [Google Earth Engine extension](#google-earth-engine-extension)
     - [Local development](#local-development)
     - [Workshop Cloud Sandbox](#workshop-cloud-sandbox)
-- [How to get started](#how-to-get-started)
-- [How to add new data source modules](#how-to-add-new-data-source-modules)
-- [Code reference API](#code-reference-api)
-- [Contributions](#contributions)
-- [Attribution and Acknowledgments](#attribution-and-acknowledgments)
-- [License](#license)
+- [How to get started](#-how-to-get-started)
+- [How to add new data source modules](#-how-to-add-new-data-source-modules)
+- [Code reference API](#-code-reference-api)
+- [Contributions](#-contributions)
+- [Attribution and Acknowledgments](#-attribution-and-acknowledgments)
+- [License](#-license)
 
 
-## Introduction
+## 💡 Introduction
 
 There is an enormous amount of national/global space-time data that is free and accessible. Examples are the numerous satellite platforms, weather, soil landscape grid of Australia. Many have a temporal dimension so for any point in Australia you can extract a time series of remote sensing and weather data and soil and terrain site variables. In the case of time series covariates there are a number of post-processing steps that a user can undertake to extract meaning, e.g. temporal means, aggregating in time. All of the above is a non-trivial task and a workflow where a user could enter a point (s) and get a tidy data frame of data cube variables would be a step towards people understanding its value and being able to jumpstart their analysis. This project will contribute processing tools for finding, extracting and converting these key data layers.
 
 Developed as part of the Agricultural Research Federation (AgReFed), Geodata-Harvester is an open-source software that allows users to jumpstart their analysis with a suitable set of spatial-temporal aligned raster maps and dataframes.
 
-## Data Sources
+## 🌍 Data Sources
 
 A detailed list of all available layers and their description can be found in [Data Overview](quarto/docs/Data_Overview.md).
 
 The following main data sources are currently implemented:
 
 - Soil and Landscape Grid of Australia (SLGA)
 - SILO Climate Database
@@ -65,15 +65,15 @@
 
 1. Retrieve: given set of locations, automatically access and download multiple data sources (APIs) from a diverse range of geospatial and soil data sources
 2. Process: Spatial and temporal processing, conversion to dataframes and custom raster-files
 3. Output: Ready-made dataset for machine learning (training set and prediction mapping)
 
 Geodata-Harvester is designed as a modular and maintainable project in the form of a multi-stage pipeline by providing explicit boundaries among tasks. To encourage interaction and experimentation with the pipeline, multiple frontend notebooks and use case scenarios are provided.
 
-## Key Features
+## 🌟 Key Features
 
 Below is a list of features available for the geodata-harvester package. Please check the project Github webpage and notebooks for examples, data selection, and other settings.
 
 - enabling reproducible workflows via YAML settings files.
 - automatic data retrieval from geodata APIs for given locations and dates.
 - automatic download and spatiotemporal processing of geo-spatial maps for user-specified bounding box, resolution, and time-scale.
 - support for time-series data extraction for multiple time slices. 
@@ -82,15 +82,15 @@
 - preview of downloaded and aligned maps.
 - support for saving and loading settings via interactive widgets.
 - with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices.
 - example notebooks and use-cases are provided for the user to get started.
 
 For more features, please see the [API reference documentation](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
 
-## Installation
+## 🔧 Installation
 
 Geodata-Harvester can be run on cloud-servers (e.g., in JupyterHub environment) or on your local machine. 
 Example notebooks for importing and using the package can be found in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks). The package can be installed via PyPI or Conda:
 
 ### Conda or Mamba
 
 The package geodata-harvester is available via the conda-forge channel:
@@ -139,15 +139,15 @@
 As play-ground for workshop training sessions and testing of the Geodata-Harvester we provide a pre-installed cloud Python Jupyterlab environment, which does not require any local installation. For login instructions and how to access the sandbox, please visit our [Python workshop page](https://sydney-informatics-hub.github.io/AgReFed-Workshop/pydocs/py00-workshop.html).
 
 The Jupyter environment is hosted on the ARDC Nectar Research Cloud in partnership with AgReFed and Australian Research Data Commons (ARDC). Note that this sandbox is currently hosted for test purposes only and generated data is not permanently stored.
 
 The Geodata-Harvester can be easily installed also on other cloud services (e.g., Google Colab, Azure Notebooks).
 
 
-## How to get started
+## 🚀 How to get started
 
 You may now invoke the geodata-harvester directly from a python terminal with:
 
 ```python
 import geodata_harvester as gdh
 gdh.harvest.run(PATH_TO_SETTINGS_YAMLFILE)
 ```
@@ -158,44 +158,44 @@
 
 1. Options and user settings are defined by the user in the settings; see for settings documentation [Settings_Overview](quarto/docs/Settings_Overview.md)
 
 2. Run the jupyter notebook in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks).
 
 If you would like to learn more about the Geodata-Harvester, please visit our [Workshop webpage](https://sydney-informatics-hub.github.io/AgReFed-Workshop/).
 
-## How to add new data source modules
+## ➕ How to add new data source modules
 
 The Geodata-Harvester is designed to be extendable and new data source modules can be added as Python modules (for examples, see `getdata_*.py` modules). If you would like to add a new data source, please follow the [adding new data source guidelines](quarto/docs/How_to_add_DataSources.md)  
 
 We recommend to fork the geodata-harvester repo and develop new modules in a local environment. If you would like to contribute your data source module to the geodata-harvester package, please visit the [geodata-harvester contribution guidelines](quarto/docs/Contributing.md).
 
 
-## Code reference API
+## 📚 Code reference API
 
 An auto-generated API reference documentation is available [here](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
 
-## Contributions
+## 🤝 Contributions
 We are happy for any contribution to the geodata-harvester, whether feedbacks and bug reports via github Issues, adding use-case examples via notebook contributions, to improving source-code and adding new or updating existing data source modules. 
 
 For more details about about how to contribute to the development, please visit the [Geodata-Harvester contribution guidelines](quarto/docs/Contributing.md).
 
 
-## Attribution and Acknowledgments
+## 👏 Attribution and Acknowledgments
 
 This software was developed by the Sydney Informatics Hub, a core research facility of the University of Sydney, as part of the Data Harvesting project for the Agricultural Research Federation (AgReFed).
 
 Acknowledgments are an important way for us to demonstrate the value we bring to your research. Your research outcomes are vital for ongoing funding of the Sydney Informatics Hub.
 
 If you make use of this software for your research project, please include the following acknowledgment:
 
 “This research was supported by the Sydney Informatics Hub, a Core Research Facility of the University of Sydney, and the Agricultural Research Federation (AgReFed)."
 
 AgReFed is supported by the Australian Research Data Commons (ARDC) and the Australian Government through the National Collaborative Research Infrastructure Strategy (NCRIS).
 
-## License
+## 📄 License
 
 Copyright 2023 The University of Sydney
 
 This is free software: you can redistribute it and/or modify it under
 the terms of the GNU Lesser General Public License (LGPL version 3) as
 published by the Free Software Foundation.
```

### Comparing `geodata-harvester-1.0.0/setup.py` & `geodata-harvester-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 try:
     from setuptools import setup, find_packages
 except ImportError:
     from distutils.core import setup
 from os import path
 import io
 
-PYPI_VERSION = '1.0.0'
+PYPI_VERSION = '1.0.1'
 
 this_directory = path.abspath(path.dirname(__file__))
 with io.open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 packages = find_packages('src')
 package_dir = {'': 'src'}
```

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/__init__.py` & `geodata-harvester-1.0.1/src/geodata_harvester/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 - SILO Climate Database, see getdata_silo.py
 - National Digital Elevation Model (DEM), see getdata_dem.py
 - Digital Earth Australia (DEA) Geoscience Earth Observations, see getdata_dea.py
 - Radiometric Data, see getdata_radiometric.py
 - Google Earth Engine Data (GEE account needed), see docs for eeharvest
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __title__ = "Geodata-Harvester"
 __description__ = """
 This Python package provides automation tools for harvesting and processing geodata from the web.
 """
 __uri__ = "https://github.com/Sydney-Informatics-Hub/geodata-harvester"
 __doc__ = __description__ + " <" + __uri__ + ">"
```

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/arc2meter.py` & `geodata-harvester-1.0.1/src/geodata_harvester/arc2meter.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/getdata_dea.py` & `geodata-harvester-1.0.1/src/geodata_harvester/getdata_dea.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/getdata_dem.py` & `geodata-harvester-1.0.1/src/geodata_harvester/getdata_dem.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/getdata_landscape.py` & `geodata-harvester-1.0.1/src/geodata_harvester/getdata_landscape.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/getdata_radiometric.py` & `geodata-harvester-1.0.1/src/geodata_harvester/getdata_radiometric.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/getdata_silo.py` & `geodata-harvester-1.0.1/src/geodata_harvester/getdata_silo.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/getdata_slga.py` & `geodata-harvester-1.0.1/src/geodata_harvester/getdata_slga.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/harvest.py` & `geodata-harvester-1.0.1/src/geodata_harvester/harvest.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/settingshandler.py` & `geodata-harvester-1.0.1/src/geodata_harvester/settingshandler.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/spatial.py` & `geodata-harvester-1.0.1/src/geodata_harvester/spatial.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/temporal.py` & `geodata-harvester-1.0.1/src/geodata_harvester/temporal.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                 + x
                 + " Options are",
                 [t for t in xds.attrs],
             )
             return None
 
         array_list.append(xds)
-        print("attrs", xds.attrs[attribute_name])
+        #print("attrs", xds.attrs[attribute_name])
         attrs = attrs + xds.attrs[attribute_name]
         if first == True:
             coords = xds[channel_name].values
 
             first = False
         else:
             coords = np.append(coords, xds[channel_name].values + coords[-1])
@@ -230,15 +230,21 @@
         xdr_groups = xdr.groupby("time.month")
 
         if buffer != None:
             xx = xdr_groups.apply(lambda x: x.isel(time=slice(0,buffer)))
             xdr_groups = xx.groupby("time.month")
 
     elif type(period) == int:
-        bins = int(np.floor(len(xdr) / period))
+        time_start = xdr.time.values[0].astype('datetime64[s]').tolist()
+        time_end = xdr.time.values[-1].astype('datetime64[s]').tolist()
+        bins = (time_end - time_start).days // period
+        #bins = int(np.floor(len(xdr) / period)) # this only works if len(xdr) is in days
+        if bins == 0:
+            # If the period is smaller than the time step, use the time step as the period
+            bins = 1
         xdr_groups = xdr.groupby_bins("time", bins)
 
         if buffer != None:
             xx = xdr_groups.apply(lambda x: x.isel(time=slice(0,buffer)))
             xdr_groups = xx.groupby_bins("time", period)
```

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/utils.py` & `geodata-harvester-1.0.1/src/geodata_harvester/utils.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/validate_settings.py` & `geodata-harvester-1.0.1/src/geodata_harvester/validate_settings.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/widgets/harvesterwidgets.py` & `geodata-harvester-1.0.1/src/geodata_harvester/widgets/harvesterwidgets.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/errors.py` & `geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/errors.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/filechooser.py` & `geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/filechooser.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipyfilechooser/utils.py` & `geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/utils.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/widgets/ipywidgets_file_selector.py` & `geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipywidgets_file_selector.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester/write_logs.py` & `geodata-harvester-1.0.1/src/geodata_harvester/write_logs.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester.egg-info/PKG-INFO` & `geodata-harvester-1.0.1/src/geodata_harvester.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodata-harvester
-Version: 1.0.0
+Version: 1.0.1
 Summary: An automation tool for harvesting and processing geodata from the web
 Home-page: https://github.com/Sydney-Informatics-Hub/geodata-harvester
 License: LGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -27,41 +27,41 @@
 
 <!-- Badges end -->
 
 The Geodata-Harvester Python package offers reusable and automated workflows for data extraction from a wide range of geospatial and environmental data sources. User provided data is auto-completed with a suitable set of spatial- and temporal-aligned covariates as a ready-made dataset for machine learning and environmental models. In addition, all requested data layer maps are automatically extracted and aligned for a specific region and time period.
 
 For the R-package wrapper of the Geodata-Harvester, please visit the [Github dataharvesteR project](https://github.com/Sydney-Informatics-Hub/dataharvester).
 
-## Content
+## 📚 Table of Contents
 
-- [Introduction](#introduction)
-- [Data Sources](#data-sources)
-- [Functionality](#functionality)
-- [Key Features](#key-features)
-- [Installation](#installation)
+- [Introduction](#-introduction)
+- [Data Sources](#-data-sources)
+- [Functionality](#-functionality)
+- [Key Features](#-key-features)
+- [Installation](#-installation)
     - [Conda or Mamba](#conda-or-mamba)
     - [PyPI](#pypi)
     - [Google Earth Engine extension](#google-earth-engine-extension)
     - [Local development](#local-development)
     - [Workshop Cloud Sandbox](#workshop-cloud-sandbox)
-- [How to get started](#how-to-get-started)
-- [How to add new data source modules](#how-to-add-new-data-source-modules)
-- [Code reference API](#code-reference-api)
-- [Contributions](#contributions)
-- [Attribution and Acknowledgments](#attribution-and-acknowledgments)
-- [License](#license)
+- [How to get started](#-how-to-get-started)
+- [How to add new data source modules](#-how-to-add-new-data-source-modules)
+- [Code reference API](#-code-reference-api)
+- [Contributions](#-contributions)
+- [Attribution and Acknowledgments](#-attribution-and-acknowledgments)
+- [License](#-license)
 
 
-## Introduction
+## 💡 Introduction
 
 There is an enormous amount of national/global space-time data that is free and accessible. Examples are the numerous satellite platforms, weather, soil landscape grid of Australia. Many have a temporal dimension so for any point in Australia you can extract a time series of remote sensing and weather data and soil and terrain site variables. In the case of time series covariates there are a number of post-processing steps that a user can undertake to extract meaning, e.g. temporal means, aggregating in time. All of the above is a non-trivial task and a workflow where a user could enter a point (s) and get a tidy data frame of data cube variables would be a step towards people understanding its value and being able to jumpstart their analysis. This project will contribute processing tools for finding, extracting and converting these key data layers.
 
 Developed as part of the Agricultural Research Federation (AgReFed), Geodata-Harvester is an open-source software that allows users to jumpstart their analysis with a suitable set of spatial-temporal aligned raster maps and dataframes.
 
-## Data Sources
+## 🌍 Data Sources
 
 A detailed list of all available layers and their description can be found in [Data Overview](quarto/docs/Data_Overview.md).
 
 The following main data sources are currently implemented:
 
 - Soil and Landscape Grid of Australia (SLGA)
 - SILO Climate Database
@@ -77,15 +77,15 @@
 
 1. Retrieve: given set of locations, automatically access and download multiple data sources (APIs) from a diverse range of geospatial and soil data sources
 2. Process: Spatial and temporal processing, conversion to dataframes and custom raster-files
 3. Output: Ready-made dataset for machine learning (training set and prediction mapping)
 
 Geodata-Harvester is designed as a modular and maintainable project in the form of a multi-stage pipeline by providing explicit boundaries among tasks. To encourage interaction and experimentation with the pipeline, multiple frontend notebooks and use case scenarios are provided.
 
-## Key Features
+## 🌟 Key Features
 
 Below is a list of features available for the geodata-harvester package. Please check the project Github webpage and notebooks for examples, data selection, and other settings.
 
 - enabling reproducible workflows via YAML settings files.
 - automatic data retrieval from geodata APIs for given locations and dates.
 - automatic download and spatiotemporal processing of geo-spatial maps for user-specified bounding box, resolution, and time-scale.
 - support for time-series data extraction for multiple time slices. 
@@ -94,15 +94,15 @@
 - preview of downloaded and aligned maps.
 - support for saving and loading settings via interactive widgets.
 - with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices.
 - example notebooks and use-cases are provided for the user to get started.
 
 For more features, please see the [API reference documentation](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
 
-## Installation
+## 🔧 Installation
 
 Geodata-Harvester can be run on cloud-servers (e.g., in JupyterHub environment) or on your local machine. 
 Example notebooks for importing and using the package can be found in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks). The package can be installed via PyPI or Conda:
 
 ### Conda or Mamba
 
 The package geodata-harvester is available via the conda-forge channel:
@@ -151,15 +151,15 @@
 As play-ground for workshop training sessions and testing of the Geodata-Harvester we provide a pre-installed cloud Python Jupyterlab environment, which does not require any local installation. For login instructions and how to access the sandbox, please visit our [Python workshop page](https://sydney-informatics-hub.github.io/AgReFed-Workshop/pydocs/py00-workshop.html).
 
 The Jupyter environment is hosted on the ARDC Nectar Research Cloud in partnership with AgReFed and Australian Research Data Commons (ARDC). Note that this sandbox is currently hosted for test purposes only and generated data is not permanently stored.
 
 The Geodata-Harvester can be easily installed also on other cloud services (e.g., Google Colab, Azure Notebooks).
 
 
-## How to get started
+## 🚀 How to get started
 
 You may now invoke the geodata-harvester directly from a python terminal with:
 
 ```python
 import geodata_harvester as gdh
 gdh.harvest.run(PATH_TO_SETTINGS_YAMLFILE)
 ```
@@ -170,44 +170,44 @@
 
 1. Options and user settings are defined by the user in the settings; see for settings documentation [Settings_Overview](quarto/docs/Settings_Overview.md)
 
 2. Run the jupyter notebook in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks).
 
 If you would like to learn more about the Geodata-Harvester, please visit our [Workshop webpage](https://sydney-informatics-hub.github.io/AgReFed-Workshop/).
 
-## How to add new data source modules
+## ➕ How to add new data source modules
 
 The Geodata-Harvester is designed to be extendable and new data source modules can be added as Python modules (for examples, see `getdata_*.py` modules). If you would like to add a new data source, please follow the [adding new data source guidelines](quarto/docs/How_to_add_DataSources.md)  
 
 We recommend to fork the geodata-harvester repo and develop new modules in a local environment. If you would like to contribute your data source module to the geodata-harvester package, please visit the [geodata-harvester contribution guidelines](quarto/docs/Contributing.md).
 
 
-## Code reference API
+## 📚 Code reference API
 
 An auto-generated API reference documentation is available [here](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
 
-## Contributions
+## 🤝 Contributions
 We are happy for any contribution to the geodata-harvester, whether feedbacks and bug reports via github Issues, adding use-case examples via notebook contributions, to improving source-code and adding new or updating existing data source modules. 
 
 For more details about about how to contribute to the development, please visit the [Geodata-Harvester contribution guidelines](quarto/docs/Contributing.md).
 
 
-## Attribution and Acknowledgments
+## 👏 Attribution and Acknowledgments
 
 This software was developed by the Sydney Informatics Hub, a core research facility of the University of Sydney, as part of the Data Harvesting project for the Agricultural Research Federation (AgReFed).
 
 Acknowledgments are an important way for us to demonstrate the value we bring to your research. Your research outcomes are vital for ongoing funding of the Sydney Informatics Hub.
 
 If you make use of this software for your research project, please include the following acknowledgment:
 
 “This research was supported by the Sydney Informatics Hub, a Core Research Facility of the University of Sydney, and the Agricultural Research Federation (AgReFed)."
 
 AgReFed is supported by the Australian Research Data Commons (ARDC) and the Australian Government through the National Collaborative Research Infrastructure Strategy (NCRIS).
 
-## License
+## 📄 License
 
 Copyright 2023 The University of Sydney
 
 This is free software: you can redistribute it and/or modify it under
 the terms of the GNU Lesser General Public License (LGPL version 3) as
 published by the Free Software Foundation.
```

### Comparing `geodata-harvester-1.0.0/src/geodata_harvester.egg-info/SOURCES.txt` & `geodata-harvester-1.0.1/src/geodata_harvester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

