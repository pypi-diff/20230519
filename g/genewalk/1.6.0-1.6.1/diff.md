# Comparing `tmp/genewalk-1.6.0.tar.gz` & `tmp/genewalk-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/genewalk-1.6.0.tar", last modified: Tue May 16 19:22:30 2023, max compression
+gzip compressed data, was "dist/genewalk-1.6.1.tar", last modified: Fri May 19 20:12:18 2023, max compression
```

## Comparing `genewalk-1.6.0.tar` & `genewalk-1.6.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-16 19:22:30.000000 genewalk-1.6.0/
--rw-r--r--   0 horizon    (501) staff       (20)       66 2021-01-27 21:08:32.000000 genewalk-1.6.0/MANIFEST.in
--rw-r--r--   0 horizon    (501) staff       (20)    23541 2023-05-16 19:22:30.000000 genewalk-1.6.0/PKG-INFO
--rw-r--r--   0 horizon    (501) staff       (20)    19851 2023-05-16 19:20:53.000000 genewalk-1.6.0/README.md
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-16 19:22:30.000000 genewalk-1.6.0/doc/
--rw-r--r--   0 horizon    (501) staff       (20)      606 2019-08-30 13:54:12.000000 genewalk-1.6.0/doc/Makefile
--rw-r--r--   0 horizon    (501) staff       (20)     5562 2023-05-16 19:20:53.000000 genewalk-1.6.0/doc/conf.py
--rw-r--r--   0 horizon    (501) staff       (20)      407 2019-08-30 13:54:12.000000 genewalk-1.6.0/doc/index.rst
--rw-r--r--   0 horizon    (501) staff       (20)      812 2019-08-30 13:54:12.000000 genewalk-1.6.0/doc/make.bat
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-16 19:22:30.000000 genewalk-1.6.0/doc/modules/
--rw-r--r--   0 horizon    (501) staff       (20)     1648 2021-01-27 21:08:32.000000 genewalk-1.6.0/doc/modules/genewalk.rst
--rw-r--r--   0 horizon    (501) staff       (20)      124 2019-08-30 13:54:12.000000 genewalk-1.6.0/doc/modules/index.rst
--rw-r--r--   0 horizon    (501) staff       (20)       83 2021-01-27 21:08:32.000000 genewalk-1.6.0/doc/requirements.txt
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk/
--rw-r--r--   0 horizon    (501) staff       (20)      478 2023-05-16 19:20:53.000000 genewalk-1.6.0/genewalk/__init__.py
--rw-r--r--   0 horizon    (501) staff       (20)    13352 2023-05-16 19:20:53.000000 genewalk-1.6.0/genewalk/cli.py
--rw-r--r--   0 horizon    (501) staff       (20)     8361 2023-05-16 19:20:53.000000 genewalk-1.6.0/genewalk/deepwalk.py
--rw-r--r--   0 horizon    (501) staff       (20)    16017 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/gene_lists.py
--rw-r--r--   0 horizon    (501) staff       (20)     7237 2020-09-21 20:38:26.000000 genewalk-1.6.0/genewalk/get_indra_stmts.py
--rw-r--r--   0 horizon    (501) staff       (20)     1613 2020-02-26 02:19:30.000000 genewalk-1.6.0/genewalk/null_distributions.py
--rw-r--r--   0 horizon    (501) staff       (20)    17380 2021-05-10 13:16:56.000000 genewalk-1.6.0/genewalk/nx_mg_assembler.py
--rw-r--r--   0 horizon    (501) staff       (20)    13342 2023-05-16 19:20:53.000000 genewalk-1.6.0/genewalk/perform_statistics.py
--rw-r--r--   0 horizon    (501) staff       (20)    18257 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/plot.py
--rw-r--r--   0 horizon    (501) staff       (20)     5406 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/resources.py
--rw-r--r--   0 horizon    (501) staff       (20)      442 2021-01-27 21:08:32.000000 genewalk-1.6.0/genewalk/results_template.html
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk/tests/
--rw-r--r--   0 horizon    (501) staff       (20)        0 2019-08-30 13:54:12.000000 genewalk-1.6.0/genewalk/tests/__init__.py
--rw-r--r--   0 horizon    (501) staff       (20)     6255 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/tests/test_cli.py
--rw-r--r--   0 horizon    (501) staff       (20)      735 2020-02-26 02:19:30.000000 genewalk-1.6.0/genewalk/tests/test_deepwalk.py
--rw-r--r--   0 horizon    (501) staff       (20)     3381 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/tests/test_gene_lists.py
--rw-r--r--   0 horizon    (501) staff       (20)      719 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/tests/test_indra_assembly.py
--rw-r--r--   0 horizon    (501) staff       (20)     5185 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/tests/test_sif_assembler.py
--rw-r--r--   0 horizon    (501) staff       (20)      988 2021-01-27 21:08:32.000000 genewalk-1.6.0/genewalk/tests/test_visualize.py
--rw-r--r--   0 horizon    (501) staff       (20)      815 2021-02-21 02:50:54.000000 genewalk-1.6.0/genewalk/tests/util.py
-drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk.egg-info/
--rw-r--r--   0 horizon    (501) staff       (20)    23541 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk.egg-info/PKG-INFO
--rw-r--r--   0 horizon    (501) staff       (20)      874 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk.egg-info/SOURCES.txt
--rw-r--r--   0 horizon    (501) staff       (20)        1 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk.egg-info/dependency_links.txt
--rw-r--r--   0 horizon    (501) staff       (20)       48 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk.egg-info/entry_points.txt
--rw-r--r--   0 horizon    (501) staff       (20)      111 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk.egg-info/requires.txt
--rw-r--r--   0 horizon    (501) staff       (20)        9 2023-05-16 19:22:30.000000 genewalk-1.6.0/genewalk.egg-info/top_level.txt
--rw-r--r--   0 horizon    (501) staff       (20)       79 2023-05-16 19:22:30.000000 genewalk-1.6.0/setup.cfg
--rwxr-xr-x   0 horizon    (501) staff       (20)     1717 2023-05-16 19:20:53.000000 genewalk-1.6.0/setup.py
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-19 20:12:18.000000 genewalk-1.6.1/
+-rw-r--r--   0 horizon    (501) staff       (20)       66 2021-01-27 21:08:32.000000 genewalk-1.6.1/MANIFEST.in
+-rw-r--r--   0 horizon    (501) staff       (20)    23541 2023-05-19 20:12:18.000000 genewalk-1.6.1/PKG-INFO
+-rw-r--r--   0 horizon    (501) staff       (20)    19851 2023-05-16 19:20:53.000000 genewalk-1.6.1/README.md
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-19 20:12:18.000000 genewalk-1.6.1/doc/
+-rw-r--r--   0 horizon    (501) staff       (20)      606 2019-08-30 13:54:12.000000 genewalk-1.6.1/doc/Makefile
+-rw-r--r--   0 horizon    (501) staff       (20)     5562 2023-05-19 20:09:59.000000 genewalk-1.6.1/doc/conf.py
+-rw-r--r--   0 horizon    (501) staff       (20)      407 2019-08-30 13:54:12.000000 genewalk-1.6.1/doc/index.rst
+-rw-r--r--   0 horizon    (501) staff       (20)      812 2019-08-30 13:54:12.000000 genewalk-1.6.1/doc/make.bat
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-19 20:12:18.000000 genewalk-1.6.1/doc/modules/
+-rw-r--r--   0 horizon    (501) staff       (20)     1648 2021-01-27 21:08:32.000000 genewalk-1.6.1/doc/modules/genewalk.rst
+-rw-r--r--   0 horizon    (501) staff       (20)      124 2019-08-30 13:54:12.000000 genewalk-1.6.1/doc/modules/index.rst
+-rw-r--r--   0 horizon    (501) staff       (20)       83 2021-01-27 21:08:32.000000 genewalk-1.6.1/doc/requirements.txt
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk/
+-rw-r--r--   0 horizon    (501) staff       (20)      478 2023-05-19 20:09:59.000000 genewalk-1.6.1/genewalk/__init__.py
+-rw-r--r--   0 horizon    (501) staff       (20)    13352 2023-05-16 19:20:53.000000 genewalk-1.6.1/genewalk/cli.py
+-rw-r--r--   0 horizon    (501) staff       (20)     8361 2023-05-16 19:20:53.000000 genewalk-1.6.1/genewalk/deepwalk.py
+-rw-r--r--   0 horizon    (501) staff       (20)    16017 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/gene_lists.py
+-rw-r--r--   0 horizon    (501) staff       (20)     7237 2020-09-21 20:38:26.000000 genewalk-1.6.1/genewalk/get_indra_stmts.py
+-rw-r--r--   0 horizon    (501) staff       (20)     1613 2020-02-26 02:19:30.000000 genewalk-1.6.1/genewalk/null_distributions.py
+-rw-r--r--   0 horizon    (501) staff       (20)    17380 2021-05-10 13:16:56.000000 genewalk-1.6.1/genewalk/nx_mg_assembler.py
+-rw-r--r--   0 horizon    (501) staff       (20)    13295 2023-05-19 20:09:59.000000 genewalk-1.6.1/genewalk/perform_statistics.py
+-rw-r--r--   0 horizon    (501) staff       (20)    18257 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/plot.py
+-rw-r--r--   0 horizon    (501) staff       (20)     5406 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/resources.py
+-rw-r--r--   0 horizon    (501) staff       (20)      442 2021-01-27 21:08:32.000000 genewalk-1.6.1/genewalk/results_template.html
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk/tests/
+-rw-r--r--   0 horizon    (501) staff       (20)        0 2019-08-30 13:54:12.000000 genewalk-1.6.1/genewalk/tests/__init__.py
+-rw-r--r--   0 horizon    (501) staff       (20)     6255 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/tests/test_cli.py
+-rw-r--r--   0 horizon    (501) staff       (20)      735 2020-02-26 02:19:30.000000 genewalk-1.6.1/genewalk/tests/test_deepwalk.py
+-rw-r--r--   0 horizon    (501) staff       (20)     3381 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/tests/test_gene_lists.py
+-rw-r--r--   0 horizon    (501) staff       (20)      719 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/tests/test_indra_assembly.py
+-rw-r--r--   0 horizon    (501) staff       (20)     5185 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/tests/test_sif_assembler.py
+-rw-r--r--   0 horizon    (501) staff       (20)      988 2021-01-27 21:08:32.000000 genewalk-1.6.1/genewalk/tests/test_visualize.py
+-rw-r--r--   0 horizon    (501) staff       (20)      815 2021-02-21 02:50:54.000000 genewalk-1.6.1/genewalk/tests/util.py
+drwxr-xr-x   0 horizon    (501) staff       (20)        0 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk.egg-info/
+-rw-r--r--   0 horizon    (501) staff       (20)    23541 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk.egg-info/PKG-INFO
+-rw-r--r--   0 horizon    (501) staff       (20)      874 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk.egg-info/SOURCES.txt
+-rw-r--r--   0 horizon    (501) staff       (20)        1 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk.egg-info/dependency_links.txt
+-rw-r--r--   0 horizon    (501) staff       (20)       48 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk.egg-info/entry_points.txt
+-rw-r--r--   0 horizon    (501) staff       (20)      111 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk.egg-info/requires.txt
+-rw-r--r--   0 horizon    (501) staff       (20)        9 2023-05-19 20:12:18.000000 genewalk-1.6.1/genewalk.egg-info/top_level.txt
+-rw-r--r--   0 horizon    (501) staff       (20)       79 2023-05-19 20:12:18.000000 genewalk-1.6.1/setup.cfg
+-rwxr-xr-x   0 horizon    (501) staff       (20)     1717 2023-05-19 20:09:59.000000 genewalk-1.6.1/setup.py
```

### Comparing `genewalk-1.6.0/PKG-INFO` & `genewalk-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genewalk
-Version: 1.6.0
+Version: 1.6.1
 Summary: Determine gene function based on network embeddings.
 Home-page: https://github.com/churchmanlab/genewalk
 Author: Robert Ietswaart
 Author-email: robert_ietswaart@hms.harvard.edu
 License: UNKNOWN
 Description: # GeneWalk
```

### Comparing `genewalk-1.6.0/README.md` & `genewalk-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/doc/Makefile` & `genewalk-1.6.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/doc/conf.py` & `genewalk-1.6.1/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 project = 'GeneWalk'
 copyright = '2019, GeneWalk Developers'
 author = 'GeneWalk Developers'
 
 # The short X.Y version
 version = '1.6'
 # The full version, including alpha/beta/rc tags
-release = '1.6.0'
+release = '1.6.1'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `genewalk-1.6.0/doc/make.bat` & `genewalk-1.6.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/doc/modules/genewalk.rst` & `genewalk-1.6.1/doc/modules/genewalk.rst`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/cli.py` & `genewalk-1.6.1/genewalk/cli.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/deepwalk.py` & `genewalk-1.6.1/genewalk/deepwalk.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/gene_lists.py` & `genewalk-1.6.1/genewalk/gene_lists.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/get_indra_stmts.py` & `genewalk-1.6.1/genewalk/get_indra_stmts.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/null_distributions.py` & `genewalk-1.6.1/genewalk/null_distributions.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/nx_mg_assembler.py` & `genewalk-1.6.1/genewalk/nx_mg_assembler.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/perform_statistics.py` & `genewalk-1.6.1/genewalk/perform_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,17 +229,16 @@
                                  'entrez_human', 'entrez_mouse', 'custom'}:
             header = [self.gene_id_type] + header
 
         df = pd.DataFrame.from_records(rows, columns=header)
         df = self.global_fdr(df,alpha_fdr)
         df.drop(['pval_rep'+str(i) for i in range(len(self.nvs))],
                 axis=1, inplace=True) 
-        df[self.gene_id_type] = df[self.gene_id_type].astype('category')
-        df[self.gene_id_type] = \
-        df[self.gene_id_type].cat.set_categories(df[self.gene_id_type].unique())
+        df[self.gene_id_type] = pd.Categorical(df[self.gene_id_type], \
+            categories=df[self.gene_id_type].unique(), ordered=True)
         df[['ncon_gene', 'ncon_go']] = \
             df[['ncon_gene', 'ncon_go']].astype('str')
         df = df.sort_values(by=[self.gene_id_type, 'global_padj', 'gene_padj',
                                 'sim', 'go_domain', 'go_name'],
                             ascending=[True, True, True, False, True, True])
         if self.gene_id_type == 'custom':
             df.drop(['hgnc_symbol','hgnc_id'],axis=1, inplace=True)
```

### Comparing `genewalk-1.6.0/genewalk/plot.py` & `genewalk-1.6.1/genewalk/plot.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/resources.py` & `genewalk-1.6.1/genewalk/resources.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/tests/test_cli.py` & `genewalk-1.6.1/genewalk/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/tests/test_deepwalk.py` & `genewalk-1.6.1/genewalk/tests/test_deepwalk.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/tests/test_gene_lists.py` & `genewalk-1.6.1/genewalk/tests/test_gene_lists.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/tests/test_indra_assembly.py` & `genewalk-1.6.1/genewalk/tests/test_indra_assembly.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/tests/test_sif_assembler.py` & `genewalk-1.6.1/genewalk/tests/test_sif_assembler.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/tests/test_visualize.py` & `genewalk-1.6.1/genewalk/tests/test_visualize.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk/tests/util.py` & `genewalk-1.6.1/genewalk/tests/util.py`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/genewalk.egg-info/PKG-INFO` & `genewalk-1.6.1/genewalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genewalk
-Version: 1.6.0
+Version: 1.6.1
 Summary: Determine gene function based on network embeddings.
 Home-page: https://github.com/churchmanlab/genewalk
 Author: Robert Ietswaart
 Author-email: robert_ietswaart@hms.harvard.edu
 License: UNKNOWN
 Description: # GeneWalk
```

### Comparing `genewalk-1.6.0/genewalk.egg-info/SOURCES.txt` & `genewalk-1.6.1/genewalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genewalk-1.6.0/setup.py` & `genewalk-1.6.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def main():
     install_list = ['numpy', 'pandas', 'networkx>=2.1', 'gensim>=4.0.0', 'goatools',
                     'scipy>=1.3.0', 'matplotlib', 'seaborn', 'plotly>=4.0.0']
 
     setup(name='genewalk',
-          version='1.6.0',
+          version='1.6.1',
           description='Determine gene function based on network embeddings.',
           long_description=long_description,
           long_description_content_type='text/markdown',
           author='Robert Ietswaart',
           author_email='robert_ietswaart@hms.harvard.edu',
           url='https://github.com/churchmanlab/genewalk',
           classifiers=[
```

