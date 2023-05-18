# Comparing `tmp/Topyfic-0.2.1.tar.gz` & `tmp/Topyfic-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Topyfic-0.2.1.tar", last modified: Wed May 17 21:52:29 2023, max compression
+gzip compressed data, was "Topyfic-0.2.2.tar", last modified: Thu May 18 22:13:08 2023, max compression
```

## Comparing `Topyfic-0.2.1.tar` & `Topyfic-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-17 21:52:29.055492 Topyfic-0.2.1/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.2.1/LICENSE.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      865 2023-05-17 21:52:29.055581 Topyfic-0.2.1/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.2.1/README.md
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-17 21:52:29.054180 Topyfic-0.2.1/Topyfic/
--rw-rw-r--   0 nargesrezaie   (501) staff       (20)      148 2022-10-21 21:50:45.000000 Topyfic-0.2.1/Topyfic/__init__.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    44549 2023-04-26 18:27:24.000000 Topyfic-0.2.1/Topyfic/analysis.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     4115 2022-12-08 00:57:41.000000 Topyfic-0.2.1/Topyfic/main.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    10863 2023-01-20 10:16:01.000000 Topyfic-0.2.1/Topyfic/topModel.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    11278 2023-05-01 21:58:44.000000 Topyfic-0.2.1/Topyfic/topic.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    10461 2023-03-29 18:16:24.000000 Topyfic-0.2.1/Topyfic/train.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    27641 2023-05-17 21:39:51.000000 Topyfic-0.2.1/Topyfic/utils.py
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-17 21:52:29.055268 Topyfic-0.2.1/Topyfic.egg-info/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      865 2023-05-17 21:52:28.000000 Topyfic-0.2.1/Topyfic.egg-info/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      321 2023-05-17 21:52:29.000000 Topyfic-0.2.1/Topyfic.egg-info/SOURCES.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-05-17 21:52:28.000000 Topyfic-0.2.1/Topyfic.egg-info/dependency_links.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      269 2023-05-17 21:52:28.000000 Topyfic-0.2.1/Topyfic.egg-info/requires.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-05-17 21:52:28.000000 Topyfic-0.2.1/Topyfic.egg-info/top_level.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-05-17 21:52:29.055908 Topyfic-0.2.1/setup.cfg
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1931 2023-05-17 21:51:55.000000 Topyfic-0.2.1/setup.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-18 22:13:08.758843 Topyfic-0.2.2/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.2.2/LICENSE.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-05-18 22:13:08.758920 Topyfic-0.2.2/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.2.2/README.md
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-18 22:13:08.757445 Topyfic-0.2.2/Topyfic/
+-rw-rw-r--   0 nargesrezaie   (501) staff       (20)      148 2022-10-21 21:50:45.000000 Topyfic-0.2.2/Topyfic/__init__.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    44549 2023-04-26 18:27:24.000000 Topyfic-0.2.2/Topyfic/analysis.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     4115 2022-12-08 00:57:41.000000 Topyfic-0.2.2/Topyfic/main.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    10863 2023-01-20 10:16:01.000000 Topyfic-0.2.2/Topyfic/topModel.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    11278 2023-05-01 21:58:44.000000 Topyfic-0.2.2/Topyfic/topic.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    10461 2023-03-29 18:16:24.000000 Topyfic-0.2.2/Topyfic/train.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    27627 2023-05-18 22:07:57.000000 Topyfic-0.2.2/Topyfic/utils.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-18 22:13:08.758702 Topyfic-0.2.2/Topyfic.egg-info/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-05-18 22:13:08.000000 Topyfic-0.2.2/Topyfic.egg-info/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      321 2023-05-18 22:13:08.000000 Topyfic-0.2.2/Topyfic.egg-info/SOURCES.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-05-18 22:13:08.000000 Topyfic-0.2.2/Topyfic.egg-info/dependency_links.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      269 2023-05-18 22:13:08.000000 Topyfic-0.2.2/Topyfic.egg-info/requires.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-05-18 22:13:08.000000 Topyfic-0.2.2/Topyfic.egg-info/top_level.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-05-18 22:13:08.759188 Topyfic-0.2.2/setup.cfg
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1975 2023-05-18 22:09:59.000000 Topyfic-0.2.2/setup.py
```

### Comparing `Topyfic-0.2.1/LICENSE.txt` & `Topyfic-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.1/PKG-INFO` & `Topyfic-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.2.1
+Version: 0.2.2
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.1.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.2.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
-Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network
+Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network,Topic Modeling,single-nucleus RNA-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 License-File: LICENSE.txt
```

### Comparing `Topyfic-0.2.1/README.md` & `Topyfic-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.1/Topyfic/analysis.py` & `Topyfic-0.2.2/Topyfic/analysis.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.1/Topyfic/main.py` & `Topyfic-0.2.2/Topyfic/main.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.1/Topyfic/topModel.py` & `Topyfic-0.2.2/Topyfic/topModel.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.1/Topyfic/topic.py` & `Topyfic-0.2.2/Topyfic/topic.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.1/Topyfic/train.py` & `Topyfic-0.2.2/Topyfic/train.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.2.1/Topyfic/utils.py` & `Topyfic-0.2.2/Topyfic/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,15 @@
     """
     n_rtopics = len(np.unique(clusters[f"leiden"]))
 
     components = np.zeros((n_rtopics, all_components.shape[1]), dtype=float)
     exp_dirichlet_component = np.zeros((n_rtopics, all_exp_dirichlet_component.shape[1]), dtype=float)
 
     topic = 0
-    for cluster in np.unique(clusters[f"leiden"]):
+    for cluster in range(n_rtopics):
         tmp = clusters[clusters["leiden"] == cluster]
 
         tmp_components = all_components.loc[tmp.index, :]
         tmp_components = tmp_components.mean(axis=0)
         components[topic, :] = tmp_components.values
 
         tmp_exp_dirichlet_component = all_exp_dirichlet_component.loc[tmp.index, :]
```

### Comparing `Topyfic-0.2.1/Topyfic.egg-info/PKG-INFO` & `Topyfic-0.2.2/Topyfic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.2.1
+Version: 0.2.2
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.1.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.2.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
-Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network
+Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network,Topic Modeling,single-nucleus RNA-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 License-File: LICENSE.txt
```

### Comparing `Topyfic-0.2.1/setup.py` & `Topyfic-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 
 setup(
     name='Topyfic',  # the name of your package
     packages=['Topyfic'],  # same as above
-    version='v0.2.1',  # version number
+    version='v0.2.2',  # version number
     license='MIT',  # license type
     description='Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) '
                 'using leiden clustering and harmony for single cell epigenomics data',
     # short description
     author='Narges Rezaie',  # your name
     author_email='nargesrezaie80@gmail.com',  # your email
     url='https://github.com/mortazavilab/Topyfic',  # url to your git repo
-    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.1.tar.gz',  # link to the tar.gz file associated with this release
+    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/V0.2.2.tar.gz',  # link to the tar.gz file associated with this release
     keywords=['Cellular Programs', 'Latent Dirichlet allocation', 'single-cell multiome', 'single-cell RNA-seq',
-              'gene regulatory network'],  #
+              'gene regulatory network', 'Topic Modeling', 'single-nucleus RNA-seq'],  #
     python_requires='>=3.8',
     install_requires=[  # these can also include >, <, == to enforce version compatibility
         'pandas>=1.4.4',  # make sure the packages you put here are those NOT included in the base python distribution
         'scikit-learn>=0.24.2',
         'pytest',
         'leidenalg',
         'setuptools',
```

