# Comparing `tmp/iga-0.0.9.tar.gz` & `tmp/iga-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iga-0.0.9.tar", last modified: Mon May  8 19:00:54 2023, max compression
+gzip compressed data, was "iga-1.0.0.tar", last modified: Fri May 19 00:22:15 2023, max compression
```

## Comparing `iga-0.0.9.tar` & `iga-1.0.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-08 19:00:54.305955 iga-0.0.9/
--rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-03-16 00:12:10.000000 iga-0.0.9/LICENSE
--rw-r--r--   0 mhucka     (503) staff       (20)    29356 2023-05-08 19:00:54.306050 iga-0.0.9/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)    28450 2023-05-08 18:59:03.000000 iga-0.0.9/README.md
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-08 19:00:54.302799 iga-0.0.9/iga/
--rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-05-08 19:00:02.000000 iga-0.0.9/iga/__init__.py
--rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-03-16 00:12:36.000000 iga-0.0.9/iga/__main__.py
--rw-r--r--   0 mhucka     (503) staff       (20)    32900 2023-05-08 18:59:03.000000 iga-0.0.9/iga/cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-03-27 20:05:34.000000 iga-0.0.9/iga/data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-04-10 21:11:51.000000 iga-0.0.9/iga/doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1179 2023-04-25 22:30:46.000000 iga-0.0.9/iga/exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1447 2023-03-28 00:40:16.000000 iga-0.0.9/iga/exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)    15031 2023-04-20 00:58:38.000000 iga-0.0.9/iga/github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4901 2023-04-26 04:08:12.000000 iga-0.0.9/iga/id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)    16908 2023-04-25 22:30:46.000000 iga-0.0.9/iga/invenio.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2058 2023-04-20 00:58:38.000000 iga-0.0.9/iga/json_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-03-08 23:12:16.000000 iga-0.0.9/iga/licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)    69659 2023-05-08 18:59:03.000000 iga-0.0.9/iga/metadata.py
--rw-r--r--   0 mhucka     (503) staff       (20)    14563 2023-04-26 04:08:12.000000 iga-0.0.9/iga/name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-04-08 02:44:39.000000 iga-0.0.9/iga/orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-04-08 02:44:39.000000 iga-0.0.9/iga/reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-04-08 02:44:39.000000 iga-0.0.9/iga/ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-04-08 02:44:39.000000 iga-0.0.9/iga/text_utils.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-08 19:00:54.303680 iga-0.0.9/iga.egg-info/
--rw-r--r--   0 mhucka     (503) staff       (20)    29356 2023-05-08 19:00:54.000000 iga-0.0.9/iga.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-05-08 19:00:54.000000 iga-0.0.9/iga.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-08 19:00:54.000000 iga-0.0.9/iga.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-05-08 19:00:54.000000 iga-0.0.9/iga.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-08 19:00:54.000000 iga-0.0.9/iga.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-05-08 19:00:54.000000 iga-0.0.9/iga.egg-info/requires.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-05-08 19:00:54.000000 iga-0.0.9/iga.egg-info/top_level.txt
--rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-05-08 19:00:54.306393 iga-0.0.9/setup.cfg
--rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-04-08 01:05:22.000000 iga-0.0.9/setup.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-08 19:00:54.305851 iga-0.0.9/tests/
--rw-r--r--   0 mhucka     (503) staff       (20)     5734 2023-04-25 22:30:46.000000 iga-0.0.9/tests/test_cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-03-27 19:38:15.000000 iga-0.0.9/tests/test_data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-03-17 23:21:28.000000 iga-0.0.9/tests/test_doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-03-02 15:36:12.000000 iga-0.0.9/tests/test_exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-01-13 03:19:50.000000 iga-0.0.9/tests/test_exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-04-07 01:26:59.000000 iga-0.0.9/tests/test_github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-04-07 01:20:36.000000 iga-0.0.9/tests/test_github_mocks.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3666 2023-04-26 04:08:12.000000 iga-0.0.9/tests/test_id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)      641 2022-12-08 00:11:08.000000 iga-0.0.9/tests/test_init.py
--rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-04-20 00:58:38.000000 iga-0.0.9/tests/test_is_person.py
--rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-03-02 15:16:32.000000 iga-0.0.9/tests/test_licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-04-20 00:58:38.000000 iga-0.0.9/tests/test_name_splitting.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-04-20 00:58:38.000000 iga-0.0.9/tests/test_name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-03-18 00:09:09.000000 iga-0.0.9/tests/test_orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1935 2023-04-08 01:31:14.000000 iga-0.0.9/tests/test_record_from_codemeta.py
--rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-03-02 23:04:18.000000 iga-0.0.9/tests/test_reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-03-18 00:05:51.000000 iga-0.0.9/tests/test_ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-04-06 22:54:59.000000 iga-0.0.9/tests/test_text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-19 00:22:15.678299 iga-1.0.0/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-03-16 00:12:10.000000 iga-1.0.0/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)    37613 2023-05-19 00:22:15.678414 iga-1.0.0/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)    36707 2023-05-18 20:14:21.000000 iga-1.0.0/README.md
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-19 00:22:15.667889 iga-1.0.0/iga/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-05-18 19:32:51.000000 iga-1.0.0/iga/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-03-16 00:12:36.000000 iga-1.0.0/iga/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    34712 2023-05-18 01:10:50.000000 iga-1.0.0/iga/cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-03-27 20:05:34.000000 iga-1.0.0/iga/data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-04-10 21:11:51.000000 iga-1.0.0/iga/doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1252 2023-05-17 19:19:30.000000 iga-1.0.0/iga/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1514 2023-05-17 19:19:30.000000 iga-1.0.0/iga/exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    15499 2023-05-09 20:43:53.000000 iga-1.0.0/iga/github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4901 2023-04-26 04:08:12.000000 iga-1.0.0/iga/id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    18504 2023-05-18 01:10:50.000000 iga-1.0.0/iga/invenio.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2058 2023-04-20 00:58:38.000000 iga-1.0.0/iga/json_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-03-08 23:12:16.000000 iga-1.0.0/iga/licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    69900 2023-05-16 20:21:25.000000 iga-1.0.0/iga/metadata.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    14563 2023-04-26 04:08:12.000000 iga-1.0.0/iga/name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-04-08 02:44:39.000000 iga-1.0.0/iga/orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-04-08 02:44:39.000000 iga-1.0.0/iga/reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-04-08 02:44:39.000000 iga-1.0.0/iga/ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-04-08 02:44:39.000000 iga-1.0.0/iga/text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-19 00:22:15.675952 iga-1.0.0/iga.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)    37613 2023-05-19 00:22:15.000000 iga-1.0.0/iga.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-05-19 00:22:15.000000 iga-1.0.0/iga.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-19 00:22:15.000000 iga-1.0.0/iga.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-05-19 00:22:15.000000 iga-1.0.0/iga.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-19 00:22:15.000000 iga-1.0.0/iga.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-05-19 00:22:15.000000 iga-1.0.0/iga.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-05-19 00:22:15.000000 iga-1.0.0/iga.egg-info/top_level.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-05-19 00:22:15.678737 iga-1.0.0/setup.cfg
+-rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-04-08 01:05:22.000000 iga-1.0.0/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-19 00:22:15.678201 iga-1.0.0/tests/
+-rw-r--r--   0 mhucka     (503) staff       (20)     6117 2023-05-18 01:03:27.000000 iga-1.0.0/tests/test_cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-03-27 19:38:15.000000 iga-1.0.0/tests/test_data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-03-17 23:21:28.000000 iga-1.0.0/tests/test_doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-03-02 15:36:12.000000 iga-1.0.0/tests/test_exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-01-13 03:19:50.000000 iga-1.0.0/tests/test_exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-04-07 01:26:59.000000 iga-1.0.0/tests/test_github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-04-07 01:20:36.000000 iga-1.0.0/tests/test_github_mocks.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3666 2023-04-26 04:08:12.000000 iga-1.0.0/tests/test_id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      641 2022-12-08 00:11:08.000000 iga-1.0.0/tests/test_init.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-04-20 00:58:38.000000 iga-1.0.0/tests/test_is_person.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-03-02 15:16:32.000000 iga-1.0.0/tests/test_licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-04-20 00:58:38.000000 iga-1.0.0/tests/test_name_splitting.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-04-20 00:58:38.000000 iga-1.0.0/tests/test_name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-03-18 00:09:09.000000 iga-1.0.0/tests/test_orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5997 2023-05-17 19:19:30.000000 iga-1.0.0/tests/test_record_from_codemeta.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-03-02 23:04:18.000000 iga-1.0.0/tests/test_reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-03-18 00:05:51.000000 iga-1.0.0/tests/test_ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-04-06 22:54:59.000000 iga-1.0.0/tests/test_text_utils.py
```

### Comparing `iga-0.0.9/LICENSE` & `iga-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/PKG-INFO` & `iga-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 0.0.9
+Version: 1.0.0
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IGA<img width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
 
-IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a GitHub Action that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
+IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Action](https://github.com/marketplace/actions/iga) that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
 [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
 [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
 [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
 
 
@@ -43,154 +43,244 @@
 * [Contributing](#contributing)
 * [License](#license)
 * [Acknowledgments](#authors-and-acknowledgments)
 
 
 ## Introduction
 
-[InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and datasets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the InvenioRDM GitHub Archiver (IGA) comes in.
+[InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and data sets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the [_InvenioRDM GitHub Archiver_](https://github.com/caltechlibrary/iga) (IGA) comes in.
 
 IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Action](https://docs.github.com/en/actions) to archive GitHub releases automatically for a repository each time they are made.
 
 <p align=center>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" width="40%">
 <span style="font-size: 150%">➜</span>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
 </p>
 
 IGA offers many notable features:
-* Automatic metadata extraction from GitHub releases plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
-* Thorough coverage of [InvenioRDM record metadata fields](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
-* Recognition of id's that appear in CodeMeta & CFF files: [ORCID](https://orcid.org), [ROR](https://ror.org), [DOI](https://www.doi.org), [arXiv](https://arxiv.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
-* Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google Books, & other sources if needed
+* Automatic metadata extraction from GitHub plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
+* Thorough coverage of [InvenioRDM record metadata](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
+* Recognition of identifiers in CodeMeta & CFF files: [ORCID](https://orcid.org),, [DOI](https://www.doi.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
+* Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google, and other sources
 * Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
-* Automatic lookup of human names in [ORCID.org](https://orcid.org) if needed (assuming ORCID id's are provided)
-* Automatic splitting of human names into family and given names using [ML](https://en.wikipedia.org/wiki/Machine_learning)-based methods
+* Automatic lookup of human names in [ORCID.org](https://orcid.org) (assuming ORCID id's are provided)
+* Automatic splitting of human names into family & given names using [ML](https://en.wikipedia.org/wiki/Machine_learning) methods
 * Support for InvenioRDM [communities](https://invenio-communities.readthedocs.io/en/latest/)
-* Support for overriding the metadata record that IGA creates, for complete control if you need it
+* Support for overriding the record that IGA creates, for complete control if you need it
 * Support for using the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in simple cases
 * Extensive use of logging so you can see what's going on under the hood
 
 
 ## Installation
 
-### As a standalone command-line program
+IGA can be installed as either (or both) a command-line program on your computer or a [GitHub Action](https://docs.github.com/en/actions) in a GitHub repository.
 
-There are multiple ways of installing IGA.  Please choose the alternative that suits you.
+### IGA as a standalone program
 
-#### _Alternative 1: installing IGA using `pipx`_
+Please choose an approach that suits your situation and preferences.
+
+<details><summary><h4><i>Alternative 1: using <code>pipx</code></i></h4></summary>
 
 [Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
 ```sh
 pipx install iga
 ```
 
 Pipx can also let you run IGA directly using `pipx run iga`, although in that case, you must always prefix every IGA command with `pipx run`.  Consult the [documentation for `pipx run`](https://github.com/pypa/pipx#walkthrough-running-an-application-in-a-temporary-virtual-environment) for more information.
+</details>
 
+<details><summary><h4><i>Alternative 2: using <code>pip</code></i></h4></summary>
 
-#### _Alternative 2: installing IGA using `pip`_
-
-You should be able to install `iga` with [`pip`](https://pip.pypa.io/en/stable/installing/) for Python&nbsp;3.  To install `iga` from the [Python package repository (PyPI)](https://pypi.org), run the following command:
+IGA is available from the [Python package repository PyPI](https://pypi.org) and can be installed using [`pip`](https://pip.pypa.io/en/stable/installing/):
 ```sh
 python3 -m pip install iga
 ```
 
-As an alternative to getting it from [PyPI](https://pypi.org), you can use `pip` to install `iga` directly from GitHub:
+As an alternative to getting it from [PyPI](https://pypi.org), you can install `iga` directly from GitHub:
 ```sh
 python3 -m pip install git+https://github.com/caltechlibrary/iga.git
 ```
 
 _If you already installed IGA once before_, and want to update to the latest version, add `--upgrade` to the end of either command line above.
+</details>
 
+<details><summary><h4><i>Alternative 3: from sources</i></h4></summary>
 
-#### _Alternative 3: installing IGA from sources_
-
-If  you prefer to install IGA directly from the source code, you can do that too. To get a copy of the files, you can clone the GitHub repository:
+If  you prefer to install IGA directly from the source code, first obtain a copy by either downloading the source archive from the [IGA releases page on GitHub](https://github.com/caltechlibrary/iga/releases), or by using `git` to clone the repository to a location on your computer. For example,
 ```sh
 git clone https://github.com/caltechlibrary/iga
 ```
 
-Alternatively, you can download the software source files as a ZIP archive directly from your browser using this link: <https://github.com/caltechlibrary/iga/archive/refs/heads/main.zip>
-
 Next, after getting a copy of the files,  run `setup.py` inside the code directory:
 ```sh
 cd iga
 python3 setup.py install
 ```
+</details>
+
+After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+```shell
+iga --help
+```
+
 
+### IGA as a GitHub Action
 
-### As a GitHub Action
+A [GitHub Action](https://docs.github.com/en/actions) is a workflow that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
 
-[...forthcoming...]
+1. In the main branch of your GitHub repository, create a `.github/workflows` directory
+2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/develop/sample-workflow.yml) into it:
+    ```yaml
+    name: InvenioRDM GitHub Archiver
+
+    env:
+      # 👋🏻 Set the next variable to your InvenioRDM server address 👋🏻
+      INVENIO_SERVER: https://your-invenio-server.org
+
+      # Set to an InvenioRDM record ID to mark releases as new versions.
+      parent_record: none
+
+      # The remaining variables are other IGA options. Please see the docs.
+      community:     none
+      draft:         false
+      all_assets:    false
+      all_metadata:  false
+      debug:         false
+
+    # ~~~~~~~~~~~~~~~~ The rest of this file should be left as-is. ~~~~~~~~~~~~~~~~
+
+    on:
+      release:
+        types: [published]
+      workflow_dispatch:
+        inputs:
+          release_tag:
+            description: "The release tag (empty = latest):"
+          draft:
+            default: false
+            description: "Mark the InvenioRDM record as a draft:"
+          parent_record:
+            description: "ID of parent record (for versioning):"
+          community:
+            description: "Name of InvenioRDM community (if any):"
+          all_assets:
+            default: false
+            description: "Attach all GitHub assets:"
+          all_metadata:
+            default: false
+            description: "Include additional GitHub metadata:"
+          debug:
+            default: false
+            description: "Print debug info in the GitHub log:"
+    jobs:
+      Send_to_InvenioRDM:
+        runs-on: ubuntu-latest
+        steps:
+          - uses: caltechlibrary/iga@main
+            with:
+              INVENIO_SERVER: ${{env.INVENIO_SERVER}}
+              INVENIO_TOKEN:  ${{secrets.INVENIO_TOKEN}}
+              all_assets:     ${{github.event.inputs.all_assets || env.all_assets}}
+              all_metadata:   ${{github.event.inputs.all_metadata || env.all_metadata}}
+              debug:          ${{github.event.inputs.debug || env.debug}}
+              draft:          ${{github.event.inputs.draft || env.draft}}
+              community:      ${{github.event.inputs.community || env.community}}
+              parent_record:  ${{github.event.inputs.parent_record || env.parent_record}}
+              release_tag:    ${{github.event.inputs.release_tag || 'latest'}}
+    ```
+3. **Edit the value of the `INVENIO_SERVER` variable (line 5 above)** ↑
+4. Optionally, change the values of other options (`parent_record`, `community`, etc.)
+5. Save the file, commit the changes to git, and push your changes to GitHub
 
 
 ## Quick start
 
-After a successful [installation](#installation) of IGA, here is how you can get started quickly.
+No matter whether IGA is run locally on your computer or as a GitHub Action, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one 
+is the first step.
 
-### Command-line use
+### Getting an InvenioRDM token
 
-If the [installation](#installation) process described above is successful, you should end up with a program named `iga` in a location where software is normally installed on your computer.  Running `iga` should be as simple as running any other command-line program. For example, the following command should print a helpful message to your terminal:
-```shell
-iga --help
-```
+<img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/get-invenio-pat.png" width="60%" align="right">
+
+1. Log in to your InvenioRDM account
+2. Go to the _Applications_ page in your account profile
+3. Click the <kbd>New token</kbd> button next to "Personal access tokens"
+4. On the page that is shown after you click that button, name your token (the name does not matter) and click the <kbd>Create</kbd> button
+5. After InvenioRDM creates and shows you the token, **copy it to a safe location** because InvenioRDM will not show it again
 
-IGA's main purpose is to create a metadata record in an InvenioRDM server and attach a GitHub release archive to the record. IGA needs 4 pieces of information to do its work, though for simple repositories you can often get by with just 3:
+### Configuring and running IGA locally
+
+To send a GitHub release to your InvenioRDM server, IGA needs this information:
 1. (Required) The identity of the GitHub release to be archived
 2. (Required) The address of the destination InvenioRDM server
-3. (Required) A Personal Access Token (PAT) for the InvenioRDM server
-4. (Optional) A Personal Access Token for GitHub
+3. (Required) A personal access token for InvenioRDM (from [above](#getting-an-inveniordm-token))
+4. (Optional) A [personal access token for GitHub](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
 
-The first one (the identity of the GitHub release) is given as arguments to IGA on the command line; the rest can be provided either via command-line options or by setting environment variables. A common way of configuring IGA is to set environment variables in your shell script or your interactive shell. Here is an example using Bash shell syntax, with realistic-looking but fake token values:
+The identity of the GitHub release is always given as an argument to IGA on the command line; the remaining values can be provided either via command-line options or environment variables. One approach is to set environment variables in shell scripts or your interactive shell. Here is an example using Bash shell syntax, with fake token values:
 ```shell
 export INVENIO_SERVER=https://data.caltech.edu
 export INVENIO_TOKEN=qKLoOH0KYf4D98PGYQGnC09hiuqw3Y1SZllYnonRVzGJbWz2
 export GITHUB_TOKEN=ghp_wQXp6sy3AsKyyEo4l9esHNxOdo6T34Zsthz
 ```
 
-Once these environment variables set in your shell, you can more easily invoke IGA. Usage can be as simple as providing a URL for a release in GitHub. For example:
+Once these are set, use of IGA can be as simple as providing a URL for a release in GitHub. For example, the following command creates a draft record (the `-d` option is short for `--draft`) for another project in GitHub and tells IGA to open (the `-o` option is short for `--open`) the newly-created InvenioRDM entry in a web browser:
 ```shell
-iga https://github.com/mhucka/taupe/releases/tag/v1.2.0
+iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
-If you give the option `--open` (or `-o` for short) to IGA, it will open the newly-created InvenioRDM entry in your default web browser when it's done:
-```shell
-iga -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
-```
+More options are described in the section on [detailed usage information](#usage) below.
 
-If you want the record to be only a draft and not a final version (perhaps so that you can inspect the result and edit it before finalizing it), use the option `--draft` (or `-d` for short):
-```shell
-iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
-```
 
-More options and examples can be found in the section on [detailed usage information](#usage) below.
+### Configuring and running IGA as a GitHub Action
+
+After doing the [GitHub Action installation](#as-a-github-action) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
+
+1. Go to the _Settings_ page of your GitHub repository<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-tabs.png" width="85%"></p>
+2. In the left-hand sidebar, find _Secrets and variables_ in the Security section, click on it to reveal _Actions_ underneath, then click on _Actions_<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-sidebar-secrets.png" width="40%"></p>
+3. In the next page, click the green <kbd>New repository secret</kbd> button<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-secrets.png" width="60%"></p>
+4. Name the variable `INVENIO_TOKEN` and paste in your InvenioRDM token
+5. Finish by clicking the green <kbd>Add secret</kbd> button
+
+#### Testing the workflow
+
+After setting up the workflow and storing the InvenioRDM token in your repository on GitHub, it's a good idea to run the workflow manually to test that it works as expected.
+
+1. Go to the _Actions_ tab in your repository and click on the name of the workflow in the sidebar on the left<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-run-workflow.png" width="90%"></p>
+2. Click the <kbd>Run workflow</kbd> button in the right-hand side of the blue strip
+3. In the pull-down, change the value of "Mark the record as a draft" to `true`<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-workflow-options-circled.png" width="40%"></p>
+4. Click the green <kbd>Run workflow</kbd> button near the bottom
+5. Refresh the web page and a new line will be shown named after your workflow file<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-running-workflow.png" width="90%"></p>
+6. Click the title of the workflow to see the IGA workflow progress and results
 
 
-### GitHub Action use
+#### Running the workflow when releasing software
 
-[...forthcoming...]
+Once the personal access token from InvenioRDM is stored as a GitHub secret, the workflow should run automatically every time a new release is made on GitHub &ndash; no further action should be needed. You can check the results (and look for errors if something went wrong) by going to the _Actions_ tab in your GitHub repository.
 
 
 ## Usage
 
 This section provides detailed information about IGA's operation and options to control it.
 
 ### Identifying the InvenioRDM server
 
 The server address must be provided either as the value of the option `--invenio-server` or in an environment variable named `INVENIO_SERVER`.  If the server address does not begin with `https://`, IGA will prepend it automatically.
 
 ### Providing an InvenioRDM access token
 
-A Personal Access Token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
+A personal access token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
 
 To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
 
 ### Providing a GitHub access token
 
-It is possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for many repositories, IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some repositories IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+
+Note that when you run IGA as a GitHub Action, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Action workflow.
 
 ### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
  1. The full URL of the web page on GitHub of a tagged release. In this case,
     the URL must be the final argument on the command line invocation of IGA
     and the options `--account` and `--repo` must be omitted.
@@ -252,17 +342,17 @@
 
 ### Other options recognized by IGA
 
 Running IGA with the option `--save-metadata` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-metadata` to save a record to a file, edit the result, then finally run IGA with the `--read-metadata` option to use the modified record to create a release in the InvenioRDM server.
 
 The `--mode` option can be used to change the run mode. Four run modes are available: `quiet`, `normal`, `verbose`, and `debug`. The default mode is `normal`, in which IGA prints a few messages while it's working. The mode `quiet` will make it avoid printing anything unless an error occurs, the mode `verbose` will make it print a detailed trace of what it is doing, and the mode `debug` will make IGA even more verbose. In addition, in `debug` mode, IGA will drop into the `pdb` debugger if it encounters an exception during execution. On Linux and macOS, debug mode also installs a signal handler on signal USR1 that causes IGA to drop into the `pdb` debugger if the signal USR1 is received. (Use `kill -USR1 NNN`, where NNN is the IGA process id.)
 
-Networks latencies are unpredicatable. Reading and writing large files may take a long time; on the other hand, IGA should not wait forever before reporting an error if a server or network becomes unresponsive. To balance these conflicting needs, IGA automatically scales its network timeout based on file sizes. To override its adaptive algorithm and set an explicit timeout value, use the option `--timeout` with a value in seconds.
+By default, informational output is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` (i.e., a dash) to indicate console output, or it can be a file path to send the output to the file. A special exception is that even if a log destination is given, IGA will still print the final record URL to stdout.  This makes it possible to invoke IGA from scripts that capture the record URL while still saving diagnostic output in case debugging is needed.
 
-By default, the output of the `verbose` and `debug` run modes is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` to indicate console output, or a file path to send the output to the file.
+Reading and writing large files may take a long time; on the other hand, IGA should not wait forever on network operations before reporting an error if a server or network becomes unresponsive. To balance these conflicting needs, IGA automatically scales its network timeout based on file sizes. To override its adaptive algorithm and set an explicit timeout value, use the option `--timeout` with a value in seconds.
 
 If given the `--version` option, this program will print its version and other information, and exit without doing anything else.
 
 Running IGA with the option `--help` will make it print help text and exit without doing anything else.
 
 ### Summary of command-line options
 
@@ -273,15 +363,15 @@
 | `--all-assets`         | `-A`     | Attach all GitHub assets | Attach only the release source ZIP| |
 | `--all-metadata`       | `-M`     | Include additional metadata from GitHub | Favor CodeMeta & CFF | |
 | `--community` _C_      | `-c` _C_ | Submit record to RDM community _C_ | Don't submit record to any community | | 
 | `--draft`              | `-d`     | Mark the RDM record as a draft | Publish record when done | |
 | `--file` _F_           | `-f` _F_ | Upload local file _F_ instead of GitHub assets | Upload only GitHub assets | ⚑ |
 | `--github-account` _A_ | `-a` _A_ | Look in GitHub account _A_ | Get account name from release URL | ✯ | 
 | `--github-repo` _R_    | `-r` _R_ | Look in GitHub repository _R_ of account _A_ | Get repo name from release URL | ✯ |
-| `--github-token` _T_   | `-t` _T_ | Use GitHub acccess token _T_| Use value in env. var. `GITHUB_TOKEN` | |
+| `--github-token` _T_   | `-t` _T_ | Use GitHub access token _T_| Use value in env. var. `GITHUB_TOKEN` | |
 | `--help`               | `-h`     | Print help info and exit | | |
 | `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
 | `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
 | `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
@@ -304,20 +394,24 @@
 |:----:|----------------------------------------------------------|
 | 0    | success &ndash; program completed normally               |
 | 1    | interrupted                                              |
 | 2    | encountered a bad or missing value for an option         |
 | 3    | encountered a problem with a file or directory           |
 | 4    | encountered a problem interacting with GitHub            |
 | 5    | encountered a problem interacting with InvenioRDM        |
-| 6    | an exception or fatal error occurred                     |
+| 6    | the personal access token was rejected                   |
+| 7    | an exception or fatal error occurred                     |
 
 
 ## Known issues and limitations
 
-_[… forthcoming …]_
+The following are known issues and limitations.
+* As of mid-2023, InvenioRDM requires names of record creators and other contributors to be split into given (first) and family (surname). This is problematic for multiple reasons. The first is that mononyms are common in many countries: a person's name may legitimately be only a single word which is not conceptually a "given" or "family" name.  To compound the difficulty for IGA, names are stored as single fields in GitHub account metadata, so unless a repository has a `codemeta.json` or `CITATION.cff` file (which allow authors more control over how they want their names represented), IGA is forced to try to split the single GitHub name string into two parts. _A foolproof algorithm for doing this does not exist_, so IGA will sometimes get it wrong. (That said, IGA goes to extraordinary lengths to try to do a good job.)
+* Some accounts on GitHub are software automation or "bot" accounts but are not labeled as such. These accounts are generally indistinguishable from human accounts on GitHub. If such an account is the creator of a release in GitHub, and IGA has to use its name-splitting algorithm on the name of the account, it may produce a nonsensical result. For example, it might turn "Travis CI" into an entry with a first name of "Travis" and last name of "CI". 
+
 
 ## Getting help
 
 If you find an issue, please submit it in [the GitHub issue tracker](https://github.com/caltechlibrary/iga/issues) for this repository.
 
 
 ## Contributing
@@ -346,38 +440,44 @@
 * [humanize](https://github.com/jmoiron/humanize) &ndash; make numbers more easily readable by humans
 * [idutils](https://github.com/inveniosoftware/idutils) &ndash; package for validating and normalizing various kinds of persistent identifiers
 * [ipdb](https://github.com/gotcha/ipdb) &ndash; the IPython debugger
 * [iptools](https://github.com/bd808/python-iptools) &ndash; utilities for dealing with IP addresses
 * [isbnlib](https://github.com/xlcnd/isbnlib) &ndash; utilities for dealing with ISBNs
 * [json5](https://github.com/dpranke/pyjson5) &ndash; extended JSON format parser
 * [latexcodec](https://github.com/mcmtroffaes/latexcodec) &ndash; lexer and codec to work with LaTeX code in Python
+* [linkify-it-py](https://github.com/tsutsu3/linkify-it-py) &ndash; a link recognition library with full unicode support
 * [lxml](https://lxml.de) &ndash; an XML parsing library
 * [Markdown](https://python-markdown.github.io) &ndash; Python package for working with Markdown
 * [markdown-checklist](https://github.com/FND/markdown-checklist) &ndash; GitHub-style checklist extension for Python Markdown package
 * [mdx-breakless-lists](https://github.com/adamb70/mdx-breakless-lists) &ndash; GitHub-style Markdown lists that don't require a line break above them
 * [mdx_linkify](https://github.com/daGrevis/mdx_linkify) &ndash; extension for Python Markdown will convert text that look like links to HTML anchors
+* [MyST-parser](https://github.com/executablebooks/MyST-Parser) &ndash; A Sphinx and Docutils extension to parse an extended version of Markdown
 * [nameparser](https://github.com/derek73/python-nameparser) &ndash; package for parsing human names into their individual components
 * [probablepeople](https://github.com/datamade/probablepeople) &ndash; package for parsing names into components using ML-based techniques
-* [pymdown-extensions](https://github.com/facelessuser/pymdown-extensions) &ndash; extensions for Python Markdown
-* [PyYAML](https://pyyaml.org) &ndash; YAML parser
 * [pybtex](https://pybtex.org) &ndash; BibTeX parser and formatter
 * [pybtex-apa7-style]() &ndash; plugin for [pybtex](https://pybtex.org) that provides APA7 style formatting
+* [pymdown-extensions](https://github.com/facelessuser/pymdown-extensions) &ndash; extensions for Python Markdown
 * [pytest](https://docs.pytest.org/en/stable/) &ndash; testing framework
 * [pytest-cov](https://github.com/pytest-dev/pytest-cov) &ndash; coverage reports for use with `pytest`
 * [pytest-mock](https://pypi.org/project/pytest-mock/) &ndash; wrapper around the `mock` package for use with `pytest`
+* [PyYAML](https://pyyaml.org) &ndash; YAML parser
 * [Rich](https://github.com/Textualize/rich) &ndash; library for writing styled text to the terminal
 * [rich-click](https://github.com/ewels/rich-click) &ndash; CLI interface built on top of [Rich](https://github.com/Textualize/rich)
+* [setuptools](https://github.com/pypa/setuptools) &ndash; library for `setup.py`
 * [Sidetrack](https://github.com/caltechlibrary/sidetrack) &ndash; simple debug logging/tracing package
 * [spaCy](https://spacy.io) &ndash; Natural Language Processing package
 * [spacy-alignments](https://github.com/explosion/spacy-alignments) &ndash; alternate alignments for [spaCy](https://spacy.io)
 * [spacy-legacy](https://pypi.org/project/spacy-legacy/) &ndash; [spaCy](https://spacy.io) legacy functions and architectures for backwards compatibility
 * [spacy-loggers](https://github.com/explosion/spacy-loggers) &ndash; loggers for [spaCy](https://spacy.io)
 * [spacy-pkuseg](https://github.com/explosion/spacy-pkuseg) &ndash; Chinese word segmentation toolkit for [spaCy](https://spacy.io)
 * [spacy-transformers](https://spacy.io) &ndash; pretrained Transformers for [spaCy](https://spacy.io)
-* [setuptools](https://github.com/pypa/setuptools) &ndash; library for `setup.py`
+* [Sphinx](https://www.sphinx-doc.org/en/master/) &ndash; documentation generator for Python
+* [sphinx-autobuild](https://pypi.org/project/sphinx-autobuild/) &ndash; rebuild Sphinx docs automatically
+* [sphinx-material](https://bashtage.github.io/sphinx-material/) &ndash; a responsive Material Design theme for Sphinx
+* [sphinxcontrib-mermaid](https://github.com/mgaitan/sphinxcontrib-mermaid) &ndash; support Mermaid diagrams in Sphinx docs
 * [StringDist](https://github.com/obulkin/string-dist) &ndash; library for calculating string distances
 * [Twine](https://github.com/pypa/twine) &ndash; utilities for publishing Python packages on [PyPI](https://pypi.org)
 * [url-normalize](https://github.com/niksite/url-normalize) &ndash; URI/URL normalization utilities
 * [validators](https://github.com/kvesteri/validators) &ndash; data validation package for Python
 * [wheel](https://pypi.org/project/wheel/) &ndash; setuptools extension for building wheels
 
 <div align="center">
```

### Comparing `iga-0.0.9/README.md` & `iga-1.0.0/iga.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,34 @@
+Metadata-Version: 2.1
+Name: iga
+Version: 1.0.0
+Summary: InvenioRDM GitHub Archiver
+Home-page: https://github.com/caltechlibrary/iga
+Author: Michael Hucka
+Author-email: helpdesk@library.caltech.edu
+License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
+Project-URL: Source Code, https://github.com/caltechlibrary/iga
+Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
+Keywords: Python,applications
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # IGA<img width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
 
-IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a GitHub Action that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
+IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Action](https://github.com/marketplace/actions/iga) that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
 [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
 [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
 [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
 
 
@@ -19,154 +43,244 @@
 * [Contributing](#contributing)
 * [License](#license)
 * [Acknowledgments](#authors-and-acknowledgments)
 
 
 ## Introduction
 
-[InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and datasets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the InvenioRDM GitHub Archiver (IGA) comes in.
+[InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and data sets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the [_InvenioRDM GitHub Archiver_](https://github.com/caltechlibrary/iga) (IGA) comes in.
 
 IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Action](https://docs.github.com/en/actions) to archive GitHub releases automatically for a repository each time they are made.
 
 <p align=center>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" width="40%">
 <span style="font-size: 150%">➜</span>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
 </p>
 
 IGA offers many notable features:
-* Automatic metadata extraction from GitHub releases plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
-* Thorough coverage of [InvenioRDM record metadata fields](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
-* Recognition of id's that appear in CodeMeta & CFF files: [ORCID](https://orcid.org), [ROR](https://ror.org), [DOI](https://www.doi.org), [arXiv](https://arxiv.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
-* Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google Books, & other sources if needed
+* Automatic metadata extraction from GitHub plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
+* Thorough coverage of [InvenioRDM record metadata](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
+* Recognition of identifiers in CodeMeta & CFF files: [ORCID](https://orcid.org),, [DOI](https://www.doi.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
+* Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google, and other sources
 * Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
-* Automatic lookup of human names in [ORCID.org](https://orcid.org) if needed (assuming ORCID id's are provided)
-* Automatic splitting of human names into family and given names using [ML](https://en.wikipedia.org/wiki/Machine_learning)-based methods
+* Automatic lookup of human names in [ORCID.org](https://orcid.org) (assuming ORCID id's are provided)
+* Automatic splitting of human names into family & given names using [ML](https://en.wikipedia.org/wiki/Machine_learning) methods
 * Support for InvenioRDM [communities](https://invenio-communities.readthedocs.io/en/latest/)
-* Support for overriding the metadata record that IGA creates, for complete control if you need it
+* Support for overriding the record that IGA creates, for complete control if you need it
 * Support for using the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in simple cases
 * Extensive use of logging so you can see what's going on under the hood
 
 
 ## Installation
 
-### As a standalone command-line program
+IGA can be installed as either (or both) a command-line program on your computer or a [GitHub Action](https://docs.github.com/en/actions) in a GitHub repository.
+
+### IGA as a standalone program
 
-There are multiple ways of installing IGA.  Please choose the alternative that suits you.
+Please choose an approach that suits your situation and preferences.
 
-#### _Alternative 1: installing IGA using `pipx`_
+<details><summary><h4><i>Alternative 1: using <code>pipx</code></i></h4></summary>
 
 [Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
 ```sh
 pipx install iga
 ```
 
 Pipx can also let you run IGA directly using `pipx run iga`, although in that case, you must always prefix every IGA command with `pipx run`.  Consult the [documentation for `pipx run`](https://github.com/pypa/pipx#walkthrough-running-an-application-in-a-temporary-virtual-environment) for more information.
+</details>
 
+<details><summary><h4><i>Alternative 2: using <code>pip</code></i></h4></summary>
 
-#### _Alternative 2: installing IGA using `pip`_
-
-You should be able to install `iga` with [`pip`](https://pip.pypa.io/en/stable/installing/) for Python&nbsp;3.  To install `iga` from the [Python package repository (PyPI)](https://pypi.org), run the following command:
+IGA is available from the [Python package repository PyPI](https://pypi.org) and can be installed using [`pip`](https://pip.pypa.io/en/stable/installing/):
 ```sh
 python3 -m pip install iga
 ```
 
-As an alternative to getting it from [PyPI](https://pypi.org), you can use `pip` to install `iga` directly from GitHub:
+As an alternative to getting it from [PyPI](https://pypi.org), you can install `iga` directly from GitHub:
 ```sh
 python3 -m pip install git+https://github.com/caltechlibrary/iga.git
 ```
 
 _If you already installed IGA once before_, and want to update to the latest version, add `--upgrade` to the end of either command line above.
+</details>
 
+<details><summary><h4><i>Alternative 3: from sources</i></h4></summary>
 
-#### _Alternative 3: installing IGA from sources_
-
-If  you prefer to install IGA directly from the source code, you can do that too. To get a copy of the files, you can clone the GitHub repository:
+If  you prefer to install IGA directly from the source code, first obtain a copy by either downloading the source archive from the [IGA releases page on GitHub](https://github.com/caltechlibrary/iga/releases), or by using `git` to clone the repository to a location on your computer. For example,
 ```sh
 git clone https://github.com/caltechlibrary/iga
 ```
 
-Alternatively, you can download the software source files as a ZIP archive directly from your browser using this link: <https://github.com/caltechlibrary/iga/archive/refs/heads/main.zip>
-
 Next, after getting a copy of the files,  run `setup.py` inside the code directory:
 ```sh
 cd iga
 python3 setup.py install
 ```
+</details>
+
+After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+```shell
+iga --help
+```
 
 
-### As a GitHub Action
+### IGA as a GitHub Action
 
-[...forthcoming...]
+A [GitHub Action](https://docs.github.com/en/actions) is a workflow that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
+
+1. In the main branch of your GitHub repository, create a `.github/workflows` directory
+2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/develop/sample-workflow.yml) into it:
+    ```yaml
+    name: InvenioRDM GitHub Archiver
+
+    env:
+      # 👋🏻 Set the next variable to your InvenioRDM server address 👋🏻
+      INVENIO_SERVER: https://your-invenio-server.org
+
+      # Set to an InvenioRDM record ID to mark releases as new versions.
+      parent_record: none
+
+      # The remaining variables are other IGA options. Please see the docs.
+      community:     none
+      draft:         false
+      all_assets:    false
+      all_metadata:  false
+      debug:         false
+
+    # ~~~~~~~~~~~~~~~~ The rest of this file should be left as-is. ~~~~~~~~~~~~~~~~
+
+    on:
+      release:
+        types: [published]
+      workflow_dispatch:
+        inputs:
+          release_tag:
+            description: "The release tag (empty = latest):"
+          draft:
+            default: false
+            description: "Mark the InvenioRDM record as a draft:"
+          parent_record:
+            description: "ID of parent record (for versioning):"
+          community:
+            description: "Name of InvenioRDM community (if any):"
+          all_assets:
+            default: false
+            description: "Attach all GitHub assets:"
+          all_metadata:
+            default: false
+            description: "Include additional GitHub metadata:"
+          debug:
+            default: false
+            description: "Print debug info in the GitHub log:"
+    jobs:
+      Send_to_InvenioRDM:
+        runs-on: ubuntu-latest
+        steps:
+          - uses: caltechlibrary/iga@main
+            with:
+              INVENIO_SERVER: ${{env.INVENIO_SERVER}}
+              INVENIO_TOKEN:  ${{secrets.INVENIO_TOKEN}}
+              all_assets:     ${{github.event.inputs.all_assets || env.all_assets}}
+              all_metadata:   ${{github.event.inputs.all_metadata || env.all_metadata}}
+              debug:          ${{github.event.inputs.debug || env.debug}}
+              draft:          ${{github.event.inputs.draft || env.draft}}
+              community:      ${{github.event.inputs.community || env.community}}
+              parent_record:  ${{github.event.inputs.parent_record || env.parent_record}}
+              release_tag:    ${{github.event.inputs.release_tag || 'latest'}}
+    ```
+3. **Edit the value of the `INVENIO_SERVER` variable (line 5 above)** ↑
+4. Optionally, change the values of other options (`parent_record`, `community`, etc.)
+5. Save the file, commit the changes to git, and push your changes to GitHub
 
 
 ## Quick start
 
-After a successful [installation](#installation) of IGA, here is how you can get started quickly.
+No matter whether IGA is run locally on your computer or as a GitHub Action, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one 
+is the first step.
 
-### Command-line use
+### Getting an InvenioRDM token
 
-If the [installation](#installation) process described above is successful, you should end up with a program named `iga` in a location where software is normally installed on your computer.  Running `iga` should be as simple as running any other command-line program. For example, the following command should print a helpful message to your terminal:
-```shell
-iga --help
-```
+<img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/get-invenio-pat.png" width="60%" align="right">
+
+1. Log in to your InvenioRDM account
+2. Go to the _Applications_ page in your account profile
+3. Click the <kbd>New token</kbd> button next to "Personal access tokens"
+4. On the page that is shown after you click that button, name your token (the name does not matter) and click the <kbd>Create</kbd> button
+5. After InvenioRDM creates and shows you the token, **copy it to a safe location** because InvenioRDM will not show it again
 
-IGA's main purpose is to create a metadata record in an InvenioRDM server and attach a GitHub release archive to the record. IGA needs 4 pieces of information to do its work, though for simple repositories you can often get by with just 3:
+### Configuring and running IGA locally
+
+To send a GitHub release to your InvenioRDM server, IGA needs this information:
 1. (Required) The identity of the GitHub release to be archived
 2. (Required) The address of the destination InvenioRDM server
-3. (Required) A Personal Access Token (PAT) for the InvenioRDM server
-4. (Optional) A Personal Access Token for GitHub
+3. (Required) A personal access token for InvenioRDM (from [above](#getting-an-inveniordm-token))
+4. (Optional) A [personal access token for GitHub](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
 
-The first one (the identity of the GitHub release) is given as arguments to IGA on the command line; the rest can be provided either via command-line options or by setting environment variables. A common way of configuring IGA is to set environment variables in your shell script or your interactive shell. Here is an example using Bash shell syntax, with realistic-looking but fake token values:
+The identity of the GitHub release is always given as an argument to IGA on the command line; the remaining values can be provided either via command-line options or environment variables. One approach is to set environment variables in shell scripts or your interactive shell. Here is an example using Bash shell syntax, with fake token values:
 ```shell
 export INVENIO_SERVER=https://data.caltech.edu
 export INVENIO_TOKEN=qKLoOH0KYf4D98PGYQGnC09hiuqw3Y1SZllYnonRVzGJbWz2
 export GITHUB_TOKEN=ghp_wQXp6sy3AsKyyEo4l9esHNxOdo6T34Zsthz
 ```
 
-Once these environment variables set in your shell, you can more easily invoke IGA. Usage can be as simple as providing a URL for a release in GitHub. For example:
+Once these are set, use of IGA can be as simple as providing a URL for a release in GitHub. For example, the following command creates a draft record (the `-d` option is short for `--draft`) for another project in GitHub and tells IGA to open (the `-o` option is short for `--open`) the newly-created InvenioRDM entry in a web browser:
 ```shell
-iga https://github.com/mhucka/taupe/releases/tag/v1.2.0
+iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
-If you give the option `--open` (or `-o` for short) to IGA, it will open the newly-created InvenioRDM entry in your default web browser when it's done:
-```shell
-iga -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
-```
+More options are described in the section on [detailed usage information](#usage) below.
 
-If you want the record to be only a draft and not a final version (perhaps so that you can inspect the result and edit it before finalizing it), use the option `--draft` (or `-d` for short):
-```shell
-iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
-```
 
-More options and examples can be found in the section on [detailed usage information](#usage) below.
+### Configuring and running IGA as a GitHub Action
+
+After doing the [GitHub Action installation](#as-a-github-action) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
+
+1. Go to the _Settings_ page of your GitHub repository<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-tabs.png" width="85%"></p>
+2. In the left-hand sidebar, find _Secrets and variables_ in the Security section, click on it to reveal _Actions_ underneath, then click on _Actions_<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-sidebar-secrets.png" width="40%"></p>
+3. In the next page, click the green <kbd>New repository secret</kbd> button<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-secrets.png" width="60%"></p>
+4. Name the variable `INVENIO_TOKEN` and paste in your InvenioRDM token
+5. Finish by clicking the green <kbd>Add secret</kbd> button
+
+#### Testing the workflow
+
+After setting up the workflow and storing the InvenioRDM token in your repository on GitHub, it's a good idea to run the workflow manually to test that it works as expected.
+
+1. Go to the _Actions_ tab in your repository and click on the name of the workflow in the sidebar on the left<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-run-workflow.png" width="90%"></p>
+2. Click the <kbd>Run workflow</kbd> button in the right-hand side of the blue strip
+3. In the pull-down, change the value of "Mark the record as a draft" to `true`<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-workflow-options-circled.png" width="40%"></p>
+4. Click the green <kbd>Run workflow</kbd> button near the bottom
+5. Refresh the web page and a new line will be shown named after your workflow file<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-running-workflow.png" width="90%"></p>
+6. Click the title of the workflow to see the IGA workflow progress and results
 
 
-### GitHub Action use
+#### Running the workflow when releasing software
 
-[...forthcoming...]
+Once the personal access token from InvenioRDM is stored as a GitHub secret, the workflow should run automatically every time a new release is made on GitHub &ndash; no further action should be needed. You can check the results (and look for errors if something went wrong) by going to the _Actions_ tab in your GitHub repository.
 
 
 ## Usage
 
 This section provides detailed information about IGA's operation and options to control it.
 
 ### Identifying the InvenioRDM server
 
 The server address must be provided either as the value of the option `--invenio-server` or in an environment variable named `INVENIO_SERVER`.  If the server address does not begin with `https://`, IGA will prepend it automatically.
 
 ### Providing an InvenioRDM access token
 
-A Personal Access Token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
+A personal access token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
 
 To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
 
 ### Providing a GitHub access token
 
-It is possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for many repositories, IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some repositories IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+
+Note that when you run IGA as a GitHub Action, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Action workflow.
 
 ### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
  1. The full URL of the web page on GitHub of a tagged release. In this case,
     the URL must be the final argument on the command line invocation of IGA
     and the options `--account` and `--repo` must be omitted.
@@ -228,17 +342,17 @@
 
 ### Other options recognized by IGA
 
 Running IGA with the option `--save-metadata` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-metadata` to save a record to a file, edit the result, then finally run IGA with the `--read-metadata` option to use the modified record to create a release in the InvenioRDM server.
 
 The `--mode` option can be used to change the run mode. Four run modes are available: `quiet`, `normal`, `verbose`, and `debug`. The default mode is `normal`, in which IGA prints a few messages while it's working. The mode `quiet` will make it avoid printing anything unless an error occurs, the mode `verbose` will make it print a detailed trace of what it is doing, and the mode `debug` will make IGA even more verbose. In addition, in `debug` mode, IGA will drop into the `pdb` debugger if it encounters an exception during execution. On Linux and macOS, debug mode also installs a signal handler on signal USR1 that causes IGA to drop into the `pdb` debugger if the signal USR1 is received. (Use `kill -USR1 NNN`, where NNN is the IGA process id.)
 
-Networks latencies are unpredicatable. Reading and writing large files may take a long time; on the other hand, IGA should not wait forever before reporting an error if a server or network becomes unresponsive. To balance these conflicting needs, IGA automatically scales its network timeout based on file sizes. To override its adaptive algorithm and set an explicit timeout value, use the option `--timeout` with a value in seconds.
+By default, informational output is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` (i.e., a dash) to indicate console output, or it can be a file path to send the output to the file. A special exception is that even if a log destination is given, IGA will still print the final record URL to stdout.  This makes it possible to invoke IGA from scripts that capture the record URL while still saving diagnostic output in case debugging is needed.
 
-By default, the output of the `verbose` and `debug` run modes is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` to indicate console output, or a file path to send the output to the file.
+Reading and writing large files may take a long time; on the other hand, IGA should not wait forever on network operations before reporting an error if a server or network becomes unresponsive. To balance these conflicting needs, IGA automatically scales its network timeout based on file sizes. To override its adaptive algorithm and set an explicit timeout value, use the option `--timeout` with a value in seconds.
 
 If given the `--version` option, this program will print its version and other information, and exit without doing anything else.
 
 Running IGA with the option `--help` will make it print help text and exit without doing anything else.
 
 ### Summary of command-line options
 
@@ -249,15 +363,15 @@
 | `--all-assets`         | `-A`     | Attach all GitHub assets | Attach only the release source ZIP| |
 | `--all-metadata`       | `-M`     | Include additional metadata from GitHub | Favor CodeMeta & CFF | |
 | `--community` _C_      | `-c` _C_ | Submit record to RDM community _C_ | Don't submit record to any community | | 
 | `--draft`              | `-d`     | Mark the RDM record as a draft | Publish record when done | |
 | `--file` _F_           | `-f` _F_ | Upload local file _F_ instead of GitHub assets | Upload only GitHub assets | ⚑ |
 | `--github-account` _A_ | `-a` _A_ | Look in GitHub account _A_ | Get account name from release URL | ✯ | 
 | `--github-repo` _R_    | `-r` _R_ | Look in GitHub repository _R_ of account _A_ | Get repo name from release URL | ✯ |
-| `--github-token` _T_   | `-t` _T_ | Use GitHub acccess token _T_| Use value in env. var. `GITHUB_TOKEN` | |
+| `--github-token` _T_   | `-t` _T_ | Use GitHub access token _T_| Use value in env. var. `GITHUB_TOKEN` | |
 | `--help`               | `-h`     | Print help info and exit | | |
 | `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
 | `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
 | `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
@@ -280,20 +394,24 @@
 |:----:|----------------------------------------------------------|
 | 0    | success &ndash; program completed normally               |
 | 1    | interrupted                                              |
 | 2    | encountered a bad or missing value for an option         |
 | 3    | encountered a problem with a file or directory           |
 | 4    | encountered a problem interacting with GitHub            |
 | 5    | encountered a problem interacting with InvenioRDM        |
-| 6    | an exception or fatal error occurred                     |
+| 6    | the personal access token was rejected                   |
+| 7    | an exception or fatal error occurred                     |
 
 
 ## Known issues and limitations
 
-_[… forthcoming …]_
+The following are known issues and limitations.
+* As of mid-2023, InvenioRDM requires names of record creators and other contributors to be split into given (first) and family (surname). This is problematic for multiple reasons. The first is that mononyms are common in many countries: a person's name may legitimately be only a single word which is not conceptually a "given" or "family" name.  To compound the difficulty for IGA, names are stored as single fields in GitHub account metadata, so unless a repository has a `codemeta.json` or `CITATION.cff` file (which allow authors more control over how they want their names represented), IGA is forced to try to split the single GitHub name string into two parts. _A foolproof algorithm for doing this does not exist_, so IGA will sometimes get it wrong. (That said, IGA goes to extraordinary lengths to try to do a good job.)
+* Some accounts on GitHub are software automation or "bot" accounts but are not labeled as such. These accounts are generally indistinguishable from human accounts on GitHub. If such an account is the creator of a release in GitHub, and IGA has to use its name-splitting algorithm on the name of the account, it may produce a nonsensical result. For example, it might turn "Travis CI" into an entry with a first name of "Travis" and last name of "CI". 
+
 
 ## Getting help
 
 If you find an issue, please submit it in [the GitHub issue tracker](https://github.com/caltechlibrary/iga/issues) for this repository.
 
 
 ## Contributing
@@ -322,38 +440,44 @@
 * [humanize](https://github.com/jmoiron/humanize) &ndash; make numbers more easily readable by humans
 * [idutils](https://github.com/inveniosoftware/idutils) &ndash; package for validating and normalizing various kinds of persistent identifiers
 * [ipdb](https://github.com/gotcha/ipdb) &ndash; the IPython debugger
 * [iptools](https://github.com/bd808/python-iptools) &ndash; utilities for dealing with IP addresses
 * [isbnlib](https://github.com/xlcnd/isbnlib) &ndash; utilities for dealing with ISBNs
 * [json5](https://github.com/dpranke/pyjson5) &ndash; extended JSON format parser
 * [latexcodec](https://github.com/mcmtroffaes/latexcodec) &ndash; lexer and codec to work with LaTeX code in Python
+* [linkify-it-py](https://github.com/tsutsu3/linkify-it-py) &ndash; a link recognition library with full unicode support
 * [lxml](https://lxml.de) &ndash; an XML parsing library
 * [Markdown](https://python-markdown.github.io) &ndash; Python package for working with Markdown
 * [markdown-checklist](https://github.com/FND/markdown-checklist) &ndash; GitHub-style checklist extension for Python Markdown package
 * [mdx-breakless-lists](https://github.com/adamb70/mdx-breakless-lists) &ndash; GitHub-style Markdown lists that don't require a line break above them
 * [mdx_linkify](https://github.com/daGrevis/mdx_linkify) &ndash; extension for Python Markdown will convert text that look like links to HTML anchors
+* [MyST-parser](https://github.com/executablebooks/MyST-Parser) &ndash; A Sphinx and Docutils extension to parse an extended version of Markdown
 * [nameparser](https://github.com/derek73/python-nameparser) &ndash; package for parsing human names into their individual components
 * [probablepeople](https://github.com/datamade/probablepeople) &ndash; package for parsing names into components using ML-based techniques
-* [pymdown-extensions](https://github.com/facelessuser/pymdown-extensions) &ndash; extensions for Python Markdown
-* [PyYAML](https://pyyaml.org) &ndash; YAML parser
 * [pybtex](https://pybtex.org) &ndash; BibTeX parser and formatter
 * [pybtex-apa7-style]() &ndash; plugin for [pybtex](https://pybtex.org) that provides APA7 style formatting
+* [pymdown-extensions](https://github.com/facelessuser/pymdown-extensions) &ndash; extensions for Python Markdown
 * [pytest](https://docs.pytest.org/en/stable/) &ndash; testing framework
 * [pytest-cov](https://github.com/pytest-dev/pytest-cov) &ndash; coverage reports for use with `pytest`
 * [pytest-mock](https://pypi.org/project/pytest-mock/) &ndash; wrapper around the `mock` package for use with `pytest`
+* [PyYAML](https://pyyaml.org) &ndash; YAML parser
 * [Rich](https://github.com/Textualize/rich) &ndash; library for writing styled text to the terminal
 * [rich-click](https://github.com/ewels/rich-click) &ndash; CLI interface built on top of [Rich](https://github.com/Textualize/rich)
+* [setuptools](https://github.com/pypa/setuptools) &ndash; library for `setup.py`
 * [Sidetrack](https://github.com/caltechlibrary/sidetrack) &ndash; simple debug logging/tracing package
 * [spaCy](https://spacy.io) &ndash; Natural Language Processing package
 * [spacy-alignments](https://github.com/explosion/spacy-alignments) &ndash; alternate alignments for [spaCy](https://spacy.io)
 * [spacy-legacy](https://pypi.org/project/spacy-legacy/) &ndash; [spaCy](https://spacy.io) legacy functions and architectures for backwards compatibility
 * [spacy-loggers](https://github.com/explosion/spacy-loggers) &ndash; loggers for [spaCy](https://spacy.io)
 * [spacy-pkuseg](https://github.com/explosion/spacy-pkuseg) &ndash; Chinese word segmentation toolkit for [spaCy](https://spacy.io)
 * [spacy-transformers](https://spacy.io) &ndash; pretrained Transformers for [spaCy](https://spacy.io)
-* [setuptools](https://github.com/pypa/setuptools) &ndash; library for `setup.py`
+* [Sphinx](https://www.sphinx-doc.org/en/master/) &ndash; documentation generator for Python
+* [sphinx-autobuild](https://pypi.org/project/sphinx-autobuild/) &ndash; rebuild Sphinx docs automatically
+* [sphinx-material](https://bashtage.github.io/sphinx-material/) &ndash; a responsive Material Design theme for Sphinx
+* [sphinxcontrib-mermaid](https://github.com/mgaitan/sphinxcontrib-mermaid) &ndash; support Mermaid diagrams in Sphinx docs
 * [StringDist](https://github.com/obulkin/string-dist) &ndash; library for calculating string distances
 * [Twine](https://github.com/pypa/twine) &ndash; utilities for publishing Python packages on [PyPI](https://pypi.org)
 * [url-normalize](https://github.com/niksite/url-normalize) &ndash; URI/URL normalization utilities
 * [validators](https://github.com/kvesteri/validators) &ndash; data validation package for Python
 * [wheel](https://pypi.org/project/wheel/) &ndash; setuptools extension for building wheels
 
 <div align="center">
```

### Comparing `iga-0.0.9/iga/__init__.py` & `iga-1.0.0/iga/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # .............................................................................
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '0.0.9'
+__version__     = '1.0.0'
 __description__ = 'InvenioRDM GitHub Archiver'
 __url__         = 'https://github.com/caltechlibrary/iga'
 __author__      = 'Michael Hucka'
 __email__       = 'helpdesk@library.caltech.edu'
 __license__     = 'https://github.com/caltechlibrary/iga/blob/main/LICENSE'
```

### Comparing `iga-0.0.9/iga/__main__.py` & `iga-1.0.0/iga/__main__.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/iga/cli.py` & `iga-1.0.0/iga/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from iga.id_utils import is_invenio_rdm
 from iga.invenio import (
     invenio_api_available,
     invenio_communities,
     invenio_community_send,
     invenio_create,
     invenio_publish,
+    invenio_server_name,
+    invenio_token_valid,
     invenio_upload,
 )
 
 
 # Main command-line interface.
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -58,15 +60,16 @@
 
 # Callback functions used in click interface ..................................
 
 def _config_mode(ctx, param, mode):
     '''Handle the --mode option and configure the run mode as needed.'''
     os.environ['IGA_RUN_MODE'] = mode or 'normal'
     if mode in ['verbose', 'debug']:
-        set_debug(True)
+        dest = os.environ.get('IGA_LOG_DEST') or '-'
+        set_debug(True, dest, show_package=True)
     if mode == 'debug':
         import faulthandler
         faulthandler.enable()
         if os.name != 'nt':                 # Can't use next part on Windows.
             import signal
             from boltons.debugutils import pdb_on_signal
             pdb_on_signal(signal.SIGUSR1)
@@ -82,18 +85,15 @@
         # The user almost certainly typed "-log" instead of "--log".
         _alert(ctx, 'No such option: `-log`. Did you mean `--log`?')
         sys.exit(int(ExitCode.bad_arg))
     elif log_dest.name == '<stdout>':
         dest = '-'
     else:
         dest = log_dest.name
-
-    if os.environ.get('IGA_RUN_MODE') in ['verbose', 'debug']:
-        set_debug(True, dest)
-        os.environ['IGA_LOG_DEST'] = dest
+    os.environ['IGA_LOG_DEST'] = dest
     return dest
 
 
 def _read_param_value(ctx, param, value, env_var, thing, required=True):
     '''Handle reading a CLI argument.
 
     If a value is passed on the command line, the environment variable
@@ -168,23 +168,30 @@
             from validators import domain
             if domain(server):
                 server = 'https://' + server
             else:
                 _alert(ctx, f'The given InvenioRDM server address ({server})'
                        ' does not appear to be a valid host or IP address.')
                 sys.exit(int(ExitCode.bad_arg))
-    # Test that the server responds to the API & simultaneously get its name.
-    if name := invenio_api_available(server):
-        os.environ['INVENIO_SERVER_NAME'] = name
-        log(f'will use {name} as the InvenioRDM publisher name')
-    else:
+    if not invenio_api_available(server):
         _alert(ctx, f'The server address ({server}) does not appear to be'
                ' reacheable or does not support the InvenioRDM API.')
         sys.exit(int(ExitCode.bad_arg))
-    log(f'will use {server} as the InvenioRDM server address')
+    if not invenio_token_valid(server):
+        _alert(ctx, f'The personal access token was rejected by {server}.')
+        sys.exit(int(ExitCode.bad_token))
+    if name := invenio_server_name(server):
+        os.environ['INVENIO_SERVER_NAME'] = name
+        log(f'using {name} as the InvenioRDM publisher name')
+    else:
+        from commonpy.network_utils import hostname
+        host_part = hostname(server)
+        os.environ['INVENIO_SERVER_NAME'] = host_part
+        log(f'unable to get a publisher name from the server; using {host_part}')
+    log(f'using {server} as the InvenioRDM server address')
     os.environ['INVENIO_SERVER'] = server
     return result
 
 
 def _read_timeout(ctx, param, value):
     '''Read the timeout value and perform some basic checks on it.'''
     if result := _read_param_value(ctx, param, value, 'IGA_NETWORK_TIMEOUT',
@@ -213,30 +220,51 @@
 def _print_help_and_exit(ctx):
     '''Print the help text and exit with a success code.'''
     click.echo(ctx.get_help())
     sys.exit(int(ExitCode.success))
 
 
 def _print_text(text, color='turquoise4', end='\n', wrap=True):
-    import shutil
-    width = (shutil.get_terminal_size().columns - 2) or 78
-    if wrap:
-        from textwrap import wrap
-        text = '\n'.join(wrap(text, width=width))
-    console = Console(width=width)
-    console.print(text, style=color, end=end, highlight=False)
+    '''Print text to the console.
+
+    If quiet mode is in effect or the log destination is not stdout, this does
+    not print output to the console.
+    '''
+    log(text)
+    if os.environ.get('IGA_RUN_MODE') == 'quiet':
+        return
+    if os.environ.get('IGA_LOG_DEST', '-') == '-':
+        import shutil
+        width = (shutil.get_terminal_size().columns - 2) or 78
+        if wrap:
+            from textwrap import wrap
+            text = '\n'.join(wrap(text, width=width))
+        console = Console(width=width)
+        console.print(text, style=color, end=end, highlight=False)
+    else:
+        with open(os.environ.get('IGA_LOG_DEST'), 'a') as dest:
+            console = Console(file=dest)
+            console.print(text)
 
 
 def _alert(ctx, msg, print_usage=True):
     '''Print an error message in the style of rich_click.
+
     This is meant to be used when reporting errors involving UI options, in
-    situations where rich_click's own error reporting can't be used directly.'''
+    situations where rich_click's own error reporting can't be used directly.
+    '''
+    if (os.environ.get('IGA_RUN_MODE') not in ['debug', 'verbose']
+            and os.environ.get('IGA_LOG_DEST') not in ['-', None]):
+        with open(os.environ.get('IGA_LOG_DEST'), 'a') as dest:
+            console = Console(file=dest)
+            console.print('Error: ' + msg)
+    else:
+        log('error: ' + msg)
     # The following code tries to emulate what rich_click does. It doesn't use
     # private methods or properties, but it might break if rich_click changes.
-    log('error: ' + msg)
     from rich.markdown import Markdown
     from rich.padding import Padding
     from rich.panel import Panel
     from rich.theme import Theme
     from rich_click.rich_click import (
         ALIGN_ERRORS_PANEL,
         ERRORS_PANEL_TITLE,
@@ -264,27 +292,33 @@
             title=ERRORS_PANEL_TITLE,
             title_align=ALIGN_ERRORS_PANEL,
         )
     )
 
 
 def _inform(text, end='\n'):
-    log('[inform] ' + text)
-    # Detect URLs are convert them into Rich links.
+    '''Print an informative message to the console.'''
+    # Detect URLs and convert them into Rich links.
     if contains_url := ('http' in text):
         import re
         if match := re.search(r'(https?://\S+)', text):
             ustart, uend = match.start(), match.end()
             url = text[ustart:uend]
             text = text[:ustart] + '[link=' + url + ']' + url + '[/]' + text[uend:]
-    if os.environ.get('IGA_RUN_MODE') != 'quiet':
-        _print_text(text, 'turquoise4', end=end, wrap=(not contains_url))
+    _print_text(text, 'turquoise4', end=end, wrap=(not contains_url))
+
+
+def _quiet_or_redirected():
+    '''Return true if the run mode is 'quiet' or the log dest is not '-'.'''
+    return (os.environ.get('IGA_RUN_MODE') == 'quiet'
+            or os.environ.get('IGA_LOG_DEST', '-') not in ['-', None])
 
 
 def _list_communities(ctx, param, value):
+    '''Get the list of InvenioRDM communities and print them to the console.'''
     if not value:
         return
     from rich import box
     from rich.table import Table
     server = os.environ.get('INVENIO_SERVER', '')
     table = Table(title=f'Communities available at server {server}',
                   pad_edge=True, box=box.MINIMAL_DOUBLE_HEAD, expand=True)
@@ -517,51 +551,59 @@
 InvenioRDM API for record versioning. The newly-created record will be linked
 to a parent record identified by the value passed to `--parent-record`. The
 value must be either an InvenioRDM record identifier (which is a sequence of
 alphanumeric characters of the form _XXXXX-XXXXX_, such as `bknz4-bch35`,
 generated by the InvenioRDM server), or a URL to the landing page of the record
 in the InvenioRDM server. (Such URLs contain an embedded record identifier.)
 Here is an example of using this option:
-```
+```shell
   iga --parent-record xbcd4-efgh5 https://github.com/foo/bar/releases/tag/v1
 ```
 \r
 _**Other options recognized by IGA**_
 \r
 Running IGA with the option `--save-record` will make it create a metadata
 record, but instead of uploading the record (and any assets) to the InvenioRDM
 server, IGA will write the result to the given destination. This can be useful
 not only for debugging but also for creating a starting point for a custom
 metadata record: first run IGA with `--save-record` to save a record to a file,
 edit the result, then finally run IGA with the `--read-record` option to use
 the modified record to create a release in the InvenioRDM server.
 \r
-The `--mode` option can be used to change the run mode. Four run modes are
-available: `quiet`, `normal`, `verbose`, and `debug`. The default mode is
-`normal`, in which IGA prints a few messages while it's working. The mode
-`quiet` will make it avoid printing anything unless an error occurs, the mode
-`verbose` will make it print a detailed trace of what it is doing, and the
-mode `debug` will make IGA even more verbose. In addition, in `debug` mode,
-IGA will drop into the `pdb` debugger if it encounters an exception during
-execution. On Linux and macOS, debug mode also installs a signal handler on
-signal USR1 that causes IGA to drop into the `pdb` debugger if the signal
-USR1 is received. (Use `kill -USR1 NNN`, where NNN is the IGA process id.)
+The `--mode` option can be used to change the amount of diagnostic output. Four
+modes are available: `quiet`, `normal`, `verbose`, and `debug`. The default is
+`normal`, in which IGA prints only a few messages while it's working. The mode
+`quiet` will make IGA avoid printing anything except the final record URL
+unless an error occurs, the mode `verbose` will make it print a detailed trace
+of what it is doing, and the mode `debug` will make IGA even more verbose. In
+addition, in `debug` mode, IGA will drop into the `pdb` debugger if it
+encounters an exception during execution. On Linux and macOS, debug mode also
+installs a signal handler on signal USR1 that causes IGA to drop into the `pdb`
+debugger if the signal USR1 is received. (Use `kill -USR1 NNN`, where NNN is
+the IGA process id.)
+\r
+By default, the output of the `normal`, `verbose`, and `debug` run modes is
+sent to the standard output (normally the terminal console). The option
+`--log-dest` can be used to send the output to the given destination
+instead. The value can be "`-`" to indicate console output, or a file path to
+send the output to the file. A special exception is that even if a log
+destination is given, IGA will still print the final record URL to stdout.
+This makes it possible to invoke IGA from scripts that capture the record URL
+while still saving diagnostic output in case debugging is needed. E.g.,
+```shell
+  record_url=`iga --mode verbose --log-dest iga.out ....`
+```
 \r
 Networks latencies are unpredicatable. Reading and writing large files may take
 a long time; on the other hand, IGA should not wait forever before reporting an
 error if a server or network becomes unresponsive. To balance these conflicting
 needs, IGA automatically scales its network timeout based on file sizes. To
 override its adaptive algorithm and set an explicit timeout value, use the
 option `--timeout` with a value in seconds.
 \r
-By default, the output of the `verbose` and `debug` run modes is sent to the
-standard output (normally the terminal console). The option `--log-dest` can
-be used to send the output to the given destination instead. The value can be
-`-` to indicate console output, or a file path to send the output to the file.
-\r
 If given the `--version` option, this program will print its version and other
 information, and exit without doing anything else.
 \r
 Running IGA with the option `--help` will make it print help text and exit
 without doing anything else.
 \r
 _**Return values**_
@@ -572,15 +614,16 @@
 \r
   0 = success – program completed normally  
   1 = interrupted  
   2 = encountered a bad or missing value for an option  
   3 = encountered a problem with a file or directory  
   4 = encountered a problem interacting with GitHub  
   5 = encountered a problem interacting with InvenioRDM  
-  6 = an exception or fatal error occurred  
+  6 = the personal access token was rejected  
+  7 = an exception or fatal error occurred  
 '''
     # Process arguments & handle early exits ..................................
 
     if url_or_tag == 'help':  # Detect if the user typed "help" without dashes.
         _print_help_and_exit(ctx)
     elif url_or_tag.startswith('http'):
         if any([account, repo]):
@@ -651,28 +694,27 @@
             _inform('Sending metadata to InvenioRDM server', end='...')
             record = invenio_create(metadata, parent_id)
             _inform(' done.')
 
             _inform('Attaching assets:')
             for item in files_to_upload or github_assets:
                 invenio_upload(record, item, _print_text)
-            _inform('Done.')
 
             if draft:
                 _inform(f'The draft record is available at {record.draft_url}')
             elif community:
                 invenio_community_send(record, community)
                 _inform(f'The record has been submitted to community "{community}"'
                         f' and the draft is available at {record.draft_url}')
             else:
                 invenio_publish(record)
                 _inform(f'The published record is available at {record.record_url}')
 
-            if os.environ.get('IGA_RUN_MODE') == 'quiet':
-                # Quiet mode => nothing else is printed, so tell user this much.
+            if _quiet_or_redirected():
+                # If no other output is printed, we still print the URL.
                 click.echo(record.record_url or record.draft_url)
             if open_in_browser:
                 log(f'opening {record.record_url or record.draft_url}')
                 click.launch(record.record_url or record.draft_url)
     except KeyboardInterrupt:
         log('keyboard interrupt received')
         exit_code = ExitCode.user_interrupt
```

### Comparing `iga-0.0.9/iga/data_utils.py` & `iga-1.0.0/iga/data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/iga/doi.py` & `iga-1.0.0/iga/doi.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/iga/exceptions.py` & `iga-1.0.0/iga/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     '''GitHub returned an error.'''
 
 
 class InvenioRDMError(IGAException):
     '''InvenioRDM returned an error.'''
 
 
+class BadToken(IGAException):
+    '''Invalid personal access token.'''
+
+
 class MissingData(IGAException):
     '''Could not obtain all the required data to create an InvenioRDM record.'''
 
 
 class RecordNotFound(IGAException):
     '''Could not find the requested record in the InvenioRDM server.'''
```

### Comparing `iga-0.0.9/iga/exit_codes.py` & `iga-1.0.0/iga/exit_codes.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,11 +28,12 @@
 
     success          = 0, "success – program completed normally"
     user_interrupt   = 1, "the user interrupted the program's execution"
     bad_arg          = 2, "encountered a bad or missing value for an option"
     file_error       = 3, "encountered a problem with a file or directory"
     github_error     = 4, "encountered a problem interacting with GitHub"
     inveniordm_error = 5, "encountered a problem interacting with InvenioRDM"
-    exception        = 6, "a miscellaneous exception or fatal error occurred"
+    bad_token        = 6, "the personal access token was rejected"
+    exception        = 7, "a miscellaneous exception or fatal error occurred"
 
     def __int__(self):
         return self.value
```

### Comparing `iga-0.0.9/iga/github.py` & `iga-1.0.0/iga/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,18 +139,33 @@
     release = github_release(account_name, repo_name, tag_name)
     assets = [release.zipball_url]
     if get_all:
         log('option to get all assets is in effect')
         assets.append(release.tarball_url)
         for asset in release.assets:
             assets.append(asset.browser_download_url)
+
     log(f'found {len(assets)} assets for release "{tag_name}"')
     return assets
 
 
+def github_asset_contents(asset_url):
+    '''Return the raw contents of a release asset file.'''
+    try:
+        response = _github_get(asset_url)
+        return response.content
+    except KeyboardInterrupt:
+        raise
+    except commonpy.exceptions.CommonPyException:
+        raise GitHubError(f'Failed to download GitHub asset at {asset_url}'
+                          ' – either it does not exist or it is inaccessible.')
+    except Exception:
+        raise
+
+
 def github_repo_filenames(repo, tag_name):
     '''Return a list of file information objects for the given repo object.
 
     The tag_name must be a release tag, and is used to find the version of
     the repository corresponding to that tag.
     '''
     if getattr(repo, '_filenames', None):
@@ -332,15 +347,15 @@
     except Exception as ex:
         # Something unexpected happened. We need to fix our handling.
         log('Error: ' + str(ex))
         raise InternalError('Encountered error trying to unpack GitHub data.')
 
 
 def _github_get(endpoint):
-    headers = {'Accept': 'application/vnd.github.v3+json'}
+    headers = {'Accept': 'application/vnd.github+json'}
     using_token = 'GITHUB_TOKEN' in os.environ
     if using_token:
         headers['Authorization'] = f'token {os.environ["GITHUB_TOKEN"]}'
     try:
         response = network('get', endpoint, headers=headers)
         return response                 # noqa PIE787
     except KeyboardInterrupt:
```

### Comparing `iga-0.0.9/iga/id_utils.py` & `iga-1.0.0/iga/id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/iga/invenio.py` & `iga-1.0.0/iga/invenio.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This file is part of https://github.com/caltechlibrary/iga/.
 
 Copyright (c) 2022-2023 by the California Institute of Technology.  This code
 is open-source software released under a BSD-type license.  Please see the
 file "LICENSE" for more information.
 '''
 
-from   commonpy.network_utils import network, netloc
+from   commonpy.network_utils import net, network, netloc
 from   commonpy.data_utils import pluralized
 import commonpy.exceptions
 from   dataclasses import dataclass
 from   functools import partial, cache
 import json
 from   sidetrack import log
 import socket
@@ -21,14 +21,15 @@
 
 import iga
 from   iga.exceptions import (
     InternalError,
     InvenioRDMError,
     RecordNotFound,
 )
+from   iga.github import github_asset_contents
 from   iga.id_utils import normalize_invenio_rdm
 
 
 # Exported data structures.
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 @dataclass
@@ -58,15 +59,41 @@
     title : str                        # The metadata['title'] value
 
 
 # Exported module functions.
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 def invenio_api_available(server_url):
-    '''Return the name of the INVENIO_SERVER if it responds to API calls.'''
+    '''Return True if the server at server_url responds to the InvenioRDM API.'''
+    # There is no 'status' or similarly simple API test endpoint for InvenioRDM,
+    # so to test that the destination is actually an InvenioRDM server, the
+    # approach here is to do some kind of minimum call that requires the API.
+    return bool(invenio_server_name(server_url))
+
+
+def invenio_token_valid(server_url):
+    '''Return True if the token in env variable INVENIO_TOKEN is valid.'''
+    # Testing things ahead of time is a Python anti-pattern, but in interactive
+    # programs (and especially ones that run as GHAs) we don't want to get far
+    # into the work before discovering we won't be able to upload the result.
+    try:
+        return bool(_invenio('get', endpoint='/api/users?size=1',
+                             msg='confirm InvenioRDM token is valid'))
+    except KeyboardInterrupt:
+        raise
+    except commonpy.exceptions.AuthenticationFailure:
+        return False
+    except Exception as ex:             # noqa PIE786
+        log('exception while testing the InvenioRDM token: ' + str(ex))
+        return False
+
+
+@cache
+def invenio_server_name(server_url):
+    '''Return the name of server at server_url if it responds to API calls.'''
     server_host = netloc(server_url)
     endpoint = '/api/records?size=1'
     try:
         log(f'testing if we can reach {server_url} in 5 sec or less')
         socket.setdefaulttimeout(5)
         # If the next one can't reach the host, it'll throw an exception.
         socket.socket(socket.AF_INET, socket.SOCK_STREAM).connect((server_host, 443))
@@ -76,22 +103,26 @@
             data = response.json()
             record = data.get('hits', {}).get('hits', {})[0]
             return record['metadata']['publisher']
     except KeyboardInterrupt:
         raise
     except socket.error:
         log(f'{server_url} did not respond')
-        return False
+        return None
+    except json.decoder.JSONDecodeError:
+        log(f'{server_url} exists but does not recognize the InvenioRDM API')
+        return None
     except commonpy.exceptions.CommonPyException as ex:
         log(f'trying to get {server_url}{endpoint} produced an error: ' + str(ex))
-        return False
-    except Exception:
+        return None
+    except Exception as ex:
+        log(f'unexpected exception accessing {server_url}{endpoint}: ' + str(ex))
         raise
     log(f'failed to reach server {server_url}')
-    return False
+    return None
 
 
 def invenio_get(record_id):
     '''Get the InvenioRDM record with the given identifier.'''
     log(f'asking InvenioRDM server for record {record_id}')
     record_id = normalize_invenio_rdm(record_id)
     result = _invenio('get', endpoint=f'/api/records/{record_id}',
@@ -167,26 +198,16 @@
     # Start by reading the assets to be sure we can actually get them, *before*
     # trying to upload them to InvenioRDM.
     import humanize
     size = ''
     if asset.startswith('http'):
         filename = _filename_from_asset_url(asset)
         print_status(f' - Downloading [bold]{filename}[/] from GitHub', end='...')
-        try:
-            response = network('get', asset)
-        except KeyboardInterrupt:
-            raise
-        except commonpy.exceptions.CommonPyException:
-            raise InvenioRDMError(f'Failed to download GitHub asset {asset} and'
-                                  ' therefore cannot attach it to the record.')
-        except Exception:
-            raise
-
+        content = github_asset_contents(asset)
         print_status('done')
-        content = response.content
         size = humanize.naturalsize(len(content))
         log(f'downloaded {size} bytes of {asset}')
     else:
         filename = path.basename(asset)
         content = None
         print_status(f' - Reading [bold]{filename}[/]', end='...')
         with open(asset, 'rb') as file:
@@ -332,37 +353,46 @@
     client = None
     if action == 'put':
         # 'put' => data is being uploaded, so we need to set longer timeouts.
         import httpx
         tmout = _network_timeout(data)
         timeout = httpx.Timeout(tmout, connect=10, read=tmout, write=tmout)
         client = httpx.Client(timeout=timeout, http2=True, verify=False)
-    api_call = partial(network, action, url, client=client, headers=headers)
+    api_call = partial(net, action, url, client=client, headers=headers)
 
     # Now perform the actual network api call.
     try:
         if data:
             log(f'data payload size = {len(data)}')
             if data_type == 'json':
-                response = api_call(json=data)
+                response, error = api_call(json=data)
             else:
-                response = api_call(content=data)
+                response, error = api_call(content=data)
         else:
-            response = api_call()
+            response, error = api_call()
+        if error:
+            raise error
         response_json = response.json()
         if os.environ.get('IGA_RUN_MODE') == 'debug':
             log(f'got response:\n{json.dumps(response_json, indent=2)}')
         return response_json
     except KeyboardInterrupt:
         raise
     except commonpy.exceptions.NoContent:
         log(f'got no content for {endpoint}')
         return None
     except commonpy.exceptions.CommonPyException as ex:
-        raise InvenioRDMError(f'Failed to {msg}: {str(ex)}')
+        # Invenio responds w/ code 400 if the token is invalid but the msg in
+        # the response ("Referer checking failed") is confusing. Let's do better.
+        if response.status_code == 400:
+            raise InvenioRDMError(f'Failed to {msg}. The server rejected the'
+                                  ' request, possibly because of an invalid'
+                                  ' InvenioRDM token.')
+        else:
+            raise InvenioRDMError(f'Failed to {msg}. {str(ex).capitalize()}')
     except Exception:
         raise
 
 
 def _network_timeout(data):
     '''Return a timeout value (in seconds) for writing the given data string.
```

### Comparing `iga-0.0.9/iga/json_utils.py` & `iga-1.0.0/iga/json_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/iga/licenses.py` & `iga-1.0.0/iga/licenses.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/iga/metadata.py` & `iga-1.0.0/iga/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,14 +278,17 @@
     # We don't want to add repeated text, so we track what we have seen. Start
     # with the text we put in the InvenioRDM "description" field.
     added = [description(repo, release, include_all, internal_call=True).lower()]
 
     # Helper functions used in what follows next. All of the fields we use
     # below are supposed to be strings or URLs, per the CodeMeta & CFF specs.
     def add(item, role, summary):
+        if item is None:
+            log(f'not using {summary} because it\'s empty')
+            return
         if item and not isinstance(item, str):
             log(f'not using {summary} because it\'s not the expected data type')
             return
         item = item.strip()
         if not item:
             return
         elif item.lower() in added:
@@ -571,17 +574,17 @@
     if text:
         if internal_call:
             return text.strip()
         else:
             log(f'adding {value_name} as "description"')
             return html_from_md(text.strip())
 
-    # Bummer.
+    # Bummer. Invenio won't accept an empty string, so we have to put something.
     log('could not find a usable value for the "description" field')
-    return ''
+    return '(No description provided.)'
 
 
 def formats(repo, release, include_all):
     '''Return InvenioRDM "formats".
     https://inveniordm.docs.cern.ch/reference/metadata/#formats-0-n
     '''
     formats = []
@@ -778,16 +781,18 @@
 def publisher(repo, release, include_all):
     '''Return InvenioRDM "publisher".
     https://inveniordm.docs.cern.ch/reference/metadata/#publisher-0-1
     '''
     if not (name := os.environ.get('INVENIO_SERVER_NAME', '')):
         # It should be set by cli.py during normal operation. During testing or
         # unanticipated situations, let's be careful to have a fallback here.
-        from iga.invenio import invenio_api_available
-        name = invenio_api_available(os.environ.get('INVENIO_SERVER', ''))
+        from iga.invenio import invenio_server_name
+        name = invenio_server_name(os.environ.get('INVENIO_SERVER', ''))
+        if name is None:
+            name = ''
     return name
 
 
 def references(repo, release, include_all):
     '''Return InvenioRDM "references".
     https://inveniordm.docs.cern.ch/reference/metadata/#references-0-n
     '''
@@ -1061,21 +1066,21 @@
                      'LICENCE', 'Licence', 'licence',
                      'COPYING', 'COPYRIGHT', 'Copyright', 'copyright']:
         for ext in ['', '.txt', '.md', '.html']:
             if basename + ext in filenames:
                 log('found a license file in the repo: "' + basename + ext + '"')
                 # There's no safe way to summarize arbitrary license text,
                 # so we can't provide a 'description' field value.
-                rights = {'title': {'en': 'License'},
-                          'link': github_file_url(repo, basename + ext)}
+                rights = [{'title': {'en': 'License'},
+                           'link': github_file_url(repo, basename + ext)}]
                 break
         else:
             continue
         break
-    return [rights]
+    return rights
 
 
 def sizes(repo, release, include_all):
     '''Return InvenioRDM "sizes".
     https://inveniordm.docs.cern.ch/reference/metadata/#sizes-0-n
     '''
     return []
```

### Comparing `iga-0.0.9/iga/name_utils.py` & `iga-1.0.0/iga/name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/iga/orcid.py` & `iga-1.0.0/iga/orcid.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/iga/reference.py` & `iga-1.0.0/iga/reference.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/iga/ror.py` & `iga-1.0.0/iga/ror.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/iga/text_utils.py` & `iga-1.0.0/iga/text_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/iga.egg-info/PKG-INFO` & `iga-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,10 @@
-Metadata-Version: 2.1
-Name: iga
-Version: 0.0.9
-Summary: InvenioRDM GitHub Archiver
-Home-page: https://github.com/caltechlibrary/iga
-Author: Michael Hucka
-Author-email: helpdesk@library.caltech.edu
-License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
-Project-URL: Source Code, https://github.com/caltechlibrary/iga
-Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
-Keywords: Python,applications
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # IGA<img width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
 
-IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a GitHub Action that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
+IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a [GitHub Action](https://github.com/marketplace/actions/iga) that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
 [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
 [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
 [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
 
 
@@ -43,154 +19,244 @@
 * [Contributing](#contributing)
 * [License](#license)
 * [Acknowledgments](#authors-and-acknowledgments)
 
 
 ## Introduction
 
-[InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and datasets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the InvenioRDM GitHub Archiver (IGA) comes in.
+[InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and data sets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the [_InvenioRDM GitHub Archiver_](https://github.com/caltechlibrary/iga) (IGA) comes in.
 
 IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Action](https://docs.github.com/en/actions) to archive GitHub releases automatically for a repository each time they are made.
 
 <p align=center>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" width="40%">
 <span style="font-size: 150%">➜</span>
 <img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
 </p>
 
 IGA offers many notable features:
-* Automatic metadata extraction from GitHub releases plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
-* Thorough coverage of [InvenioRDM record metadata fields](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
-* Recognition of id's that appear in CodeMeta & CFF files: [ORCID](https://orcid.org), [ROR](https://ror.org), [DOI](https://www.doi.org), [arXiv](https://arxiv.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
-* Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google Books, & other sources if needed
+* Automatic metadata extraction from GitHub plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
+* Thorough coverage of [InvenioRDM record metadata](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
+* Recognition of identifiers in CodeMeta & CFF files: [ORCID](https://orcid.org),, [DOI](https://www.doi.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
+* Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google, and other sources
 * Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
-* Automatic lookup of human names in [ORCID.org](https://orcid.org) if needed (assuming ORCID id's are provided)
-* Automatic splitting of human names into family and given names using [ML](https://en.wikipedia.org/wiki/Machine_learning)-based methods
+* Automatic lookup of human names in [ORCID.org](https://orcid.org) (assuming ORCID id's are provided)
+* Automatic splitting of human names into family & given names using [ML](https://en.wikipedia.org/wiki/Machine_learning) methods
 * Support for InvenioRDM [communities](https://invenio-communities.readthedocs.io/en/latest/)
-* Support for overriding the metadata record that IGA creates, for complete control if you need it
+* Support for overriding the record that IGA creates, for complete control if you need it
 * Support for using the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in simple cases
 * Extensive use of logging so you can see what's going on under the hood
 
 
 ## Installation
 
-### As a standalone command-line program
+IGA can be installed as either (or both) a command-line program on your computer or a [GitHub Action](https://docs.github.com/en/actions) in a GitHub repository.
+
+### IGA as a standalone program
 
-There are multiple ways of installing IGA.  Please choose the alternative that suits you.
+Please choose an approach that suits your situation and preferences.
 
-#### _Alternative 1: installing IGA using `pipx`_
+<details><summary><h4><i>Alternative 1: using <code>pipx</code></i></h4></summary>
 
 [Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
 ```sh
 pipx install iga
 ```
 
 Pipx can also let you run IGA directly using `pipx run iga`, although in that case, you must always prefix every IGA command with `pipx run`.  Consult the [documentation for `pipx run`](https://github.com/pypa/pipx#walkthrough-running-an-application-in-a-temporary-virtual-environment) for more information.
+</details>
 
+<details><summary><h4><i>Alternative 2: using <code>pip</code></i></h4></summary>
 
-#### _Alternative 2: installing IGA using `pip`_
-
-You should be able to install `iga` with [`pip`](https://pip.pypa.io/en/stable/installing/) for Python&nbsp;3.  To install `iga` from the [Python package repository (PyPI)](https://pypi.org), run the following command:
+IGA is available from the [Python package repository PyPI](https://pypi.org) and can be installed using [`pip`](https://pip.pypa.io/en/stable/installing/):
 ```sh
 python3 -m pip install iga
 ```
 
-As an alternative to getting it from [PyPI](https://pypi.org), you can use `pip` to install `iga` directly from GitHub:
+As an alternative to getting it from [PyPI](https://pypi.org), you can install `iga` directly from GitHub:
 ```sh
 python3 -m pip install git+https://github.com/caltechlibrary/iga.git
 ```
 
 _If you already installed IGA once before_, and want to update to the latest version, add `--upgrade` to the end of either command line above.
+</details>
 
+<details><summary><h4><i>Alternative 3: from sources</i></h4></summary>
 
-#### _Alternative 3: installing IGA from sources_
-
-If  you prefer to install IGA directly from the source code, you can do that too. To get a copy of the files, you can clone the GitHub repository:
+If  you prefer to install IGA directly from the source code, first obtain a copy by either downloading the source archive from the [IGA releases page on GitHub](https://github.com/caltechlibrary/iga/releases), or by using `git` to clone the repository to a location on your computer. For example,
 ```sh
 git clone https://github.com/caltechlibrary/iga
 ```
 
-Alternatively, you can download the software source files as a ZIP archive directly from your browser using this link: <https://github.com/caltechlibrary/iga/archive/refs/heads/main.zip>
-
 Next, after getting a copy of the files,  run `setup.py` inside the code directory:
 ```sh
 cd iga
 python3 setup.py install
 ```
+</details>
+
+After installation, a program named `iga` should end up in a location where other command-line programs are installed on your computer.  Test it by running the following command in a shell:
+```shell
+iga --help
+```
 
 
-### As a GitHub Action
+### IGA as a GitHub Action
 
-[...forthcoming...]
+A [GitHub Action](https://docs.github.com/en/actions) is a workflow that runs on GitHub's servers under control of a file in your repository. Follow these steps to create the IGA workflow file:
+
+1. In the main branch of your GitHub repository, create a `.github/workflows` directory
+2. In the `.github/workflows` directory, create a file named (e.g.) `iga.yml` and copy the [following contents](https://raw.githubusercontent.com/caltechlibrary/iga/develop/sample-workflow.yml) into it:
+    ```yaml
+    name: InvenioRDM GitHub Archiver
+
+    env:
+      # 👋🏻 Set the next variable to your InvenioRDM server address 👋🏻
+      INVENIO_SERVER: https://your-invenio-server.org
+
+      # Set to an InvenioRDM record ID to mark releases as new versions.
+      parent_record: none
+
+      # The remaining variables are other IGA options. Please see the docs.
+      community:     none
+      draft:         false
+      all_assets:    false
+      all_metadata:  false
+      debug:         false
+
+    # ~~~~~~~~~~~~~~~~ The rest of this file should be left as-is. ~~~~~~~~~~~~~~~~
+
+    on:
+      release:
+        types: [published]
+      workflow_dispatch:
+        inputs:
+          release_tag:
+            description: "The release tag (empty = latest):"
+          draft:
+            default: false
+            description: "Mark the InvenioRDM record as a draft:"
+          parent_record:
+            description: "ID of parent record (for versioning):"
+          community:
+            description: "Name of InvenioRDM community (if any):"
+          all_assets:
+            default: false
+            description: "Attach all GitHub assets:"
+          all_metadata:
+            default: false
+            description: "Include additional GitHub metadata:"
+          debug:
+            default: false
+            description: "Print debug info in the GitHub log:"
+    jobs:
+      Send_to_InvenioRDM:
+        runs-on: ubuntu-latest
+        steps:
+          - uses: caltechlibrary/iga@main
+            with:
+              INVENIO_SERVER: ${{env.INVENIO_SERVER}}
+              INVENIO_TOKEN:  ${{secrets.INVENIO_TOKEN}}
+              all_assets:     ${{github.event.inputs.all_assets || env.all_assets}}
+              all_metadata:   ${{github.event.inputs.all_metadata || env.all_metadata}}
+              debug:          ${{github.event.inputs.debug || env.debug}}
+              draft:          ${{github.event.inputs.draft || env.draft}}
+              community:      ${{github.event.inputs.community || env.community}}
+              parent_record:  ${{github.event.inputs.parent_record || env.parent_record}}
+              release_tag:    ${{github.event.inputs.release_tag || 'latest'}}
+    ```
+3. **Edit the value of the `INVENIO_SERVER` variable (line 5 above)** ↑
+4. Optionally, change the values of other options (`parent_record`, `community`, etc.)
+5. Save the file, commit the changes to git, and push your changes to GitHub
 
 
 ## Quick start
 
-After a successful [installation](#installation) of IGA, here is how you can get started quickly.
+No matter whether IGA is run locally on your computer or as a GitHub Action, in both cases it must be provided with a personal access token (PAT) for your InvenioRDM server. Getting one 
+is the first step.
 
-### Command-line use
+### Getting an InvenioRDM token
 
-If the [installation](#installation) process described above is successful, you should end up with a program named `iga` in a location where software is normally installed on your computer.  Running `iga` should be as simple as running any other command-line program. For example, the following command should print a helpful message to your terminal:
-```shell
-iga --help
-```
+<img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/get-invenio-pat.png" width="60%" align="right">
+
+1. Log in to your InvenioRDM account
+2. Go to the _Applications_ page in your account profile
+3. Click the <kbd>New token</kbd> button next to "Personal access tokens"
+4. On the page that is shown after you click that button, name your token (the name does not matter) and click the <kbd>Create</kbd> button
+5. After InvenioRDM creates and shows you the token, **copy it to a safe location** because InvenioRDM will not show it again
 
-IGA's main purpose is to create a metadata record in an InvenioRDM server and attach a GitHub release archive to the record. IGA needs 4 pieces of information to do its work, though for simple repositories you can often get by with just 3:
+### Configuring and running IGA locally
+
+To send a GitHub release to your InvenioRDM server, IGA needs this information:
 1. (Required) The identity of the GitHub release to be archived
 2. (Required) The address of the destination InvenioRDM server
-3. (Required) A Personal Access Token (PAT) for the InvenioRDM server
-4. (Optional) A Personal Access Token for GitHub
+3. (Required) A personal access token for InvenioRDM (from [above](#getting-an-inveniordm-token))
+4. (Optional) A [personal access token for GitHub](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
 
-The first one (the identity of the GitHub release) is given as arguments to IGA on the command line; the rest can be provided either via command-line options or by setting environment variables. A common way of configuring IGA is to set environment variables in your shell script or your interactive shell. Here is an example using Bash shell syntax, with realistic-looking but fake token values:
+The identity of the GitHub release is always given as an argument to IGA on the command line; the remaining values can be provided either via command-line options or environment variables. One approach is to set environment variables in shell scripts or your interactive shell. Here is an example using Bash shell syntax, with fake token values:
 ```shell
 export INVENIO_SERVER=https://data.caltech.edu
 export INVENIO_TOKEN=qKLoOH0KYf4D98PGYQGnC09hiuqw3Y1SZllYnonRVzGJbWz2
 export GITHUB_TOKEN=ghp_wQXp6sy3AsKyyEo4l9esHNxOdo6T34Zsthz
 ```
 
-Once these environment variables set in your shell, you can more easily invoke IGA. Usage can be as simple as providing a URL for a release in GitHub. For example:
+Once these are set, use of IGA can be as simple as providing a URL for a release in GitHub. For example, the following command creates a draft record (the `-d` option is short for `--draft`) for another project in GitHub and tells IGA to open (the `-o` option is short for `--open`) the newly-created InvenioRDM entry in a web browser:
 ```shell
-iga https://github.com/mhucka/taupe/releases/tag/v1.2.0
+iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
-If you give the option `--open` (or `-o` for short) to IGA, it will open the newly-created InvenioRDM entry in your default web browser when it's done:
-```shell
-iga -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
-```
+More options are described in the section on [detailed usage information](#usage) below.
 
-If you want the record to be only a draft and not a final version (perhaps so that you can inspect the result and edit it before finalizing it), use the option `--draft` (or `-d` for short):
-```shell
-iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
-```
 
-More options and examples can be found in the section on [detailed usage information](#usage) below.
+### Configuring and running IGA as a GitHub Action
+
+After doing the [GitHub Action installation](#as-a-github-action) steps and [obtaining an InvenioRDM token](#getting-an-inveniordm-token), one more step is needed: the token must be stored as a "secret" in your GitHub repository.
+
+1. Go to the _Settings_ page of your GitHub repository<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-tabs.png" width="85%"></p>
+2. In the left-hand sidebar, find _Secrets and variables_ in the Security section, click on it to reveal _Actions_ underneath, then click on _Actions_<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-sidebar-secrets.png" width="40%"></p>
+3. In the next page, click the green <kbd>New repository secret</kbd> button<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-secrets.png" width="60%"></p>
+4. Name the variable `INVENIO_TOKEN` and paste in your InvenioRDM token
+5. Finish by clicking the green <kbd>Add secret</kbd> button
+
+#### Testing the workflow
+
+After setting up the workflow and storing the InvenioRDM token in your repository on GitHub, it's a good idea to run the workflow manually to test that it works as expected.
+
+1. Go to the _Actions_ tab in your repository and click on the name of the workflow in the sidebar on the left<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-run-workflow.png" width="90%"></p>
+2. Click the <kbd>Run workflow</kbd> button in the right-hand side of the blue strip
+3. In the pull-down, change the value of "Mark the record as a draft" to `true`<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-workflow-options-circled.png" width="40%"></p>
+4. Click the green <kbd>Run workflow</kbd> button near the bottom
+5. Refresh the web page and a new line will be shown named after your workflow file<p align="center"><img src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/github-running-workflow.png" width="90%"></p>
+6. Click the title of the workflow to see the IGA workflow progress and results
 
 
-### GitHub Action use
+#### Running the workflow when releasing software
 
-[...forthcoming...]
+Once the personal access token from InvenioRDM is stored as a GitHub secret, the workflow should run automatically every time a new release is made on GitHub &ndash; no further action should be needed. You can check the results (and look for errors if something went wrong) by going to the _Actions_ tab in your GitHub repository.
 
 
 ## Usage
 
 This section provides detailed information about IGA's operation and options to control it.
 
 ### Identifying the InvenioRDM server
 
 The server address must be provided either as the value of the option `--invenio-server` or in an environment variable named `INVENIO_SERVER`.  If the server address does not begin with `https://`, IGA will prepend it automatically.
 
 ### Providing an InvenioRDM access token
 
-A Personal Access Token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
+A personal access token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
 
 To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
 
 ### Providing a GitHub access token
 
-It is possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for many repositories, IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+It _may_ be possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for some repositories IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+
+Note that when you run IGA as a GitHub Action, you do not need to create or set a GitHub token because it is obtained automatically by the GitHub Action workflow.
 
 ### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
  1. The full URL of the web page on GitHub of a tagged release. In this case,
     the URL must be the final argument on the command line invocation of IGA
     and the options `--account` and `--repo` must be omitted.
@@ -252,17 +318,17 @@
 
 ### Other options recognized by IGA
 
 Running IGA with the option `--save-metadata` will make it create a metadata record, but instead of uploading the record (and any assets) to the InvenioRDM server, IGA will write the result to the given destination. This can be useful not only for debugging but also for creating a starting point for a custom metadata record: first run IGA with `--save-metadata` to save a record to a file, edit the result, then finally run IGA with the `--read-metadata` option to use the modified record to create a release in the InvenioRDM server.
 
 The `--mode` option can be used to change the run mode. Four run modes are available: `quiet`, `normal`, `verbose`, and `debug`. The default mode is `normal`, in which IGA prints a few messages while it's working. The mode `quiet` will make it avoid printing anything unless an error occurs, the mode `verbose` will make it print a detailed trace of what it is doing, and the mode `debug` will make IGA even more verbose. In addition, in `debug` mode, IGA will drop into the `pdb` debugger if it encounters an exception during execution. On Linux and macOS, debug mode also installs a signal handler on signal USR1 that causes IGA to drop into the `pdb` debugger if the signal USR1 is received. (Use `kill -USR1 NNN`, where NNN is the IGA process id.)
 
-Networks latencies are unpredicatable. Reading and writing large files may take a long time; on the other hand, IGA should not wait forever before reporting an error if a server or network becomes unresponsive. To balance these conflicting needs, IGA automatically scales its network timeout based on file sizes. To override its adaptive algorithm and set an explicit timeout value, use the option `--timeout` with a value in seconds.
+By default, informational output is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` (i.e., a dash) to indicate console output, or it can be a file path to send the output to the file. A special exception is that even if a log destination is given, IGA will still print the final record URL to stdout.  This makes it possible to invoke IGA from scripts that capture the record URL while still saving diagnostic output in case debugging is needed.
 
-By default, the output of the `verbose` and `debug` run modes is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` to indicate console output, or a file path to send the output to the file.
+Reading and writing large files may take a long time; on the other hand, IGA should not wait forever on network operations before reporting an error if a server or network becomes unresponsive. To balance these conflicting needs, IGA automatically scales its network timeout based on file sizes. To override its adaptive algorithm and set an explicit timeout value, use the option `--timeout` with a value in seconds.
 
 If given the `--version` option, this program will print its version and other information, and exit without doing anything else.
 
 Running IGA with the option `--help` will make it print help text and exit without doing anything else.
 
 ### Summary of command-line options
 
@@ -273,15 +339,15 @@
 | `--all-assets`         | `-A`     | Attach all GitHub assets | Attach only the release source ZIP| |
 | `--all-metadata`       | `-M`     | Include additional metadata from GitHub | Favor CodeMeta & CFF | |
 | `--community` _C_      | `-c` _C_ | Submit record to RDM community _C_ | Don't submit record to any community | | 
 | `--draft`              | `-d`     | Mark the RDM record as a draft | Publish record when done | |
 | `--file` _F_           | `-f` _F_ | Upload local file _F_ instead of GitHub assets | Upload only GitHub assets | ⚑ |
 | `--github-account` _A_ | `-a` _A_ | Look in GitHub account _A_ | Get account name from release URL | ✯ | 
 | `--github-repo` _R_    | `-r` _R_ | Look in GitHub repository _R_ of account _A_ | Get repo name from release URL | ✯ |
-| `--github-token` _T_   | `-t` _T_ | Use GitHub acccess token _T_| Use value in env. var. `GITHUB_TOKEN` | |
+| `--github-token` _T_   | `-t` _T_ | Use GitHub access token _T_| Use value in env. var. `GITHUB_TOKEN` | |
 | `--help`               | `-h`     | Print help info and exit | | |
 | `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
 | `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
 | `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
@@ -304,20 +370,24 @@
 |:----:|----------------------------------------------------------|
 | 0    | success &ndash; program completed normally               |
 | 1    | interrupted                                              |
 | 2    | encountered a bad or missing value for an option         |
 | 3    | encountered a problem with a file or directory           |
 | 4    | encountered a problem interacting with GitHub            |
 | 5    | encountered a problem interacting with InvenioRDM        |
-| 6    | an exception or fatal error occurred                     |
+| 6    | the personal access token was rejected                   |
+| 7    | an exception or fatal error occurred                     |
 
 
 ## Known issues and limitations
 
-_[… forthcoming …]_
+The following are known issues and limitations.
+* As of mid-2023, InvenioRDM requires names of record creators and other contributors to be split into given (first) and family (surname). This is problematic for multiple reasons. The first is that mononyms are common in many countries: a person's name may legitimately be only a single word which is not conceptually a "given" or "family" name.  To compound the difficulty for IGA, names are stored as single fields in GitHub account metadata, so unless a repository has a `codemeta.json` or `CITATION.cff` file (which allow authors more control over how they want their names represented), IGA is forced to try to split the single GitHub name string into two parts. _A foolproof algorithm for doing this does not exist_, so IGA will sometimes get it wrong. (That said, IGA goes to extraordinary lengths to try to do a good job.)
+* Some accounts on GitHub are software automation or "bot" accounts but are not labeled as such. These accounts are generally indistinguishable from human accounts on GitHub. If such an account is the creator of a release in GitHub, and IGA has to use its name-splitting algorithm on the name of the account, it may produce a nonsensical result. For example, it might turn "Travis CI" into an entry with a first name of "Travis" and last name of "CI". 
+
 
 ## Getting help
 
 If you find an issue, please submit it in [the GitHub issue tracker](https://github.com/caltechlibrary/iga/issues) for this repository.
 
 
 ## Contributing
@@ -346,38 +416,44 @@
 * [humanize](https://github.com/jmoiron/humanize) &ndash; make numbers more easily readable by humans
 * [idutils](https://github.com/inveniosoftware/idutils) &ndash; package for validating and normalizing various kinds of persistent identifiers
 * [ipdb](https://github.com/gotcha/ipdb) &ndash; the IPython debugger
 * [iptools](https://github.com/bd808/python-iptools) &ndash; utilities for dealing with IP addresses
 * [isbnlib](https://github.com/xlcnd/isbnlib) &ndash; utilities for dealing with ISBNs
 * [json5](https://github.com/dpranke/pyjson5) &ndash; extended JSON format parser
 * [latexcodec](https://github.com/mcmtroffaes/latexcodec) &ndash; lexer and codec to work with LaTeX code in Python
+* [linkify-it-py](https://github.com/tsutsu3/linkify-it-py) &ndash; a link recognition library with full unicode support
 * [lxml](https://lxml.de) &ndash; an XML parsing library
 * [Markdown](https://python-markdown.github.io) &ndash; Python package for working with Markdown
 * [markdown-checklist](https://github.com/FND/markdown-checklist) &ndash; GitHub-style checklist extension for Python Markdown package
 * [mdx-breakless-lists](https://github.com/adamb70/mdx-breakless-lists) &ndash; GitHub-style Markdown lists that don't require a line break above them
 * [mdx_linkify](https://github.com/daGrevis/mdx_linkify) &ndash; extension for Python Markdown will convert text that look like links to HTML anchors
+* [MyST-parser](https://github.com/executablebooks/MyST-Parser) &ndash; A Sphinx and Docutils extension to parse an extended version of Markdown
 * [nameparser](https://github.com/derek73/python-nameparser) &ndash; package for parsing human names into their individual components
 * [probablepeople](https://github.com/datamade/probablepeople) &ndash; package for parsing names into components using ML-based techniques
-* [pymdown-extensions](https://github.com/facelessuser/pymdown-extensions) &ndash; extensions for Python Markdown
-* [PyYAML](https://pyyaml.org) &ndash; YAML parser
 * [pybtex](https://pybtex.org) &ndash; BibTeX parser and formatter
 * [pybtex-apa7-style]() &ndash; plugin for [pybtex](https://pybtex.org) that provides APA7 style formatting
+* [pymdown-extensions](https://github.com/facelessuser/pymdown-extensions) &ndash; extensions for Python Markdown
 * [pytest](https://docs.pytest.org/en/stable/) &ndash; testing framework
 * [pytest-cov](https://github.com/pytest-dev/pytest-cov) &ndash; coverage reports for use with `pytest`
 * [pytest-mock](https://pypi.org/project/pytest-mock/) &ndash; wrapper around the `mock` package for use with `pytest`
+* [PyYAML](https://pyyaml.org) &ndash; YAML parser
 * [Rich](https://github.com/Textualize/rich) &ndash; library for writing styled text to the terminal
 * [rich-click](https://github.com/ewels/rich-click) &ndash; CLI interface built on top of [Rich](https://github.com/Textualize/rich)
+* [setuptools](https://github.com/pypa/setuptools) &ndash; library for `setup.py`
 * [Sidetrack](https://github.com/caltechlibrary/sidetrack) &ndash; simple debug logging/tracing package
 * [spaCy](https://spacy.io) &ndash; Natural Language Processing package
 * [spacy-alignments](https://github.com/explosion/spacy-alignments) &ndash; alternate alignments for [spaCy](https://spacy.io)
 * [spacy-legacy](https://pypi.org/project/spacy-legacy/) &ndash; [spaCy](https://spacy.io) legacy functions and architectures for backwards compatibility
 * [spacy-loggers](https://github.com/explosion/spacy-loggers) &ndash; loggers for [spaCy](https://spacy.io)
 * [spacy-pkuseg](https://github.com/explosion/spacy-pkuseg) &ndash; Chinese word segmentation toolkit for [spaCy](https://spacy.io)
 * [spacy-transformers](https://spacy.io) &ndash; pretrained Transformers for [spaCy](https://spacy.io)
-* [setuptools](https://github.com/pypa/setuptools) &ndash; library for `setup.py`
+* [Sphinx](https://www.sphinx-doc.org/en/master/) &ndash; documentation generator for Python
+* [sphinx-autobuild](https://pypi.org/project/sphinx-autobuild/) &ndash; rebuild Sphinx docs automatically
+* [sphinx-material](https://bashtage.github.io/sphinx-material/) &ndash; a responsive Material Design theme for Sphinx
+* [sphinxcontrib-mermaid](https://github.com/mgaitan/sphinxcontrib-mermaid) &ndash; support Mermaid diagrams in Sphinx docs
 * [StringDist](https://github.com/obulkin/string-dist) &ndash; library for calculating string distances
 * [Twine](https://github.com/pypa/twine) &ndash; utilities for publishing Python packages on [PyPI](https://pypi.org)
 * [url-normalize](https://github.com/niksite/url-normalize) &ndash; URI/URL normalization utilities
 * [validators](https://github.com/kvesteri/validators) &ndash; data validation package for Python
 * [wheel](https://pypi.org/project/wheel/) &ndash; setuptools extension for building wheels
 
 <div align="center">
```

### Comparing `iga-0.0.9/iga.egg-info/SOURCES.txt` & `iga-1.0.0/iga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/iga.egg-info/requires.txt` & `iga-1.0.0/iga.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/setup.cfg` & `iga-1.0.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iga
-version = 0.0.9
+version = 1.0.0
 description = InvenioRDM GitHub Archiver
 author = Michael Hucka
 author_email = helpdesk@library.caltech.edu
 license = https://github.com/caltechlibrary/iga/blob/main/LICENSE
 license_files = LICENSE
 url = https://github.com/caltechlibrary/iga
 project_urls =
```

### Comparing `iga-0.0.9/setup.py` & `iga-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_cli.py` & `iga-1.0.0/tests/test_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,32 +8,44 @@
 
 import click
 import click.testing
 import json5
 import os
 from   os import path
 from   sidetrack import log
-from   unittest import mock
+from   unittest.mock import patch
 
 from   iga.exit_codes import ExitCode
 from iga.github import (
-    GitHubRepo,
     GitHubAccount,
     GitHubRelease,
+    GitHubRepo,
 )
 
 
 # Mocks
 # .............................................................................
 
 here      = path.dirname(path.abspath(__file__))
 repo_dir  = path.join(here, 'data/fake-example/')
 orcid_dir = path.join(here, 'data/orcid-examples/')
 
 
+def mocked_invenio_api_available(server_url):
+    return True
+
+
+def mocked_invenio_token_valid(server_url):
+    return True
+
+
+def mocked_invenio_server_name(server_url):
+    return 'TestServer'
+
+
 def mocked_github_account(account_name):
     log(f'returing mocked GitHubAccount for {account_name}')
     with open(path.join(repo_dir, 'account.json'), 'r') as f:
         return GitHubAccount(json5.loads(f.read()))
 
 
 def mocked_github_repo(account_name, repo_name):
@@ -78,23 +90,26 @@
     with open(path.join(orcid_dir, orcid_filename), 'r') as f:
         return json5.load(f)
 
 
 # Tests
 # .............................................................................
 
-@mock.patch.dict(os.environ, {}, clear=True)
-@mock.patch('iga.github.github_repo_file', new=mocked_github_repo_file)
-@mock.patch('iga.github.github_repo_filenames', new=mocked_github_repo_filenames)
-@mock.patch('iga.github.github_repo_languages', new=mocked_github_repo_languages)
-@mock.patch('iga.github.github_repo_contributors', new=mocked_github_repo_contributors)
-@mock.patch('iga.github.github_account', new=mocked_github_account)
-@mock.patch('iga.github.github_repo', new=mocked_github_repo)
-@mock.patch('iga.github.github_release', new=mocked_github_release)
-@mock.patch('iga.orcid.orcid_data', new=mocked_orcid_data)
+@patch.dict(os.environ, {}, clear=True)
+@patch('iga.invenio.invenio_api_available', new=mocked_invenio_api_available)
+@patch('iga.invenio.invenio_token_valid', new=mocked_invenio_token_valid)
+@patch('iga.invenio.invenio_server_name', new=mocked_invenio_server_name)
+@patch('iga.github.github_repo_file', new=mocked_github_repo_file)
+@patch('iga.github.github_repo_filenames', new=mocked_github_repo_filenames)
+@patch('iga.github.github_repo_languages', new=mocked_github_repo_languages)
+@patch('iga.github.github_repo_contributors', new=mocked_github_repo_contributors)
+@patch('iga.github.github_account', new=mocked_github_account)
+@patch('iga.github.github_repo', new=mocked_github_repo)
+@patch('iga.github.github_release', new=mocked_github_release)
+@patch('iga.orcid.orcid_data', new=mocked_orcid_data)
 def test_environment_vars_from_options(capsys):
     from iga.cli import cli
     runner = click.testing.CliRunner()
     args = ['--invenio-server', 'https://data.caltechlibrary.dev',
             '--invenio-token', 'itoken',
             '--github-token', 'gtoken',
             '--save-metadata', '/tmp/fake.json',
```

### Comparing `iga-0.0.9/tests/test_data_utils.py` & `iga-1.0.0/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_doi.py` & `iga-1.0.0/tests/test_doi.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_exceptions.py` & `iga-1.0.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_github.py` & `iga-1.0.0/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_github_mocks.py` & `iga-1.0.0/tests/test_github_mocks.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_id_utils.py` & `iga-1.0.0/tests/test_id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_init.py` & `iga-1.0.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_is_person.py` & `iga-1.0.0/tests/test_is_person.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_licenses.py` & `iga-1.0.0/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_name_splitting.py` & `iga-1.0.0/tests/test_name_splitting.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_name_utils.py` & `iga-1.0.0/tests/test_name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_orcid.py` & `iga-1.0.0/tests/test_orcid.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_reference.py` & `iga-1.0.0/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_ror.py` & `iga-1.0.0/tests/test_ror.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.9/tests/test_text_utils.py` & `iga-1.0.0/tests/test_text_utils.py`

 * *Files identical despite different names*

