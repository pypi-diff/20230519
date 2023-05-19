# Comparing `tmp/favapy-0.3.9.2.tar.gz` & `tmp/favapy-0.3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/favapy-0.3.9.2.tar", last modified: Wed Jan 18 21:26:38 2023, max compression
+gzip compressed data, was "favapy-0.3.9.3.tar", last modified: Fri May 19 14:16:27 2023, max compression
```

## Comparing `favapy-0.3.9.2.tar` & `favapy-0.3.9.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-01-18 21:26:38.000000 favapy-0.3.9.2/
--rw-r--r--   0 tgn531     (501) staff       (20)     1065 2022-03-14 10:14:48.000000 favapy-0.3.9.2/LICENSE
--rw-r--r--   0 tgn531     (501) staff       (20)     3897 2023-01-18 21:26:38.000000 favapy-0.3.9.2/PKG-INFO
--rw-r--r--   0 tgn531     (501) staff       (20)     2772 2023-01-18 19:54:25.000000 favapy-0.3.9.2/README.md
--rw-r--r--   0 tgn531     (501) staff       (20)       85 2022-03-16 16:20:29.000000 favapy-0.3.9.2/pyproject.toml
--rw-r--r--   0 tgn531     (501) staff       (20)      948 2023-01-18 21:26:38.000000 favapy-0.3.9.2/setup.cfg
--rw-r--r--   0 tgn531     (501) staff       (20)     1080 2023-01-18 21:25:45.000000 favapy-0.3.9.2/setup.py
-drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-01-18 21:26:38.000000 favapy-0.3.9.2/src/
-drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-01-18 21:26:38.000000 favapy-0.3.9.2/src/favapy/
--rw-r--r--   0 tgn531     (501) staff       (20)        0 2022-03-16 11:55:28.000000 favapy-0.3.9.2/src/favapy/__init__.py
--rw-r--r--   0 tgn531     (501) staff       (20)     9357 2023-01-18 21:25:27.000000 favapy-0.3.9.2/src/favapy/fava.py
-drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-01-18 21:26:38.000000 favapy-0.3.9.2/src/favapy.egg-info/
--rw-r--r--   0 tgn531     (501) staff       (20)     3897 2023-01-18 21:26:38.000000 favapy-0.3.9.2/src/favapy.egg-info/PKG-INFO
--rw-r--r--   0 tgn531     (501) staff       (20)      299 2023-01-18 21:26:38.000000 favapy-0.3.9.2/src/favapy.egg-info/SOURCES.txt
--rw-r--r--   0 tgn531     (501) staff       (20)        1 2023-01-18 21:26:38.000000 favapy-0.3.9.2/src/favapy.egg-info/dependency_links.txt
--rw-r--r--   0 tgn531     (501) staff       (20)       45 2023-01-18 21:26:38.000000 favapy-0.3.9.2/src/favapy.egg-info/entry_points.txt
--rw-r--r--   0 tgn531     (501) staff       (20)       38 2023-01-18 21:26:38.000000 favapy-0.3.9.2/src/favapy.egg-info/requires.txt
--rw-r--r--   0 tgn531     (501) staff       (20)        7 2023-01-18 21:26:38.000000 favapy-0.3.9.2/src/favapy.egg-info/top_level.txt
+drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-05-19 14:16:27.519131 favapy-0.3.9.3/
+-rw-r--r--   0 tgn531     (501) staff       (20)     1065 2022-03-14 10:14:48.000000 favapy-0.3.9.3/LICENSE
+-rw-r--r--   0 tgn531     (501) staff       (20)     4067 2023-05-19 14:16:27.519429 favapy-0.3.9.3/PKG-INFO
+-rw-r--r--   0 tgn531     (501) staff       (20)     3360 2023-05-19 14:13:30.000000 favapy-0.3.9.3/README.md
+-rw-r--r--   0 tgn531     (501) staff       (20)       85 2022-03-16 16:20:29.000000 favapy-0.3.9.3/pyproject.toml
+-rw-r--r--   0 tgn531     (501) staff       (20)      948 2023-05-19 14:16:27.695779 favapy-0.3.9.3/setup.cfg
+-rw-r--r--   0 tgn531     (501) staff       (20)     1080 2023-05-19 14:09:41.000000 favapy-0.3.9.3/setup.py
+drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-05-19 14:16:27.252994 favapy-0.3.9.3/src/
+drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-05-19 14:16:27.464150 favapy-0.3.9.3/src/favapy/
+-rw-r--r--   0 tgn531     (501) staff       (20)        0 2022-03-16 11:55:28.000000 favapy-0.3.9.3/src/favapy/__init__.py
+-rw-r--r--   0 tgn531     (501) staff       (20)    10296 2023-05-19 14:08:39.000000 favapy-0.3.9.3/src/favapy/fava.py
+drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-05-19 14:16:27.517946 favapy-0.3.9.3/src/favapy.egg-info/
+-rw-r--r--   0 tgn531     (501) staff       (20)     4067 2023-05-19 14:16:26.000000 favapy-0.3.9.3/src/favapy.egg-info/PKG-INFO
+-rw-r--r--   0 tgn531     (501) staff       (20)      299 2023-05-19 14:16:26.000000 favapy-0.3.9.3/src/favapy.egg-info/SOURCES.txt
+-rw-r--r--   0 tgn531     (501) staff       (20)        1 2023-05-19 14:16:26.000000 favapy-0.3.9.3/src/favapy.egg-info/dependency_links.txt
+-rw-r--r--   0 tgn531     (501) staff       (20)       44 2023-05-19 14:16:26.000000 favapy-0.3.9.3/src/favapy.egg-info/entry_points.txt
+-rw-r--r--   0 tgn531     (501) staff       (20)       38 2023-05-19 14:16:26.000000 favapy-0.3.9.3/src/favapy.egg-info/requires.txt
+-rw-r--r--   0 tgn531     (501) staff       (20)        7 2023-05-19 14:16:26.000000 favapy-0.3.9.3/src/favapy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `favapy-0.3.9.2/LICENSE` & `favapy-0.3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `favapy-0.3.9.2/PKG-INFO` & `favapy-0.3.9.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 Metadata-Version: 2.1
 Name: favapy
-Version: 0.3.9.2
+Version: 0.3.9.3
 Summary: Infer Functional Associations using Variational Autoencoders on -Omics data.
 Home-page: https://github.com/mikelkou/VAE_Functional_associations
 Author: Mikaela Koutrouli
 Author-email: mikaela.koutrouli@cpr.ku.dk
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/mikelkou/VAE_Functional_associations/issues
-Description: # FAVA: Functional Associations using Variational Autoencoders
-        ![Fava](https://user-images.githubusercontent.com/81096946/177743627-2e6a7447-3fc1-48a8-a6bb-003a3ace223a.png)
-        
-        Protein networks are commonly used for understanding the interplay between proteins in the cell as well as for visualizing omics data. Unfortunately, most existing high-quality networks are heavily biased by data availability, in the sense that well-studied proteins have many more interactions than understudied proteins. To create networks that can help elucidate functions for the latter, we must start from data that are not affected by this literature bias, in other words, from omics data such as single cell RNA-seq (scRNA-seq) and proteomics. While networks can be inferred from such data through simple co-expression analysis, this approach does not work well due to high sparseness (many transcripts/proteins are not consistently observed in each cell/sample) and redundancy (many similar cells/samples are analyzed) of such data. We have therefore developed FAVA, Functional Associations using Variational Autoencoders, which deals with both issues by compressing these high-dimensional data into a dense, low-dimensional latent space. We demonstrate that calculating correlations in this latent space results in much improved networks compared to the original representation for large-scale scRNA-seq and proteomics data from the Human Protein Atlas, and from PRIDE, respectively. We show that these networks, which given the nature of the input data should be free of literature bias, indeed have much better coverage of understudied proteins than existing networks.
-        
-        
-        ## Data availability
-        #### The Combined Network: https://doi.org/10.5281/zenodo.6803472 
-        
-        #### Relevant publications:
-        FAVA: High-quality functional association networks inferred from scRNA-seq and proteomics data
-        https://doi.org/10.1101/2022.07.06.499022
-        
-        The STRING database in 2023
-        https://doi.org/10.1093/nar/gkac1000
-        
-        
-        ## Installation:
-        `pip install favapy`
-        
-        ## favapy as Python library
-        Read the jupyter-notebook: How_to_use_favapy_in_a_notebook
-        It supports both AnnData objects and counts matrices without any preprocessing setps.
-        
-        
-        ## Command line interface
-        Run favapy from the command line as follows:
-        
-        `favapy <path-to-data-file> <path-to-save-output>`
-        
-        
-        ### Optional parameters:
-        
-        `-t` Type of input data ('tsv' or 'csv'). Default value = 'tsv'.
-        
-        `-c` The cut-off on the Pearson Correlation scores. Default value = 0.7.
-        
-        `-d` The dimensions of the intermediate\hidden layer. Default value depends on the input size.
-        
-        `-l` The dimensions of the latent space. Default value depends on the size of the hidden layer.
-        
-        `-e` The number of epochs. Default value = 50.
-        
-        `-b` The  batch size. Default value = 32.
-        
-        
-        
-        
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# FAVA: Functional Associations using Variational Autoencoders
+<!-- ![Fava](https://user-images.githubusercontent.com/81096946/177743627-2e6a7447-3fc1-48a8-a6bb-003a3ace223a.png) -->
+<img src="https://user-images.githubusercontent.com/81096946/177743627-2e6a7447-3fc1-48a8-a6bb-003a3ace223a.png" alt="fava" width="500"/>
+
+Protein networks are commonly used for understanding the interplay between proteins in the cell as well as for visualizing omics data. Unfortunately, most existing high-quality networks are heavily biased by data availability, in the sense that well-studied proteins have many more interactions than understudied proteins. To create networks that can help elucidate functions for the latter, we must start from data that are not affected by this literature bias, in other words, from omics data such as single cell RNA-seq (scRNA-seq) and proteomics. While networks can be inferred from such data through simple co-expression analysis, this approach does not work well due to high sparseness (many transcripts/proteins are not consistently observed in each cell/sample) and redundancy (many similar cells/samples are analyzed) of such data. We have therefore developed FAVA, Functional Associations using Variational Autoencoders, which deals with both issues by compressing these high-dimensional data into a dense, low-dimensional latent space. Calculating correlations in this latent space results in much improved networks compared to the original representation for large-scale scRNA-seq and proteomics data from the Human Protein Atlas, and from PRIDE, respectively. Additionally, these networks, which given the nature of the input data should be free of literature bias, have much better coverage of understudied proteins than existing networks.
+
+[![PyPI version](https://badge.fury.io/py/favapy.svg)](https://badge.fury.io/py/favapy)
+[![Documentation Status](https://readthedocs.org/projects/fava/badge/?version=latest)](https://fava.readthedocs.io/en/latest/?badge=latest)
+
+## Data availability
+[The Combined Network](https://doi.org/10.5281/zenodo.6803472)
+
+## Installation:
+```
+pip install favapy
+```
+
+## favapy as Python library
+Read the jupyter-notebook: [How_to_use_favapy_in_a_notebook](https://github.com/mikelkou/fava/blob/main/How_to_use_favapy_in_a_notebook.ipynb)
+
+favapy supports both AnnData objects and count/abundance matrices.
+
+
+## Command line interface
+Run favapy from the command line as follows:
+```
+favapy <path-to-data-file> <path-to-save-output>
+```
+
+### Optional parameters:
+```
+
+-t Type of input data ('tsv' or 'csv'). Default value = 'tsv'.
+
+-n The number of interactions in the output file (with both directions, proteinA-proteinB and proteinB-proteinA). Default value = 100000.
+
+-c The cut-off on the Pearson Correlation scores. This option overwrites the number of interactions. Default value = None.
+
+-d The dimensions of the intermediate\hidden layer. Default value depends on the input size.
+
+-l The dimensions of the latent space. Default value depends on the size of the hidden layer.
+
+-e The number of epochs. Default value = 50.
+
+-b The  batch size. Default value = 32.
+
+```
+
+If FAVA is useful for your research, consider citing [FAVA BiorXiv](https://doi.org/10.1101/2022.07.06.499022).
+
+#### Other Relevant publications:
+[The STRING database in 2023](https://doi.org/10.1093/nar/gkac1000).
```

### Comparing `favapy-0.3.9.2/README.md` & `favapy-0.3.9.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 # FAVA: Functional Associations using Variational Autoencoders
-![Fava](https://user-images.githubusercontent.com/81096946/177743627-2e6a7447-3fc1-48a8-a6bb-003a3ace223a.png)
+<!-- ![Fava](https://user-images.githubusercontent.com/81096946/177743627-2e6a7447-3fc1-48a8-a6bb-003a3ace223a.png) -->
+<img src="https://user-images.githubusercontent.com/81096946/177743627-2e6a7447-3fc1-48a8-a6bb-003a3ace223a.png" alt="fava" width="500"/>
 
-Protein networks are commonly used for understanding the interplay between proteins in the cell as well as for visualizing omics data. Unfortunately, most existing high-quality networks are heavily biased by data availability, in the sense that well-studied proteins have many more interactions than understudied proteins. To create networks that can help elucidate functions for the latter, we must start from data that are not affected by this literature bias, in other words, from omics data such as single cell RNA-seq (scRNA-seq) and proteomics. While networks can be inferred from such data through simple co-expression analysis, this approach does not work well due to high sparseness (many transcripts/proteins are not consistently observed in each cell/sample) and redundancy (many similar cells/samples are analyzed) of such data. We have therefore developed FAVA, Functional Associations using Variational Autoencoders, which deals with both issues by compressing these high-dimensional data into a dense, low-dimensional latent space. We demonstrate that calculating correlations in this latent space results in much improved networks compared to the original representation for large-scale scRNA-seq and proteomics data from the Human Protein Atlas, and from PRIDE, respectively. We show that these networks, which given the nature of the input data should be free of literature bias, indeed have much better coverage of understudied proteins than existing networks.
+Protein networks are commonly used for understanding the interplay between proteins in the cell as well as for visualizing omics data. Unfortunately, most existing high-quality networks are heavily biased by data availability, in the sense that well-studied proteins have many more interactions than understudied proteins. To create networks that can help elucidate functions for the latter, we must start from data that are not affected by this literature bias, in other words, from omics data such as single cell RNA-seq (scRNA-seq) and proteomics. While networks can be inferred from such data through simple co-expression analysis, this approach does not work well due to high sparseness (many transcripts/proteins are not consistently observed in each cell/sample) and redundancy (many similar cells/samples are analyzed) of such data. We have therefore developed FAVA, Functional Associations using Variational Autoencoders, which deals with both issues by compressing these high-dimensional data into a dense, low-dimensional latent space. Calculating correlations in this latent space results in much improved networks compared to the original representation for large-scale scRNA-seq and proteomics data from the Human Protein Atlas, and from PRIDE, respectively. Additionally, these networks, which given the nature of the input data should be free of literature bias, have much better coverage of understudied proteins than existing networks.
 
+[![PyPI version](https://badge.fury.io/py/favapy.svg)](https://badge.fury.io/py/favapy)
+[![Documentation Status](https://readthedocs.org/projects/fava/badge/?version=latest)](https://fava.readthedocs.io/en/latest/?badge=latest)
 
 ## Data availability
-#### The Combined Network: https://doi.org/10.5281/zenodo.6803472 
-
-#### Relevant publications:
-FAVA: High-quality functional association networks inferred from scRNA-seq and proteomics data
-https://doi.org/10.1101/2022.07.06.499022
-
-The STRING database in 2023
-https://doi.org/10.1093/nar/gkac1000
-
+[The Combined Network](https://doi.org/10.5281/zenodo.6803472)
 
 ## Installation:
-`pip install favapy`
+```
+pip install favapy
+```
 
 ## favapy as Python library
-Read the jupyter-notebook: How_to_use_favapy_in_a_notebook
-It supports both AnnData objects and counts matrices without any preprocessing setps.
+Read the jupyter-notebook: [How_to_use_favapy_in_a_notebook](https://github.com/mikelkou/fava/blob/main/How_to_use_favapy_in_a_notebook.ipynb)
+
+favapy supports both AnnData objects and count/abundance matrices.
 
 
 ## Command line interface
 Run favapy from the command line as follows:
-
-`favapy <path-to-data-file> <path-to-save-output>`
-
+```
+favapy <path-to-data-file> <path-to-save-output>
+```
 
 ### Optional parameters:
+```
 
-`-t` Type of input data ('tsv' or 'csv'). Default value = 'tsv'.
-
-`-c` The cut-off on the Pearson Correlation scores. Default value = 0.7.
+-t Type of input data ('tsv' or 'csv'). Default value = 'tsv'.
 
-`-d` The dimensions of the intermediate\hidden layer. Default value depends on the input size.
+-n The number of interactions in the output file (with both directions, proteinA-proteinB and proteinB-proteinA). Default value = 100000.
 
-`-l` The dimensions of the latent space. Default value depends on the size of the hidden layer.
+-c The cut-off on the Pearson Correlation scores. This option overwrites the number of interactions. Default value = None.
 
-`-e` The number of epochs. Default value = 50.
+-d The dimensions of the intermediate\hidden layer. Default value depends on the input size.
 
-`-b` The  batch size. Default value = 32.
+-l The dimensions of the latent space. Default value depends on the size of the hidden layer.
 
+-e The number of epochs. Default value = 50.
 
+-b The  batch size. Default value = 32.
 
+```
 
+If FAVA is useful for your research, consider citing [FAVA BiorXiv](https://doi.org/10.1101/2022.07.06.499022).
 
+#### Other Relevant publications:
+[The STRING database in 2023](https://doi.org/10.1093/nar/gkac1000).
```

### Comparing `favapy-0.3.9.2/setup.cfg` & `favapy-0.3.9.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = favapy
-version = 0.3.9.2
+version = 0.3.9.3
 author = Mikaela Koutrouli
 author_email = mikaela.koutrouli@cpr.ku.dk
 description = Infer Functional Associations using Variational Autoencoders on -Omics data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mikelkou/VAE_Functional_associations
 project_urls =
```

### Comparing `favapy-0.3.9.2/setup.py` & `favapy-0.3.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="favapy",
-    version="0.3.9.2",
+    version="0.3.9.3",
     author="Mikaela Koutrouli",
     author_email="mikaela.koutrouli@cpr.ku.dk",
     description="Infer Functional Associations using Variational Autoencoders on -Omics data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mikelkou/VAE_Functional_associations",
     project_urls={
```

### Comparing `favapy-0.3.9.2/src/favapy/fava.py` & `favapy-0.3.9.3/src/favapy/fava.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,15 +33,17 @@
     )
     parser.add_argument('input_file', type=str, 
                         help='The absolute path of the data.')
     parser.add_argument('output_file', type=str,
                         help='The absolute path where the output will be saved')
     parser.add_argument('-t', '--data_type', type=str, default='tsv', choices=['tsv', 'csv'], 
                         help='Type of input data.')
-    parser.add_argument('-c', dest='PCC_cutoff', type=float, default=0.7,
+    parser.add_argument('-n', dest='interaction_count', type=int, default=100000,
+                    help='The number of interactions in the output file.')
+    parser.add_argument('-c', dest='PCC_cutoff', type=float, default=None,
                     help='The cut-off on the Pearson Correlation scores.')
     parser.add_argument('-d', dest='hidden_layer', default=None, type=int,
                         help='Intermediate/hidden layer dimensions')
     parser.add_argument('-l', dest='latent_dim', default=None, type=int,
                         help='Latent space dimensions')
     parser.add_argument('-e', dest='epochs', type=int, default=50,
                         help='How many epochs?')
@@ -69,15 +71,17 @@
     expr = np.asarray(array, dtype=np.float32)
     
     if np.all(expr >= 0):
         expr = np.log2(1+expr[:])
     else:
         logging.warn(" Negative values are detected, so log2 normalization is not applied.")
     
-    expr = expr / np.max(expr, axis=1, keepdims=True)
+    # expr = expr / np.max(expr, axis=1, keepdims=True)
+    constant = 1e-8  # small constant to avoid division by zero
+    expr = (expr - np.min(expr, axis=1, keepdims=True)) / (np.max(expr, axis=1, keepdims=True) - np.min(expr, axis=1, keepdims=True) + constant)
     expr = np.nan_to_num(expr)
     return expr, row_names
 
 
 class VAE(keras.Model):
     def __init__(self, opt, x_train, x_test, batch_size, original_dim, hidden_layer, latent_dim, epochs):
         super(VAE, self).__init__()
@@ -141,51 +145,56 @@
     correlation_df = corr_pears.stack().reset_index()
 
     #set column names
     correlation_df.columns = ['Protein_1','Protein_2','Score']
     return correlation_df
 
 
-def pairs_after_cutoff(correlation, PCC_cutoff=0.7):
-    correlation_df_new = correlation.loc[(correlation['Score'] >= PCC_cutoff)]
+def pairs_after_cutoff(correlation, interaction_count=100000, PCC_cutoff=None):
+    if PCC_cutoff is not None and isinstance(PCC_cutoff, (int, float)):
+        logging.info(" A cut-off of " + str(PCC_cutoff) + " is applied.")
+        correlation_df_new = correlation.loc[(correlation['Score'] >= PCC_cutoff)]
+    else:
+        correlation_df_new = correlation.head(interaction_count+1)
+        logging.warn(" The number of interactions in the output file is " + str(interaction_count) + " in which both directions are included: proteinA - proteinB and proteinB - proteinA.")
     return correlation_df_new
 
-
 def cook(data,
 	log2_normalization = True,
 	hidden_layer = None,
         latent_dim = None,
         epochs = 50,
         batch_size = 32,
-        PCC_cutoff = 0.7,
+        interaction_count = 100000,
+        PCC_cutoff = None,
         ):
     
     if type(data)==anndata._core.anndata.AnnData:
         x = data.X.T
         row_names = data.var.index
     else:
         x = np.asarray(data, dtype=np.float32)
         row_names = data.index
     
     if np.any(x < 0):
         log2_normalization = False
-        logging.warn(" Negative values are detected, so log2 normalization is not applied.")
+        logging.warn(" Negative values are detected or log2_normalization was set to False, so log2 normalization is not applied.")
     
     if log2_normalization == True:
         x = np.log2(1+x[:])
         logging.warn(" log2 normalization is applied.")
 
     x = x / np.max(x, axis=1, keepdims=True)
     x = np.nan_to_num(x)
     
     original_dim = x.shape[1]
     if hidden_layer==None:
-        if original_dim >= 10000:
+        if original_dim >= 2000:
             hidden_layer = 1000
-        if original_dim > 500 and original_dim < 10000:
+        if original_dim > 500 and original_dim < 2000:
             hidden_layer = 500
         if original_dim <= 500:
             hidden_layer = 50
 
     if latent_dim==None:
         if hidden_layer >= 1000:
             latent_dim = 100
@@ -195,30 +204,30 @@
             latent_dim = 5
 
     opt = tf.keras.optimizers.Adam(learning_rate=0.001, clipnorm=0.001)
     x_train = x_test = np.array(x) 
     vae = VAE(opt, x_train, x_test, batch_size, original_dim, hidden_layer, latent_dim, epochs)
     x_test_encoded = np.array(vae.encoder.predict(x_test, batch_size=batch_size))
     correlation = create_protein_pairs(x_test_encoded, row_names)
-    final_pairs =  pairs_after_cutoff(correlation,PCC_cutoff=PCC_cutoff)
+    final_pairs =  pairs_after_cutoff(correlation, interaction_count=interaction_count, PCC_cutoff=PCC_cutoff)
     final_pairs = final_pairs[final_pairs.iloc[:,0] != final_pairs.iloc[:,1]]
     final_pairs = final_pairs.sort_values(by=['Score'], ascending=False)
     return final_pairs
 
 
 def main():
     args = argument_parser()
 
     x, row_names = load_data(args.input_file,args.data_type)
     original_dim = x.shape[1]
     
     if args.hidden_layer==None:
-        if original_dim >= 10000:
+        if original_dim >= 2000:
             args.hidden_layer = 1000
-        if original_dim > 500 and original_dim < 10000:
+        if original_dim > 500 and original_dim < 2000:
             args.hidden_layer = 500
         if original_dim <= 500:
             args.hidden_layer = 50
 
     if args.latent_dim==None:
         if args.hidden_layer >= 1000:
             args.latent_dim = 100
@@ -227,22 +236,21 @@
         if args.hidden_layer <= 500:
             args.latent_dim = 5
 
     opt = tf.keras.optimizers.Adam(learning_rate=0.001, clipnorm=0.001)
     x_train = x_test = np.array(x) 
     vae = VAE(opt, x_train, x_test, args.batch_size, original_dim, args.hidden_layer, args.latent_dim, args.epochs)
     x_test_encoded = np.array(vae.encoder.predict(x_test, batch_size=args.batch_size))
+    
+    logging.info(" Calculating Pearson correlation scores.")
 
-    logging.info(" Calculating Pearson correlation scores. A cut-off of " + str(args.PCC_cutoff) + " is applied.")
-
-    correlation = create_protein_pairs(x_test_encoded, row_names)
+    correlation = create_protein_pairs(x_test_encoded, row_names)    
+    final_pairs =  pairs_after_cutoff(correlation, interaction_count=args.interaction_count, PCC_cutoff=args.PCC_cutoff)
+    logging.warn(" If it is not the desired cut-off, please check again the value assigned to the related parameter (-n or interaction_count | -c or PCC_cutoff).")
 
-    logging.warn(" If it is not the desired cut-off, please check again the value assigned to the related parameter (-c or PCC_cutoff).")
-    
-    final_pairs =  pairs_after_cutoff(correlation,PCC_cutoff=args.PCC_cutoff)
     final_pairs = final_pairs[final_pairs.iloc[:,0] != final_pairs.iloc[:,1]]
     final_pairs = final_pairs.sort_values(by=['Score'], ascending=False)
     logging.info(" Saving the file with the interactions in the chosen directory ...")
 
     # Save the file
     np.savetxt(args.output_file, final_pairs, fmt='%s')
     logging.info(" Congratulations! A file is waitiing for you here: " + args.output_file)
```

### Comparing `favapy-0.3.9.2/src/favapy.egg-info/PKG-INFO` & `favapy-0.3.9.3/src/favapy.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 Metadata-Version: 2.1
 Name: favapy
-Version: 0.3.9.2
+Version: 0.3.9.3
 Summary: Infer Functional Associations using Variational Autoencoders on -Omics data.
 Home-page: https://github.com/mikelkou/VAE_Functional_associations
 Author: Mikaela Koutrouli
 Author-email: mikaela.koutrouli@cpr.ku.dk
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/mikelkou/VAE_Functional_associations/issues
-Description: # FAVA: Functional Associations using Variational Autoencoders
-        ![Fava](https://user-images.githubusercontent.com/81096946/177743627-2e6a7447-3fc1-48a8-a6bb-003a3ace223a.png)
-        
-        Protein networks are commonly used for understanding the interplay between proteins in the cell as well as for visualizing omics data. Unfortunately, most existing high-quality networks are heavily biased by data availability, in the sense that well-studied proteins have many more interactions than understudied proteins. To create networks that can help elucidate functions for the latter, we must start from data that are not affected by this literature bias, in other words, from omics data such as single cell RNA-seq (scRNA-seq) and proteomics. While networks can be inferred from such data through simple co-expression analysis, this approach does not work well due to high sparseness (many transcripts/proteins are not consistently observed in each cell/sample) and redundancy (many similar cells/samples are analyzed) of such data. We have therefore developed FAVA, Functional Associations using Variational Autoencoders, which deals with both issues by compressing these high-dimensional data into a dense, low-dimensional latent space. We demonstrate that calculating correlations in this latent space results in much improved networks compared to the original representation for large-scale scRNA-seq and proteomics data from the Human Protein Atlas, and from PRIDE, respectively. We show that these networks, which given the nature of the input data should be free of literature bias, indeed have much better coverage of understudied proteins than existing networks.
-        
-        
-        ## Data availability
-        #### The Combined Network: https://doi.org/10.5281/zenodo.6803472 
-        
-        #### Relevant publications:
-        FAVA: High-quality functional association networks inferred from scRNA-seq and proteomics data
-        https://doi.org/10.1101/2022.07.06.499022
-        
-        The STRING database in 2023
-        https://doi.org/10.1093/nar/gkac1000
-        
-        
-        ## Installation:
-        `pip install favapy`
-        
-        ## favapy as Python library
-        Read the jupyter-notebook: How_to_use_favapy_in_a_notebook
-        It supports both AnnData objects and counts matrices without any preprocessing setps.
-        
-        
-        ## Command line interface
-        Run favapy from the command line as follows:
-        
-        `favapy <path-to-data-file> <path-to-save-output>`
-        
-        
-        ### Optional parameters:
-        
-        `-t` Type of input data ('tsv' or 'csv'). Default value = 'tsv'.
-        
-        `-c` The cut-off on the Pearson Correlation scores. Default value = 0.7.
-        
-        `-d` The dimensions of the intermediate\hidden layer. Default value depends on the input size.
-        
-        `-l` The dimensions of the latent space. Default value depends on the size of the hidden layer.
-        
-        `-e` The number of epochs. Default value = 50.
-        
-        `-b` The  batch size. Default value = 32.
-        
-        
-        
-        
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# FAVA: Functional Associations using Variational Autoencoders
+<!-- ![Fava](https://user-images.githubusercontent.com/81096946/177743627-2e6a7447-3fc1-48a8-a6bb-003a3ace223a.png) -->
+<img src="https://user-images.githubusercontent.com/81096946/177743627-2e6a7447-3fc1-48a8-a6bb-003a3ace223a.png" alt="fava" width="500"/>
+
+Protein networks are commonly used for understanding the interplay between proteins in the cell as well as for visualizing omics data. Unfortunately, most existing high-quality networks are heavily biased by data availability, in the sense that well-studied proteins have many more interactions than understudied proteins. To create networks that can help elucidate functions for the latter, we must start from data that are not affected by this literature bias, in other words, from omics data such as single cell RNA-seq (scRNA-seq) and proteomics. While networks can be inferred from such data through simple co-expression analysis, this approach does not work well due to high sparseness (many transcripts/proteins are not consistently observed in each cell/sample) and redundancy (many similar cells/samples are analyzed) of such data. We have therefore developed FAVA, Functional Associations using Variational Autoencoders, which deals with both issues by compressing these high-dimensional data into a dense, low-dimensional latent space. Calculating correlations in this latent space results in much improved networks compared to the original representation for large-scale scRNA-seq and proteomics data from the Human Protein Atlas, and from PRIDE, respectively. Additionally, these networks, which given the nature of the input data should be free of literature bias, have much better coverage of understudied proteins than existing networks.
+
+[![PyPI version](https://badge.fury.io/py/favapy.svg)](https://badge.fury.io/py/favapy)
+[![Documentation Status](https://readthedocs.org/projects/fava/badge/?version=latest)](https://fava.readthedocs.io/en/latest/?badge=latest)
+
+## Data availability
+[The Combined Network](https://doi.org/10.5281/zenodo.6803472)
+
+## Installation:
+```
+pip install favapy
+```
+
+## favapy as Python library
+Read the jupyter-notebook: [How_to_use_favapy_in_a_notebook](https://github.com/mikelkou/fava/blob/main/How_to_use_favapy_in_a_notebook.ipynb)
+
+favapy supports both AnnData objects and count/abundance matrices.
+
+
+## Command line interface
+Run favapy from the command line as follows:
+```
+favapy <path-to-data-file> <path-to-save-output>
+```
+
+### Optional parameters:
+```
+
+-t Type of input data ('tsv' or 'csv'). Default value = 'tsv'.
+
+-n The number of interactions in the output file (with both directions, proteinA-proteinB and proteinB-proteinA). Default value = 100000.
+
+-c The cut-off on the Pearson Correlation scores. This option overwrites the number of interactions. Default value = None.
+
+-d The dimensions of the intermediate\hidden layer. Default value depends on the input size.
+
+-l The dimensions of the latent space. Default value depends on the size of the hidden layer.
+
+-e The number of epochs. Default value = 50.
+
+-b The  batch size. Default value = 32.
+
+```
+
+If FAVA is useful for your research, consider citing [FAVA BiorXiv](https://doi.org/10.1101/2022.07.06.499022).
+
+#### Other Relevant publications:
+[The STRING database in 2023](https://doi.org/10.1093/nar/gkac1000).
```

