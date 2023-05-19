# Comparing `tmp/vgd_counterfactuals-0.1.3.tar.gz` & `tmp/vgd_counterfactuals-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vgd_counterfactuals-0.1.3.tar", max compression
+gzip compressed data, was "vgd_counterfactuals-0.1.4.tar", max compression
```

## Comparing `vgd_counterfactuals-0.1.3.tar` & `vgd_counterfactuals-0.1.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.1.3/LICENSE
--rwxr-xr-x   0        0        0     6577 2023-05-16 07:28:37.070671 vgd_counterfactuals-0.1.3/README.rst
--rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.1.3/banner.png
--rwxr-xr-x   0        0        0     1514 2023-05-16 07:28:37.058671 vgd_counterfactuals-0.1.3/pyproject.toml
--rwxr-xr-x   0        0        0        5 2023-05-16 07:28:37.070671 vgd_counterfactuals-0.1.3/vgd_counterfactuals/VERSION
--rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.1.3/vgd_counterfactuals/__init__.py
--rw-r--r--   0        0        0    10221 2023-05-16 07:28:31.190627 vgd_counterfactuals-0.1.3/vgd_counterfactuals/base.py
--rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.1.3/vgd_counterfactuals/cli.py
--rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/00_quickstart.py
--rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/01_visualization.py
--rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/README.rst
--rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/__init__.py
--rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
--rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
--rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
--rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
--rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
--rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
--rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
--rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
--rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
--rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
--rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
--rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
--rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
--rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
--rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
--rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
--rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
--rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
--rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
--rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
--rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
--rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
--rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
--rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
--rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
--rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
--rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.3/vgd_counterfactuals/experiments/README.rst
--rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.3/vgd_counterfactuals/experiments/results/README.rst
--rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.3/vgd_counterfactuals/experiments/template_experiment.py
--rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.3/vgd_counterfactuals/experiments/template_experiment_sub.py
--rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.1.3/vgd_counterfactuals/generate/__init__.py
--rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.1.3/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6697 2023-05-15 12:10:39.475247 vgd_counterfactuals-0.1.3/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
--rw-r--r--   0        0        0     9534 2023-05-15 12:10:38.963244 vgd_counterfactuals-0.1.3/vgd_counterfactuals/generate/molecules.py
--rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.1.3/vgd_counterfactuals/generate/smiles_one_step_changes.py
--rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.3/vgd_counterfactuals/templates/article.tex.j2
--rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.3/vgd_counterfactuals/testing.py
--rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.1.3/vgd_counterfactuals/utils.py
--rw-r--r--   0        0        0     3370 2023-05-01 16:09:36.020519 vgd_counterfactuals-0.1.3/vgd_counterfactuals/visualization.py
--rw-r--r--   0        0        0     7622 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.1.4/LICENSE
+-rwxr-xr-x   0        0        0     6577 2023-05-19 11:40:29.896952 vgd_counterfactuals-0.1.4/README.rst
+-rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.1.4/banner.png
+-rwxr-xr-x   0        0        0     1514 2023-05-19 11:40:29.888952 vgd_counterfactuals-0.1.4/pyproject.toml
+-rwxr-xr-x   0        0        0        5 2023-05-19 11:40:29.896952 vgd_counterfactuals-0.1.4/vgd_counterfactuals/VERSION
+-rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.1.4/vgd_counterfactuals/__init__.py
+-rw-r--r--   0        0        0    10221 2023-05-16 07:28:31.190627 vgd_counterfactuals-0.1.4/vgd_counterfactuals/base.py
+-rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.1.4/vgd_counterfactuals/cli.py
+-rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/00_quickstart.py
+-rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/01_visualization.py
+-rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/README.rst
+-rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/__init__.py
+-rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
+-rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
+-rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
+-rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
+-rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
+-rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
+-rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
+-rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
+-rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
+-rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
+-rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
+-rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
+-rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
+-rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
+-rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
+-rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
+-rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
+-rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
+-rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
+-rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
+-rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
+-rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
+-rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
+-rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
+-rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
+-rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
+-rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.4/vgd_counterfactuals/experiments/README.rst
+-rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.4/vgd_counterfactuals/experiments/results/README.rst
+-rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.4/vgd_counterfactuals/experiments/template_experiment.py
+-rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.4/vgd_counterfactuals/experiments/template_experiment_sub.py
+-rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6996 2023-05-19 08:56:41.054361 vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
+-rw-r--r--   0        0        0     9753 2023-05-19 08:57:53.758885 vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/molecules.py
+-rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/smiles_one_step_changes.py
+-rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.4/vgd_counterfactuals/templates/article.tex.j2
+-rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.4/vgd_counterfactuals/testing.py
+-rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.1.4/vgd_counterfactuals/utils.py
+-rw-r--r--   0        0        0     3370 2023-05-01 16:09:36.020519 vgd_counterfactuals-0.1.4/vgd_counterfactuals/visualization.py
+-rw-r--r--   0        0        0     7622 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.1.4/PKG-INFO
```

### Comparing `vgd_counterfactuals-0.1.3/LICENSE` & `vgd_counterfactuals-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/README.rst` & `vgd_counterfactuals-0.1.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.1.3-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.1.4-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

### Comparing `vgd_counterfactuals-0.1.3/banner.png` & `vgd_counterfactuals-0.1.4/banner.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/pyproject.toml` & `vgd_counterfactuals-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0b2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vgd_counterfactuals"
-version = "0.1.3"
+version = "0.1.4"
 description = "Counterfactual explanations for GNNs based on the visual graph dataset format"
 license = "MIT license"
 authors = ["Jonas Teufel <jonseb1998@gmail.com>"]
 maintainers = ["Jonas Teufel <jonseb1998@gmail.com>"]
 readme = "README.rst"
 keywords = ["graph neural networks", "counterfactuals", "explainable AI"]
 packages = [
```

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/base.py` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/base.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/cli.py` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/cli.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/00_quickstart.py` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/00_quickstart.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/01_visualization.py` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/01_visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/code.py` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/code.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/experiments/README.rst` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/experiments/README.rst`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/experiments/template_experiment.py` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/experiments/template_experiment.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/experiments/template_experiment_sub.py` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/experiments/template_experiment_sub.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 15 12:10:38 2023 UTC, .py size: 9534 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,419 +1,438 @@
-00000000: 6f0d 0d0a 0000 0000 3e21 6264 3e25 0000  o.......>!bd>%..
+00000000: 6f0d 0d0a 0000 0000 c839 6764 3126 0000  o........9gd1&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 2c01 0000 6400  .....@...s,...d.
+00000020: 0009 0000 0040 0000 0073 4201 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6404 6405 6405 6406 6407  m.Z...d.d.d.d.d.
-00000060: 6408 6406 6409 9c07 5a07 6420 640b 6504  d.d.d...Z.d d.e.
-00000070: 6a08 640c 6509 6604 640d 640e 8405 5a0a  j.d.e.f.d.d...Z.
-00000080: 6507 650a 6601 6602 640f 6509 6410 6502  e.e.f.f.d.e.d.e.
-00000090: 6a0b 6502 6a0c 6504 6a08 6701 650d 6602  j.e.j.e.j.g.e.f.
-000000a0: 1900 1900 6411 6502 6a0e 6509 1900 6606  ....d.e.j.e...f.
-000000b0: 6412 6413 8405 5a0f 6421 640b 6504 6a08  d.d...Z.d!d.e.j.
-000000c0: 6415 6510 6411 6511 6606 6416 6417 8405  d.e.d.e.f.d.d...
-000000d0: 5a12 640b 6504 6a08 6418 6502 6a13 6509  Z.d.e.j.d.e.j.e.
-000000e0: 6510 6602 1900 6419 6502 6a13 6510 6502  e.f...d.e.j.e.e.
-000000f0: 6a0e 6510 1900 6602 1900 6411 6502 6a14  j.e...f...d.e.j.
-00000100: 6509 1900 6608 641a 641b 8404 5a15 640b  e...f.d.d...Z.d.
-00000110: 6504 6a08 6419 6502 6a13 6510 6502 6a0e  e.j.d.e.j.e.e.j.
-00000120: 6510 1900 6602 1900 6411 6502 6a14 6509  e...f...d.e.j.e.
-00000130: 1900 6606 641c 641d 8404 5a16 640b 6504  ..f.d.d...Z.d.e.
-00000140: 6a08 6411 6502 6a14 6509 1900 6604 641e  j.d.e.j.e...f.d.
-00000150: 641f 8404 5a17 6401 5300 2922 e900 0000  d...Z.d.S.)"....
-00000160: 004e 2901 da04 4368 656d 2901 da0b 696e  .N)...Chem)...in
-00000170: 7665 7274 5f64 6963 74e9 0400 0000 e905  vert_dict.......
-00000180: 0000 00e9 0600 0000 e901 0000 00e9 0700  ................
-00000190: 0000 2907 da01 43da 014e da01 50da 014f  ..)...C..N..P..O
-000001a0: da01 46da 0243 6cda 0153 fa0e 2a31 3d2a  ..F..Cl..S..*1=*
-000001b0: 2a32 3d2a 2a3d 2a31 2a32 da03 6d6f 6cda  *2=**=*1*2..mol.
-000001c0: 0770 6174 7465 726e 6302 0000 0000 0000  .patternc.......
-000001d0: 0000 0000 0004 0000 0003 0000 0043 0000  .............C..
-000001e0: 0073 1800 0000 7400 a001 7c01 a101 7d02  .s....t...|...}.
-000001f0: 7c00 a002 7c02 a101 7d03 7c03 5300 2901  |...|...}.|.S.).
-00000200: 7a83 0a20 2020 2043 6865 636b 7320 6966  z..    Checks if
-00000210: 2074 6865 2067 6976 656e 206d 6f6c 6563   the given molec
-00000220: 756c 6520 6060 6d6f 6c60 6020 6973 2061  ule ``mol`` is a
-00000230: 2062 7269 6467 6520 6865 6164 2063 6172   bridge head car
-00000240: 626f 6e20 7374 7275 6374 7572 6520 7768  bon structure wh
-00000250: 6963 6820 6170 7061 7265 6e74 6c79 2064  ich apparently d
-00000260: 6f65 7320 6e6f 740a 2020 2020 6170 7065  oes not.    appe
-00000270: 6172 2069 6e20 6368 656d 6973 7472 792e  ar in chemistry.
-00000280: 0a20 2020 2029 0372 0200 0000 da0d 4d6f  .    ).r......Mo
-00000290: 6c46 726f 6d53 6d61 7274 73da 1148 6173  lFromSmarts..Has
-000002a0: 5375 6273 7472 7563 744d 6174 6368 2904  SubstructMatch).
-000002b0: 7211 0000 0072 1200 0000 da06 736d 6172  r....r......smar
-000002c0: 7473 da08 6973 5f6d 6174 6368 a900 7217  ts..is_match..r.
-000002d0: 0000 00fa 542f 6d65 6469 612f 7373 642f  ....T/media/ssd/
-000002e0: 5072 6f67 7261 6d6d 696e 672f 7667 645f  Programming/vgd_
-000002f0: 636f 756e 7465 7266 6163 7475 616c 732f  counterfactuals/
-00000300: 7667 645f 636f 756e 7465 7266 6163 7475  vgd_counterfactu
-00000310: 616c 732f 6765 6e65 7261 7465 2f6d 6f6c  als/generate/mol
-00000320: 6563 756c 6573 2e70 79da 1569 735f 6272  ecules.py..is_br
-00000330: 6964 6765 5f68 6561 645f 6361 7262 6f6e  idge_head_carbon
-00000340: 1400 0000 7306 0000 000a 050a 0104 0172  ....s..........r
-00000350: 1900 0000 da06 736d 696c 6573 da0b 6d6f  ......smiles..mo
-00000360: 6c5f 6669 6c74 6572 73da 0672 6574 7572  l_filters..retur
-00000370: 6e63 0300 0000 0000 0000 0000 0000 0800  nc..............
-00000380: 0000 0700 0000 4300 0000 7388 0000 0074  ......C...s....t
-00000390: 0083 007d 0374 01a0 027c 00a1 017d 0474  ...}.t...|...}.t
-000003a0: 037c 0483 017d 057c 03a0 0474 057c 047c  .|...}.|...t.|.|
-000003b0: 017c 0564 018d 03a1 0101 007c 03a0 0474  .|.d.......|...t
-000003c0: 067c 047c 0564 028d 02a1 0101 007c 03a0  .|.|.d.......|..
-000003d0: 0474 077c 0464 038d 01a1 0101 0067 007d  .t.|.d.......g.}
-000003e0: 067c 0344 005d 167d 0074 01a0 027c 00a1  .|.D.].}.t...|..
-000003f0: 017d 047c 0244 005d 077d 077c 077c 0483  .}.|.D.].}.|.|..
-00000400: 0173 3b71 3471 347c 06a0 087c 00a1 0101  .s;q4q4|...|....
-00000410: 0071 2b7c 0653 0029 0461 b103 0000 0a20  .q+|.S.).a..... 
-00000420: 2020 2047 6976 656e 2061 2060 6073 6d69     Given a ``smi
-00000430: 6c65 7360 6020 7265 7072 6573 656e 7461  les`` representa
-00000440: 7469 6f6e 206f 6620 6120 6d6f 6c65 6375  tion of a molecu
-00000450: 6c65 2c20 7468 6973 2066 756e 6374 696f  le, this functio
-00000460: 6e20 7769 6c6c 2072 6574 7572 6e20 6120  n will return a 
-00000470: 6c69 7374 206f 6620 7468 6520 534d 494c  list of the SMIL
-00000480: 4553 0a20 2020 2072 6570 7265 7365 6e74  ES.    represent
-00000490: 6174 696f 6e73 206f 6620 616c 6c20 7468  ations of all th
-000004a0: 6520 7661 6c69 6420 6d6f 6c65 6375 6c65  e valid molecule
-000004b0: 7320 7769 7468 696e 2061 2031 2d65 6469  s within a 1-edi
-000004c0: 7420 6e65 6967 6862 6f72 686f 6f64 2e20  t neighborhood. 
-000004d0: 4f70 7469 6f6e 616c 6c79 2c20 6120 6c69  Optionally, a li
-000004e0: 7374 206f 6620 626f 6f6c 6561 6e0a 2020  st of boolean.  
-000004f0: 2020 6675 6e63 7469 6f6e 7320 6361 6e20    functions can 
-00000500: 6265 2070 726f 7669 6465 6420 666f 7220  be provided for 
-00000510: 6060 6d6f 6c5f 6669 6c74 6572 7360 6020  ``mol_filters`` 
-00000520: 746f 2066 7572 7468 6572 206c 696d 6974  to further limit
-00000530: 2074 6865 206b 696e 6473 206f 6620 6d6f   the kinds of mo
-00000540: 6c65 6375 6c65 7320 696e 636c 7564 6564  lecules included
-00000550: 2069 6e20 7468 650a 2020 2020 7265 7375   in the.    resu
-00000560: 6c74 2e0a 0a20 2020 203a 7061 7261 6d20  lt...    :param 
-00000570: 736d 696c 6573 3a20 5468 6520 534d 494c  smiles: The SMIL
-00000580: 4553 2073 7472 696e 6720 7265 7072 6573  ES string repres
-00000590: 656e 7461 7469 6f6e 206f 660a 2020 2020  entation of.    
-000005a0: 3a70 6172 616d 2061 746f 6d5f 7661 6c65  :param atom_vale
-000005b0: 6e63 655f 6d61 703a 2041 2064 6963 7469  nce_map: A dicti
-000005c0: 6f6e 6172 792c 2077 686f 7365 206b 6579  onary, whose key
-000005d0: 7320 6172 6520 7374 7269 6e67 7320 7468  s are strings th
-000005e0: 6174 2069 6465 6e74 6966 7920 6174 6f6d  at identify atom
-000005f0: 2074 7970 6573 206f 6620 7468 6520 534d   types of the SM
-00000600: 494c 4553 0a20 2020 2020 2020 206e 6f74  ILES.        not
-00000610: 6174 696f 6e20 284f 2c20 4e2c 2043 6c20  ation (O, N, Cl 
-00000620: 2e2e 2e29 2061 6e64 2074 6865 2076 616c  ...) and the val
-00000630: 7565 7320 6172 6520 7468 6520 696e 7465  ues are the inte
-00000640: 6765 7220 7661 6c65 6e63 6520 6f66 2074  ger valence of t
-00000650: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
-00000660: 2061 746f 6d2e 204f 6e6c 790a 2020 2020   atom. Only.    
-00000670: 2020 2020 6174 6f6d 7320 7468 6174 2061      atoms that a
-00000680: 7265 206c 6973 7465 6420 696e 2074 6869  re listed in thi
-00000690: 7320 6469 6374 2077 696c 6c20 6265 2063  s dict will be c
-000006a0: 6f6e 7369 6465 7265 6420 666f 7220 6564  onsidered for ed
-000006b0: 6974 206f 7065 7261 7469 6f6e 7320 7375  it operations su
-000006c0: 6368 2061 7320 6164 6469 6e67 206f 720a  ch as adding or.
-000006d0: 2020 2020 2020 2020 7265 706c 6163 696e          replacin
-000006e0: 6720 616e 6420 6174 6f6d 210a 2020 2020  g and atom!.    
-000006f0: 3a70 6172 616d 206d 6f6c 5f66 696c 7465  :param mol_filte
-00000700: 7273 3a20 4120 6c69 7374 206f 6620 6675  rs: A list of fu
-00000710: 6e63 7469 6f6e 7320 7768 6963 6820 6561  nctions which ea
-00000720: 6368 2074 616b 6520 6120 4d6f 6c20 6f62  ch take a Mol ob
-00000730: 6a65 6374 2061 7320 696e 7075 7420 616e  ject as input an
-00000740: 6420 7265 7475 726e 2061 2062 6f6f 6c65  d return a boole
-00000750: 616e 2076 616c 7565 0a20 2020 2020 2020  an value.       
-00000760: 2074 6f20 6465 7465 726d 696e 6520 7768   to determine wh
-00000770: 6574 6865 7220 7468 6174 2061 746f 6d20  ether that atom 
-00000780: 7368 6f75 6c64 2062 6520 6578 636c 7564  should be exclud
-00000790: 6564 2028 5472 7565 2920 6f72 206e 6f74  ed (True) or not
-000007a0: 2028 4661 6c73 6529 2e0a 0a20 2020 203a   (False)...    :
-000007b0: 7265 7475 726e 733a 2041 206c 6973 7420  returns: A list 
-000007c0: 6f66 2073 7472 696e 6773 0a20 2020 2029  of strings.    )
-000007d0: 0372 1100 0000 da10 6174 6f6d 5f76 616c  .r......atom_val
-000007e0: 656e 6365 5f6d 6170 da18 6672 6565 5f76  ence_map..free_v
-000007f0: 616c 656e 6365 5f69 6e64 6963 6573 5f6d  alence_indices_m
-00000800: 6170 2902 7211 0000 0072 1e00 0000 2901  ap).r....r....).
-00000810: 7211 0000 0029 09da 0373 6574 7202 0000  r....)...setr...
-00000820: 00da 0d4d 6f6c 4672 6f6d 536d 696c 6573  ...MolFromSmiles
-00000830: da14 6765 745f 6672 6565 5f76 616c 656e  ..get_free_valen
-00000840: 6365 5f6d 6170 da06 7570 6461 7465 da18  ce_map..update..
-00000850: 6765 745f 7661 6c69 645f 6174 6f6d 5f61  get_valid_atom_a
-00000860: 6464 6974 696f 6e73 da18 6765 745f 7661  dditions..get_va
-00000870: 6c69 645f 626f 6e64 5f61 6464 6974 696f  lid_bond_additio
-00000880: 6e73 da17 6765 745f 7661 6c69 645f 626f  ns..get_valid_bo
-00000890: 6e64 5f72 656d 6f76 616c 73da 0661 7070  nd_removals..app
-000008a0: 656e 6429 0872 1a00 0000 721d 0000 0072  end).r....r....r
-000008b0: 1b00 0000 da0d 6e65 6967 6862 6f72 735f  ......neighbors_
-000008c0: 7365 7472 1100 0000 721e 0000 00da 126e  setr....r......n
-000008d0: 6569 6768 626f 7273 5f66 696c 7465 7265  eighbors_filtere
-000008e0: 64da 0466 756e 6372 1700 0000 7217 0000  d..funcr....r...
-000008f0: 0072 1800 0000 da10 6765 745f 6e65 6967  .r......get_neig
-00000900: 6862 6f72 686f 6f64 1e00 0000 7330 0000  hborhood....s0..
-00000910: 0006 160a 0208 0106 0202 0102 0102 0108  ................
-00000920: fd06 0602 0102 0108 fe06 0502 0108 ff04  ................
-00000930: 0808 010a 0108 0108 0102 0102 ff0c 0304  ................
-00000940: 0272 2a00 0000 e908 0000 00da 0b6d 6178  .r*..........max
-00000950: 5f76 616c 656e 6365 6302 0000 0000 0000  _valencec.......
-00000960: 0000 0000 0003 0000 0004 0000 0003 0000  ................
-00000970: 0073 3200 0000 6900 7d02 7400 6401 7c01  .s2...i.}.t.d.|.
-00000980: 8302 4400 5d0f 8900 8700 6601 6402 6403  ..D.].....f.d.d.
-00000990: 8408 7c00 a001 a100 4400 8301 7c02 8800  ..|.....D...|...
-000009a0: 3c00 7107 7c02 5300 2904 4e72 0700 0000  <.q.|.S.).Nr....
-000009b0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000009c0: 0004 0000 0013 0000 0073 2000 0000 6700  .........s ...g.
-000009d0: 7c00 5d0c 7d01 7c01 a000 a100 8800 6b05  |.].}.|.......k.
-000009e0: 7202 7c01 a001 a100 9102 7102 5300 7217  r.|.......q.S.r.
-000009f0: 0000 0029 02da 1047 6574 4e75 6d49 6d70  ...)...GetNumImp
-00000a00: 6c69 6369 7448 73da 0647 6574 4964 7829  licitHs..GetIdx)
-00000a10: 02da 022e 30da 0461 746f 6da9 01da 0169  ....0..atom....i
-00000a20: 7217 0000 0072 1800 0000 da0a 3c6c 6973  r....r......<lis
-00000a30: 7463 6f6d 703e 5b00 0000 730c 0000 0006  tcomp>[...s.....
-00000a40: 0002 020a 0102 fd06 0106 ff7a 2867 6574  ...........z(get
-00000a50: 5f66 7265 655f 7661 6c65 6e63 655f 6d61  _free_valence_ma
-00000a60: 702e 3c6c 6f63 616c 733e 2e3c 6c69 7374  p.<locals>.<list
-00000a70: 636f 6d70 3e29 02da 0572 616e 6765 da08  comp>)...range..
-00000a80: 4765 7441 746f 6d73 2903 7211 0000 0072  GetAtoms).r....r
-00000a90: 2c00 0000 da06 7265 7375 6c74 7217 0000  ,.....resultr...
-00000aa0: 0072 3100 0000 7218 0000 0072 2100 0000  .r1...r....r!...
-00000ab0: 5800 0000 730c 0000 0004 010e 010a 0106  X...s...........
-00000ac0: 020c fe04 0672 2100 0000 721d 0000 0072  .....r!...r....r
-00000ad0: 1e00 0000 6303 0000 0000 0000 0000 0000  ....c...........
-00000ae0: 000e 0000 0008 0000 0043 0000 0073 a400  .........C...s..
-00000af0: 0000 7400 8300 7d03 7401 6a02 6a03 7401  ..t...}.t.j.j.t.
-00000b00: 6a02 6a04 7401 6a02 6a05 6401 9c03 7d04  j.j.t.j.j.d...}.
-00000b10: 7c04 a006 a100 4400 5d3c 5c02 7d05 7d06  |.....D.]<\.}.}.
-00000b20: 7c02 7c05 1900 4400 5d33 7d07 7c01 a006  |.|...D.]3}.|...
-00000b30: a100 4400 5d2c 5c02 7d08 7d09 7401 a007  ..D.],\.}.}.t...
-00000b40: 7c00 a101 7d0a 7c0a a008 7401 a009 7c08  |...}.|...t...|.
-00000b50: a101 a101 7d0b 7c0a a00a 7c07 7c0b 7c06  ....}.|...|.|.|.
-00000b60: a103 0100 7401 6a0b 7c0a 6402 6403 8d02  ....t.j.|.d.d...
-00000b70: 7d0c 7c0c 7243 7121 7401 a00c 7c0a a101  }.|.rCq!t...|...
-00000b80: 7d0d 7c03 a00d 7c0d a101 0100 7121 711b  }.|...|.....q!q.
-00000b90: 7113 7c03 5300 2904 7ab6 0a20 2020 2047  q.|.S.).z..    G
-00000ba0: 6976 656e 2061 206d 6f6c 6563 756c 6520  iven a molecule 
-00000bb0: 6060 6d6f 6c60 602c 2074 6869 7320 6675  ``mol``, this fu
-00000bc0: 6e63 7469 6f6e 2077 696c 6c20 7265 7475  nction will retu
-00000bd0: 726e 2061 206c 6973 7420 6f66 2053 4d49  rn a list of SMI
-00000be0: 4c45 5320 7374 7269 6e67 7320 7468 6174  LES strings that
-00000bf0: 2072 6570 7265 7365 6e74 2076 616c 6964   represent valid
-00000c00: 0a20 2020 2061 746f 6d20 6164 6469 7469  .    atom additi
-00000c10: 6f6e 7320 746f 2074 6865 2062 6173 6520  ons to the base 
-00000c20: 6d6f 6c65 6375 6c65 2e0a 0a20 2020 203a  molecule...    :
-00000c30: 7265 7475 726e 733a 2041 206c 6973 7420  returns: A list 
-00000c40: 6f66 2073 7472 696e 6773 2e0a 2020 2020  of strings..    
-00000c50: a903 7207 0000 00e9 0200 0000 e903 0000  ..r.............
-00000c60: 0054 a901 da0b 6361 7463 6845 7272 6f72  .T....catchError
-00000c70: 7329 0e72 1f00 0000 7202 0000 00da 0842  s).r....r......B
-00000c80: 6f6e 6454 7970 65da 0653 494e 474c 45da  ondType..SINGLE.
-00000c90: 0644 4f55 424c 45da 0654 5249 504c 45da  .DOUBLE..TRIPLE.
-00000ca0: 0569 7465 6d73 da05 5257 4d6f 6cda 0741  .items..RWMol..A
-00000cb0: 6464 4174 6f6d da04 4174 6f6d da07 4164  ddAtom..Atom..Ad
-00000cc0: 6442 6f6e 64da 0b53 616e 6974 697a 654d  dBond..SanitizeM
-00000cd0: 6f6c da0b 4d6f 6c54 6f53 6d69 6c65 73da  ol..MolToSmiles.
-00000ce0: 0361 6464 290e 7211 0000 0072 1d00 0000  .add).r....r....
-00000cf0: 721e 0000 00da 0772 6573 756c 7473 da13  r......results..
-00000d00: 7661 6c75 655f 626f 6e64 5f74 7970 655f  value_bond_type_
-00000d10: 6d61 7072 3200 0000 da09 626f 6e64 5f74  mapr2.....bond_t
-00000d20: 7970 6572 3000 0000 da07 656c 656d 656e  yper0.....elemen
-00000d30: 74da 0776 616c 656e 6365 da07 6e65 775f  t..valence..new_
-00000d40: 6d6f 6cda 0369 6478 da13 7361 6e69 7469  mol..idx..saniti
-00000d50: 7a61 7469 6f6e 5f72 6573 756c 7472 1a00  zation_resultr..
-00000d60: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00000d70: 0072 2300 0000 6400 0000 7326 0000 0006  .r#...d...s&....
-00000d80: 0a06 0306 0106 0106 fd10 050c 0210 010a  ................
-00000d90: 0110 010e 010e 0104 0102 010a 020c 0102  ................
-00000da0: f702 ff04 0c72 2300 0000 6302 0000 0000  .....r#...c.....
-00000db0: 0000 0000 0000 0010 0000 0007 0000 0043  ...............C
-00000dc0: 0000 0073 3601 0000 7400 8300 7d02 6401  ...s6...t...}.d.
-00000dd0: 7401 6a02 6a03 7401 6a02 6a04 7401 6a02  t.j.j.t.j.j.t.j.
-00000de0: 6a05 6402 9c04 7d03 7406 7c03 8301 7d04  j.d...}.t.|...}.
-00000df0: 7c01 a007 a100 4400 5d80 5c02 7d05 7d06  |.....D.].\.}.}.
-00000e00: 7408 a009 7c06 6403 a102 4400 5d75 5c02  t...|.d...D.]u\.
-00000e10: 7d07 7d08 7c00 a00a 7c07 a101 a00b a100  }.}.|...|.......
-00000e20: 7235 7c00 a00a 7c08 a101 a00b a100 7235  r5|...|.......r5
-00000e30: 7122 7401 a00c 7c00 a101 a00d 7c07 7c08  q"t...|.....|.|.
-00000e40: a102 7d09 7401 a00e 7c00 a101 7d0a 7401  ..}.t...|...}.t.
-00000e50: 6a0f 7c0a 6404 6405 8d02 0100 7c09 6401  j.|.d.d.....|.d.
-00000e60: 7501 7278 7c09 a010 a100 7d0b 7c0b 7c03  u.rx|.....}.|.|.
-00000e70: a011 a100 7601 7259 7122 7c04 7c0b 1900  ....v.rYq"|.|...
-00000e80: 7d0c 7c0c 7c05 3700 7d0c 7c0c 6406 6b04  }.|.|.7.}.|.d.k.
-00000e90: 7266 7122 7c09 a012 a100 7d0d 7c09 a013  rfq"|.....}.|...
-00000ea0: 7c03 7c0c 1900 a101 0100 7c0a a014 7c0d  |.|.......|...|.
-00000eb0: 7c09 a102 0100 6e0b 7c03 7c05 1900 7d0b  |.....n.|.|...}.
-00000ec0: 7c0a a015 7c07 7c08 7c0b a103 0100 7401  |...|.|.|.....t.
-00000ed0: 6a16 7c0a 6404 6407 8d02 7d0e 7c0e 728d  j.|.d.d...}.|.r.
-00000ee0: 7122 7401 a017 7c0a a101 7d0f 7c02 a018  q"t...|...}.|...
-00000ef0: 7c0f a101 0100 7122 7118 7c02 5300 2908  |.....q"q.|.S.).
-00000f00: 6140 0300 000a 2020 2020 4769 7665 6e20  a@....    Given 
-00000f10: 6120 6d6f 6c65 6375 6c65 2060 606d 6f6c  a molecule ``mol
-00000f20: 6060 2c20 7468 6973 2066 756e 6374 696f  ``, this functio
-00000f30: 6e20 7769 6c6c 2072 6574 7572 6e20 6120  n will return a 
-00000f40: 6c69 7374 206f 6620 534d 494c 4553 2073  list of SMILES s
-00000f50: 7472 696e 6773 2077 6869 6368 2072 6573  trings which res
-00000f60: 756c 7473 2066 726f 6d20 7661 6c69 640a  ults from valid.
-00000f70: 2020 2020 626f 6e64 2061 6464 6974 696f      bond additio
-00000f80: 6e73 2074 6f20 7468 6174 2062 6173 6520  ns to that base 
-00000f90: 6d6f 6c65 6375 6c65 2e20 5661 6c69 6420  molecule. Valid 
-00000fa0: 626f 6e64 2061 6464 6974 696f 6e73 2069  bond additions i
-00000fb0: 6e20 7468 6973 2063 6173 6520 6172 6520  n this case are 
-00000fc0: 6465 6669 6e65 6420 6173 2061 6c6c 6f77  defined as allow
-00000fd0: 6564 2069 6e0a 2020 2020 7465 726d 7320  ed in.    terms 
-00000fe0: 6f66 2074 6865 2061 746f 6d20 7661 6c65  of the atom vale
-00000ff0: 6e63 6573 2e20 626f 6e64 2061 6464 6974  nces. bond addit
-00001000: 696f 6e73 206d 6179 2063 6f6e 6e65 6374  ions may connect
-00001010: 2074 776f 2061 746f 6d73 2077 6869 6368   two atoms which
-00001020: 2061 7265 206e 6f74 2079 6574 2064 6972   are not yet dir
-00001030: 6563 746c 7920 636f 6e6e 6563 7465 640a  ectly connected.
-00001040: 2020 2020 6f72 2075 7067 7261 6465 2061      or upgrade a
-00001050: 6e20 6578 6973 7469 6e67 2062 6f6e 6420  n existing bond 
-00001060: 2873 696e 676c 6520 746f 2064 6f75 626c  (single to doubl
-00001070: 6529 2e0a 0a20 2020 2041 6c73 6f20 6469  e)...    Also di
-00001080: 7361 6c6c 6f77 6564 2061 7265 2062 6f6e  sallowed are bon
-00001090: 6473 2062 6574 7765 656e 2074 776f 2061  ds between two a
-000010a0: 746f 6d73 2077 6869 6368 2061 7265 2074  toms which are t
-000010b0: 6865 6d73 656c 7665 7320 616c 7265 6164  hemselves alread
-000010c0: 7920 7061 7274 206f 6620 6120 7269 6e67  y part of a ring
-000010d0: 2e0a 0a20 2020 203a 7061 7261 6d20 6d6f  ...    :param mo
-000010e0: 6c3a 2054 6865 2062 6173 6520 6d6f 6c65  l: The base mole
-000010f0: 6375 6c65 0a20 2020 203a 7061 7261 6d20  cule.    :param 
-00001100: 6672 6565 5f76 616c 656e 6365 5f69 6e64  free_valence_ind
-00001110: 6963 6573 5f6d 6170 3a20 4120 6469 6374  ices_map: A dict
-00001120: 2077 686f 7365 206b 6579 7320 6172 6520   whose keys are 
-00001130: 696e 7465 6765 7273 2073 7461 7274 696e  integers startin
-00001140: 6720 6672 6f6d 2030 2e20 5448 6520 6b65  g from 0. THe ke
-00001150: 7920 7661 6c75 6573 0a20 2020 2020 2020  y values.       
-00001160: 2072 6570 7265 7365 6e74 2074 6865 202a   represent the *
-00001170: 6672 6565 206e 756d 6265 7220 6f66 2076  free number of v
-00001180: 616c 656e 6365 732a 2e20 5468 6520 7661  alences*. The va
-00001190: 6c75 6573 2061 7265 206c 6973 7473 206f  lues are lists o
-000011a0: 6620 6174 6f6d 2069 6e64 6963 6573 2077  f atom indices w
-000011b0: 6865 7265 2065 6163 6820 6174 6f6d 2069  here each atom i
-000011c0: 6e0a 2020 2020 2020 2020 7468 6520 6c69  n.        the li
-000011d0: 7374 2068 6173 2074 6f20 6861 7665 2074  st has to have t
-000011e0: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
-000011f0: 206e 756d 6265 7220 6f66 2066 7265 6520   number of free 
-00001200: 7661 6c65 6e63 6573 2067 6976 656e 2062  valences given b
-00001210: 7920 7468 6520 6469 6374 206b 6579 2e0a  y the dict key..
-00001220: 0a20 2020 203a 7265 7475 726e 733a 2041  .    :returns: A
-00001230: 206c 6973 7420 6f66 2073 7472 696e 6773   list of strings
-00001240: 0a20 2020 204e a904 7201 0000 0072 0700  .    N..r....r..
-00001250: 0000 7238 0000 0072 3900 0000 7238 0000  ..r8...r9...r8..
-00001260: 0054 a901 da12 636c 6561 7241 726f 6d61  .T....clearAroma
-00001270: 7469 6346 6c61 6773 7239 0000 0072 3a00  ticFlagsr9...r:.
-00001280: 0000 2919 721f 0000 0072 0200 0000 723c  ..).r....r....r<
-00001290: 0000 0072 3d00 0000 723e 0000 0072 3f00  ...r=...r>...r?.
-000012a0: 0000 7203 0000 0072 4000 0000 da09 6974  ..r....r@.....it
-000012b0: 6572 746f 6f6c 73da 0c63 6f6d 6269 6e61  ertools..combina
-000012c0: 7469 6f6e 73da 0e47 6574 4174 6f6d 5769  tions..GetAtomWi
-000012d0: 7468 4964 78da 0849 7349 6e52 696e 67da  thIdx..IsInRing.
-000012e0: 034d 6f6c da13 4765 7442 6f6e 6442 6574  .Mol..GetBondBet
-000012f0: 7765 656e 4174 6f6d 7372 4100 0000 da08  weenAtomsrA.....
-00001300: 4b65 6b75 6c69 7a65 da0b 4765 7442 6f6e  Kekulize..GetBon
-00001310: 6454 7970 65da 0676 616c 7565 7372 2e00  dType..valuesr..
-00001320: 0000 da0b 5365 7442 6f6e 6454 7970 65da  ....SetBondType.
-00001330: 0b52 6570 6c61 6365 426f 6e64 7244 0000  .ReplaceBondrD..
-00001340: 0072 4500 0000 7246 0000 0072 4700 0000  .rE...rF...rG...
-00001350: 2910 7211 0000 0072 1e00 0000 7248 0000  ).r....r....rH..
-00001360: 0072 4900 0000 da13 626f 6e64 5f74 7970  .rI.....bond_typ
-00001370: 655f 7661 6c75 655f 6d61 7072 4c00 0000  e_value_maprL...
-00001380: da05 6174 6f6d 73da 0561 746f 6d31 da05  ..atoms..atom1..
-00001390: 6174 6f6d 32da 0462 6f6e 6472 4d00 0000  atom2..bondrM...
-000013a0: 724a 0000 00da 0a62 6f6e 645f 7661 6c75  rJ.....bond_valu
-000013b0: 65da 0569 6e64 6578 724f 0000 0072 1a00  e..indexrO...r..
-000013c0: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
-000013d0: 0072 2400 0000 8600 0000 7344 0000 0006  .r$.......sD....
-000013e0: 1202 0306 0106 0106 0106 fc08 0610 0214  ................
-000013f0: 011c 0302 0112 020a 010e 0208 0108 010c  ................
-00001400: 0102 0108 0208 0108 0102 0108 020e 010e  ................
-00001410: 0108 030e 010e 0204 0102 010a 020c 0102  ................
-00001420: df04 2372 2400 0000 6301 0000 0000 0000  ..#r$...c.......
-00001430: 0000 0000 000f 0000 0007 0000 0043 0000  .............C..
-00001440: 0073 6201 0000 7400 8300 7d01 6401 7401  .sb...t...}.d.t.
-00001450: 6a02 6a03 7401 6a02 6a04 7401 6a02 6a05  j.j.t.j.j.t.j.j.
-00001460: 6402 9c04 7d02 7406 7c02 8301 7d03 6403  d...}.t.|...}.d.
-00001470: 4400 5d98 7d04 7c00 a007 a100 4400 5d91  D.].}.|.....D.].
-00001480: 7d05 7c05 a008 a100 7c05 a009 a100 0202  }.|.....|.......
-00001490: 7d06 7d07 7401 a00a 7c00 a101 a00b 7c06  }.}.t...|.....|.
-000014a0: 7c07 a102 7d05 7c05 a00c a100 7d08 7c08  |...}.|.....}.|.
-000014b0: 7c02 a00d a100 7601 723b 711c 7401 a00e  |.....v.r;q.t...
-000014c0: 7c00 a101 7d09 7401 6a0f 7c09 6404 6405  |...}.t.j.|.d.d.
-000014d0: 8d02 0100 7c03 7c08 1900 7d0a 7c0a 7c04  ....|.|...}.|.|.
-000014e0: 3800 7d0a 7c0a 6406 6b02 725a 7c09 a010  8.}.|.d.k.rZ|...
-000014f0: 7c06 7c07 a102 0100 6e17 7c0a 6406 6b04  |.|.....n.|.d.k.
-00001500: 7270 7c05 a011 7c02 7c0a 1900 a101 0100  rp|...|.|.......
-00001510: 7c05 a012 a100 7d0b 7c09 a013 7c0b 7c05  |.....}.|...|.|.
-00001520: a102 0100 6e01 711c 7401 6a14 7c09 6404  ....n.q.t.j.|.d.
-00001530: 6407 8d02 7d0c 7c0c 727b 711c 7401 a015  d...}.|.r{q.t...
-00001540: 7c09 a101 7d0d 6408 7c0d 7600 72a8 7416  |...}.d.|.v.r.t.
-00001550: 7c0d a017 6408 a101 7418 6409 8d02 7d0e  |...d...t.d...}.
-00001560: 7418 7c0e 6406 1900 8301 640a 6b04 7296  t.|.d.....d.k.r.
-00001570: 711c 7418 7401 a019 7c0e 640a 1900 a101  q.t.t...|.d.....
-00001580: a01a a100 8301 640b 6b00 72a4 711c 7c0e  ......d.k.r.q.|.
-00001590: 640a 1900 7d0d 7c01 a01b 7c0d a101 0100  d...}.|...|.....
-000015a0: 711c 7116 7c01 5300 290c 61a2 0100 000a  q.q.|.S.).a.....
-000015b0: 2020 2020 4769 7665 6e20 6120 6d6f 6c65      Given a mole
-000015c0: 6375 6c65 2060 606d 6f6c 6060 2c20 7468  cule ``mol``, th
-000015d0: 6973 2066 756e 6374 696f 6e20 7769 6c6c  is function will
-000015e0: 2072 6574 7572 6e20 6120 6c69 7374 206f   return a list o
-000015f0: 6620 534d 494c 4553 2073 7472 696e 6773  f SMILES strings
-00001600: 2077 6869 6368 2072 6570 7265 7365 6e74   which represent
-00001610: 2076 616c 6964 0a20 2020 2062 6f6e 6420   valid.    bond 
-00001620: 7265 6d6f 7661 6c73 2e20 4120 626f 6e64  removals. A bond
-00001630: 2072 656d 6f76 616c 2069 7320 6569 7468   removal is eith
-00001640: 6572 2061 2064 6f77 6e67 7261 6465 206f  er a downgrade o
-00001650: 6620 616e 2065 7869 7374 696e 6720 626f  f an existing bo
-00001660: 6e64 2028 652e 672e 2064 6f75 626c 6520  nd (e.g. double 
-00001670: 746f 2073 696e 676c 6529 206f 7220 7468  to single) or th
-00001680: 650a 2020 2020 7265 6d6f 7661 6c20 6f66  e.    removal of
-00001690: 2061 2073 696e 676c 6520 626f 6e64 2077   a single bond w
-000016a0: 6869 6368 2077 6f75 6c64 206d 6561 6e20  hich would mean 
-000016b0: 746f 2064 6973 636f 6e6e 6563 7420 6174  to disconnect at
-000016c0: 206d 6f73 7420 6120 7369 6e67 6c65 2061   most a single a
-000016d0: 746f 6d20 6672 6f6d 2074 6865 2072 6573  tom from the res
-000016e0: 7420 6f66 2074 6865 0a20 2020 206d 6f6c  t of the.    mol
-000016f0: 6563 756c 6521 0a0a 2020 2020 3a70 6172  ecule!..    :par
-00001700: 616d 206d 6f6c 3a20 5468 6520 6261 7365  am mol: The base
-00001710: 206d 6f6c 6563 756c 6520 666f 7220 7468   molecule for th
-00001720: 6520 7265 6d6f 7661 6c73 2e0a 0a20 2020  e removals...   
-00001730: 203a 7265 7475 726e 733a 2041 206c 6973   :returns: A lis
-00001740: 7420 6f66 2073 7472 696e 6773 0a20 2020  t of strings.   
-00001750: 204e 7250 0000 0072 3700 0000 5472 5100   NrP...r7...TrQ.
-00001760: 0000 7201 0000 0072 3a00 0000 da01 2e29  ..r....r:......)
-00001770: 01da 036b 6579 7207 0000 0072 3800 0000  ...keyr....r8...
-00001780: 291c 721f 0000 0072 0200 0000 723c 0000  ).r....r....r<..
-00001790: 0072 3d00 0000 723e 0000 0072 3f00 0000  .r=...r>...r?...
-000017a0: 7203 0000 00da 0847 6574 426f 6e64 73da  r......GetBonds.
-000017b0: 0f47 6574 4265 6769 6e41 746f 6d49 6478  .GetBeginAtomIdx
-000017c0: da0d 4765 7445 6e64 4174 6f6d 4964 7872  ..GetEndAtomIdxr
-000017d0: 5700 0000 7258 0000 0072 5a00 0000 725b  W...rX...rZ...r[
-000017e0: 0000 0072 4100 0000 7259 0000 00da 0a52  ...rA...rY.....R
-000017f0: 656d 6f76 6542 6f6e 6472 5c00 0000 722e  emoveBondr\...r.
-00001800: 0000 0072 5d00 0000 7245 0000 0072 4600  ...r]...rE...rF.
-00001810: 0000 da06 736f 7274 6564 da05 7370 6c69  ....sorted..spli
-00001820: 74da 036c 656e 7220 0000 0072 3500 0000  t..lenr ...r5...
-00001830: 7247 0000 0029 0f72 1100 0000 7248 0000  rG...).r....rH..
-00001840: 0072 4900 0000 725e 0000 0072 4c00 0000  .rI...r^...rL...
-00001850: 7262 0000 0072 6000 0000 7261 0000 0072  rb...r`...ra...r
-00001860: 4a00 0000 724d 0000 0072 6300 0000 7264  J...rM...rc...rd
-00001870: 0000 0072 4f00 0000 721a 0000 00da 0570  ...rO...r......p
-00001880: 6172 7473 7217 0000 0072 1700 0000 7218  artsr....r....r.
-00001890: 0000 0072 2500 0000 c900 0000 734e 0000  ...r%.......sN..
-000018a0: 0006 0c02 0306 0106 0106 0106 fc08 0608  ................
-000018b0: 020c 0112 0112 0108 020c 0102 010a 020e  ................
-000018c0: 0108 0208 0108 020e 0108 020e 0108 010e  ................
-000018d0: 0102 030e 0204 0102 010a 0208 0112 0110  ................
-000018e0: 0102 011a 0602 0108 020c 0202 d404 2e72  ...............r
-000018f0: 2500 0000 2901 7210 0000 0029 0172 2b00  %...).r....).r+.
-00001900: 0000 2918 7253 0000 00da 0674 7970 696e  ..).rS.....typin
-00001910: 67da 0174 da05 7264 6b69 7472 0200 0000  g..t..rdkitr....
-00001920: da19 7667 645f 636f 756e 7465 7266 6163  ..vgd_counterfac
-00001930: 7475 616c 732e 7574 696c 7372 0300 0000  tuals.utilsr....
-00001940: da18 4445 4641 554c 545f 4154 4f4d 5f56  ..DEFAULT_ATOM_V
-00001950: 414c 454e 4345 5f4d 4150 7257 0000 00da  ALENCE_MAPrW....
-00001960: 0373 7472 7219 0000 00da 0853 6571 7565  .strr......Seque
-00001970: 6e63 65da 0843 616c 6c61 626c 65da 0462  nce..Callable..b
-00001980: 6f6f 6cda 044c 6973 7472 2a00 0000 da03  ool..Listr*.....
-00001990: 696e 74da 0464 6963 7472 2100 0000 da04  int..dictr!.....
-000019a0: 4469 6374 da03 5365 7472 2300 0000 7224  Dict..Setr#...r$
-000019b0: 0000 0072 2500 0000 7217 0000 0072 1700  ...r%...r....r..
-000019c0: 0000 7217 0000 0072 1800 0000 da08 3c6d  ..r....r......<m
-000019d0: 6f64 756c 653e 0100 0000 734a 0000 0008  odule>....sJ....
-000019e0: 0008 010c 010c 0202 0402 0102 0102 0102  ................
-000019f0: 0102 0102 0106 f916 0c02 0b02 0202 ff08  ................
-00001a00: fe16 0202 fe08 050a fb1a 3a08 0c0c 0102  ..........:.....
-00001a10: ff12 0202 fe08 030a fd08 2212 0102 ff08  ..........".....
-00001a20: 020a fe08 4308 010e ff                   ....C....
+00000050: 6d06 5a06 0100 6404 6405 6406 6407 6408  m.Z...d.d.d.d.d.
+00000060: 6406 6409 9c06 5a07 6423 640b 6504 6a08  d.d...Z.d#d.e.j.
+00000070: 640c 6509 6604 640d 640e 8405 5a0a 6424  d.e.f.d.d...Z.d$
+00000080: 640b 6504 6a08 640c 6509 6604 6410 6411  d.e.j.d.e.f.d.d.
+00000090: 8405 5a0b 6507 650a 650b 6602 6602 6412  ..Z.e.e.e.f.f.d.
+000000a0: 6509 6413 6502 6a0c 6502 6a0d 6504 6a08  e.d.e.j.e.j.e.j.
+000000b0: 6701 650e 6602 1900 1900 6414 6502 6a0f  g.e.f.....d.e.j.
+000000c0: 6509 1900 6606 6415 6416 8405 5a10 6425  e...f.d.d...Z.d%
+000000d0: 640b 6504 6a08 6418 6511 6414 6512 6606  d.e.j.d.e.d.e.f.
+000000e0: 6419 641a 8405 5a13 640b 6504 6a08 641b  d.d...Z.d.e.j.d.
+000000f0: 6502 6a14 6509 6511 6602 1900 641c 6502  e.j.e.e.f...d.e.
+00000100: 6a14 6511 6502 6a0f 6511 1900 6602 1900  j.e.e.j.e...f...
+00000110: 6414 6502 6a15 6509 1900 6608 641d 641e  d.e.j.e...f.d.d.
+00000120: 8404 5a16 640b 6504 6a08 641c 6502 6a14  ..Z.d.e.j.d.e.j.
+00000130: 6511 6502 6a0f 6511 1900 6602 1900 6414  e.e.j.e...f...d.
+00000140: 6502 6a15 6509 1900 6606 641f 6420 8404  e.j.e...f.d.d ..
+00000150: 5a17 640b 6504 6a08 6414 6502 6a15 6509  Z.d.e.j.d.e.j.e.
+00000160: 1900 6604 6421 6422 8404 5a18 6401 5300  ..f.d!d"..Z.d.S.
+00000170: 2926 e900 0000 004e 2901 da04 4368 656d  )&.....N)...Chem
+00000180: 2901 da0b 696e 7665 7274 5f64 6963 74e9  )...invert_dict.
+00000190: 0400 0000 e905 0000 00e9 0600 0000 e901  ................
+000001a0: 0000 00e9 0700 0000 2906 da01 43da 014e  ........)...C..N
+000001b0: da01 4fda 0146 da02 436c da01 53fa 0e2a  ..O..F..Cl..S..*
+000001c0: 313d 2a2a 323d 2a2a 3d2a 312a 32da 036d  1=**2=**=*1*2..m
+000001d0: 6f6c da07 7061 7474 6572 6e63 0200 0000  ol..patternc....
+000001e0: 0000 0000 0000 0000 0400 0000 0300 0000  ................
+000001f0: 4300 0000 f318 0000 0074 00a0 017c 01a1  C........t...|..
+00000200: 017d 027c 00a0 027c 02a1 017d 037c 0353  .}.|...|...}.|.S
+00000210: 0029 017a 830a 2020 2020 4368 6563 6b73  .).z..    Checks
+00000220: 2069 6620 7468 6520 6769 7665 6e20 6d6f   if the given mo
+00000230: 6c65 6375 6c65 2060 606d 6f6c 6060 2069  lecule ``mol`` i
+00000240: 7320 6120 6272 6964 6765 2068 6561 6420  s a bridge head 
+00000250: 6361 7262 6f6e 2073 7472 7563 7475 7265  carbon structure
+00000260: 2077 6869 6368 2061 7070 6172 656e 746c   which apparentl
+00000270: 7920 646f 6573 206e 6f74 0a20 2020 2061  y does not.    a
+00000280: 7070 6561 7220 696e 2063 6865 6d69 7374  ppear in chemist
+00000290: 7279 2e0a 2020 2020 a903 7202 0000 00da  ry..    ..r.....
+000002a0: 0d4d 6f6c 4672 6f6d 536d 6172 7473 da11  .MolFromSmarts..
+000002b0: 4861 7353 7562 7374 7275 6374 4d61 7463  HasSubstructMatc
+000002c0: 68a9 0472 1000 0000 7211 0000 00da 0673  h..r....r......s
+000002d0: 6d61 7274 73da 0869 735f 6d61 7463 68a9  marts..is_match.
+000002e0: 0072 1900 0000 fa54 2f6d 6564 6961 2f73  .r.....T/media/s
+000002f0: 7364 2f50 726f 6772 616d 6d69 6e67 2f76  sd/Programming/v
+00000300: 6764 5f63 6f75 6e74 6572 6661 6374 7561  gd_counterfactua
+00000310: 6c73 2f76 6764 5f63 6f75 6e74 6572 6661  ls/vgd_counterfa
+00000320: 6374 7561 6c73 2f67 656e 6572 6174 652f  ctuals/generate/
+00000330: 6d6f 6c65 6375 6c65 732e 7079 da15 6973  molecules.py..is
+00000340: 5f62 7269 6467 655f 6865 6164 5f63 6172  _bridge_head_car
+00000350: 626f 6e14 0000 0073 0600 0000 0a05 0a01  bon....s........
+00000360: 0401 721b 0000 00da 0353 4e4e 6302 0000  ..r......SNNc...
+00000370: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+00000380: 0043 0000 0072 1200 0000 2901 4e72 1300  .C...r....).Nr..
+00000390: 0000 7216 0000 0072 1900 0000 7219 0000  ..r....r....r...
+000003a0: 0072 1a00 0000 da1b 6973 5f6e 6974 726f  .r......is_nitro
+000003b0: 6765 6e5f 6e69 7472 6f67 656e 5f73 756c  gen_nitrogen_sul
+000003c0: 6675 721e 0000 0073 0600 0000 0a01 0a01  fur....s........
+000003d0: 0401 721d 0000 00da 0673 6d69 6c65 73da  ..r......smiles.
+000003e0: 0b6d 6f6c 5f66 696c 7465 7273 da06 7265  .mol_filters..re
+000003f0: 7475 726e 6303 0000 0000 0000 0000 0000  turnc...........
+00000400: 0006 0000 0007 0000 0003 0000 0073 9400  .............s..
+00000410: 0000 7400 8300 7d03 7401 a002 7c00 a101  ..t...}.t...|...
+00000420: 8900 7403 8800 8301 7d04 7c03 a004 7405  ..t.....}.|...t.
+00000430: 8800 7c01 7c04 6401 8d03 a101 0100 7c03  ..|.|.d.......|.
+00000440: a004 7406 8800 7c04 6402 8d02 a101 0100  ..t...|.d.......
+00000450: 7c03 a004 7407 8800 6403 8d01 a101 0100  |...t...d.......
+00000460: 6700 7d05 7c03 4400 5d1c 7d00 7401 a002  g.}.|.D.].}.t...
+00000470: 7c00 a101 8900 7408 8700 6601 6404 6405  |.....t...f.d.d.
+00000480: 8408 7c02 4400 8301 8301 7242 7409 6406  ..|.D.....rBt.d.
+00000490: 8301 0100 712b 7c05 a00a 7c00 a101 0100  ....q+|...|.....
+000004a0: 712b 7c05 5300 2907 61b1 0300 000a 2020  q+|.S.).a.....  
+000004b0: 2020 4769 7665 6e20 6120 6060 736d 696c    Given a ``smil
+000004c0: 6573 6060 2072 6570 7265 7365 6e74 6174  es`` representat
+000004d0: 696f 6e20 6f66 2061 206d 6f6c 6563 756c  ion of a molecul
+000004e0: 652c 2074 6869 7320 6675 6e63 7469 6f6e  e, this function
+000004f0: 2077 696c 6c20 7265 7475 726e 2061 206c   will return a l
+00000500: 6973 7420 6f66 2074 6865 2053 4d49 4c45  ist of the SMILE
+00000510: 530a 2020 2020 7265 7072 6573 656e 7461  S.    representa
+00000520: 7469 6f6e 7320 6f66 2061 6c6c 2074 6865  tions of all the
+00000530: 2076 616c 6964 206d 6f6c 6563 756c 6573   valid molecules
+00000540: 2077 6974 6869 6e20 6120 312d 6564 6974   within a 1-edit
+00000550: 206e 6569 6768 626f 7268 6f6f 642e 204f   neighborhood. O
+00000560: 7074 696f 6e61 6c6c 792c 2061 206c 6973  ptionally, a lis
+00000570: 7420 6f66 2062 6f6f 6c65 616e 0a20 2020  t of boolean.   
+00000580: 2066 756e 6374 696f 6e73 2063 616e 2062   functions can b
+00000590: 6520 7072 6f76 6964 6564 2066 6f72 2060  e provided for `
+000005a0: 606d 6f6c 5f66 696c 7465 7273 6060 2074  `mol_filters`` t
+000005b0: 6f20 6675 7274 6865 7220 6c69 6d69 7420  o further limit 
+000005c0: 7468 6520 6b69 6e64 7320 6f66 206d 6f6c  the kinds of mol
+000005d0: 6563 756c 6573 2069 6e63 6c75 6465 6420  ecules included 
+000005e0: 696e 2074 6865 0a20 2020 2072 6573 756c  in the.    resul
+000005f0: 742e 0a0a 2020 2020 3a70 6172 616d 2073  t...    :param s
+00000600: 6d69 6c65 733a 2054 6865 2053 4d49 4c45  miles: The SMILE
+00000610: 5320 7374 7269 6e67 2072 6570 7265 7365  S string represe
+00000620: 6e74 6174 696f 6e20 6f66 0a20 2020 203a  ntation of.    :
+00000630: 7061 7261 6d20 6174 6f6d 5f76 616c 656e  param atom_valen
+00000640: 6365 5f6d 6170 3a20 4120 6469 6374 696f  ce_map: A dictio
+00000650: 6e61 7279 2c20 7768 6f73 6520 6b65 7973  nary, whose keys
+00000660: 2061 7265 2073 7472 696e 6773 2074 6861   are strings tha
+00000670: 7420 6964 656e 7469 6679 2061 746f 6d20  t identify atom 
+00000680: 7479 7065 7320 6f66 2074 6865 2053 4d49  types of the SMI
+00000690: 4c45 530a 2020 2020 2020 2020 6e6f 7461  LES.        nota
+000006a0: 7469 6f6e 2028 4f2c 204e 2c20 436c 202e  tion (O, N, Cl .
+000006b0: 2e2e 2920 616e 6420 7468 6520 7661 6c75  ..) and the valu
+000006c0: 6573 2061 7265 2074 6865 2069 6e74 6567  es are the integ
+000006d0: 6572 2076 616c 656e 6365 206f 6620 7468  er valence of th
+000006e0: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
+000006f0: 6174 6f6d 2e20 4f6e 6c79 0a20 2020 2020  atom. Only.     
+00000700: 2020 2061 746f 6d73 2074 6861 7420 6172     atoms that ar
+00000710: 6520 6c69 7374 6564 2069 6e20 7468 6973  e listed in this
+00000720: 2064 6963 7420 7769 6c6c 2062 6520 636f   dict will be co
+00000730: 6e73 6964 6572 6564 2066 6f72 2065 6469  nsidered for edi
+00000740: 7420 6f70 6572 6174 696f 6e73 2073 7563  t operations suc
+00000750: 6820 6173 2061 6464 696e 6720 6f72 0a20  h as adding or. 
+00000760: 2020 2020 2020 2072 6570 6c61 6369 6e67         replacing
+00000770: 2061 6e64 2061 746f 6d21 0a20 2020 203a   and atom!.    :
+00000780: 7061 7261 6d20 6d6f 6c5f 6669 6c74 6572  param mol_filter
+00000790: 733a 2041 206c 6973 7420 6f66 2066 756e  s: A list of fun
+000007a0: 6374 696f 6e73 2077 6869 6368 2065 6163  ctions which eac
+000007b0: 6820 7461 6b65 2061 204d 6f6c 206f 626a  h take a Mol obj
+000007c0: 6563 7420 6173 2069 6e70 7574 2061 6e64  ect as input and
+000007d0: 2072 6574 7572 6e20 6120 626f 6f6c 6561   return a boolea
+000007e0: 6e20 7661 6c75 650a 2020 2020 2020 2020  n value.        
+000007f0: 746f 2064 6574 6572 6d69 6e65 2077 6865  to determine whe
+00000800: 7468 6572 2074 6861 7420 6174 6f6d 2073  ther that atom s
+00000810: 686f 756c 6420 6265 2065 7863 6c75 6465  hould be exclude
+00000820: 6420 2854 7275 6529 206f 7220 6e6f 7420  d (True) or not 
+00000830: 2846 616c 7365 292e 0a0a 2020 2020 3a72  (False)...    :r
+00000840: 6574 7572 6e73 3a20 4120 6c69 7374 206f  eturns: A list o
+00000850: 6620 7374 7269 6e67 730a 2020 2020 2903  f strings.    ).
+00000860: 7210 0000 00da 1061 746f 6d5f 7661 6c65  r......atom_vale
+00000870: 6e63 655f 6d61 70da 1866 7265 655f 7661  nce_map..free_va
+00000880: 6c65 6e63 655f 696e 6469 6365 735f 6d61  lence_indices_ma
+00000890: 7029 0272 1000 0000 7222 0000 00a9 0172  p).r....r".....r
+000008a0: 1000 0000 6301 0000 0000 0000 0000 0000  ....c...........
+000008b0: 0002 0000 0004 0000 0013 0000 0073 1400  .............s..
+000008c0: 0000 6700 7c00 5d06 7d01 7c01 8800 8301  ..g.|.].}.|.....
+000008d0: 9102 7102 5300 7219 0000 0072 1900 0000  ..q.S.r....r....
+000008e0: 2902 da02 2e30 da04 6675 6e63 7223 0000  )....0..funcr#..
+000008f0: 0072 1900 0000 721a 0000 00da 0a3c 6c69  .r....r......<li
+00000900: 7374 636f 6d70 3e56 0000 0073 0200 0000  stcomp>V...s....
+00000910: 1400 7a24 6765 745f 6e65 6967 6862 6f72  ..z$get_neighbor
+00000920: 686f 6f64 2e3c 6c6f 6361 6c73 3e2e 3c6c  hood.<locals>.<l
+00000930: 6973 7463 6f6d 703e 5429 0bda 0373 6574  istcomp>T)...set
+00000940: 7202 0000 00da 0d4d 6f6c 4672 6f6d 536d  r......MolFromSm
+00000950: 696c 6573 da14 6765 745f 6672 6565 5f76  iles..get_free_v
+00000960: 616c 656e 6365 5f6d 6170 da06 7570 6461  alence_map..upda
+00000970: 7465 da18 6765 745f 7661 6c69 645f 6174  te..get_valid_at
+00000980: 6f6d 5f61 6464 6974 696f 6e73 da18 6765  om_additions..ge
+00000990: 745f 7661 6c69 645f 626f 6e64 5f61 6464  t_valid_bond_add
+000009a0: 6974 696f 6e73 da17 6765 745f 7661 6c69  itions..get_vali
+000009b0: 645f 626f 6e64 5f72 656d 6f76 616c 73da  d_bond_removals.
+000009c0: 0361 6e79 da05 7072 696e 74da 0661 7070  .any..print..app
+000009d0: 656e 6429 0672 1e00 0000 7221 0000 0072  end).r....r!...r
+000009e0: 1f00 0000 da0d 6e65 6967 6862 6f72 735f  ......neighbors_
+000009f0: 7365 7472 2200 0000 da12 6e65 6967 6862  setr".....neighb
+00000a00: 6f72 735f 6669 6c74 6572 6564 7219 0000  ors_filteredr...
+00000a10: 0072 2300 0000 721a 0000 00da 1067 6574  .r#...r......get
+00000a20: 5f6e 6569 6768 626f 7268 6f6f 6424 0000  _neighborhood$..
+00000a30: 0073 2e00 0000 0617 0a02 0801 0602 0201  .s..............
+00000a40: 0201 0201 08fd 0606 0201 0201 08fe 0605  ................
+00000a50: 0201 08ff 0408 0801 0a01 1601 0801 0201  ................
+00000a60: 0c02 0402 7233 0000 00e9 0800 0000 da0b  ....r3..........
+00000a70: 6d61 785f 7661 6c65 6e63 6563 0200 0000  max_valencec....
+00000a80: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00000a90: 0300 0000 7332 0000 0069 007d 0274 0064  ....s2...i.}.t.d
+00000aa0: 017c 0183 0244 005d 0f89 0087 0066 0164  .|...D.].....f.d
+00000ab0: 0264 0384 087c 00a0 01a1 0044 0083 017c  .d...|.....D...|
+00000ac0: 0288 003c 0071 077c 0253 0029 044e 7207  ...<.q.|.S.).Nr.
+00000ad0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000ae0: 0200 0000 0400 0000 1300 0000 7320 0000  ............s ..
+00000af0: 0067 007c 005d 0c7d 017c 01a0 00a1 0088  .g.|.].}.|......
+00000b00: 006b 0572 027c 01a0 01a1 0091 0271 0253  .k.r.|.......q.S
+00000b10: 0072 1900 0000 2902 da10 4765 744e 756d  .r....)...GetNum
+00000b20: 496d 706c 6963 6974 4873 da06 4765 7449  ImplicitHs..GetI
+00000b30: 6478 2902 7224 0000 00da 0461 746f 6da9  dx).r$.....atom.
+00000b40: 01da 0169 7219 0000 0072 1a00 0000 7226  ...ir....r....r&
+00000b50: 0000 0062 0000 0073 0c00 0000 0600 0202  ...b...s........
+00000b60: 0a01 02fd 0601 06ff 7a28 6765 745f 6672  ........z(get_fr
+00000b70: 6565 5f76 616c 656e 6365 5f6d 6170 2e3c  ee_valence_map.<
+00000b80: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00000b90: 703e 2902 da05 7261 6e67 65da 0847 6574  p>)...range..Get
+00000ba0: 4174 6f6d 7329 0372 1000 0000 7235 0000  Atoms).r....r5..
+00000bb0: 00da 0672 6573 756c 7472 1900 0000 7239  ...resultr....r9
+00000bc0: 0000 0072 1a00 0000 7229 0000 005f 0000  ...r....r)..._..
+00000bd0: 0073 0c00 0000 0401 0e01 0a01 0602 0cfe  .s..............
+00000be0: 0406 7229 0000 0072 2100 0000 7222 0000  ..r)...r!...r"..
+00000bf0: 0063 0300 0000 0000 0000 0000 0000 0e00  .c..............
+00000c00: 0000 0800 0000 4300 0000 73a4 0000 0074  ......C...s....t
+00000c10: 0083 007d 0374 016a 026a 0374 016a 026a  ...}.t.j.j.t.j.j
+00000c20: 0474 016a 026a 0564 019c 037d 047c 04a0  .t.j.j.d...}.|..
+00000c30: 06a1 0044 005d 3c5c 027d 057d 067c 027c  ...D.]<\.}.}.|.|
+00000c40: 0519 0044 005d 337d 077c 01a0 06a1 0044  ...D.]3}.|.....D
+00000c50: 005d 2c5c 027d 087d 0974 01a0 077c 00a1  .],\.}.}.t...|..
+00000c60: 017d 0a7c 0aa0 0874 01a0 097c 08a1 01a1  .}.|...t...|....
+00000c70: 017d 0b7c 0aa0 0a7c 077c 0b7c 06a1 0301  .}.|...|.|.|....
+00000c80: 0074 016a 0b7c 0a64 0264 038d 027d 0c7c  .t.j.|.d.d...}.|
+00000c90: 0c72 4371 2174 01a0 0c7c 0aa1 017d 0d7c  .rCq!t...|...}.|
+00000ca0: 03a0 0d7c 0da1 0101 0071 2171 1b71 137c  ...|.....q!q.q.|
+00000cb0: 0353 0029 047a b60a 2020 2020 4769 7665  .S.).z..    Give
+00000cc0: 6e20 6120 6d6f 6c65 6375 6c65 2060 606d  n a molecule ``m
+00000cd0: 6f6c 6060 2c20 7468 6973 2066 756e 6374  ol``, this funct
+00000ce0: 696f 6e20 7769 6c6c 2072 6574 7572 6e20  ion will return 
+00000cf0: 6120 6c69 7374 206f 6620 534d 494c 4553  a list of SMILES
+00000d00: 2073 7472 696e 6773 2074 6861 7420 7265   strings that re
+00000d10: 7072 6573 656e 7420 7661 6c69 640a 2020  present valid.  
+00000d20: 2020 6174 6f6d 2061 6464 6974 696f 6e73    atom additions
+00000d30: 2074 6f20 7468 6520 6261 7365 206d 6f6c   to the base mol
+00000d40: 6563 756c 652e 0a0a 2020 2020 3a72 6574  ecule...    :ret
+00000d50: 7572 6e73 3a20 4120 6c69 7374 206f 6620  urns: A list of 
+00000d60: 7374 7269 6e67 732e 0a20 2020 20a9 0372  strings..    ..r
+00000d70: 0700 0000 e902 0000 00e9 0300 0000 54a9  ..............T.
+00000d80: 01da 0b63 6174 6368 4572 726f 7273 290e  ...catchErrors).
+00000d90: 7227 0000 0072 0200 0000 da08 426f 6e64  r'...r......Bond
+00000da0: 5479 7065 da06 5349 4e47 4c45 da06 444f  Type..SINGLE..DO
+00000db0: 5542 4c45 da06 5452 4950 4c45 da05 6974  UBLE..TRIPLE..it
+00000dc0: 656d 73da 0552 574d 6f6c da07 4164 6441  ems..RWMol..AddA
+00000dd0: 746f 6dda 0441 746f 6dda 0741 6464 426f  tom..Atom..AddBo
+00000de0: 6e64 da0b 5361 6e69 7469 7a65 4d6f 6cda  nd..SanitizeMol.
+00000df0: 0b4d 6f6c 546f 536d 696c 6573 da03 6164  .MolToSmiles..ad
+00000e00: 6429 0e72 1000 0000 7221 0000 0072 2200  d).r....r!...r".
+00000e10: 0000 da07 7265 7375 6c74 73da 1376 616c  ....results..val
+00000e20: 7565 5f62 6f6e 645f 7479 7065 5f6d 6170  ue_bond_type_map
+00000e30: 723a 0000 00da 0962 6f6e 645f 7479 7065  r:.....bond_type
+00000e40: 7238 0000 00da 0765 6c65 6d65 6e74 da07  r8.....element..
+00000e50: 7661 6c65 6e63 65da 076e 6577 5f6d 6f6c  valence..new_mol
+00000e60: da03 6964 78da 1373 616e 6974 697a 6174  ..idx..sanitizat
+00000e70: 696f 6e5f 7265 7375 6c74 721e 0000 0072  ion_resultr....r
+00000e80: 1900 0000 7219 0000 0072 1a00 0000 722b  ....r....r....r+
+00000e90: 0000 006b 0000 0073 2600 0000 060a 0603  ...k...s&.......
+00000ea0: 0601 0601 06fd 1005 0c02 1001 0a01 1001  ................
+00000eb0: 0e01 0e01 0401 0201 0a02 0c01 02f7 02ff  ................
+00000ec0: 040c 722b 0000 0063 0200 0000 0000 0000  ..r+...c........
+00000ed0: 0000 0000 1000 0000 0700 0000 4300 0000  ............C...
+00000ee0: 7336 0100 0074 0083 007d 0264 0174 016a  s6...t...}.d.t.j
+00000ef0: 026a 0374 016a 026a 0474 016a 026a 0564  .j.t.j.j.t.j.j.d
+00000f00: 029c 047d 0374 067c 0383 017d 047c 01a0  ...}.t.|...}.|..
+00000f10: 07a1 0044 005d 805c 027d 057d 0674 08a0  ...D.].\.}.}.t..
+00000f20: 097c 0664 03a1 0244 005d 755c 027d 077d  .|.d...D.]u\.}.}
+00000f30: 087c 00a0 0a7c 07a1 01a0 0ba1 0072 357c  .|...|.......r5|
+00000f40: 00a0 0a7c 08a1 01a0 0ba1 0072 3571 2274  ...|.......r5q"t
+00000f50: 01a0 0c7c 00a1 01a0 0d7c 077c 08a1 027d  ...|.....|.|...}
+00000f60: 0974 01a0 0e7c 00a1 017d 0a74 016a 0f7c  .t...|...}.t.j.|
+00000f70: 0a64 0464 058d 0201 007c 0964 0175 0172  .d.d.....|.d.u.r
+00000f80: 787c 09a0 10a1 007d 0b7c 0b7c 03a0 11a1  x|.....}.|.|....
+00000f90: 0076 0172 5971 227c 047c 0b19 007d 0c7c  .v.rYq"|.|...}.|
+00000fa0: 0c7c 0537 007d 0c7c 0c64 066b 0472 6671  .|.7.}.|.d.k.rfq
+00000fb0: 227c 09a0 12a1 007d 0d7c 09a0 137c 037c  "|.....}.|...|.|
+00000fc0: 0c19 00a1 0101 007c 0aa0 147c 0d7c 09a1  .......|...|.|..
+00000fd0: 0201 006e 0b7c 037c 0519 007d 0b7c 0aa0  ...n.|.|...}.|..
+00000fe0: 157c 077c 087c 0ba1 0301 0074 016a 167c  .|.|.|.....t.j.|
+00000ff0: 0a64 0464 078d 027d 0e7c 0e72 8d71 2274  .d.d...}.|.r.q"t
+00001000: 01a0 177c 0aa1 017d 0f7c 02a0 187c 0fa1  ...|...}.|...|..
+00001010: 0101 0071 2271 187c 0253 0029 0861 4003  ...q"q.|.S.).a@.
+00001020: 0000 0a20 2020 2047 6976 656e 2061 206d  ...    Given a m
+00001030: 6f6c 6563 756c 6520 6060 6d6f 6c60 602c  olecule ``mol``,
+00001040: 2074 6869 7320 6675 6e63 7469 6f6e 2077   this function w
+00001050: 696c 6c20 7265 7475 726e 2061 206c 6973  ill return a lis
+00001060: 7420 6f66 2053 4d49 4c45 5320 7374 7269  t of SMILES stri
+00001070: 6e67 7320 7768 6963 6820 7265 7375 6c74  ngs which result
+00001080: 7320 6672 6f6d 2076 616c 6964 0a20 2020  s from valid.   
+00001090: 2062 6f6e 6420 6164 6469 7469 6f6e 7320   bond additions 
+000010a0: 746f 2074 6861 7420 6261 7365 206d 6f6c  to that base mol
+000010b0: 6563 756c 652e 2056 616c 6964 2062 6f6e  ecule. Valid bon
+000010c0: 6420 6164 6469 7469 6f6e 7320 696e 2074  d additions in t
+000010d0: 6869 7320 6361 7365 2061 7265 2064 6566  his case are def
+000010e0: 696e 6564 2061 7320 616c 6c6f 7765 6420  ined as allowed 
+000010f0: 696e 0a20 2020 2074 6572 6d73 206f 6620  in.    terms of 
+00001100: 7468 6520 6174 6f6d 2076 616c 656e 6365  the atom valence
+00001110: 732e 2062 6f6e 6420 6164 6469 7469 6f6e  s. bond addition
+00001120: 7320 6d61 7920 636f 6e6e 6563 7420 7477  s may connect tw
+00001130: 6f20 6174 6f6d 7320 7768 6963 6820 6172  o atoms which ar
+00001140: 6520 6e6f 7420 7965 7420 6469 7265 6374  e not yet direct
+00001150: 6c79 2063 6f6e 6e65 6374 6564 0a20 2020  ly connected.   
+00001160: 206f 7220 7570 6772 6164 6520 616e 2065   or upgrade an e
+00001170: 7869 7374 696e 6720 626f 6e64 2028 7369  xisting bond (si
+00001180: 6e67 6c65 2074 6f20 646f 7562 6c65 292e  ngle to double).
+00001190: 0a0a 2020 2020 416c 736f 2064 6973 616c  ..    Also disal
+000011a0: 6c6f 7765 6420 6172 6520 626f 6e64 7320  lowed are bonds 
+000011b0: 6265 7477 6565 6e20 7477 6f20 6174 6f6d  between two atom
+000011c0: 7320 7768 6963 6820 6172 6520 7468 656d  s which are them
+000011d0: 7365 6c76 6573 2061 6c72 6561 6479 2070  selves already p
+000011e0: 6172 7420 6f66 2061 2072 696e 672e 0a0a  art of a ring...
+000011f0: 2020 2020 3a70 6172 616d 206d 6f6c 3a20      :param mol: 
+00001200: 5468 6520 6261 7365 206d 6f6c 6563 756c  The base molecul
+00001210: 650a 2020 2020 3a70 6172 616d 2066 7265  e.    :param fre
+00001220: 655f 7661 6c65 6e63 655f 696e 6469 6365  e_valence_indice
+00001230: 735f 6d61 703a 2041 2064 6963 7420 7768  s_map: A dict wh
+00001240: 6f73 6520 6b65 7973 2061 7265 2069 6e74  ose keys are int
+00001250: 6567 6572 7320 7374 6172 7469 6e67 2066  egers starting f
+00001260: 726f 6d20 302e 2054 4865 206b 6579 2076  rom 0. THe key v
+00001270: 616c 7565 730a 2020 2020 2020 2020 7265  alues.        re
+00001280: 7072 6573 656e 7420 7468 6520 2a66 7265  present the *fre
+00001290: 6520 6e75 6d62 6572 206f 6620 7661 6c65  e number of vale
+000012a0: 6e63 6573 2a2e 2054 6865 2076 616c 7565  nces*. The value
+000012b0: 7320 6172 6520 6c69 7374 7320 6f66 2061  s are lists of a
+000012c0: 746f 6d20 696e 6469 6365 7320 7768 6572  tom indices wher
+000012d0: 6520 6561 6368 2061 746f 6d20 696e 0a20  e each atom in. 
+000012e0: 2020 2020 2020 2074 6865 206c 6973 7420         the list 
+000012f0: 6861 7320 746f 2068 6176 6520 7468 6520  has to have the 
+00001300: 636f 7272 6573 706f 6e64 696e 6720 6e75  corresponding nu
+00001310: 6d62 6572 206f 6620 6672 6565 2076 616c  mber of free val
+00001320: 656e 6365 7320 6769 7665 6e20 6279 2074  ences given by t
+00001330: 6865 2064 6963 7420 6b65 792e 0a0a 2020  he dict key...  
+00001340: 2020 3a72 6574 7572 6e73 3a20 4120 6c69    :returns: A li
+00001350: 7374 206f 6620 7374 7269 6e67 730a 2020  st of strings.  
+00001360: 2020 4ea9 0472 0100 0000 7207 0000 0072    N..r....r....r
+00001370: 3f00 0000 7240 0000 0072 3f00 0000 54a9  ?...r@...r?...T.
+00001380: 01da 1263 6c65 6172 4172 6f6d 6174 6963  ...clearAromatic
+00001390: 466c 6167 7372 4000 0000 7241 0000 0029  Flagsr@...rA...)
+000013a0: 1972 2700 0000 7202 0000 0072 4300 0000  .r'...r....rC...
+000013b0: 7244 0000 0072 4500 0000 7246 0000 0072  rD...rE...rF...r
+000013c0: 0300 0000 7247 0000 00da 0969 7465 7274  ....rG.....itert
+000013d0: 6f6f 6c73 da0c 636f 6d62 696e 6174 696f  ools..combinatio
+000013e0: 6e73 da0e 4765 7441 746f 6d57 6974 6849  ns..GetAtomWithI
+000013f0: 6478 da08 4973 496e 5269 6e67 da03 4d6f  dx..IsInRing..Mo
+00001400: 6cda 1347 6574 426f 6e64 4265 7477 6565  l..GetBondBetwee
+00001410: 6e41 746f 6d73 7248 0000 00da 084b 656b  nAtomsrH.....Kek
+00001420: 756c 697a 65da 0b47 6574 426f 6e64 5479  ulize..GetBondTy
+00001430: 7065 da06 7661 6c75 6573 7237 0000 00da  pe..valuesr7....
+00001440: 0b53 6574 426f 6e64 5479 7065 da0b 5265  .SetBondType..Re
+00001450: 706c 6163 6542 6f6e 6472 4b00 0000 724c  placeBondrK...rL
+00001460: 0000 0072 4d00 0000 724e 0000 0029 1072  ...rM...rN...).r
+00001470: 1000 0000 7222 0000 0072 4f00 0000 7250  ....r"...rO...rP
+00001480: 0000 00da 1362 6f6e 645f 7479 7065 5f76  .....bond_type_v
+00001490: 616c 7565 5f6d 6170 7253 0000 00da 0561  alue_maprS.....a
+000014a0: 746f 6d73 da05 6174 6f6d 31da 0561 746f  toms..atom1..ato
+000014b0: 6d32 da04 626f 6e64 7254 0000 0072 5100  m2..bondrT...rQ.
+000014c0: 0000 da0a 626f 6e64 5f76 616c 7565 da05  ....bond_value..
+000014d0: 696e 6465 7872 5600 0000 721e 0000 0072  indexrV...r....r
+000014e0: 1900 0000 7219 0000 0072 1a00 0000 722c  ....r....r....r,
+000014f0: 0000 008d 0000 0073 4400 0000 0612 0203  .......sD.......
+00001500: 0601 0601 0601 06fc 0806 1002 1401 1c03  ................
+00001510: 0201 1202 0a01 0e02 0801 0801 0c01 0201  ................
+00001520: 0802 0801 0801 0201 0802 0e01 0e01 0803  ................
+00001530: 0e01 0e02 0401 0201 0a02 0c01 02df 0423  ...............#
+00001540: 722c 0000 0063 0100 0000 0000 0000 0000  r,...c..........
+00001550: 0000 0f00 0000 0700 0000 4300 0000 7362  ..........C...sb
+00001560: 0100 0074 0083 007d 0164 0174 016a 026a  ...t...}.d.t.j.j
+00001570: 0374 016a 026a 0474 016a 026a 0564 029c  .t.j.j.t.j.j.d..
+00001580: 047d 0274 067c 0283 017d 0364 0344 005d  .}.t.|...}.d.D.]
+00001590: 987d 047c 00a0 07a1 0044 005d 917d 057c  .}.|.....D.].}.|
+000015a0: 05a0 08a1 007c 05a0 09a1 0002 027d 067d  .....|.......}.}
+000015b0: 0774 01a0 0a7c 00a1 01a0 0b7c 067c 07a1  .t...|.....|.|..
+000015c0: 027d 057c 05a0 0ca1 007d 087c 087c 02a0  .}.|.....}.|.|..
+000015d0: 0da1 0076 0172 3b71 1c74 01a0 0e7c 00a1  ...v.r;q.t...|..
+000015e0: 017d 0974 016a 0f7c 0964 0464 058d 0201  .}.t.j.|.d.d....
+000015f0: 007c 037c 0819 007d 0a7c 0a7c 0438 007d  .|.|...}.|.|.8.}
+00001600: 0a7c 0a64 066b 0272 5a7c 09a0 107c 067c  .|.d.k.rZ|...|.|
+00001610: 07a1 0201 006e 177c 0a64 066b 0472 707c  .....n.|.d.k.rp|
+00001620: 05a0 117c 027c 0a19 00a1 0101 007c 05a0  ...|.|.......|..
+00001630: 12a1 007d 0b7c 09a0 137c 0b7c 05a1 0201  ...}.|...|.|....
+00001640: 006e 0171 1c74 016a 147c 0964 0464 078d  .n.q.t.j.|.d.d..
+00001650: 027d 0c7c 0c72 7b71 1c74 01a0 157c 09a1  .}.|.r{q.t...|..
+00001660: 017d 0d64 087c 0d76 0072 a874 167c 0da0  .}.d.|.v.r.t.|..
+00001670: 1764 08a1 0174 1864 098d 027d 0e74 187c  .d...t.d...}.t.|
+00001680: 0e64 0619 0083 0164 0a6b 0472 9671 1c74  .d.....d.k.r.q.t
+00001690: 1874 01a0 197c 0e64 0a19 00a1 01a0 1aa1  .t...|.d........
+000016a0: 0083 0164 0b6b 0072 a471 1c7c 0e64 0a19  ...d.k.r.q.|.d..
+000016b0: 007d 0d7c 01a0 1b7c 0da1 0101 0071 1c71  .}.|...|.....q.q
+000016c0: 167c 0153 0029 0c61 a201 0000 0a20 2020  .|.S.).a.....   
+000016d0: 2047 6976 656e 2061 206d 6f6c 6563 756c   Given a molecul
+000016e0: 6520 6060 6d6f 6c60 602c 2074 6869 7320  e ``mol``, this 
+000016f0: 6675 6e63 7469 6f6e 2077 696c 6c20 7265  function will re
+00001700: 7475 726e 2061 206c 6973 7420 6f66 2053  turn a list of S
+00001710: 4d49 4c45 5320 7374 7269 6e67 7320 7768  MILES strings wh
+00001720: 6963 6820 7265 7072 6573 656e 7420 7661  ich represent va
+00001730: 6c69 640a 2020 2020 626f 6e64 2072 656d  lid.    bond rem
+00001740: 6f76 616c 732e 2041 2062 6f6e 6420 7265  ovals. A bond re
+00001750: 6d6f 7661 6c20 6973 2065 6974 6865 7220  moval is either 
+00001760: 6120 646f 776e 6772 6164 6520 6f66 2061  a downgrade of a
+00001770: 6e20 6578 6973 7469 6e67 2062 6f6e 6420  n existing bond 
+00001780: 2865 2e67 2e20 646f 7562 6c65 2074 6f20  (e.g. double to 
+00001790: 7369 6e67 6c65 2920 6f72 2074 6865 0a20  single) or the. 
+000017a0: 2020 2072 656d 6f76 616c 206f 6620 6120     removal of a 
+000017b0: 7369 6e67 6c65 2062 6f6e 6420 7768 6963  single bond whic
+000017c0: 6820 776f 756c 6420 6d65 616e 2074 6f20  h would mean to 
+000017d0: 6469 7363 6f6e 6e65 6374 2061 7420 6d6f  disconnect at mo
+000017e0: 7374 2061 2073 696e 676c 6520 6174 6f6d  st a single atom
+000017f0: 2066 726f 6d20 7468 6520 7265 7374 206f   from the rest o
+00001800: 6620 7468 650a 2020 2020 6d6f 6c65 6375  f the.    molecu
+00001810: 6c65 210a 0a20 2020 203a 7061 7261 6d20  le!..    :param 
+00001820: 6d6f 6c3a 2054 6865 2062 6173 6520 6d6f  mol: The base mo
+00001830: 6c65 6375 6c65 2066 6f72 2074 6865 2072  lecule for the r
+00001840: 656d 6f76 616c 732e 0a0a 2020 2020 3a72  emovals...    :r
+00001850: 6574 7572 6e73 3a20 4120 6c69 7374 206f  eturns: A list o
+00001860: 6620 7374 7269 6e67 730a 2020 2020 4e72  f strings.    Nr
+00001870: 5700 0000 723e 0000 0054 7258 0000 0072  W...r>...TrX...r
+00001880: 0100 0000 7241 0000 00da 012e 2901 da03  ....rA......)...
+00001890: 6b65 7972 0700 0000 723f 0000 0029 1c72  keyr....r?...).r
+000018a0: 2700 0000 7202 0000 0072 4300 0000 7244  '...r....rC...rD
+000018b0: 0000 0072 4500 0000 7246 0000 0072 0300  ...rE...rF...r..
+000018c0: 0000 da08 4765 7442 6f6e 6473 da0f 4765  ....GetBonds..Ge
+000018d0: 7442 6567 696e 4174 6f6d 4964 78da 0d47  tBeginAtomIdx..G
+000018e0: 6574 456e 6441 746f 6d49 6478 725e 0000  etEndAtomIdxr^..
+000018f0: 0072 5f00 0000 7261 0000 0072 6200 0000  .r_...ra...rb...
+00001900: 7248 0000 0072 6000 0000 da0a 5265 6d6f  rH...r`.....Remo
+00001910: 7665 426f 6e64 7263 0000 0072 3700 0000  veBondrc...r7...
+00001920: 7264 0000 0072 4c00 0000 724d 0000 00da  rd...rL...rM....
+00001930: 0673 6f72 7465 64da 0573 706c 6974 da03  .sorted..split..
+00001940: 6c65 6e72 2800 0000 723c 0000 0072 4e00  lenr(...r<...rN.
+00001950: 0000 290f 7210 0000 0072 4f00 0000 7250  ..).r....rO...rP
+00001960: 0000 0072 6500 0000 7253 0000 0072 6900  ...re...rS...ri.
+00001970: 0000 7267 0000 0072 6800 0000 7251 0000  ..rg...rh...rQ..
+00001980: 0072 5400 0000 726a 0000 0072 6b00 0000  .rT...rj...rk...
+00001990: 7256 0000 0072 1e00 0000 da05 7061 7274  rV...r......part
+000019a0: 7372 1900 0000 7219 0000 0072 1a00 0000  sr....r....r....
+000019b0: 722d 0000 00d0 0000 0073 4e00 0000 060c  r-.......sN.....
+000019c0: 0203 0601 0601 0601 06fc 0806 0802 0c01  ................
+000019d0: 1201 1201 0802 0c01 0201 0a02 0e01 0802  ................
+000019e0: 0801 0802 0e01 0802 0e01 0801 0e01 0203  ................
+000019f0: 0e02 0401 0201 0a02 0801 1201 1001 0201  ................
+00001a00: 1a06 0201 0802 0c02 02d4 042e 722d 0000  ............r-..
+00001a10: 0029 0172 0f00 0000 2901 721c 0000 0029  .).r....).r....)
+00001a20: 0172 3400 0000 2919 725a 0000 00da 0674  .r4...).rZ.....t
+00001a30: 7970 696e 67da 0174 da05 7264 6b69 7472  yping..t..rdkitr
+00001a40: 0200 0000 da19 7667 645f 636f 756e 7465  ......vgd_counte
+00001a50: 7266 6163 7475 616c 732e 7574 696c 7372  rfactuals.utilsr
+00001a60: 0300 0000 da18 4445 4641 554c 545f 4154  ......DEFAULT_AT
+00001a70: 4f4d 5f56 414c 454e 4345 5f4d 4150 725e  OM_VALENCE_MAPr^
+00001a80: 0000 00da 0373 7472 721b 0000 0072 1d00  .....strr....r..
+00001a90: 0000 da08 5365 7175 656e 6365 da08 4361  ....Sequence..Ca
+00001aa0: 6c6c 6162 6c65 da04 626f 6f6c da04 4c69  llable..bool..Li
+00001ab0: 7374 7233 0000 00da 0369 6e74 da04 6469  str3.....int..di
+00001ac0: 6374 7229 0000 00da 0444 6963 74da 0353  ctr).....Dict..S
+00001ad0: 6574 722b 0000 0072 2c00 0000 722d 0000  etr+...r,...r-..
+00001ae0: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
+00001af0: 721a 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00001b00: 0000 0073 4c00 0000 0800 0801 0c01 0c02  ...sL...........
+00001b10: 0204 0201 0202 0201 0201 0201 06f9 160c  ................
+00001b20: 160a 0207 0202 0201 02fe 08fe 1602 02fe  ................
+00001b30: 0806 0afa 1a3b 080c 0c01 02ff 1202 02fe  .....;..........
+00001b40: 0803 0afd 0822 1201 02ff 0802 0afe 0843  .....".........C
+00001b50: 0801 0eff                                ....
```

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/generate/molecules.py` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/molecules.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from vgd_counterfactuals.utils import invert_dict
 
 
 DEFAULT_ATOM_VALENCE_MAP = {
     'C': 4,
     'N': 5,
-    'P': 5,
+    # 'P': 5,
     'O': 6,
     'F': 1,
     'Cl': 7,
     'S': 6,
 
 }
 
@@ -23,18 +23,25 @@
     appear in chemistry.
     """
     smarts = Chem.MolFromSmarts(pattern)
     is_match = mol.HasSubstructMatch(smarts)
     return is_match
 
 
+def is_nitrogen_nitrogen_sulfur(mol: Chem.Mol, pattern: str = 'SNN'):
+    smarts = Chem.MolFromSmarts(pattern)
+    is_match = mol.HasSubstructMatch(smarts)
+    return is_match
+
+
 def get_neighborhood(smiles: str,
                      atom_valence_map=DEFAULT_ATOM_VALENCE_MAP,
                      mol_filters: t.Sequence[t.Callable[[Chem.Mol], bool]] = (
                         is_bridge_head_carbon,
+                        is_nitrogen_nitrogen_sulfur,
                      ),
                      ) -> t.List[str]:
     """
     Given a ``smiles`` representation of a molecule, this function will return a list of the SMILES
     representations of all the valid molecules within a 1-edit neighborhood. Optionally, a list of boolean
     functions can be provided for ``mol_filters`` to further limit the kinds of molecules included in the
     result.
@@ -72,17 +79,16 @@
     # 15.05.23 - All of the above functions will create "valid" molecular SMILES in the sense that RDKit
     # does not tell us that they are completely wrong, but the molecules that are created might still not
     # realistically exist in chemistry, which is why we additionally apply a set of filters that decide
     # for each molecule if it should be included
     neighbors_filtered = []
     for smiles in neighbors_set:
         mol = Chem.MolFromSmiles(smiles)
-        for func in mol_filters:
-            if not func(mol):
-                continue
+        if any([func(mol) for func in mol_filters]):
+            continue
 
         neighbors_filtered.append(smiles)
 
     return neighbors_filtered
 
 
 def get_free_valence_map(mol: Chem.Mol, max_valence: int = 8) -> dict:
```

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/generate/smiles_one_step_changes.py` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/generate/smiles_one_step_changes.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/templates/article.tex.j2` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/templates/article.tex.j2`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/utils.py` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/utils.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/vgd_counterfactuals/visualization.py` & `vgd_counterfactuals-0.1.4/vgd_counterfactuals/visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.3/PKG-INFO` & `vgd_counterfactuals-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgd-counterfactuals
-Version: 0.1.3
+Version: 0.1.4
 Summary: Counterfactual explanations for GNNs based on the visual graph dataset format
 License: MIT
 Keywords: graph neural networks,counterfactuals,explainable AI
 Author: Jonas Teufel
 Author-email: jonseb1998@gmail.com
 Maintainer: Jonas Teufel
 Maintainer-email: jonseb1998@gmail.com
@@ -32,15 +32,15 @@
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.1.3-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.1.4-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

