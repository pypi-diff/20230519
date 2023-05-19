# Comparing `tmp/biocartograph-0.5.1.tar.gz` & `tmp/biocartograph-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biocartograph-0.5.1.tar", last modified: Tue May 16 13:52:00 2023, max compression
+gzip compressed data, was "biocartograph-0.5.3.tar", last modified: Fri May 19 09:24:42 2023, max compression
```

## Comparing `biocartograph-0.5.1.tar` & `biocartograph-0.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-16 13:52:00.694829 biocartograph-0.5.1/
--rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-01-03 14:01:46.000000 biocartograph-0.5.1/LICENSE
--rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-05-16 13:52:00.694829 biocartograph-0.5.1/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-04-04 06:38:15.000000 biocartograph-0.5.1/README.md
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-16 13:52:00.693829 biocartograph-0.5.1/biocartograph.egg-info/
--rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-05-16 13:52:00.000000 biocartograph-0.5.1/biocartograph.egg-info/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)      301 2023-05-16 13:52:00.000000 biocartograph-0.5.1/biocartograph.egg-info/SOURCES.txt
--rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-05-16 13:52:00.000000 biocartograph-0.5.1/biocartograph.egg-info/dependency_links.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-05-16 13:52:00.000000 biocartograph-0.5.1/biocartograph.egg-info/top_level.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-05-16 13:52:00.694829 biocartograph-0.5.1/setup.cfg
--rw-r--r--   0 rictjo    (1000) users      (100)      910 2023-05-16 13:50:30.000000 biocartograph-0.5.1/setup.py
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-16 13:52:00.693829 biocartograph-0.5.1/src/
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-16 13:52:00.694829 biocartograph-0.5.1/src/biocartograph/
--rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-03-26 08:32:40.000000 biocartograph-0.5.1/src/biocartograph/__init__.py
--rw-r--r--   0 rictjo    (1000) users      (100)    14381 2023-03-26 10:38:54.000000 biocartograph-0.5.1/src/biocartograph/enrichment.py
--rw-r--r--   0 rictjo    (1000) users      (100)    19937 2023-05-16 13:50:30.000000 biocartograph-0.5.1/src/biocartograph/quantification.py
--rw-r--r--   0 rictjo    (1000) users      (100)    27027 2023-05-16 13:50:30.000000 biocartograph-0.5.1/src/biocartograph/special.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-19 09:24:42.262913 biocartograph-0.5.3/
+-rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-01-03 14:01:46.000000 biocartograph-0.5.3/LICENSE
+-rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-05-19 09:24:42.262913 biocartograph-0.5.3/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-04-04 06:38:15.000000 biocartograph-0.5.3/README.md
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-19 09:24:42.260913 biocartograph-0.5.3/biocartograph.egg-info/
+-rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-05-19 09:24:42.000000 biocartograph-0.5.3/biocartograph.egg-info/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)      301 2023-05-19 09:24:42.000000 biocartograph-0.5.3/biocartograph.egg-info/SOURCES.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-05-19 09:24:42.000000 biocartograph-0.5.3/biocartograph.egg-info/dependency_links.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-05-19 09:24:42.000000 biocartograph-0.5.3/biocartograph.egg-info/top_level.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-05-19 09:24:42.262913 biocartograph-0.5.3/setup.cfg
+-rw-r--r--   0 rictjo    (1000) users      (100)      910 2023-05-19 09:14:57.000000 biocartograph-0.5.3/setup.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-19 09:24:42.259913 biocartograph-0.5.3/src/
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-19 09:24:42.261913 biocartograph-0.5.3/src/biocartograph/
+-rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-03-26 08:32:40.000000 biocartograph-0.5.3/src/biocartograph/__init__.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    14381 2023-03-26 10:38:54.000000 biocartograph-0.5.3/src/biocartograph/enrichment.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    20536 2023-05-19 09:17:35.000000 biocartograph-0.5.3/src/biocartograph/quantification.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    27027 2023-05-16 13:50:30.000000 biocartograph-0.5.3/src/biocartograph/special.py
```

### Comparing `biocartograph-0.5.1/LICENSE` & `biocartograph-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `biocartograph-0.5.1/PKG-INFO` & `biocartograph-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.5.1
+Version: 0.5.3
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biocartograph-0.5.1/README.md` & `biocartograph-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `biocartograph-0.5.1/biocartograph.egg-info/PKG-INFO` & `biocartograph-0.5.3/biocartograph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.5.1
+Version: 0.5.3
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biocartograph-0.5.1/setup.py` & `biocartograph-0.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name         = "biocartograph",
-    version      = "0.5.1",
+    version      = "0.5.3",
     author       = "Richard Tjörnhammar",
     author_email = "richard.tjornhammar@gmail.com",
     description  = "Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/rictjo/biocarta",
     packages = setuptools.find_packages('src'),
```

### Comparing `biocartograph-0.5.1/src/biocartograph/enrichment.py` & `biocartograph-0.5.3/src/biocartograph/enrichment.py`

 * *Files identical despite different names*

### Comparing `biocartograph-0.5.1/src/biocartograph/quantification.py` & `biocartograph-0.5.3/src/biocartograph/quantification.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,15 @@
         umap_seed:int = 42 , hierarchy_cmd:str = 'ward' , divergence = lambda r : np.exp(r) ,
         add_labels:list[str] = None , sample_label:str = None , alignment_label:str = None , bRemoveCurse:bool=False ,
         n_projections:int = 2 , directory:str = './' , bQN:int = None ,
         nNeighborFilter:list[int] = None , heal_symmetry_break_method:str = 'average' ,
         epls_ownership:str = 'angle' , bNonEuclideanBackprojection:bool = False ,
         Sfunc = lambda x:np.mean(x,0) , bAddPies:bool=False , bUseTDA:bool = False ,
         consensus_function = lambda x:np.sum(x) , consensus_labels:list[str] = None ,
+        bUseGeometricallyCenteredZvalues:bool = False ,
         contraction_quantile:float = None   ,
         contraction_depth:float    = None   ) -> tuple[pd.DataFrame] :
     #
     import biocartograph.special as biox
     #
     if bVerbose :
         print ( "TO DISABLE WRITING OF RESULTS TO", directory )
@@ -154,14 +155,15 @@
         'umap_seed:int':umap_seed , 'hierarchy_cmd:str':hierarchy_cmd , 'divergence:lambda function': divergence ,
         'add_labels:list[str]':add_labels , 'sample_label:str':sample_label , 'alignment_label:str':alignment_label ,
         'bRemoveCurse:bool':bRemoveCurse , 'n_projections:int':n_projections , 'directory:str':directory , 'bQN:int':bQN ,
         'nNeighborFilter:list[int]':nNeighborFilter , 'heal_symmetry_break_method:str':heal_symmetry_break_method ,
         'epls_ownership:str':epls_ownership , 'bNonEuclideanBackprojection:bool':bNonEuclideanBackprojection ,
         'Sfunc':Sfunc , 'bAddPies:bool':bAddPies , 'bUseTDA':bUseTDA ,
         'consensus_function':consensus_function , 'consensus_labels:list[str]':consensus_labels ,
+        'bUseGeometricallyCenteredZvalues:bool' : bUseGeometricallyCenteredZvalues ,
 	'contraction_quantile:float': contraction_quantile , ' contraction_depth:float': contraction_depth }
             ofile = open ( header_str + runinfo_file , 'w' )
             for item in run_dict.items():
                 if 'list' in str(type(item[1])):
                     print ( item[0],'\t=\t [', ','.join([str(i) for i in item[1]]) ,']', file=ofile )
                 else :
                     print ( item[0],'\t=\t [', str(item[1]) ,']', file=ofile )
@@ -200,16 +202,20 @@
     nRound_		= None
     if not n_components is None :
         m = np.min(np.shape(adf.values))
         if n_components >= m :
             n_components = m - 1
             print ( 'WARNING SETTING n_components TO :' , n_components )
     #
-    from impetuous.special import zvals
-    input_values = zvals( adf.values )['z']
+    if bUseGeometricallyCenteredZvalues :
+        from impetuous.quantification import mean_field,std_field
+        input_values = ( adf.values - mean_field(adf.values) ) / std_field(adf.values)
+    else :
+        from impetuous.special import zvals
+        input_values = zvals( adf.values )['z']
     #
     input_values_f = input_values
     input_values_s = input_values.T
     MF_f , MF_s = None , None
     if 'covariation' in distance_type or 'coexpression' in distance_type or bPreCompute :
         u , s , vt = np.linalg.svd ( input_values , False )
         # SINCE INPUT IS MEAN CENTERED THE COMPONENT COORDINATES CORRESPOND TO THE COVARIATION MATRIX
@@ -227,15 +233,19 @@
     # NOT THE bUseUMAP IS SET TRUE
     if not consensus_labels is None :
         if 'list' in str(type(consensus_labels)) :
             for label in consensus_labels :
                 if 'str' in str(type(label)) :
                     if label in jdf.index :
                         gdf = adf.T.groupby(jdf.loc[label]).apply( consensus_function ).T
-                        aux_vals = np.linalg.svd( zvals(gdf.values)['z'] , False )
+                        if bUseGeometricallyCenteredZvalues :
+                            z_values = ( gdf.values - mean_field(gdf.values) ) / std_field(gdf.values)
+                        else :
+                            z_values = zvals(gdf.values)['z']
+                        aux_vals = np.linalg.svd( z_values , False )
                         aux_vals = aux_vals[0]*aux_vals[1]
                         MF_f = np.concatenate([MF_f.T,aux_vals.T]).T
     #
     if 'covariation' in distance_type or 'coexpression' in distance_type :
         input_values_f = MF_f
         input_values_s = MF_s
         if 'secondary[' in distance_type :	# THIS IS ACTUALLY A RATHER ODD THING TO DO
```

### Comparing `biocartograph-0.5.1/src/biocartograph/special.py` & `biocartograph-0.5.3/src/biocartograph/special.py`

 * *Files identical despite different names*

